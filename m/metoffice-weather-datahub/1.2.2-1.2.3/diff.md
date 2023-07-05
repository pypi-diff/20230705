# Comparing `tmp/metoffice-weather-datahub-1.2.2.tar.gz` & `tmp/metoffice-weather-datahub-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metoffice-weather-datahub-1.2.2.tar", last modified: Thu May 25 13:34:32 2023, max compression
+gzip compressed data, was "metoffice-weather-datahub-1.2.3.tar", last modified: Wed Jul  5 10:27:57 2023, max compression
```

## Comparing `metoffice-weather-datahub-1.2.2.tar` & `metoffice-weather-datahub-1.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:34:32.222864 metoffice-weather-datahub-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-25 13:34:18.000000 metoffice-weather-datahub-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 13:34:18.000000 metoffice-weather-datahub-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-25 13:34:32.222864 metoffice-weather-datahub-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-25 13:34:18.000000 metoffice-weather-datahub-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:34:32.222864 metoffice-weather-datahub-1.2.2/metoffice_weather_datahub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-25 13:34:32.000000 metoffice-weather-datahub-1.2.2/metoffice_weather_datahub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-25 13:34:32.000000 metoffice-weather-datahub-1.2.2/metoffice_weather_datahub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:34:32.000000 metoffice-weather-datahub-1.2.2/metoffice_weather_datahub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-25 13:34:32.000000 metoffice-weather-datahub-1.2.2/metoffice_weather_datahub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 13:34:32.000000 metoffice-weather-datahub-1.2.2/metoffice_weather_datahub.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:34:32.222864 metoffice-weather-datahub-1.2.2/metofficedatahub/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-25 13:34:18.000000 metoffice-weather-datahub-1.2.2/metofficedatahub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-25 13:34:18.000000 metoffice-weather-datahub-1.2.2/metofficedatahub/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-05-25 13:34:18.000000 metoffice-weather-datahub-1.2.2/metofficedatahub/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-25 13:34:18.000000 metoffice-weather-datahub-1.2.2/metofficedatahub/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-25 13:34:18.000000 metoffice-weather-datahub-1.2.2/metofficedatahub/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-05-25 13:34:18.000000 metoffice-weather-datahub-1.2.2/metofficedatahub/multiple_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-25 13:34:18.000000 metoffice-weather-datahub-1.2.2/metofficedatahub/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-25 13:34:18.000000 metoffice-weather-datahub-1.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 13:34:32.222864 metoffice-weather-datahub-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-25 13:34:18.000000 metoffice-weather-datahub-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:34:32.222864 metoffice-weather-datahub-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-25 13:34:18.000000 metoffice-weather-datahub-1.2.2/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-25 13:34:18.000000 metoffice-weather-datahub-1.2.2/tests/test_multiple_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-25 13:34:18.000000 metoffice-weather-datahub-1.2.2/tests/test_orders.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-25 13:34:18.000000 metoffice-weather-datahub-1.2.2/tests/test_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-25 13:34:18.000000 metoffice-weather-datahub-1.2.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:27:57.099102 metoffice-weather-datahub-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-05 10:27:47.000000 metoffice-weather-datahub-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 10:27:47.000000 metoffice-weather-datahub-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-05 10:27:57.099102 metoffice-weather-datahub-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-05 10:27:47.000000 metoffice-weather-datahub-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:27:57.099102 metoffice-weather-datahub-1.2.3/metoffice_weather_datahub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-05 10:27:57.000000 metoffice-weather-datahub-1.2.3/metoffice_weather_datahub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-05 10:27:57.000000 metoffice-weather-datahub-1.2.3/metoffice_weather_datahub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 10:27:57.000000 metoffice-weather-datahub-1.2.3/metoffice_weather_datahub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-05 10:27:57.000000 metoffice-weather-datahub-1.2.3/metoffice_weather_datahub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 10:27:57.000000 metoffice-weather-datahub-1.2.3/metoffice_weather_datahub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:27:57.099102 metoffice-weather-datahub-1.2.3/metofficedatahub/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-05 10:27:47.000000 metoffice-weather-datahub-1.2.3/metofficedatahub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-05 10:27:47.000000 metoffice-weather-datahub-1.2.3/metofficedatahub/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-07-05 10:27:47.000000 metoffice-weather-datahub-1.2.3/metofficedatahub/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-05 10:27:47.000000 metoffice-weather-datahub-1.2.3/metofficedatahub/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-05 10:27:47.000000 metoffice-weather-datahub-1.2.3/metofficedatahub/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-05 10:27:47.000000 metoffice-weather-datahub-1.2.3/metofficedatahub/multiple_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-05 10:27:47.000000 metoffice-weather-datahub-1.2.3/metofficedatahub/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-05 10:27:47.000000 metoffice-weather-datahub-1.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 10:27:57.099102 metoffice-weather-datahub-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-05 10:27:47.000000 metoffice-weather-datahub-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:27:57.099102 metoffice-weather-datahub-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-05 10:27:47.000000 metoffice-weather-datahub-1.2.3/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-05 10:27:47.000000 metoffice-weather-datahub-1.2.3/tests/test_multiple_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-05 10:27:47.000000 metoffice-weather-datahub-1.2.3/tests/test_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-05 10:27:47.000000 metoffice-weather-datahub-1.2.3/tests/test_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-05 10:27:47.000000 metoffice-weather-datahub-1.2.3/tests/test_utils.py
```

### Comparing `metoffice-weather-datahub-1.2.2/LICENSE` & `metoffice-weather-datahub-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metoffice-weather-datahub-1.2.2/PKG-INFO` & `metoffice-weather-datahub-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metoffice-weather-datahub
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python wrapper for the UK Met Office Weather DataHub API
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `metoffice-weather-datahub-1.2.2/README.md` & `metoffice-weather-datahub-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `metoffice-weather-datahub-1.2.2/metoffice_weather_datahub.egg-info/PKG-INFO` & `metoffice-weather-datahub-1.2.3/metoffice_weather_datahub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metoffice-weather-datahub
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python wrapper for the UK Met Office Weather DataHub API
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `metoffice-weather-datahub-1.2.2/metoffice_weather_datahub.egg-info/SOURCES.txt` & `metoffice-weather-datahub-1.2.3/metoffice_weather_datahub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metoffice-weather-datahub-1.2.2/metofficedatahub/app.py` & `metoffice-weather-datahub-1.2.3/metofficedatahub/app.py`

 * *Files identical despite different names*

### Comparing `metoffice-weather-datahub-1.2.2/metofficedatahub/base.py` & `metoffice-weather-datahub-1.2.3/metofficedatahub/base.py`

 * *Files identical despite different names*

### Comparing `metoffice-weather-datahub-1.2.2/metofficedatahub/models.py` & `metoffice-weather-datahub-1.2.3/metofficedatahub/models.py`

 * *Files identical despite different names*

### Comparing `metoffice-weather-datahub-1.2.2/metofficedatahub/multiple_files.py` & `metoffice-weather-datahub-1.2.3/metofficedatahub/multiple_files.py`

 * *Files identical despite different names*

### Comparing `metoffice-weather-datahub-1.2.2/metofficedatahub/utils.py` & `metoffice-weather-datahub-1.2.3/metofficedatahub/utils.py`

 * *Files identical despite different names*

### Comparing `metoffice-weather-datahub-1.2.2/setup.py` & `metoffice-weather-datahub-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 install_requires = (this_directory / "requirements.txt").read_text().splitlines()
 
 setup(
     name="metoffice-weather-datahub",
-    version="1.2.2",
+    version="1.2.3",
     license="MIT",
     description="Python wrapper for the UK Met Office Weather DataHub API",
     author="Peter Dudfield",
     author_email="info@openclimatefix.org",
     company="Open Climate Fix Ltd",
     install_requires=install_requires,
     long_description=long_description,
```

### Comparing `metoffice-weather-datahub-1.2.2/tests/test_app.py` & `metoffice-weather-datahub-1.2.3/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `metoffice-weather-datahub-1.2.2/tests/test_multiple_files.py` & `metoffice-weather-datahub-1.2.3/tests/test_multiple_files.py`

 * *Files identical despite different names*

### Comparing `metoffice-weather-datahub-1.2.2/tests/test_orders.py` & `metoffice-weather-datahub-1.2.3/tests/test_orders.py`

 * *Files identical despite different names*

### Comparing `metoffice-weather-datahub-1.2.2/tests/test_utils.py` & `metoffice-weather-datahub-1.2.3/tests/test_utils.py`

 * *Files identical despite different names*

