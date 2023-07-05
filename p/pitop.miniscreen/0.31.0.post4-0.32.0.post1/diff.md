# Comparing `tmp/pitop.miniscreen-0.31.0.post4.tar.gz` & `tmp/pitop.miniscreen-0.32.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitop.miniscreen-0.31.0.post4.tar", last modified: Tue Jun 13 18:30:07 2023, max compression
+gzip compressed data, was "dist/pitop.miniscreen-0.32.0.post1.tar", last modified: Wed Jul  5 13:37:07 2023, max compression
```

## Comparing `pitop.miniscreen-0.31.0.post4.tar` & `pitop.miniscreen-0.32.0.post1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:07.000000 pitop.miniscreen-0.31.0.post4/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      966 2023-06-13 18:30:07.000000 pitop.miniscreen-0.31.0.post4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:07.000000 pitop.miniscreen-0.31.0.post4/pitop/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:07.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:07.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/buttons/
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/buttons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4448 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/buttons/buttons.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:07.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/images/
--rw-r--r--   0 runner    (1001) docker     (122)    80224 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/images/rocket.gif
--rw-r--r--   0 runner    (1001) docker     (122)     5895 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/miniscreen.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:07.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7871 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:07.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15619 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/canvas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:07.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:07.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/
--rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:07.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      237 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/core/const.py
--rw-r--r--   0 runner    (1001) docker     (122)     2641 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/core/device.py
--rw-r--r--   0 runner    (1001) docker     (122)      640 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/core/error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:07.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/core/interface/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/core/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7433 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/core/interface/serial.py
--rw-r--r--   0 runner    (1001) docker     (122)     2407 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/core/mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     1258 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/core/threadpool.py
--rw-r--r--   0 runner    (1001) docker     (122)     7044 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/core/virtual.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:07.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/oled/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/oled/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/oled/const.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:07.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/oled/device/
--rw-r--r--   0 runner    (1001) docker     (122)     3432 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/oled/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3980 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/device_controller.py
--rw-r--r--   0 runner    (1001) docker     (122)     3387 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/fps_regulator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/lock.py
--rw-r--r--   0 runner    (1001) docker     (122)    22475 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/oled.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:07.000000 pitop.miniscreen-0.31.0.post4/pitop.miniscreen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      966 2023-06-13 18:30:07.000000 pitop.miniscreen-0.31.0.post4/pitop.miniscreen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-06-13 18:30:07.000000 pitop.miniscreen-0.31.0.post4/pitop.miniscreen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 18:30:07.000000 pitop.miniscreen-0.31.0.post4/pitop.miniscreen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      145 2023-06-13 18:30:07.000000 pitop.miniscreen-0.31.0.post4/pitop.miniscreen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-13 18:30:07.000000 pitop.miniscreen-0.31.0.post4/pitop.miniscreen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 18:30:07.000000 pitop.miniscreen-0.31.0.post4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2128 2023-06-13 18:29:44.000000 pitop.miniscreen-0.31.0.post4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:07.000000 pitop.miniscreen-0.32.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      966 2023-07-05 13:37:07.000000 pitop.miniscreen-0.32.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:07.000000 pitop.miniscreen-0.32.0.post1/pitop/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:07.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:07.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/buttons/
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/buttons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/buttons/buttons.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:07.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/images/
+-rw-r--r--   0 runner    (1001) docker     (122)    80224 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/images/rocket.gif
+-rw-r--r--   0 runner    (1001) docker     (122)     9099 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/miniscreen.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:07.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7871 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:07.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15619 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/canvas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:07.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:07.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/
+-rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:07.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/const.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2641 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/device.py
+-rw-r--r--   0 runner    (1001) docker     (122)      640 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:07.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/interface/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7433 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/interface/serial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2407 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1258 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/threadpool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7044 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/virtual.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:07.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/oled/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/oled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/oled/const.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:07.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/oled/device/
+-rw-r--r--   0 runner    (1001) docker     (122)     3432 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/oled/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3607 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/device_controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3387 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/fps_regulator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19626 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/oled.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:07.000000 pitop.miniscreen-0.32.0.post1/pitop.miniscreen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      966 2023-07-05 13:37:07.000000 pitop.miniscreen-0.32.0.post1/pitop.miniscreen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-07-05 13:37:07.000000 pitop.miniscreen-0.32.0.post1/pitop.miniscreen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 13:37:07.000000 pitop.miniscreen-0.32.0.post1/pitop.miniscreen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-07-05 13:37:07.000000 pitop.miniscreen-0.32.0.post1/pitop.miniscreen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-05 13:37:07.000000 pitop.miniscreen-0.32.0.post1/pitop.miniscreen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-05 13:37:07.000000 pitop.miniscreen-0.32.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2128 2023-07-05 13:36:52.000000 pitop.miniscreen-0.32.0.post1/setup.py
```

### Comparing `pitop.miniscreen-0.31.0.post4/PKG-INFO` & `pitop.miniscreen-0.32.0.post1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.miniscreen
-Version: 0.31.0.post4
+Version: 0.32.0.post1
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Miniscreen
```

### Comparing `pitop.miniscreen-0.31.0.post4/pitop/miniscreen/buttons/buttons.py` & `pitop.miniscreen-0.32.0.post1/pitop/miniscreen/buttons/buttons.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import atexit
-from os import getenv
 
-from pitop.common.lock import PTLock
 from pitop.common.ptdm import Message, PTDMSubscribeClient
 from pitop.common.singleton import Singleton
 from pitop.miniscreen import MiniscreenButton
 
 
 class MiniscreenButtonLegacy(MiniscreenButton):
     def __init__(self, button_type):
@@ -32,27 +30,14 @@
         self.cancel = MiniscreenButtonLegacy(self.CANCEL)
 
         self.__ptdm_subscribe_client = None
         self.__setup_subscribe_client()
 
         atexit.register(self.__clean_up)
 
-        self.lock = PTLock("pt-buttons")
-
-        if getenv("PT_MINISCREEN_SYSTEM", "0") != "1":
-            self.lock.acquire()
-
-    @property
-    def is_active(self):
-        """Determine if the current instance is in control of the buttons.
-
-        :rtype: bool
-        """
-        return self.lock.is_locked()
-
     def __setup_subscribe_client(self):
         def set_button_state(button, pressed):
             button.is_pressed = pressed
             self.__ptdm_subscribe_client.invoke_callback_func_if_exists(
                 button.when_pressed if button.is_pressed else button.when_released
             )
 
@@ -86,21 +71,15 @@
                 Message.PUB_V3_BUTTON_CANCEL_RELEASED: lambda: set_button_state(
                     self.cancel, pressed=False
                 ),
             }
         )
         self.__ptdm_subscribe_client.start_listening()
 
-    def __clean_up_lock(self):
-        if self.is_active:
-            self.lock.release()
-
     def __clean_up(self):
-        self.__clean_up_lock()
-
         try:
             self.__ptdm_subscribe_client.stop_listening()
         except Exception:
             pass
 
 
 class UpButton(MiniscreenButton):
```

### Comparing `pitop.miniscreen-0.31.0.post4/pitop/miniscreen/images/rocket.gif` & `pitop.miniscreen-0.32.0.post1/pitop/miniscreen/images/rocket.gif`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/assistant.py` & `pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/assistant.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/canvas.py` & `pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/canvas.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/LICENSE.rst` & `pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/core/device.py` & `pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/device.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/core/error.py` & `pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/error.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/core/interface/serial.py` & `pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/interface/serial.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/core/mixin.py` & `pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/mixin.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/core/threadpool.py` & `pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/threadpool.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/core/virtual.py` & `pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/virtual.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/contrib/luma/oled/device/__init__.py` & `pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/contrib/luma/oled/device/__init__.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/device_controller.py` & `pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/device_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import atexit
-from os import getenv
 
-from pitop.common.lock import PTLock
 from pitop.common.ptdm import Message, PTDMRequestClient, PTDMSubscribeClient
 
 from .contrib.luma.core.interface.serial import spi
 from .contrib.luma.oled.device import sh1106
 
 
 class OledDeviceController:
@@ -17,15 +15,14 @@
     #
     # this is only necessary to support users with SPI0 on device
     # with older SDK version that only supported SPI1
     def __init__(self, redraw_last_image_func):
         self.__redraw_last_image_func = redraw_last_image_func
         self.__spi_bus = self.__get_spi_bus_from_ptdm()
         self._device = None
-        self.lock = PTLock("miniscreen")
 
         self.__ptdm_subscribe_client = None
         self.__setup_subscribe_client()
 
         atexit.register(self.__clean_up)
 
     def __setup_subscribe_client(self):
@@ -51,18 +48,14 @@
             Message.REQ_SET_OLED_CONTROL, [str(int(controlled_by_pi))]
         )
 
         with PTDMRequestClient() as request_client:
             request_client.send_message(message)
 
     def __setup_device(self):
-        if getenv("PT_MINISCREEN_SYSTEM", "0") != "1":
-            self.lock.acquire()
-            atexit.register(self.reset_device)
-
         self._device = sh1106(
             serial_interface=spi(
                 port=self.__spi_bus,
                 device=self.SPI_DEVICE,
                 bus_speed_hz=self.SPI_BUS_SPEED_HZ,
                 transfer_size=self.SPI_TRANSFER_SIZE,
                 gpio_DC=17 if self.__spi_bus == 1 else 7,  # Always use CE1
@@ -79,21 +72,16 @@
 
         return int(response.parameters[0])
 
     ##############################
     # Public methods
     ##############################
 
-    def device_is_active(self):
-        return self.lock.is_locked()
-
     def reset_device(self):
         self._device = None
-        if self.device_is_active():
-            self.lock.release()
 
     def get_device(self):
         if self._device is None:
             self.__setup_device()
 
         return self._device
```

### Comparing `pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/fps_regulator.py` & `pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/fps_regulator.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/core/lock.py` & `pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/core/lock.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.31.0.post4/pitop/miniscreen/oled/oled.py` & `pitop.miniscreen-0.32.0.post1/pitop/miniscreen/oled/oled.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,26 +3,25 @@
 from threading import Thread, current_thread, main_thread
 from time import sleep
 
 from pitop.common.ptdm import Message, PTDMSubscribeClient
 from pitop.core import ImageFunctions
 
 from .assistant import MiniscreenAssistant
-from .core import FPS_Regulator, MiniscreenLockFileMonitor, OledDeviceController
+from .core import FPS_Regulator, OledDeviceController
 
 logger = logging.getLogger(__name__)
 
 
 class OLED:
     """Provides access to the miniscreen display on the pi-top [4], and exposes
     methods for simple rendering of text or images to the screen."""
 
     def __init__(self):
         self._controller = OledDeviceController(self._redraw_last_image)
-        self.lock_file_monitor = MiniscreenLockFileMonitor(self._controller.lock.path)
 
         self.assistant = MiniscreenAssistant(self.mode, self.size)
 
         self.image = self.assistant.empty_image
         self._image = self.assistant.empty_image
 
         self.__fps_regulator = FPS_Regulator()
@@ -128,24 +127,14 @@
         return self.size[1]
 
     @property
     def mode(self):
         return self.device.mode
 
     @property
-    def is_active(self):
-        """Determine if the current OLED instance is in control of the OLED
-        hardware.
-
-        :return: whether the OLED instance is in control of the OLED hardware.
-        :rtype: bool
-        """
-        return self._controller.device_is_active()
-
-    @property
     def visible(self):
         """Gets whether the device is currently in low power state.
 
         :return: whether the screen is in low power mode
         :rtype: bool
         """
         return not self.__visible
@@ -553,80 +542,10 @@
                 # Wait for animated image's frame length
                 sleep(float(frame.info["duration"] / 1000))  # ms to s
 
             if self.__kill_thread or not loop:
                 self.reset()
                 break
 
-    @property
-    def when_user_controlled(self):
-        """Function to call when user takes control of the miniscreen.
-
-        This is used by pt-miniscreen to update its 'user-controlled'
-        application state.
-        """
-        return self.lock_file_monitor.when_user_starts_using_oled
-
-    @when_user_controlled.setter
-    def when_user_controlled(self, callback):
-        """Setter for function to call when user takes control of the
-        miniscreen.
-
-        This is used by pt-miniscreen to update its 'user-controlled'
-        application state.
-        """
-        if not callable(callback):
-            raise ValueError("Callback must be callable")
-
-        self.lock_file_monitor.when_user_starts_using_oled = callback
-        # Lockfile thread needs to be restarted to get updated callback reference
-        self.lock_file_monitor.start()
-
-    @property
-    def when_system_controlled(self):
-        """Function to call when user gives back control of the miniscreen to
-        the system.
-
-        This is used by pt-miniscreen to update its 'user-controlled'
-        application state.
-        """
-        return self.lock_file_monitor.when_user_stops_using_oled
-
-    @when_system_controlled.setter
-    def when_system_controlled(self, callback):
-        """Setter for function to call when user gives back control of the
-        miniscreen to the system.
-
-        This is used by pt-miniscreen to update its 'user-controlled'
-        application state.
-        """
-        if not callable(callback):
-            raise ValueError("Callback must be callable")
-
-        self.lock_file_monitor.when_user_stops_using_oled = callback
-        # Lockfile thread needs to be restarted to get updated callback reference
-        self.lock_file_monitor.start()
-
-    @property
-    def _when_user_starts_using_oled(self):
-        """Deprecated function."""
-        return self.when_user_controlled
-
-    @_when_user_starts_using_oled.setter
-    def _when_user_starts_using_oled(self, callback):
-        """Deprecated function."""
-        self.when_user_controlled = callback
-
-    @property
-    def _when_user_stops_using_oled(self):
-        """Deprecated function."""
-        return self.when_system_controlled
-
-    @_when_user_stops_using_oled.setter
-    def _when_user_stops_using_oled(self, callback):
-        """Deprecated function."""
-        self.when_system_controlled = callback
-
     def __cleanup(self):
         self.stop_animated_image()
-        self.lock_file_monitor.stop()
         self._ptdm_subscribe_client.stop_listening()
```

### Comparing `pitop.miniscreen-0.31.0.post4/pitop.miniscreen.egg-info/PKG-INFO` & `pitop.miniscreen-0.32.0.post1/pitop.miniscreen.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.miniscreen
-Version: 0.31.0.post4
+Version: 0.32.0.post1
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Miniscreen
```

### Comparing `pitop.miniscreen-0.31.0.post4/pitop.miniscreen.egg-info/SOURCES.txt` & `pitop.miniscreen-0.32.0.post1/pitop.miniscreen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.31.0.post4/setup.py` & `pitop.miniscreen-0.32.0.post1/setup.py`

 * *Files identical despite different names*

