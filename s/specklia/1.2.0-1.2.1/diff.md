# Comparing `tmp/specklia-1.2.0.tar.gz` & `tmp/specklia-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specklia-1.2.0.tar", last modified: Fri Jun 30 15:16:51 2023, max compression
+gzip compressed data, was "specklia-1.2.1.tar", last modified: Wed Jul  5 09:35:17 2023, max compression
```

## Comparing `specklia-1.2.0.tar` & `specklia-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:16:51.493293 specklia-1.2.0/
--rw-r--r--   0 root         (0) root         (0)     1061 2023-06-30 13:03:23.000000 specklia-1.2.0/LICENCE
--rw-r--r--   0 root         (0) root         (0)     2711 2023-06-30 15:16:51.493293 specklia-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1603 2023-06-30 13:03:23.000000 specklia-1.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)      484 2023-06-30 15:16:51.493293 specklia-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2364 2023-06-30 13:03:23.000000 specklia-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:16:51.493293 specklia-1.2.0/specklia/
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-30 13:03:23.000000 specklia-1.2.0/specklia/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3250 2023-06-30 13:03:23.000000 specklia-1.2.0/specklia/_websocket_helpers.py
--rw-r--r--   0 root         (0) root         (0)    35189 2023-06-30 13:03:23.000000 specklia-1.2.0/specklia/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:16:51.493293 specklia-1.2.0/specklia.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2711 2023-06-30 15:16:51.000000 specklia-1.2.0/specklia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      319 2023-06-30 15:16:51.000000 specklia-1.2.0/specklia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 15:16:51.000000 specklia-1.2.0/specklia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-30 15:16:51.000000 specklia-1.2.0/specklia.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-30 15:16:51.000000 specklia-1.2.0/specklia.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:16:51.493293 specklia-1.2.0/tests/
--rw-r--r--   0 root         (0) root         (0)    10184 2023-06-30 13:03:23.000000 specklia-1.2.0/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)     6632 2023-06-30 13:03:23.000000 specklia-1.2.0/tests/test_websocket_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 09:35:17.003114 specklia-1.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-07-04 23:08:53.000000 specklia-1.2.1/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-07-05 09:35:17.003114 specklia-1.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-07-04 23:08:53.000000 specklia-1.2.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      484 2023-07-05 09:35:17.007114 specklia-1.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-07-04 23:08:53.000000 specklia-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 09:35:17.003114 specklia-1.2.1/specklia/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-07-04 23:08:53.000000 specklia-1.2.1/specklia/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2023-07-04 23:08:53.000000 specklia-1.2.1/specklia/_websocket_helpers.py
+-rw-r--r--   0 root         (0) root         (0)    35189 2023-07-04 23:08:53.000000 specklia-1.2.1/specklia/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 09:35:17.003114 specklia-1.2.1/specklia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-07-05 09:35:16.000000 specklia-1.2.1/specklia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      319 2023-07-05 09:35:16.000000 specklia-1.2.1/specklia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 09:35:16.000000 specklia-1.2.1/specklia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-05 09:35:16.000000 specklia-1.2.1/specklia.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-05 09:35:16.000000 specklia-1.2.1/specklia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 09:35:17.003114 specklia-1.2.1/tests/
+-rw-r--r--   0 root         (0) root         (0)    10184 2023-07-04 23:08:53.000000 specklia-1.2.1/tests/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     6632 2023-07-04 23:08:53.000000 specklia-1.2.1/tests/test_websocket_helpers.py
```

### Comparing `specklia-1.2.0/LICENCE` & `specklia-1.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `specklia-1.2.0/PKG-INFO` & `specklia-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/static/docs/index.html
 Author: Earthwave Ltd
 Author-email: support@earthwave.co.uk
 License: MIT
 Project-URL: Homepage, https://specklia.earthwave.co.uk/static/docs/index.html
 Project-URL: Changelog, https://specklia.earthwave.co.uk/static/docs/changelog.html
```

### Comparing `specklia-1.2.0/README.md` & `specklia-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `specklia-1.2.0/setup.py` & `specklia-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `specklia-1.2.0/specklia/_websocket_helpers.py` & `specklia-1.2.1/specklia/_websocket_helpers.py`

 * *Files identical despite different names*

### Comparing `specklia-1.2.0/specklia/client.py` & `specklia-1.2.1/specklia/client.py`

 * *Files identical despite different names*

### Comparing `specklia-1.2.0/specklia.egg-info/PKG-INFO` & `specklia-1.2.1/specklia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/static/docs/index.html
 Author: Earthwave Ltd
 Author-email: support@earthwave.co.uk
 License: MIT
 Project-URL: Homepage, https://specklia.earthwave.co.uk/static/docs/index.html
 Project-URL: Changelog, https://specklia.earthwave.co.uk/static/docs/changelog.html
```

### Comparing `specklia-1.2.0/tests/test_client.py` & `specklia-1.2.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `specklia-1.2.0/tests/test_websocket_helpers.py` & `specklia-1.2.1/tests/test_websocket_helpers.py`

 * *Files identical despite different names*

