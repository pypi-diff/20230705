# Comparing `tmp/pitopcli-0.31.0.post4.tar.gz` & `tmp/pitopcli-0.32.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitopcli-0.31.0.post4.tar", last modified: Tue Jun 13 18:30:06 2023, max compression
+gzip compressed data, was "dist/pitopcli-0.32.0.post1.tar", last modified: Wed Jul  5 13:37:05 2023, max compression
```

## Comparing `pitopcli-0.31.0.post4.tar` & `pitopcli-0.32.0.post1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:06.000000 pitopcli-0.31.0.post4/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      960 2023-06-13 18:30:06.000000 pitopcli-0.31.0.post4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:06.000000 pitopcli-0.31.0.post4/pitopcli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/pitopcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1774 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/pitopcli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/pitopcli/battery.py
--rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/pitopcli/cli_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1920 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/pitopcli/deprecated_cli_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     4442 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/pitopcli/devices.py
--rw-r--r--   0 runner    (1001) docker     (122)     5168 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/pitopcli/display.py
--rw-r--r--   0 runner    (1001) docker     (122)     3283 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/pitopcli/formatter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2323 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/pitopcli/imu.py
--rw-r--r--   0 runner    (1001) docker     (122)    14042 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/pitopcli/imu_calibration.py
--rw-r--r--   0 runner    (1001) docker     (122)     6189 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/pitopcli/oled.py
--rw-r--r--   0 runner    (1001) docker     (122)     1774 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/pitopcli/pitop.py
--rw-r--r--   0 runner    (1001) docker     (122)     2385 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/pitopcli/support.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:06.000000 pitopcli-0.31.0.post4/pitopcli/support_core/
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/pitopcli/support_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12012 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/pitopcli/support_core/health_check.py
--rw-r--r--   0 runner    (1001) docker     (122)    11142 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/pitopcli/support_core/hub_communication.py
--rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/pitopcli/support_core/links.py
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/pitopcli/support_core/ptsoftware.py
--rw-r--r--   0 runner    (1001) docker     (122)     4568 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/pitopcli/support_core/systemd_service.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:06.000000 pitopcli-0.31.0.post4/pitopcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      960 2023-06-13 18:30:06.000000 pitopcli-0.31.0.post4/pitopcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      726 2023-06-13 18:30:06.000000 pitopcli-0.31.0.post4/pitopcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 18:30:06.000000 pitopcli-0.31.0.post4/pitopcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-13 18:30:06.000000 pitopcli-0.31.0.post4/pitopcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      249 2023-06-13 18:30:06.000000 pitopcli-0.31.0.post4/pitopcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-13 18:30:06.000000 pitopcli-0.31.0.post4/pitopcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 18:30:06.000000 pitopcli-0.31.0.post4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2522 2023-06-13 18:29:44.000000 pitopcli-0.31.0.post4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:05.000000 pitopcli-0.32.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      960 2023-07-05 13:37:05.000000 pitopcli-0.32.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:05.000000 pitopcli-0.32.0.post1/pitopcli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/pitopcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1774 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/pitopcli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/pitopcli/battery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/pitopcli/cli_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1920 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/pitopcli/deprecated_cli_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4442 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/pitopcli/devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5168 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/pitopcli/display.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3283 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/pitopcli/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2323 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/pitopcli/imu.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14042 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/pitopcli/imu_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6189 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/pitopcli/oled.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1774 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/pitopcli/pitop.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2385 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/pitopcli/support.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:05.000000 pitopcli-0.32.0.post1/pitopcli/support_core/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/pitopcli/support_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12012 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/pitopcli/support_core/health_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11142 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/pitopcli/support_core/hub_communication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/pitopcli/support_core/links.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/pitopcli/support_core/ptsoftware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4568 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/pitopcli/support_core/systemd_service.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:05.000000 pitopcli-0.32.0.post1/pitopcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      960 2023-07-05 13:37:05.000000 pitopcli-0.32.0.post1/pitopcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      726 2023-07-05 13:37:05.000000 pitopcli-0.32.0.post1/pitopcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 13:37:05.000000 pitopcli-0.32.0.post1/pitopcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-05 13:37:05.000000 pitopcli-0.32.0.post1/pitopcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-07-05 13:37:05.000000 pitopcli-0.32.0.post1/pitopcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-05 13:37:05.000000 pitopcli-0.32.0.post1/pitopcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-05 13:37:05.000000 pitopcli-0.32.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2522 2023-07-05 13:36:52.000000 pitopcli-0.32.0.post1/setup.py
```

### Comparing `pitopcli-0.31.0.post4/PKG-INFO` & `pitopcli-0.32.0.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitopcli
-Version: 0.31.0.post4
+Version: 0.32.0.post1
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python CLI
```

### Comparing `pitopcli-0.31.0.post4/pitopcli/__main__.py` & `pitopcli-0.32.0.post1/pitopcli/__main__.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.31.0.post4/pitopcli/battery.py` & `pitopcli-0.32.0.post1/pitopcli/battery.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.31.0.post4/pitopcli/cli_base.py` & `pitopcli-0.32.0.post1/pitopcli/cli_base.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.31.0.post4/pitopcli/deprecated_cli_runner.py` & `pitopcli-0.32.0.post1/pitopcli/deprecated_cli_runner.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.31.0.post4/pitopcli/devices.py` & `pitopcli-0.32.0.post1/pitopcli/devices.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.31.0.post4/pitopcli/display.py` & `pitopcli-0.32.0.post1/pitopcli/display.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.31.0.post4/pitopcli/formatter.py` & `pitopcli-0.32.0.post1/pitopcli/formatter.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.31.0.post4/pitopcli/imu.py` & `pitopcli-0.32.0.post1/pitopcli/imu.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.31.0.post4/pitopcli/imu_calibration.py` & `pitopcli-0.32.0.post1/pitopcli/imu_calibration.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.31.0.post4/pitopcli/oled.py` & `pitopcli-0.32.0.post1/pitopcli/oled.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.31.0.post4/pitopcli/pitop.py` & `pitopcli-0.32.0.post1/pitopcli/pitop.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.31.0.post4/pitopcli/support.py` & `pitopcli-0.32.0.post1/pitopcli/support.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.31.0.post4/pitopcli/support_core/health_check.py` & `pitopcli-0.32.0.post1/pitopcli/support_core/health_check.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.31.0.post4/pitopcli/support_core/hub_communication.py` & `pitopcli-0.32.0.post1/pitopcli/support_core/hub_communication.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.31.0.post4/pitopcli/support_core/links.py` & `pitopcli-0.32.0.post1/pitopcli/support_core/links.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.31.0.post4/pitopcli/support_core/ptsoftware.py` & `pitopcli-0.32.0.post1/pitopcli/support_core/ptsoftware.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.31.0.post4/pitopcli/support_core/systemd_service.py` & `pitopcli-0.32.0.post1/pitopcli/support_core/systemd_service.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.31.0.post4/pitopcli.egg-info/PKG-INFO` & `pitopcli-0.32.0.post1/pitopcli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitopcli
-Version: 0.31.0.post4
+Version: 0.32.0.post1
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python CLI
```

### Comparing `pitopcli-0.31.0.post4/pitopcli.egg-info/SOURCES.txt` & `pitopcli-0.32.0.post1/pitopcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pitopcli-0.31.0.post4/setup.py` & `pitopcli-0.32.0.post1/setup.py`

 * *Files identical despite different names*

