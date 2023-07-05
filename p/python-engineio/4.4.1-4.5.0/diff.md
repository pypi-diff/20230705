# Comparing `tmp/python-engineio-4.4.1.tar.gz` & `tmp/python-engineio-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-engineio-4.4.1.tar", last modified: Wed Apr 19 15:21:32 2023, max compression
+gzip compressed data, was "python-engineio-4.5.0.tar", last modified: Wed Jul  5 12:30:15 2023, max compression
```

## Comparing `python-engineio-4.4.1.tar` & `python-engineio-4.5.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-19 15:21:32.148364 python-engineio-4.4.1/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1082 2019-11-17 19:17:59.000000 python-engineio-4.4.1/LICENSE
--rw-r--r--   0 mgrinberg   (502) staff       (20)       26 2019-11-17 19:17:59.000000 python-engineio-4.4.1/MANIFEST.in
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1976 2023-04-19 15:21:32.148601 python-engineio-4.4.1/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1288 2021-06-03 19:08:45.000000 python-engineio-4.4.1/README.md
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1012 2021-02-22 00:17:35.000000 python-engineio-4.4.1/README.rst
--rw-r--r--   0 mgrinberg   (502) staff       (20)      104 2021-06-07 19:39:18.000000 python-engineio-4.4.1/pyproject.toml
--rw-r--r--   0 mgrinberg   (502) staff       (20)      920 2023-04-19 15:21:32.149724 python-engineio-4.4.1/setup.cfg
--rw-r--r--   0 mgrinberg   (502) staff       (20)       38 2021-07-21 22:23:41.000000 python-engineio-4.4.1/setup.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-19 15:21:32.112815 python-engineio-4.4.1/src/
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-19 15:21:32.131685 python-engineio-4.4.1/src/engineio/
--rw-r--r--   0 mgrinberg   (502) staff       (20)      748 2021-11-30 15:30:22.000000 python-engineio-4.4.1/src/engineio/__init__.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-19 15:21:32.142337 python-engineio-4.4.1/src/engineio/async_drivers/
--rw-r--r--   0 mgrinberg   (502) staff       (20)        0 2019-11-17 19:17:59.000000 python-engineio-4.4.1/src/engineio/async_drivers/__init__.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     3746 2021-02-22 00:17:35.000000 python-engineio-4.4.1/src/engineio/async_drivers/aiohttp.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    10181 2022-08-02 18:37:30.000000 python-engineio-4.4.1/src/engineio/async_drivers/asgi.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)      981 2019-11-17 19:17:59.000000 python-engineio-4.4.1/src/engineio/async_drivers/eventlet.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1803 2023-03-21 23:31:31.000000 python-engineio-4.4.1/src/engineio/async_drivers/gevent.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5912 2023-02-02 11:35:37.000000 python-engineio-4.4.1/src/engineio/async_drivers/gevent_uwsgi.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     4468 2022-01-04 23:17:35.000000 python-engineio-4.4.1/src/engineio/async_drivers/sanic.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1154 2023-03-21 23:31:12.000000 python-engineio-4.4.1/src/engineio/async_drivers/threading.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5901 2021-02-22 00:17:35.000000 python-engineio-4.4.1/src/engineio/async_drivers/tornado.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    27033 2023-04-14 11:54:46.000000 python-engineio-4.4.1/src/engineio/asyncio_client.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    22691 2023-03-16 20:03:22.000000 python-engineio-4.4.1/src/engineio/asyncio_server.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    10248 2021-11-14 13:11:24.000000 python-engineio-4.4.1/src/engineio/asyncio_socket.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    30109 2023-04-14 11:54:46.000000 python-engineio-4.4.1/src/engineio/client.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)      292 2019-11-17 19:17:59.000000 python-engineio-4.4.1/src/engineio/exceptions.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)      405 2021-04-14 23:00:40.000000 python-engineio-4.4.1/src/engineio/json.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     3823 2021-07-26 22:32:50.000000 python-engineio-4.4.1/src/engineio/middleware.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2884 2022-05-29 14:42:07.000000 python-engineio-4.4.1/src/engineio/packet.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1547 2021-02-22 00:17:35.000000 python-engineio-4.4.1/src/engineio/payload.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    33757 2023-03-16 20:03:22.000000 python-engineio-4.4.1/src/engineio/server.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    10299 2021-11-14 13:11:24.000000 python-engineio-4.4.1/src/engineio/socket.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2064 2021-05-02 23:23:10.000000 python-engineio-4.4.1/src/engineio/static_files.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-19 15:21:32.147822 python-engineio-4.4.1/src/python_engineio.egg-info/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1976 2023-04-19 15:21:32.000000 python-engineio-4.4.1/src/python_engineio.egg-info/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1013 2023-04-19 15:21:32.000000 python-engineio-4.4.1/src/python_engineio.egg-info/SOURCES.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2023-04-19 15:21:32.000000 python-engineio-4.4.1/src/python_engineio.egg-info/dependency_links.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2021-06-07 19:44:43.000000 python-engineio-4.4.1/src/python_engineio.egg-info/not-zip-safe
--rw-r--r--   0 mgrinberg   (502) staff       (20)       83 2023-04-19 15:21:32.000000 python-engineio-4.4.1/src/python_engineio.egg-info/requires.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        9 2023-04-19 15:21:32.000000 python-engineio-4.4.1/src/python_engineio.egg-info/top_level.txt
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-05 12:30:15.801900 python-engineio-4.5.0/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1082 2023-06-13 09:40:52.000000 python-engineio-4.5.0/LICENSE
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       26 2023-06-13 09:40:52.000000 python-engineio-4.5.0/MANIFEST.in
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1997 2023-07-05 12:30:15.801900 python-engineio-4.5.0/PKG-INFO
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1288 2023-06-13 09:40:52.000000 python-engineio-4.5.0/README.md
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1012 2023-06-13 09:40:52.000000 python-engineio-4.5.0/README.rst
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      104 2023-06-13 09:40:52.000000 python-engineio-4.5.0/pyproject.toml
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      936 2023-07-05 12:30:15.801900 python-engineio-4.5.0/setup.cfg
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       38 2023-06-13 09:40:52.000000 python-engineio-4.5.0/setup.py
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-05 12:30:15.797899 python-engineio-4.5.0/src/
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-05 12:30:15.801900 python-engineio-4.5.0/src/engineio/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      747 2023-06-20 11:10:32.000000 python-engineio-4.5.0/src/engineio/__init__.py
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-05 12:30:15.801900 python-engineio-4.5.0/src/engineio/async_drivers/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        0 2023-06-13 09:40:52.000000 python-engineio-4.5.0/src/engineio/async_drivers/__init__.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     3768 2023-07-05 10:38:20.000000 python-engineio-4.5.0/src/engineio/async_drivers/aiohttp.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    10189 2023-07-05 10:38:20.000000 python-engineio-4.5.0/src/engineio/async_drivers/asgi.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1042 2023-07-05 11:02:37.000000 python-engineio-4.5.0/src/engineio/async_drivers/eventlet.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1807 2023-07-05 11:02:18.000000 python-engineio-4.5.0/src/engineio/async_drivers/gevent.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     5916 2023-07-05 11:02:48.000000 python-engineio-4.5.0/src/engineio/async_drivers/gevent_uwsgi.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     4476 2023-07-05 10:38:20.000000 python-engineio-4.5.0/src/engineio/async_drivers/sanic.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1170 2023-07-05 10:55:29.000000 python-engineio-4.5.0/src/engineio/async_drivers/threading.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     5909 2023-07-05 11:03:10.000000 python-engineio-4.5.0/src/engineio/async_drivers/tornado.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    27033 2023-06-13 09:40:52.000000 python-engineio-4.5.0/src/engineio/asyncio_client.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    22691 2023-06-13 09:40:52.000000 python-engineio-4.5.0/src/engineio/asyncio_server.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    10274 2023-07-05 10:50:32.000000 python-engineio-4.5.0/src/engineio/asyncio_socket.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    30109 2023-06-13 09:40:52.000000 python-engineio-4.5.0/src/engineio/client.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      292 2023-06-13 09:40:52.000000 python-engineio-4.5.0/src/engineio/exceptions.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      405 2023-06-13 09:40:52.000000 python-engineio-4.5.0/src/engineio/json.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     3766 2023-07-05 11:03:29.000000 python-engineio-4.5.0/src/engineio/middleware.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2884 2023-06-13 09:40:52.000000 python-engineio-4.5.0/src/engineio/packet.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1547 2023-06-13 09:40:52.000000 python-engineio-4.5.0/src/engineio/payload.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    33757 2023-06-13 09:40:52.000000 python-engineio-4.5.0/src/engineio/server.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    10325 2023-07-05 10:38:20.000000 python-engineio-4.5.0/src/engineio/socket.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2064 2023-06-13 09:40:52.000000 python-engineio-4.5.0/src/engineio/static_files.py
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-05 12:30:15.801900 python-engineio-4.5.0/src/python_engineio.egg-info/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1997 2023-07-05 12:30:15.000000 python-engineio-4.5.0/src/python_engineio.egg-info/PKG-INFO
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1013 2023-07-05 12:30:15.000000 python-engineio-4.5.0/src/python_engineio.egg-info/SOURCES.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        1 2023-07-05 12:30:15.000000 python-engineio-4.5.0/src/python_engineio.egg-info/dependency_links.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        1 2023-06-13 10:11:32.000000 python-engineio-4.5.0/src/python_engineio.egg-info/not-zip-safe
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       98 2023-07-05 12:30:15.000000 python-engineio-4.5.0/src/python_engineio.egg-info/requires.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        9 2023-07-05 12:30:15.000000 python-engineio-4.5.0/src/python_engineio.egg-info/top_level.txt
```

### Comparing `python-engineio-4.4.1/LICENSE` & `python-engineio-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.1/PKG-INFO` & `python-engineio-4.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: python-engineio
-Version: 4.4.1
+Version: 4.5.0
 Summary: Engine.IO server and client for Python
 Home-page: https://github.com/miguelgrinberg/python-engineio
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/python-engineio/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: client
 Provides-Extra: asyncio_client
+Provides-Extra: docs
 License-File: LICENSE
 
 python-engineio
 ===============
 
 [![Build status](https://github.com/miguelgrinberg/python-engineio/workflows/build/badge.svg)](https://github.com/miguelgrinberg/python-engineio/actions) [![codecov](https://codecov.io/gh/miguelgrinberg/python-engineio/branch/main/graph/badge.svg)](https://codecov.io/gh/miguelgrinberg/python-engineio)
```

### Comparing `python-engineio-4.4.1/README.md` & `python-engineio-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.1/README.rst` & `python-engineio-4.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.1/setup.cfg` & `python-engineio-4.5.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-engineio
-version = 4.4.1
+version = 4.5.0
 author = Miguel Grinberg
 author_email = miguel.grinberg@gmail.com
 description = Engine.IO server and client for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/miguelgrinberg/python-engineio
 project_urls = 
@@ -30,12 +30,14 @@
 
 [options.extras_require]
 client = 
 	requests >= 2.21.0
 	websocket-client >= 0.54.0
 asyncio_client = 
 	aiohttp >= 3.4
+docs = 
+	sphinx
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `python-engineio-4.4.1/src/engineio/__init__.py` & `python-engineio-4.5.0/src/engineio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     AsyncClient = None
     get_tornado_handler = None
     ASGIApp = None
 
 __all__ = ['Server', 'WSGIApp', 'Middleware', 'Client']
 if AsyncServer is not None:  # pragma: no cover
     __all__ += ['AsyncServer', 'ASGIApp', 'get_tornado_handler',
-                'AsyncClient'],
+                'AsyncClient']
```

### Comparing `python-engineio-4.4.1/src/engineio/async_drivers/aiohttp.py` & `python-engineio-4.5.0/src/engineio/async_drivers/aiohttp.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,21 +80,21 @@
 
 
 class WebSocket(object):  # pragma: no cover
     """
     This wrapper class provides a aiohttp WebSocket interface that is
     somewhat compatible with eventlet's implementation.
     """
-    def __init__(self, handler):
+    def __init__(self, handler, server):
         self.handler = handler
         self._sock = None
 
     async def __call__(self, environ):
         request = environ['aiohttp.request']
-        self._sock = WebSocketResponse()
+        self._sock = WebSocketResponse(max_msg_size=0)
         await self._sock.prepare(request)
 
         self.environ = environ
         await self.handler(self)
         return self._sock
 
     async def close(self):
```

### Comparing `python-engineio-4.4.1/src/engineio/async_drivers/asgi.py` & `python-engineio-4.5.0/src/engineio/async_drivers/asgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
 
 
 class WebSocket(object):  # pragma: no cover
     """
     This wrapper class provides an asgi WebSocket interface that is
     somewhat compatible with eventlet's implementation.
     """
-    def __init__(self, handler):
+    def __init__(self, handler, server):
         self.handler = handler
         self.asgi_receive = None
         self.asgi_send = None
 
     async def __call__(self, environ):
         self.asgi_receive = environ['asgi.receive']
         self.asgi_send = environ['asgi.send']
```

### Comparing `python-engineio-4.4.1/src/engineio/async_drivers/eventlet.py` & `python-engineio-4.5.0/src/engineio/async_drivers/eventlet.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 from eventlet.green.threading import Thread, Event
 from eventlet import queue
 from eventlet import sleep
 from eventlet.websocket import WebSocketWSGI as _WebSocketWSGI
 
 
 class WebSocketWSGI(_WebSocketWSGI):
-    def __init__(self, *args, **kwargs):
-        super(WebSocketWSGI, self).__init__(*args, **kwargs)
+    def __init__(self, handler, server):
+        print(server.max_http_buffer_size)
+        super().__init__(
+            handler, max_frame_length=int(server.max_http_buffer_size))
         self._sock = None
 
     def __call__(self, environ, start_response):
         if 'eventlet.input' not in environ:
             raise RuntimeError('You need to use the eventlet server. '
                                'See the Deployment section of the '
                                'documentation for more information.')
         self._sock = environ['eventlet.input'].get_socket()
-        return super(WebSocketWSGI, self).__call__(environ, start_response)
+        return super().__call__(environ, start_response)
 
 
 _async = {
     'thread': Thread,
     'queue': queue.Queue,
     'queue_empty': queue.Empty,
     'event': Event,
```

### Comparing `python-engineio-4.4.1/src/engineio/async_drivers/gevent.py` & `python-engineio-4.5.0/src/engineio/async_drivers/gevent.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 
 class Thread(gevent.Greenlet):  # pragma: no cover
     """
     This wrapper class provides gevent Greenlet interface that is compatible
     with the standard library's Thread class.
     """
     def __init__(self, target, args=[], kwargs={}):
-        super(Thread, self).__init__(target, *args, **kwargs)
+        super().__init__(target, *args, **kwargs)
 
     def _run(self):
         return self.run()
 
 
 class WebSocketWSGI(object):  # pragma: no cover
     """
     This wrapper class provides a gevent WebSocket interface that is
     compatible with eventlet's implementation.
     """
-    def __init__(self, app):
-        self.app = app
+    def __init__(self, handler, server):
+        self.app = handler
 
     def __call__(self, environ, start_response):
         if 'wsgi.websocket' not in environ:
             raise RuntimeError('You need to use the gevent-websocket server. '
                                'See the Deployment section of the '
                                'documentation for more information.')
         self._sock = environ['wsgi.websocket']
```

### Comparing `python-engineio-4.4.1/src/engineio/async_drivers/gevent_uwsgi.py` & `python-engineio-4.5.0/src/engineio/async_drivers/gevent_uwsgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 
 class Thread(gevent.Greenlet):  # pragma: no cover
     """
     This wrapper class provides gevent Greenlet interface that is compatible
     with the standard library's Thread class.
     """
     def __init__(self, target, args=[], kwargs={}):
-        super(Thread, self).__init__(target, *args, **kwargs)
+        super().__init__(target, *args, **kwargs)
 
     def _run(self):
         return self.run()
 
 
 class uWSGIWebSocket(object):  # pragma: no cover
     """
     This wrapper class provides a uWSGI WebSocket interface that is
     compatible with eventlet's implementation.
     """
-    def __init__(self, app):
-        self.app = app
+    def __init__(self, handler, server):
+        self.app = handler
         self._sock = None
         self.received_messages = []
 
     def __call__(self, environ, start_response):
         self._sock = uwsgi.connection_fd()
         self.environ = environ
```

### Comparing `python-engineio-4.4.1/src/engineio/async_drivers/sanic.py` & `python-engineio-4.5.0/src/engineio/async_drivers/sanic.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
 
 class WebSocket(object):  # pragma: no cover
     """
     This wrapper class provides a sanic WebSocket interface that is
     somewhat compatible with eventlet's implementation.
     """
-    def __init__(self, handler):
+    def __init__(self, handler, server):
         self.handler = handler
         self._sock = None
 
     async def __call__(self, environ):
         request = environ['sanic.request']
         protocol = request.transport.get_protocol()
         self._sock = await protocol.websocket_handshake(request)
```

### Comparing `python-engineio-4.4.1/src/engineio/async_drivers/threading.py` & `python-engineio-4.5.0/src/engineio/async_drivers/threading.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 
 class WebSocketWSGI(object):  # pragma: no cover
     """
     This wrapper class provides a threading WebSocket interface that is
     compatible with eventlet's implementation.
     """
-    def __init__(self, app):
-        self.app = app
+    def __init__(self, handler, server):
+        self.app = handler
 
     def __call__(self, environ, start_response):
         self.ws = Server(environ)
         return self.app(self)
 
     def close(self):
         return self.ws.close()
```

### Comparing `python-engineio-4.4.1/src/engineio/async_drivers/tornado.py` & `python-engineio-4.5.0/src/engineio/async_drivers/tornado.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 
 
 class WebSocket(object):  # pragma: no cover
     """
     This wrapper class provides a tornado WebSocket interface that is
     somewhat compatible with eventlet's implementation.
     """
-    def __init__(self, handler):
+    def __init__(self, handler, server):
         self.handler = handler
         self.tornado_handler = None
 
     async def __call__(self, environ):
         self.tornado_handler = environ['tornado.handler']
         self.environ = environ
         await self.handler(self)
```

### Comparing `python-engineio-4.4.1/src/engineio/asyncio_client.py` & `python-engineio-4.5.0/src/engineio/asyncio_client.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.1/src/engineio/asyncio_server.py` & `python-engineio-4.5.0/src/engineio/asyncio_server.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.1/src/engineio/asyncio_socket.py` & `python-engineio-4.5.0/src/engineio/asyncio_socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,16 @@
     async def _upgrade_websocket(self, environ):
         """Upgrade the connection from polling to websocket."""
         if self.upgraded:
             raise IOError('Socket has been upgraded already')
         if self.server._async['websocket'] is None:
             # the selected async mode does not support websocket
             return self.server._bad_request()
-        ws = self.server._async['websocket'](self._websocket_handler)
+        ws = self.server._async['websocket'](
+            self._websocket_handler, self.server)
         return await ws(environ)
 
     async def _websocket_handler(self, ws):
         """Engine.IO handler for websocket transport."""
         async def websocket_wait():
             data = await ws.wait()
             if data and len(data) > self.server.max_http_buffer_size:
```

### Comparing `python-engineio-4.4.1/src/engineio/client.py` & `python-engineio-4.5.0/src/engineio/client.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.1/src/engineio/middleware.py` & `python-engineio-4.5.0/src/engineio/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,9 +79,8 @@
         return [b'Not Found']
 
 
 class Middleware(WSGIApp):
     """This class has been renamed to ``WSGIApp`` and is now deprecated."""
     def __init__(self, engineio_app, wsgi_app=None,
                  engineio_path='engine.io'):
-        super(Middleware, self).__init__(engineio_app, wsgi_app,
-                                         engineio_path=engineio_path)
+        super().__init__(engineio_app, wsgi_app, engineio_path=engineio_path)
```

### Comparing `python-engineio-4.4.1/src/engineio/packet.py` & `python-engineio-4.5.0/src/engineio/packet.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.1/src/engineio/payload.py` & `python-engineio-4.5.0/src/engineio/payload.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.1/src/engineio/server.py` & `python-engineio-4.5.0/src/engineio/server.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.1/src/engineio/socket.py` & `python-engineio-4.5.0/src/engineio/socket.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,16 @@
     def _upgrade_websocket(self, environ, start_response):
         """Upgrade the connection from polling to websocket."""
         if self.upgraded:
             raise IOError('Socket has been upgraded already')
         if self.server._async['websocket'] is None:
             # the selected async mode does not support websocket
             return self.server._bad_request()
-        ws = self.server._async['websocket'](self._websocket_handler)
+        ws = self.server._async['websocket'](
+            self._websocket_handler, self.server)
         return ws(environ, start_response)
 
     def _websocket_handler(self, ws):
         """Engine.IO handler for websocket transport."""
         def websocket_wait():
             data = ws.wait()
             if data and len(data) > self.server.max_http_buffer_size:
```

### Comparing `python-engineio-4.4.1/src/engineio/static_files.py` & `python-engineio-4.5.0/src/engineio/static_files.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.1/src/python_engineio.egg-info/PKG-INFO` & `python-engineio-4.5.0/src/python_engineio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: python-engineio
-Version: 4.4.1
+Version: 4.5.0
 Summary: Engine.IO server and client for Python
 Home-page: https://github.com/miguelgrinberg/python-engineio
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/python-engineio/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: client
 Provides-Extra: asyncio_client
+Provides-Extra: docs
 License-File: LICENSE
 
 python-engineio
 ===============
 
 [![Build status](https://github.com/miguelgrinberg/python-engineio/workflows/build/badge.svg)](https://github.com/miguelgrinberg/python-engineio/actions) [![codecov](https://codecov.io/gh/miguelgrinberg/python-engineio/branch/main/graph/badge.svg)](https://codecov.io/gh/miguelgrinberg/python-engineio)
```

### Comparing `python-engineio-4.4.1/src/python_engineio.egg-info/SOURCES.txt` & `python-engineio-4.5.0/src/python_engineio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

