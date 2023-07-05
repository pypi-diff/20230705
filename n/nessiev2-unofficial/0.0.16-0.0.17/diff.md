# Comparing `tmp/nessiev2_unofficial-0.0.16.tar.gz` & `tmp/nessiev2_unofficial-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nessiev2_unofficial-0.0.16.tar", last modified: Wed Jul  5 20:37:49 2023, max compression
+gzip compressed data, was "nessiev2_unofficial-0.0.17.tar", last modified: Wed Jul  5 20:43:36 2023, max compression
```

## Comparing `nessiev2_unofficial-0.0.16.tar` & `nessiev2_unofficial-0.0.17.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 alexmerced  (1000) alexmerced  (1000)        0 2023-07-05 20:37:49.432860 nessiev2_unofficial-0.0.16/
--rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)     1070 2023-06-30 20:45:00.000000 nessiev2_unofficial-0.0.16/LICENSE
--rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)      966 2023-07-05 20:37:49.432860 nessiev2_unofficial-0.0.16/PKG-INFO
--rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)      750 2023-07-05 20:37:25.000000 nessiev2_unofficial-0.0.16/pyproject.toml
--rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)      384 2023-07-05 20:04:57.000000 nessiev2_unofficial-0.0.16/readme.md
--rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)       38 2023-07-05 20:37:49.432860 nessiev2_unofficial-0.0.16/setup.cfg
-drwxrwxr-x   0 alexmerced  (1000) alexmerced  (1000)        0 2023-07-05 20:37:49.428860 nessiev2_unofficial-0.0.16/src/
-drwxrwxr-x   0 alexmerced  (1000) alexmerced  (1000)        0 2023-07-05 20:37:49.432860 nessiev2_unofficial-0.0.16/src/nessiev2_unofficial.egg-info/
--rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)      966 2023-07-05 20:37:49.000000 nessiev2_unofficial-0.0.16/src/nessiev2_unofficial.egg-info/PKG-INFO
--rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)      581 2023-07-05 20:37:49.000000 nessiev2_unofficial-0.0.16/src/nessiev2_unofficial.egg-info/SOURCES.txt
--rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)        1 2023-07-05 20:37:49.000000 nessiev2_unofficial-0.0.16/src/nessiev2_unofficial.egg-info/dependency_links.txt
--rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)       61 2023-07-05 20:37:49.000000 nessiev2_unofficial-0.0.16/src/nessiev2_unofficial.egg-info/requires.txt
--rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)       26 2023-07-05 20:37:49.000000 nessiev2_unofficial-0.0.16/src/nessiev2_unofficial.egg-info/top_level.txt
-drwxrwxr-x   0 alexmerced  (1000) alexmerced  (1000)        0 2023-07-05 20:37:49.432860 nessiev2_unofficial-0.0.16/src/unofficial_nessiev2_tools/
--rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)        0 2023-06-30 20:20:34.000000 nessiev2_unofficial-0.0.16/src/unofficial_nessiev2_tools/__init__.py
--rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)      262 2023-06-30 20:31:40.000000 nessiev2_unofficial-0.0.16/src/unofficial_nessiev2_tools/catalog.py
--rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)    15643 2023-07-05 18:01:08.000000 nessiev2_unofficial-0.0.16/src/unofficial_nessiev2_tools/client.py
-drwxrwxr-x   0 alexmerced  (1000) alexmerced  (1000)        0 2023-07-05 20:37:49.432860 nessiev2_unofficial-0.0.16/src/unofficial_nessiev2_tools/generators/
--rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)     8032 2023-06-30 20:24:57.000000 nessiev2_unofficial-0.0.16/src/unofficial_nessiev2_tools/generators/__init__.py
--rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)     3210 2023-07-05 18:01:51.000000 nessiev2_unofficial-0.0.16/src/unofficial_nessiev2_tools/test_client.py
--rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)     1148 2023-07-05 18:07:19.000000 nessiev2_unofficial-0.0.16/src/unofficial_nessiev2_tools/test_objects.py
-drwxrwxr-x   0 alexmerced  (1000) alexmerced  (1000)        0 2023-07-05 20:37:49.432860 nessiev2_unofficial-0.0.16/src/unofficial_nessiev2_tools/utils/
--rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)      936 2023-06-23 14:37:59.000000 nessiev2_unofficial-0.0.16/src/unofficial_nessiev2_tools/utils/__init__.py
+drwxrwxr-x   0 alexmerced  (1000) alexmerced  (1000)        0 2023-07-05 20:43:36.971114 nessiev2_unofficial-0.0.17/
+-rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)     1070 2023-06-30 20:45:00.000000 nessiev2_unofficial-0.0.17/LICENSE
+-rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)      966 2023-07-05 20:43:36.971114 nessiev2_unofficial-0.0.17/PKG-INFO
+-rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)      750 2023-07-05 20:43:27.000000 nessiev2_unofficial-0.0.17/pyproject.toml
+-rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)      384 2023-07-05 20:04:57.000000 nessiev2_unofficial-0.0.17/readme.md
+-rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)       38 2023-07-05 20:43:36.971114 nessiev2_unofficial-0.0.17/setup.cfg
+drwxrwxr-x   0 alexmerced  (1000) alexmerced  (1000)        0 2023-07-05 20:43:36.967114 nessiev2_unofficial-0.0.17/src/
+drwxrwxr-x   0 alexmerced  (1000) alexmerced  (1000)        0 2023-07-05 20:43:36.967114 nessiev2_unofficial-0.0.17/src/nessiev2_unofficial/
+-rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)        0 2023-06-30 20:20:34.000000 nessiev2_unofficial-0.0.17/src/nessiev2_unofficial/__init__.py
+-rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)      262 2023-06-30 20:31:40.000000 nessiev2_unofficial-0.0.17/src/nessiev2_unofficial/catalog.py
+-rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)    15643 2023-07-05 18:01:08.000000 nessiev2_unofficial-0.0.17/src/nessiev2_unofficial/client.py
+drwxrwxr-x   0 alexmerced  (1000) alexmerced  (1000)        0 2023-07-05 20:43:36.967114 nessiev2_unofficial-0.0.17/src/nessiev2_unofficial/generators/
+-rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)     8032 2023-06-30 20:24:57.000000 nessiev2_unofficial-0.0.17/src/nessiev2_unofficial/generators/__init__.py
+-rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)     3210 2023-07-05 18:01:51.000000 nessiev2_unofficial-0.0.17/src/nessiev2_unofficial/test_client.py
+-rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)     1148 2023-07-05 18:07:19.000000 nessiev2_unofficial-0.0.17/src/nessiev2_unofficial/test_objects.py
+drwxrwxr-x   0 alexmerced  (1000) alexmerced  (1000)        0 2023-07-05 20:43:36.971114 nessiev2_unofficial-0.0.17/src/nessiev2_unofficial/utils/
+-rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)      936 2023-06-23 14:37:59.000000 nessiev2_unofficial-0.0.17/src/nessiev2_unofficial/utils/__init__.py
+drwxrwxr-x   0 alexmerced  (1000) alexmerced  (1000)        0 2023-07-05 20:43:36.967114 nessiev2_unofficial-0.0.17/src/nessiev2_unofficial.egg-info/
+-rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)      966 2023-07-05 20:43:36.000000 nessiev2_unofficial-0.0.17/src/nessiev2_unofficial.egg-info/PKG-INFO
+-rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)      539 2023-07-05 20:43:36.000000 nessiev2_unofficial-0.0.17/src/nessiev2_unofficial.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)        1 2023-07-05 20:43:36.000000 nessiev2_unofficial-0.0.17/src/nessiev2_unofficial.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)       61 2023-07-05 20:43:36.000000 nessiev2_unofficial-0.0.17/src/nessiev2_unofficial.egg-info/requires.txt
+-rw-rw-r--   0 alexmerced  (1000) alexmerced  (1000)       20 2023-07-05 20:43:36.000000 nessiev2_unofficial-0.0.17/src/nessiev2_unofficial.egg-info/top_level.txt
```

### Comparing `nessiev2_unofficial-0.0.16/LICENSE` & `nessiev2_unofficial-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `nessiev2_unofficial-0.0.16/PKG-INFO` & `nessiev2_unofficial-0.0.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nessiev2_unofficial
-Version: 0.0.16
+Version: 0.0.17
 Summary: An unofficial example of a Nessie V2 Client
 Author-email: Alex Merced <alex.merced@dremio.com>
 Project-URL: Homepage, https://github.com/AlexMercedCoder/UnofficialNessieV2ClientPython
 Project-URL: Bug Tracker, https://github.com/AlexMercedCoder/UnofficialNessieV2ClientPython
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nessiev2_unofficial-0.0.16/pyproject.toml` & `nessiev2_unofficial-0.0.17/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nessiev2_unofficial"
-version = "0.0.16"
+version = "0.0.17"
 authors = [
   { name="Alex Merced", email="alex.merced@dremio.com" },
 ]
 description = "An unofficial example of a Nessie V2 Client"
 readme = "readme.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `nessiev2_unofficial-0.0.16/src/nessiev2_unofficial.egg-info/PKG-INFO` & `nessiev2_unofficial-0.0.17/src/nessiev2_unofficial.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nessiev2-unofficial
-Version: 0.0.16
+Version: 0.0.17
 Summary: An unofficial example of a Nessie V2 Client
 Author-email: Alex Merced <alex.merced@dremio.com>
 Project-URL: Homepage, https://github.com/AlexMercedCoder/UnofficialNessieV2ClientPython
 Project-URL: Bug Tracker, https://github.com/AlexMercedCoder/UnofficialNessieV2ClientPython
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nessiev2_unofficial-0.0.16/src/unofficial_nessiev2_tools/client.py` & `nessiev2_unofficial-0.0.17/src/nessiev2_unofficial/client.py`

 * *Files identical despite different names*

### Comparing `nessiev2_unofficial-0.0.16/src/unofficial_nessiev2_tools/generators/__init__.py` & `nessiev2_unofficial-0.0.17/src/nessiev2_unofficial/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `nessiev2_unofficial-0.0.16/src/unofficial_nessiev2_tools/test_client.py` & `nessiev2_unofficial-0.0.17/src/nessiev2_unofficial/test_client.py`

 * *Files identical despite different names*

### Comparing `nessiev2_unofficial-0.0.16/src/unofficial_nessiev2_tools/test_objects.py` & `nessiev2_unofficial-0.0.17/src/nessiev2_unofficial/test_objects.py`

 * *Files identical despite different names*

### Comparing `nessiev2_unofficial-0.0.16/src/unofficial_nessiev2_tools/utils/__init__.py` & `nessiev2_unofficial-0.0.17/src/nessiev2_unofficial/utils/__init__.py`

 * *Files identical despite different names*

