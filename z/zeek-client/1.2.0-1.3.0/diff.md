# Comparing `tmp/zeek-client-1.2.0.tar.gz` & `tmp/zeek-client-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeek-client-1.2.0.tar", last modified: Wed Feb  1 22:23:52 2023, max compression
+gzip compressed data, was "zeek-client-1.3.0.tar", last modified: Wed Jul  5 17:15:23 2023, max compression
```

## Comparing `zeek-client-1.2.0.tar` & `zeek-client-1.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 22:23:52.238633 zeek-client-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-02-01 22:23:49.000000 zeek-client-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-01 22:23:49.000000 zeek-client-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-02-01 22:23:52.238633 zeek-client-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-02-01 22:23:49.000000 zeek-client-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-01 22:23:49.000000 zeek-client-1.2.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-01 22:23:52.238633 zeek-client-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-02-01 22:23:49.000000 zeek-client-1.2.0/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2057 2023-02-01 22:23:49.000000 zeek-client-1.2.0/zeek-client
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 22:23:52.238633 zeek-client-1.2.0/zeek_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-02-01 22:23:52.000000 zeek-client-1.2.0/zeek_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-02-01 22:23:52.000000 zeek-client-1.2.0/zeek_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 22:23:52.000000 zeek-client-1.2.0/zeek_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-01 22:23:52.000000 zeek-client-1.2.0/zeek_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-01 22:23:52.000000 zeek-client-1.2.0/zeek_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 22:23:52.238633 zeek-client-1.2.0/zeekclient/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-02-01 22:23:49.000000 zeek-client-1.2.0/zeekclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34883 2023-02-01 22:23:49.000000 zeek-client-1.2.0/zeekclient/brokertypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    22038 2023-02-01 22:23:49.000000 zeek-client-1.2.0/zeekclient/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-02-01 22:23:49.000000 zeek-client-1.2.0/zeekclient/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-01 22:23:49.000000 zeek-client-1.2.0/zeekclient/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-02-01 22:23:49.000000 zeek-client-1.2.0/zeekclient/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-02-01 22:23:49.000000 zeek-client-1.2.0/zeekclient/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-02-01 22:23:49.000000 zeek-client-1.2.0/zeekclient/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-02-01 22:23:49.000000 zeek-client-1.2.0/zeekclient/ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    29929 2023-02-01 22:23:49.000000 zeek-client-1.2.0/zeekclient/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-02-01 22:23:49.000000 zeek-client-1.2.0/zeekclient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:15:23.225946 zeek-client-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-05 17:15:22.000000 zeek-client-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-05 17:15:22.000000 zeek-client-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-05 17:15:23.225946 zeek-client-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-07-05 17:15:22.000000 zeek-client-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 17:15:22.000000 zeek-client-1.3.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 17:15:23.225946 zeek-client-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-05 17:15:22.000000 zeek-client-1.3.0/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2057 2023-07-05 17:15:22.000000 zeek-client-1.3.0/zeek-client
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:15:23.221946 zeek-client-1.3.0/zeek_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-05 17:15:23.000000 zeek-client-1.3.0/zeek_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-05 17:15:23.000000 zeek-client-1.3.0/zeek_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 17:15:23.000000 zeek-client-1.3.0/zeek_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 17:15:23.000000 zeek-client-1.3.0/zeek_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 17:15:23.000000 zeek-client-1.3.0/zeek_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:15:23.225946 zeek-client-1.3.0/zeekclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-05 17:15:22.000000 zeek-client-1.3.0/zeekclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34917 2023-07-05 17:15:22.000000 zeek-client-1.3.0/zeekclient/brokertypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22038 2023-07-05 17:15:22.000000 zeek-client-1.3.0/zeekclient/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-05 17:15:22.000000 zeek-client-1.3.0/zeekclient/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-05 17:15:22.000000 zeek-client-1.3.0/zeekclient/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-07-05 17:15:22.000000 zeek-client-1.3.0/zeekclient/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-07-05 17:15:22.000000 zeek-client-1.3.0/zeekclient/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-05 17:15:22.000000 zeek-client-1.3.0/zeekclient/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-07-05 17:15:22.000000 zeek-client-1.3.0/zeekclient/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29929 2023-07-05 17:15:22.000000 zeek-client-1.3.0/zeekclient/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-05 17:15:22.000000 zeek-client-1.3.0/zeekclient/utils.py
```

### Comparing `zeek-client-1.2.0/LICENSE` & `zeek-client-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zeek-client-1.2.0/PKG-INFO` & `zeek-client-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeek-client
-Version: 1.2.0
+Version: 1.3.0
 Summary: A CLI for Zeek's Management Framework
 Home-page: https://github.com/zeek/zeek-client
 Maintainer: The Zeek Project
 Maintainer-email: info@zeek.org
 License: 3-clause BSD License
 Keywords: zeek management client cluster
 Platform: UNKNOWN
```

### Comparing `zeek-client-1.2.0/README.md` & `zeek-client-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `zeek-client-1.2.0/setup.py` & `zeek-client-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `zeek-client-1.2.0/zeek-client` & `zeek-client-1.3.0/zeek-client`

 * *Files identical despite different names*

### Comparing `zeek-client-1.2.0/zeek_client.egg-info/PKG-INFO` & `zeek-client-1.3.0/zeek_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeek-client
-Version: 1.2.0
+Version: 1.3.0
 Summary: A CLI for Zeek's Management Framework
 Home-page: https://github.com/zeek/zeek-client
 Maintainer: The Zeek Project
 Maintainer-email: info@zeek.org
 License: 3-clause BSD License
 Keywords: zeek management client cluster
 Platform: UNKNOWN
```

### Comparing `zeek-client-1.2.0/zeekclient/__init__.py` & `zeek-client-1.3.0/zeekclient/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,10 +22,10 @@
 from .consts import (
     CONTROLLER_TOPIC,
     CONFIG_FILE,
 )
 
 from .logs import LOG
 
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 __all__ = ['brokertypes', 'cli', 'config', 'consts', 'controller', 'events',
            'logs', 'ssl', 'types', 'utils']
```

### Comparing `zeek-client-1.2.0/zeekclient/brokertypes.py` & `zeek-client-1.3.0/zeekclient/brokertypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -813,23 +813,26 @@
 
     @classmethod
     def from_vector(cls, vec):
         """Special case for an existing Vector instance: recast as Zeek event."""
         if not isinstance(vec, Vector):
             raise TypeError('cannot convert non-vector to Zeek event')
 
-        if (not len(vec) == 3 or
+        if (len(vec) < 3 or
             not isinstance(vec[2], Vector) or
-            not len(vec[2]) == 2 or
+            len(vec[2]) < 2 or
             not isinstance(vec[2][0], String) or
             not isinstance(vec[2][1], Vector)):
             raise TypeError('invalid vector layout for Zeek event')
 
         name = vec[2][0].to_py()
         args = vec[2][1]
+
+        # TODO: Extend to handle metadata
+
         return ZeekEvent(name, *args._elements)
 
     @classmethod
     def from_broker(cls, data):
         name = data['data'][2]['data'][0]['data']
         res = ZeekEvent(name)
         for argdata in data['data'][2]['data'][1]['data']:
```

### Comparing `zeek-client-1.2.0/zeekclient/cli.py` & `zeek-client-1.3.0/zeekclient/cli.py`

 * *Files identical despite different names*

### Comparing `zeek-client-1.2.0/zeekclient/config.py` & `zeek-client-1.3.0/zeekclient/config.py`

 * *Files identical despite different names*

### Comparing `zeek-client-1.2.0/zeekclient/controller.py` & `zeek-client-1.3.0/zeekclient/controller.py`

 * *Files identical despite different names*

### Comparing `zeek-client-1.2.0/zeekclient/events.py` & `zeek-client-1.3.0/zeekclient/events.py`

 * *Files identical despite different names*

### Comparing `zeek-client-1.2.0/zeekclient/logs.py` & `zeek-client-1.3.0/zeekclient/logs.py`

 * *Files identical despite different names*

### Comparing `zeek-client-1.2.0/zeekclient/ssl.py` & `zeek-client-1.3.0/zeekclient/ssl.py`

 * *Files identical despite different names*

### Comparing `zeek-client-1.2.0/zeekclient/types.py` & `zeek-client-1.3.0/zeekclient/types.py`

 * *Files identical despite different names*

