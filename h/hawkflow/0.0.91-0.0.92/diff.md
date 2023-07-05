# Comparing `tmp/hawkflow-0.0.91.tar.gz` & `tmp/hawkflow-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/felbus/github/hawkflow-py/dist/.tmp-mag3eo2z/hawkflow-0.0.91.tar", last modified: Tue Jul  4 08:31:22 2023, max compression
+gzip compressed data, was "/Users/felbus/github/hawkflow-py/dist/.tmp-fci3zisu/hawkflow-0.0.92.tar", last modified: Wed Jul  5 08:46:22 2023, max compression
```

## Comparing `hawkflow-0.0.91.tar` & `hawkflow-0.0.92.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-04 08:31:22.000000 hawkflow-0.0.91/
--rw-r--r--   0 felbus     (501) staff       (20)     1054 2023-02-20 15:32:46.000000 hawkflow-0.0.91/LICENSE
--rw-r--r--   0 felbus     (501) staff       (20)     1956 2023-07-04 08:31:22.000000 hawkflow-0.0.91/PKG-INFO
--rw-r--r--   0 felbus     (501) staff       (20)     1264 2023-03-15 18:47:38.000000 hawkflow-0.0.91/README.md
--rw-r--r--   0 felbus     (501) staff       (20)      843 2023-07-04 08:30:57.000000 hawkflow-0.0.91/pyproject.toml
--rw-r--r--   0 felbus     (501) staff       (20)       38 2023-07-04 08:31:22.000000 hawkflow-0.0.91/setup.cfg
-drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-04 08:31:22.000000 hawkflow-0.0.91/src/
-drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-04 08:31:22.000000 hawkflow-0.0.91/src/hawkflow.egg-info/
--rw-r--r--   0 felbus     (501) staff       (20)     1956 2023-07-04 08:31:22.000000 hawkflow-0.0.91/src/hawkflow.egg-info/PKG-INFO
--rw-r--r--   0 felbus     (501) staff       (20)      556 2023-07-04 08:31:22.000000 hawkflow-0.0.91/src/hawkflow.egg-info/SOURCES.txt
--rw-r--r--   0 felbus     (501) staff       (20)        1 2023-07-04 08:31:22.000000 hawkflow-0.0.91/src/hawkflow.egg-info/dependency_links.txt
--rw-r--r--   0 felbus     (501) staff       (20)       17 2023-07-04 08:31:22.000000 hawkflow-0.0.91/src/hawkflow.egg-info/requires.txt
--rw-r--r--   0 felbus     (501) staff       (20)       15 2023-07-04 08:31:22.000000 hawkflow-0.0.91/src/hawkflow.egg-info/top_level.txt
-drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-04 08:31:22.000000 hawkflow-0.0.91/src/hawkflowclient/
--rw-r--r--   0 felbus     (501) staff       (20)      199 2023-03-03 15:13:44.000000 hawkflow-0.0.91/src/hawkflowclient/__init__.py
--rw-r--r--   0 felbus     (501) staff       (20)      879 2023-02-27 16:57:39.000000 hawkflow-0.0.91/src/hawkflowclient/_endpoints.py
--rw-r--r--   0 felbus     (501) staff       (20)     1045 2023-02-20 15:32:46.000000 hawkflow-0.0.91/src/hawkflowclient/_hawkflow_exceptions.py
--rw-r--r--   0 felbus     (501) staff       (20)     3459 2023-07-04 08:28:09.000000 hawkflow-0.0.91/src/hawkflowclient/_validation.py
--rw-r--r--   0 felbus     (501) staff       (20)     2714 2023-03-03 15:36:38.000000 hawkflow-0.0.91/src/hawkflowclient/hawkflow_api.py
--rw-r--r--   0 felbus     (501) staff       (20)     1816 2023-02-20 15:32:46.000000 hawkflow-0.0.91/src/hawkflowclient/hawkflow_decorators.py
-drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-04 08:31:22.000000 hawkflow-0.0.91/src/hawkflowclient/tests/
--rw-r--r--   0 felbus     (501) staff       (20)        0 2023-02-20 15:32:46.000000 hawkflow-0.0.91/src/hawkflowclient/tests/__init__.py
--rw-r--r--   0 felbus     (501) staff       (20)     3276 2023-02-20 15:32:46.000000 hawkflow-0.0.91/src/hawkflowclient/tests/test_hawkflow_api.py
--rw-r--r--   0 felbus     (501) staff       (20)     3980 2023-07-04 08:17:17.000000 hawkflow-0.0.91/src/hawkflowclient/tests/test_validation.py
+drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-05 08:46:22.000000 hawkflow-0.0.92/
+-rw-r--r--   0 felbus     (501) staff       (20)     1054 2023-02-20 15:32:46.000000 hawkflow-0.0.92/LICENSE
+-rw-r--r--   0 felbus     (501) staff       (20)     1956 2023-07-05 08:46:22.000000 hawkflow-0.0.92/PKG-INFO
+-rw-r--r--   0 felbus     (501) staff       (20)     1264 2023-03-15 18:47:38.000000 hawkflow-0.0.92/README.md
+-rw-r--r--   0 felbus     (501) staff       (20)      843 2023-07-05 08:44:15.000000 hawkflow-0.0.92/pyproject.toml
+-rw-r--r--   0 felbus     (501) staff       (20)       38 2023-07-05 08:46:22.000000 hawkflow-0.0.92/setup.cfg
+drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-05 08:46:22.000000 hawkflow-0.0.92/src/
+drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-05 08:46:22.000000 hawkflow-0.0.92/src/hawkflow.egg-info/
+-rw-r--r--   0 felbus     (501) staff       (20)     1956 2023-07-05 08:46:22.000000 hawkflow-0.0.92/src/hawkflow.egg-info/PKG-INFO
+-rw-r--r--   0 felbus     (501) staff       (20)      556 2023-07-05 08:46:22.000000 hawkflow-0.0.92/src/hawkflow.egg-info/SOURCES.txt
+-rw-r--r--   0 felbus     (501) staff       (20)        1 2023-07-05 08:46:22.000000 hawkflow-0.0.92/src/hawkflow.egg-info/dependency_links.txt
+-rw-r--r--   0 felbus     (501) staff       (20)       17 2023-07-05 08:46:22.000000 hawkflow-0.0.92/src/hawkflow.egg-info/requires.txt
+-rw-r--r--   0 felbus     (501) staff       (20)       15 2023-07-05 08:46:22.000000 hawkflow-0.0.92/src/hawkflow.egg-info/top_level.txt
+drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-05 08:46:22.000000 hawkflow-0.0.92/src/hawkflowclient/
+-rw-r--r--   0 felbus     (501) staff       (20)      199 2023-03-03 15:13:44.000000 hawkflow-0.0.92/src/hawkflowclient/__init__.py
+-rw-r--r--   0 felbus     (501) staff       (20)      879 2023-02-27 16:57:39.000000 hawkflow-0.0.92/src/hawkflowclient/_endpoints.py
+-rw-r--r--   0 felbus     (501) staff       (20)     1045 2023-02-20 15:32:46.000000 hawkflow-0.0.92/src/hawkflowclient/_hawkflow_exceptions.py
+-rw-r--r--   0 felbus     (501) staff       (20)     3463 2023-07-05 08:45:37.000000 hawkflow-0.0.92/src/hawkflowclient/_validation.py
+-rw-r--r--   0 felbus     (501) staff       (20)     2714 2023-03-03 15:36:38.000000 hawkflow-0.0.92/src/hawkflowclient/hawkflow_api.py
+-rw-r--r--   0 felbus     (501) staff       (20)     1816 2023-02-20 15:32:46.000000 hawkflow-0.0.92/src/hawkflowclient/hawkflow_decorators.py
+drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-05 08:46:22.000000 hawkflow-0.0.92/src/hawkflowclient/tests/
+-rw-r--r--   0 felbus     (501) staff       (20)        0 2023-02-20 15:32:46.000000 hawkflow-0.0.92/src/hawkflowclient/tests/__init__.py
+-rw-r--r--   0 felbus     (501) staff       (20)     3276 2023-02-20 15:32:46.000000 hawkflow-0.0.92/src/hawkflowclient/tests/test_hawkflow_api.py
+-rw-r--r--   0 felbus     (501) staff       (20)     4518 2023-07-05 08:45:23.000000 hawkflow-0.0.92/src/hawkflowclient/tests/test_validation.py
```

### Comparing `hawkflow-0.0.91/LICENSE` & `hawkflow-0.0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.91/PKG-INFO` & `hawkflow-0.0.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hawkflow
-Version: 0.0.91
+Version: 0.0.92
 Summary: HawkFlow.ai
 License: LICENSE
 Project-URL: Homepage, https://github.com/hawkflow/hawkflow-py
 Keywords: hawkflow,hawkflowclient,monitoring
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `hawkflow-0.0.91/README.md` & `hawkflow-0.0.92/README.md`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.91/pyproject.toml` & `hawkflow-0.0.92/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="hawkflow"
-version="0.0.91"
+version="0.0.92"
 description="HawkFlow.ai"
 readme = "README.md"
 keywords=["hawkflow", "hawkflowclient", "monitoring"]
 license = {text = "LICENSE"}
 requires-python = ">=3.7"
 dependencies=[
     "requests>=2.25.1"
```

### Comparing `hawkflow-0.0.91/src/hawkflow.egg-info/PKG-INFO` & `hawkflow-0.0.92/src/hawkflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hawkflow
-Version: 0.0.91
+Version: 0.0.92
 Summary: HawkFlow.ai
 License: LICENSE
 Project-URL: Homepage, https://github.com/hawkflow/hawkflow-py
 Keywords: hawkflow,hawkflowclient,monitoring
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `hawkflow-0.0.91/src/hawkflow.egg-info/SOURCES.txt` & `hawkflow-0.0.92/src/hawkflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.91/src/hawkflowclient/_endpoints.py` & `hawkflow-0.0.92/src/hawkflowclient/_endpoints.py`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.91/src/hawkflowclient/_hawkflow_exceptions.py` & `hawkflow-0.0.92/src/hawkflowclient/_hawkflow_exceptions.py`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.91/src/hawkflowclient/_validation.py` & `hawkflow-0.0.92/src/hawkflowclient/_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import re
 import os
 
 from ._hawkflow_exceptions import *
 
 
 PROCESS_REGEX = r'^[a-zA-Z\d\s_-]*$'
-META_REGEX = r'^[\w\s\\/\-\_\*\&\=\.\+\?\@\:]*$'
+META_REGEX = r'^[\w\s\\/\-\_\*\&\=\.\,\+\?\@\:]*$'
+METRIC_KEY_REGEX = r'^[\w\s\\/\-\_\*\&\=\.\,\+\?\@\:]*$'
 API_KEY_REGEX = r'^[a-zA-Z0-9_-]+$'
-METRIC_KEY_REGEX = r'^[\w\s\\/\-\_\*\&\=\.\+\?\@\:]*$'
 UID_REGEX = r'^[a-zA-Z0-9_-]*$'
 
 
 def _validate_timed_data(process: str, meta: str, uid: str):
     _validate_core(process, meta)
     _validate_uid(uid)
```

### Comparing `hawkflow-0.0.91/src/hawkflowclient/hawkflow_api.py` & `hawkflow-0.0.92/src/hawkflowclient/hawkflow_api.py`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.91/src/hawkflowclient/hawkflow_decorators.py` & `hawkflow-0.0.92/src/hawkflowclient/hawkflow_decorators.py`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.91/src/hawkflowclient/tests/test_hawkflow_api.py` & `hawkflow-0.0.92/src/hawkflowclient/tests/test_hawkflow_api.py`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.91/src/hawkflowclient/tests/test_validation.py` & `hawkflow-0.0.92/src/hawkflowclient/tests/test_validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,21 @@
     def test_valid_meta_regex_2(self):
         try:
             key = r'127.0.0.1 story /'
             _validate_meta(key)
         except HawkFlowDataTypesException:
             self.fail("test_valid_api_meta_regex raised Exception")
 
+    def test_valid_meta_regex_4(self):
+        try:
+            key = r'127.0.0.1 story / ,'
+            _validate_meta(key)
+        except HawkFlowDataTypesException:
+            self.fail("test_valid_api_meta_regex raised Exception")
+
     def test_valid_meta_regex_3(self):
         try:
             key = r'http://127.0.0.1:5001/v1/start'
             _validate_meta(key)
         except HawkFlowDataTypesException:
             self.fail("test_valid_api_meta_regex raised Exception")
 
@@ -97,14 +104,22 @@
         try:
             key = r'xfghgh456456-_ads_fd345345'
             items = {key: 45}
             _validate_metric_items(items)
         except HawkFlowDataTypesException:
             self.fail("test_valid_api_metric_items_regex raised Exception")
 
+    def test_valid_metric_items_regex_1(self):
+        try:
+            key = r'xfghgh456456-_ads_fd345345,'
+            items = {key: 45}
+            _validate_metric_items(items)
+        except HawkFlowDataTypesException:
+            self.fail("test_valid_api_metric_items_regex raised Exception")
+
     def test_valid_metric_items_empty_string_regex(self):
         with self.assertRaises(HawkFlowDataTypesException):
             key = r''
             items = {key: 45}
             _validate_metric_items(items)
 
     def test_invalid_metric_items_regex(self):
```

