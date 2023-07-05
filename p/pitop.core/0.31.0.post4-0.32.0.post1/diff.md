# Comparing `tmp/pitop.core-0.31.0.post4.tar.gz` & `tmp/pitop.core-0.32.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitop.core-0.31.0.post4.tar", last modified: Tue Jun 13 18:30:06 2023, max compression
+gzip compressed data, was "dist/pitop.core-0.32.0.post1.tar", last modified: Wed Jul  5 13:37:06 2023, max compression
```

## Comparing `pitop.core-0.31.0.post4.tar` & `pitop.core-0.32.0.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:06.000000 pitop.core-0.31.0.post4/
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-13 18:29:44.000000 pitop.core-0.31.0.post4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-06-13 18:30:06.000000 pitop.core-0.31.0.post4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-13 18:29:44.000000 pitop.core-0.31.0.post4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:06.000000 pitop.core-0.31.0.post4/pitop/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:06.000000 pitop.core-0.31.0.post4/pitop/core/
--rw-r--r--   0 runner    (1001) docker     (122)     1663 2023-06-13 18:29:44.000000 pitop.core-0.31.0.post4/pitop/core/ImageFunctions.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 18:29:44.000000 pitop.core-0.31.0.post4/pitop/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-13 18:29:44.000000 pitop.core-0.31.0.post4/pitop/core/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-13 18:29:44.000000 pitop.core-0.31.0.post4/pitop/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      308 2023-06-13 18:29:44.000000 pitop.core-0.31.0.post4/pitop/core/import_opencv.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:06.000000 pitop.core-0.31.0.post4/pitop/core/mixins/
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-06-13 18:29:44.000000 pitop.core-0.31.0.post4/pitop/core/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3309 2023-06-13 18:29:44.000000 pitop.core-0.31.0.post4/pitop/core/mixins/componentable.py
--rw-r--r--   0 runner    (1001) docker     (122)     2737 2023-06-13 18:29:44.000000 pitop.core-0.31.0.post4/pitop/core/mixins/recreatable.py
--rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-06-13 18:29:44.000000 pitop.core-0.31.0.post4/pitop/core/mixins/stateful.py
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-06-13 18:29:44.000000 pitop.core-0.31.0.post4/pitop/core/mixins/supports_battery.py
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-06-13 18:29:44.000000 pitop.core-0.31.0.post4/pitop/core/mixins/supports_miniscreen.py
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-06-13 18:29:44.000000 pitop.core-0.31.0.post4/pitop/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:06.000000 pitop.core-0.31.0.post4/pitop.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-06-13 18:30:06.000000 pitop.core-0.31.0.post4/pitop.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-06-13 18:30:06.000000 pitop.core-0.31.0.post4/pitop.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 18:30:06.000000 pitop.core-0.31.0.post4/pitop.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-13 18:30:06.000000 pitop.core-0.31.0.post4/pitop.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-13 18:30:06.000000 pitop.core-0.31.0.post4/pitop.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 18:30:06.000000 pitop.core-0.31.0.post4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2034 2023-06-13 18:29:44.000000 pitop.core-0.31.0.post4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:06.000000 pitop.core-0.32.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-05 13:36:52.000000 pitop.core-0.32.0.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-07-05 13:37:06.000000 pitop.core-0.32.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-07-05 13:36:52.000000 pitop.core-0.32.0.post1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:06.000000 pitop.core-0.32.0.post1/pitop/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:06.000000 pitop.core-0.32.0.post1/pitop/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     1663 2023-07-05 13:36:52.000000 pitop.core-0.32.0.post1/pitop/core/ImageFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 13:36:52.000000 pitop.core-0.32.0.post1/pitop/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-07-05 13:36:52.000000 pitop.core-0.32.0.post1/pitop/core/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-05 13:36:52.000000 pitop.core-0.32.0.post1/pitop/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-07-05 13:36:52.000000 pitop.core-0.32.0.post1/pitop/core/import_opencv.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:06.000000 pitop.core-0.32.0.post1/pitop/core/mixins/
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-05 13:36:52.000000 pitop.core-0.32.0.post1/pitop/core/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3309 2023-07-05 13:36:52.000000 pitop.core-0.32.0.post1/pitop/core/mixins/componentable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2737 2023-07-05 13:36:52.000000 pitop.core-0.32.0.post1/pitop/core/mixins/recreatable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-07-05 13:36:52.000000 pitop.core-0.32.0.post1/pitop/core/mixins/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-05 13:36:52.000000 pitop.core-0.32.0.post1/pitop/core/mixins/supports_battery.py
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-07-05 13:36:52.000000 pitop.core-0.32.0.post1/pitop/core/mixins/supports_miniscreen.py
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-07-05 13:36:52.000000 pitop.core-0.32.0.post1/pitop/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:06.000000 pitop.core-0.32.0.post1/pitop.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-07-05 13:37:06.000000 pitop.core-0.32.0.post1/pitop.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-07-05 13:37:06.000000 pitop.core-0.32.0.post1/pitop.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 13:37:06.000000 pitop.core-0.32.0.post1/pitop.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-07-05 13:37:06.000000 pitop.core-0.32.0.post1/pitop.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-05 13:37:06.000000 pitop.core-0.32.0.post1/pitop.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-05 13:37:06.000000 pitop.core-0.32.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2034 2023-07-05 13:36:52.000000 pitop.core-0.32.0.post1/setup.py
```

### Comparing `pitop.core-0.31.0.post4/PKG-INFO` & `pitop.core-0.32.0.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.core
-Version: 0.31.0.post4
+Version: 0.32.0.post1
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Core
```

### Comparing `pitop.core-0.31.0.post4/pitop/core/ImageFunctions.py` & `pitop.core-0.32.0.post1/pitop/core/ImageFunctions.py`

 * *Files identical despite different names*

### Comparing `pitop.core-0.31.0.post4/pitop/core/mixins/componentable.py` & `pitop.core-0.32.0.post1/pitop/core/mixins/componentable.py`

 * *Files identical despite different names*

### Comparing `pitop.core-0.31.0.post4/pitop/core/mixins/recreatable.py` & `pitop.core-0.32.0.post1/pitop/core/mixins/recreatable.py`

 * *Files identical despite different names*

### Comparing `pitop.core-0.31.0.post4/pitop/core/mixins/stateful.py` & `pitop.core-0.32.0.post1/pitop/core/mixins/stateful.py`

 * *Files identical despite different names*

### Comparing `pitop.core-0.31.0.post4/pitop/core/mixins/supports_battery.py` & `pitop.core-0.32.0.post1/pitop/core/mixins/supports_battery.py`

 * *Files identical despite different names*

### Comparing `pitop.core-0.31.0.post4/pitop/core/mixins/supports_miniscreen.py` & `pitop.core-0.32.0.post1/pitop/core/mixins/supports_miniscreen.py`

 * *Files identical despite different names*

### Comparing `pitop.core-0.31.0.post4/pitop.core.egg-info/PKG-INFO` & `pitop.core-0.32.0.post1/pitop.core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.core
-Version: 0.31.0.post4
+Version: 0.32.0.post1
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Core
```

### Comparing `pitop.core-0.31.0.post4/pitop.core.egg-info/SOURCES.txt` & `pitop.core-0.32.0.post1/pitop.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pitop.core-0.31.0.post4/setup.py` & `pitop.core-0.32.0.post1/setup.py`

 * *Files identical despite different names*

