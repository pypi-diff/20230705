# Comparing `tmp/asyncore-wsgi-0.0.6.tar.gz` & `tmp/asyncore-wsgi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/asyncore-wsgi-0.0.6.tar", last modified: Thu Aug  9 09:04:47 2018, max compression
+gzip compressed data, was "dist/asyncore-wsgi-0.0.9.tar", last modified: Tue Dec 11 18:40:31 2018, max compression
```

## Comparing `asyncore-wsgi-0.0.6.tar` & `asyncore-wsgi-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2018-08-09 09:04:47.000000 asyncore-wsgi-0.0.6/
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2018-08-09 09:04:47.000000 asyncore-wsgi-0.0.6/asyncore_wsgi.egg-info/
--rwxrwxrwx   0 roman     (1000) roman     (1000)       14 2018-08-09 09:04:46.000000 asyncore-wsgi-0.0.6/asyncore_wsgi.egg-info/top_level.txt
--rwxrwxrwx   0 roman     (1000) roman     (1000)      267 2018-08-09 09:04:47.000000 asyncore-wsgi-0.0.6/asyncore_wsgi.egg-info/SOURCES.txt
--rwxrwxrwx   0 roman     (1000) roman     (1000)        1 2018-03-15 20:38:08.000000 asyncore-wsgi-0.0.6/asyncore_wsgi.egg-info/not-zip-safe
--rwxrwxrwx   0 roman     (1000) roman     (1000)     2287 2018-08-09 09:04:46.000000 asyncore-wsgi-0.0.6/asyncore_wsgi.egg-info/PKG-INFO
--rwxrwxrwx   0 roman     (1000) roman     (1000)        1 2018-08-09 09:04:46.000000 asyncore-wsgi-0.0.6/asyncore_wsgi.egg-info/dependency_links.txt
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2018-08-09 09:04:47.000000 asyncore-wsgi-0.0.6/asyncore_wsgi/
--rw-rw-r--   0 roman     (1000) roman     (1000)    19501 2018-08-01 21:11:10.000000 asyncore-wsgi-0.0.6/asyncore_wsgi/SimpleWebSocketServer.py
--rw-rw-r--   0 roman     (1000) roman     (1000)    11841 2018-08-09 07:43:59.000000 asyncore-wsgi-0.0.6/asyncore_wsgi/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)       67 2018-08-09 09:04:47.000000 asyncore-wsgi-0.0.6/setup.cfg
--rw-rw-r--   0 roman     (1000) roman     (1000)     2287 2018-08-09 09:04:47.000000 asyncore-wsgi-0.0.6/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)     1264 2018-07-26 15:34:55.000000 asyncore-wsgi-0.0.6/setup.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2018-12-11 18:40:31.000000 asyncore-wsgi-0.0.9/
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1264 2018-12-11 18:28:55.000000 asyncore-wsgi-0.0.9/setup.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)       67 2018-12-11 18:40:31.000000 asyncore-wsgi-0.0.9/setup.cfg
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2018-12-11 18:40:31.000000 asyncore-wsgi-0.0.9/asyncore_wsgi.egg-info/
+-rwxrwxrwx   0 roman     (1000) roman     (1000)        1 2018-12-11 18:40:31.000000 asyncore-wsgi-0.0.9/asyncore_wsgi.egg-info/dependency_links.txt
+-rwxrwxrwx   0 roman     (1000) roman     (1000)        1 2018-03-15 20:38:08.000000 asyncore-wsgi-0.0.9/asyncore_wsgi.egg-info/not-zip-safe
+-rwxrwxrwx   0 roman     (1000) roman     (1000)     2287 2018-12-11 18:40:31.000000 asyncore-wsgi-0.0.9/asyncore_wsgi.egg-info/PKG-INFO
+-rwxrwxrwx   0 roman     (1000) roman     (1000)       14 2018-12-11 18:40:31.000000 asyncore-wsgi-0.0.9/asyncore_wsgi.egg-info/top_level.txt
+-rwxrwxrwx   0 roman     (1000) roman     (1000)      302 2018-12-11 18:40:31.000000 asyncore-wsgi-0.0.9/asyncore_wsgi.egg-info/SOURCES.txt
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2018-12-11 18:40:31.000000 asyncore-wsgi-0.0.9/asyncore_wsgi/
+-rw-rw-r--   0 roman     (1000) roman     (1000)    19501 2018-12-11 18:28:55.000000 asyncore-wsgi-0.0.9/asyncore_wsgi/SimpleWebSocketServer.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)    12220 2018-12-11 18:39:48.000000 asyncore-wsgi-0.0.9/asyncore_wsgi/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     2287 2018-12-11 18:40:31.000000 asyncore-wsgi-0.0.9/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1116 2018-12-11 18:28:55.000000 asyncore-wsgi-0.0.9/Readme.rst
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1086 2018-12-11 18:28:55.000000 asyncore-wsgi-0.0.9/LICENSE.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)       20 2018-12-11 18:39:48.000000 asyncore-wsgi-0.0.9/MANIFEST.in
```

### Comparing `asyncore-wsgi-0.0.6/asyncore_wsgi.egg-info/PKG-INFO` & `asyncore-wsgi-0.0.9/asyncore_wsgi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: asyncore-wsgi
-Version: 0.0.6
+Version: 0.0.9
 Summary: Asynchronous WSGI and WebSocket server based on asyncore module
 Home-page: https://github.com/romanvm/asyncore-wsgi
 Author: Roman Miroshnychenko
 Author-email: roman1972@gmail.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: asyncore-wsgi
```

### Comparing `asyncore-wsgi-0.0.6/asyncore_wsgi/SimpleWebSocketServer.py` & `asyncore-wsgi-0.0.9/asyncore_wsgi/SimpleWebSocketServer.py`

 * *Files identical despite different names*

### Comparing `asyncore-wsgi-0.0.6/asyncore_wsgi/__init__.py` & `asyncore-wsgi-0.0.9/asyncore_wsgi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,45 +32,53 @@
 """
 
 from __future__ import absolute_import
 import asyncore
 import logging
 import select
 import socket
+import sys
 from errno import EINTR
 from io import BytesIO
 from shutil import copyfileobj
 from tempfile import TemporaryFile
 from wsgiref.simple_server import WSGIServer, ServerHandler, WSGIRequestHandler
 from .SimpleWebSocketServer import AsyncWebSocketHandler
 
 __all__ = ['AsyncWsgiHandler', 'AsyncWebSocketHandler', 'AsyncWsgiServer',
             'make_server']
 
-__version__ = '0.0.6'
+__version__ = '0.0.9'
 
 logging.basicConfig(
     format='%(asctime)s: %(name)s - %(module)s:%(lineno)d - %(levelname)s - %(message)s',
     level=logging.DEBUG
 )
 logger = logging.getLogger('asyncore_wsgi')
 
 
+def iteritems(dct):
+    """Get iterator for dict items"""
+    if sys.version_info[0] == 2:
+        return dct.iteritems()
+    return dct.items()
+
+
 def epoll_poller(timeout=0.0, map=None):
     """
     A poller which uses epoll(), supported on Linux 2.5.44 and newer
 
     Borrowed from here:
     https://github.com/m13253/python-asyncore-epoll/blob/master/asyncore_epoll.py#L200
     """
     if map is None:
         map = asyncore.socket_map
     pollster = select.epoll()
     if map:
-        for fd, obj in map.items():
+        for fd, obj in iteritems(map):
             flags = 0
             if obj.readable():
                 flags |= select.POLLIN | select.POLLPRI
             if obj.writable():
                 flags |= select.POLLOUT
             if flags:
                 # Only check for exceptions if object was either readable
@@ -124,22 +132,22 @@
 class AsyncWsgiHandler(asyncore.dispatcher, WSGIRequestHandler):
     """
     Asynchronous WSGI request handler with optional WebSocket support
 
     If ``ws_handler_class`` is set, a request to ``ws_path` is
     upgraded to WebSocket protocol.
     """
-    accepting = False
     server_version = 'AsyncWsgiServer/' + __version__
     protocol_version = 'HTTP/1.1'
     max_input_content_length = 1024 * 1024 * 1024
     max_input_in_memory = 16 * 1024
     ws_path = '/ws'
     ws_handler_class = None
     verbose_logging = False
+    pratchett_tribute = True
 
     def __init__(self, request, client_address, server, map):
         self._can_read = True
         self._can_write = False
         self._server_handler = None
         self._transfer_chunked = False
         self.request = request
@@ -207,14 +215,17 @@
             self._server_handler.run(self.server.get_app())
         except Exception:
             self.handle_error()
         else:
             if 'Content-Length' not in self._server_handler.headers:
                 self._transfer_chunked = True
                 self._server_handler.headers['Transfer-Encoding'] = 'chunked'
+            if (self.pratchett_tribute and
+                    'X-Clacks-Overhead' not in self._server_handler.headers):
+                self._server_handler.headers['X-Clacks-Overhead'] = 'GNU Terry Pratchett'
             self._can_write = True
 
     def handle_write(self):
         self._can_write = False
         try:
             chunk = next(self._server_handler.iterator)
             if self._transfer_chunked:
```

### Comparing `asyncore-wsgi-0.0.6/PKG-INFO` & `asyncore-wsgi-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: asyncore-wsgi
-Version: 0.0.6
+Version: 0.0.9
 Summary: Asynchronous WSGI and WebSocket server based on asyncore module
 Home-page: https://github.com/romanvm/asyncore-wsgi
 Author: Roman Miroshnychenko
 Author-email: roman1972@gmail.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: asyncore-wsgi
```

### Comparing `asyncore-wsgi-0.0.6/setup.py` & `asyncore-wsgi-0.0.9/setup.py`

 * *Files identical despite different names*

