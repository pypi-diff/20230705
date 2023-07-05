# Comparing `tmp/dynami-1.0.5.tar.gz` & `tmp/dynami-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynami-1.0.5.tar", last modified: Sat Mar 25 22:20:59 2023, max compression
+gzip compressed data, was "dynami-1.0.6.tar", last modified: Wed Jul  5 09:06:20 2023, max compression
```

## Comparing `dynami-1.0.5.tar` & `dynami-1.0.6.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 22:20:59.128061 dynami-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-25 22:20:46.000000 dynami-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-03-25 22:20:59.128061 dynami-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-03-25 22:20:46.000000 dynami-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 22:20:59.128061 dynami-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-25 22:20:46.000000 dynami-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 22:20:59.120061 dynami-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 22:20:59.120061 dynami-1.0.5/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 22:20:59.124061 dynami-1.0.5/src/python/dynami/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-25 22:20:46.000000 dynami-1.0.5/src/python/dynami/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-03-25 22:20:46.000000 dynami-1.0.5/src/python/dynami/dynami.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 22:20:59.128061 dynami-1.0.5/src/python/dynami/ext/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-25 22:20:46.000000 dynami-1.0.5/src/python/dynami/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-25 22:20:46.000000 dynami-1.0.5/src/python/dynami/ext/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 22:20:59.128061 dynami-1.0.5/src/python/dynami/ext/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-25 22:20:46.000000 dynami-1.0.5/src/python/dynami/ext/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-25 22:20:46.000000 dynami-1.0.5/src/python/dynami/ext/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-25 22:20:46.000000 dynami-1.0.5/src/python/dynami/ext/utils/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-25 22:20:46.000000 dynami-1.0.5/src/python/dynami/ext/utils/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 22:20:59.128061 dynami-1.0.5/src/python/dynami/provider/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-25 22:20:46.000000 dynami-1.0.5/src/python/dynami/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-03-25 22:20:46.000000 dynami-1.0.5/src/python/dynami/provider/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-03-25 22:20:46.000000 dynami-1.0.5/src/python/dynami/provider/hetzner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 22:20:59.128061 dynami-1.0.5/src/python/dynami.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-03-25 22:20:59.000000 dynami-1.0.5/src/python/dynami.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-25 22:20:59.000000 dynami-1.0.5/src/python/dynami.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 22:20:59.000000 dynami-1.0.5/src/python/dynami.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-25 22:20:59.000000 dynami-1.0.5/src/python/dynami.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 22:20:59.000000 dynami-1.0.5/src/python/dynami.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-25 22:20:59.000000 dynami-1.0.5/src/python/dynami.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:06:20.870170 dynami-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-05 09:06:07.000000 dynami-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-05 09:06:20.870170 dynami-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-05 09:06:07.000000 dynami-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 09:06:20.870170 dynami-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-05 09:06:07.000000 dynami-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:06:20.870170 dynami-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:06:20.870170 dynami-1.0.6/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:06:20.870170 dynami-1.0.6/src/python/dynami/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-05 09:06:07.000000 dynami-1.0.6/src/python/dynami/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-07-05 09:06:07.000000 dynami-1.0.6/src/python/dynami/dynami.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:06:20.870170 dynami-1.0.6/src/python/dynami/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 09:06:07.000000 dynami-1.0.6/src/python/dynami/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-05 09:06:07.000000 dynami-1.0.6/src/python/dynami/ext/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:06:20.870170 dynami-1.0.6/src/python/dynami/ext/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 09:06:07.000000 dynami-1.0.6/src/python/dynami/ext/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-05 09:06:07.000000 dynami-1.0.6/src/python/dynami/ext/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-05 09:06:07.000000 dynami-1.0.6/src/python/dynami/ext/utils/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-05 09:06:07.000000 dynami-1.0.6/src/python/dynami/ext/utils/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:06:20.870170 dynami-1.0.6/src/python/dynami/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-05 09:06:07.000000 dynami-1.0.6/src/python/dynami/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-05 09:06:07.000000 dynami-1.0.6/src/python/dynami/provider/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-05 09:06:07.000000 dynami-1.0.6/src/python/dynami/provider/godaddy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-05 09:06:07.000000 dynami-1.0.6/src/python/dynami/provider/hetzner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:06:20.870170 dynami-1.0.6/src/python/dynami.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-05 09:06:20.000000 dynami-1.0.6/src/python/dynami.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-05 09:06:20.000000 dynami-1.0.6/src/python/dynami.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:06:20.000000 dynami-1.0.6/src/python/dynami.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-05 09:06:20.000000 dynami-1.0.6/src/python/dynami.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 09:06:20.000000 dynami-1.0.6/src/python/dynami.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-05 09:06:20.000000 dynami-1.0.6/src/python/dynami.egg-info/top_level.txt
```

### Comparing `dynami-1.0.5/LICENSE` & `dynami-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dynami-1.0.5/PKG-INFO` & `dynami-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynami
-Version: 1.0.5
+Version: 1.0.6
 Summary: Module to dynamically update DNS records from multiple services like Hetzner, Amazon, Microsoft... 
 Home-page: https://github.com/bytesentinel/dynami
 Author: ByteSentinel
 Author-email: info@bytesentinel.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dynami-1.0.5/README.md` & `dynami-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dynami-1.0.5/setup.py` & `dynami-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 SRC_DIR = "src/python"
 
 setup(
     name="dynami",
-    version="1.0.5",
+    version="1.0.6",
     author="ByteSentinel",
     author_email="info@bytesentinel.io",
     description="Module to dynamically update DNS records from multiple services like Hetzner, Amazon, Microsoft... ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bytesentinel/dynami",
     classifiers=[
```

### Comparing `dynami-1.0.5/src/python/dynami/dynami.py` & `dynami-1.0.6/src/python/dynami/dynami.py`

 * *Files identical despite different names*

### Comparing `dynami-1.0.5/src/python/dynami/ext/client.py` & `dynami-1.0.6/src/python/dynami/ext/client.py`

 * *Files identical despite different names*

### Comparing `dynami-1.0.5/src/python/dynami/ext/utils/config.py` & `dynami-1.0.6/src/python/dynami/ext/utils/config.py`

 * *Files identical despite different names*

### Comparing `dynami-1.0.5/src/python/dynami/ext/utils/system.py` & `dynami-1.0.6/src/python/dynami/ext/utils/system.py`

 * *Files identical despite different names*

### Comparing `dynami-1.0.5/src/python/dynami/provider/gcp.py` & `dynami-1.0.6/src/python/dynami/provider/gcp.py`

 * *Files identical despite different names*

### Comparing `dynami-1.0.5/src/python/dynami/provider/hetzner.py` & `dynami-1.0.6/src/python/dynami/provider/hetzner.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,29 +17,29 @@
         data = json.dumps({
             "value": value,
             "ttl": 86400,
             "type": str(self.record_type),
             "name": record,
             "zone_id": self.zone_id
         })
-        result = requests.post(url, headers=self.headers, data=data)
+        result = requests.post(url, headers=self.headers, data=data).json()
         return result
 
     def update_record(self, value: str, type: str, record: str) -> dict:
         self.record_type.set(type)
         record_id = self.get_record_id(record=record)
         url = "https://dns.hetzner.com/api/v1/records/" + record
         data = json.dumps({
             "value": value,
             "ttl": 86400,
             "type": str(self.record_type),
             "name": record,
             "zone_id": self.zone_id
         })
-        result = requests.put(url, headers=self.headers, data=data)
+        result = requests.put(url, headers=self.headers, data=data).json()
         return result
 
     def get_zone_id(self, zone: str) -> str:
         url = "https://dns.hetzner.com/api/v1/zones"
         zones = requests.get(url, headers=self.headers).json()
         for z in zones["zones"]:
             if z["name"] == zone:
```

### Comparing `dynami-1.0.5/src/python/dynami.egg-info/PKG-INFO` & `dynami-1.0.6/src/python/dynami.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynami
-Version: 1.0.5
+Version: 1.0.6
 Summary: Module to dynamically update DNS records from multiple services like Hetzner, Amazon, Microsoft... 
 Home-page: https://github.com/bytesentinel/dynami
 Author: ByteSentinel
 Author-email: info@bytesentinel.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dynami-1.0.5/src/python/dynami.egg-info/SOURCES.txt` & `dynami-1.0.6/src/python/dynami.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 src/python/dynami/ext/client.py
 src/python/dynami/ext/utils/__init__.py
 src/python/dynami/ext/utils/config.py
 src/python/dynami/ext/utils/ip.py
 src/python/dynami/ext/utils/system.py
 src/python/dynami/provider/__init__.py
 src/python/dynami/provider/gcp.py
+src/python/dynami/provider/godaddy.py
 src/python/dynami/provider/hetzner.py
```

