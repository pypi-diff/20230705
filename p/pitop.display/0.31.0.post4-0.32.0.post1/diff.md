# Comparing `tmp/pitop.display-0.31.0.post4.tar.gz` & `tmp/pitop.display-0.32.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitop.display-0.31.0.post4.tar", last modified: Tue Jun 13 18:30:07 2023, max compression
+gzip compressed data, was "dist/pitop.display-0.32.0.post1.tar", last modified: Wed Jul  5 13:37:06 2023, max compression
```

## Comparing `pitop.display-0.31.0.post4.tar` & `pitop.display-0.32.0.post1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:07.000000 pitop.display-0.31.0.post4/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-06-13 18:29:44.000000 pitop.display-0.31.0.post4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-06-13 18:30:07.000000 pitop.display-0.31.0.post4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-06-13 18:29:44.000000 pitop.display-0.31.0.post4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:07.000000 pitop.display-0.31.0.post4/pitop/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:07.000000 pitop.display-0.31.0.post4/pitop/display/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-13 18:29:44.000000 pitop.display-0.31.0.post4/pitop/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5417 2023-06-13 18:29:44.000000 pitop.display-0.31.0.post4/pitop/display/display.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:07.000000 pitop.display-0.31.0.post4/pitop.display.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-06-13 18:30:07.000000 pitop.display-0.31.0.post4/pitop.display.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      266 2023-06-13 18:30:07.000000 pitop.display-0.31.0.post4/pitop.display.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 18:30:07.000000 pitop.display-0.31.0.post4/pitop.display.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-13 18:30:07.000000 pitop.display-0.31.0.post4/pitop.display.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-13 18:30:07.000000 pitop.display-0.31.0.post4/pitop.display.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 18:30:07.000000 pitop.display-0.31.0.post4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1952 2023-06-13 18:29:44.000000 pitop.display-0.31.0.post4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:06.000000 pitop.display-0.32.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-07-05 13:36:52.000000 pitop.display-0.32.0.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-05 13:37:06.000000 pitop.display-0.32.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-05 13:36:52.000000 pitop.display-0.32.0.post1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:06.000000 pitop.display-0.32.0.post1/pitop/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:06.000000 pitop.display-0.32.0.post1/pitop/display/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-05 13:36:52.000000 pitop.display-0.32.0.post1/pitop/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5417 2023-07-05 13:36:52.000000 pitop.display-0.32.0.post1/pitop/display/display.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:06.000000 pitop.display-0.32.0.post1/pitop.display.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-05 13:37:06.000000 pitop.display-0.32.0.post1/pitop.display.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-07-05 13:37:06.000000 pitop.display-0.32.0.post1/pitop.display.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 13:37:06.000000 pitop.display-0.32.0.post1/pitop.display.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-05 13:37:06.000000 pitop.display-0.32.0.post1/pitop.display.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-05 13:37:06.000000 pitop.display-0.32.0.post1/pitop.display.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-05 13:37:06.000000 pitop.display-0.32.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1952 2023-07-05 13:36:52.000000 pitop.display-0.32.0.post1/setup.py
```

### Comparing `pitop.display-0.31.0.post4/PKG-INFO` & `pitop.display-0.32.0.post1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.display
-Version: 0.31.0.post4
+Version: 0.32.0.post1
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Display
```

### Comparing `pitop.display-0.31.0.post4/pitop/display/display.py` & `pitop.display-0.32.0.post1/pitop/display/display.py`

 * *Files identical despite different names*

### Comparing `pitop.display-0.31.0.post4/pitop.display.egg-info/PKG-INFO` & `pitop.display-0.32.0.post1/pitop.display.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.display
-Version: 0.31.0.post4
+Version: 0.32.0.post1
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Display
```

### Comparing `pitop.display-0.31.0.post4/setup.py` & `pitop.display-0.32.0.post1/setup.py`

 * *Files identical despite different names*

