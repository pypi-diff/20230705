# Comparing `tmp/datadog-cdk-constructs-v2-1.7.3.tar.gz` & `tmp/datadog-cdk-constructs-v2-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadog-cdk-constructs-v2-1.7.3.tar", last modified: Tue Jun 13 19:44:37 2023, max compression
+gzip compressed data, was "datadog-cdk-constructs-v2-1.7.4.tar", last modified: Wed Jul  5 20:00:01 2023, max compression
```

## Comparing `datadog-cdk-constructs-v2-1.7.3.tar` & `datadog-cdk-constructs-v2-1.7.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dylan.yang   (502) staff       (20)        0 2023-06-13 19:44:37.784273 datadog-cdk-constructs-v2-1.7.3/
--rw-r--r--   0 dylan.yang   (502) staff       (20)    11358 2023-06-13 19:44:33.000000 datadog-cdk-constructs-v2-1.7.3/LICENSE
--rw-r--r--   0 dylan.yang   (502) staff       (20)       23 2023-06-13 19:44:33.000000 datadog-cdk-constructs-v2-1.7.3/MANIFEST.in
--rw-r--r--   0 dylan.yang   (502) staff       (20)    24060 2023-06-13 19:44:37.784114 datadog-cdk-constructs-v2-1.7.3/PKG-INFO
--rw-r--r--   0 dylan.yang   (502) staff       (20)    23080 2023-06-13 19:44:33.000000 datadog-cdk-constructs-v2-1.7.3/README.md
--rw-r--r--   0 dylan.yang   (502) staff       (20)      236 2023-06-13 19:44:33.000000 datadog-cdk-constructs-v2-1.7.3/pyproject.toml
--rw-r--r--   0 dylan.yang   (502) staff       (20)       38 2023-06-13 19:44:37.784316 datadog-cdk-constructs-v2-1.7.3/setup.cfg
--rw-r--r--   0 dylan.yang   (502) staff       (20)     1921 2023-06-13 19:44:33.000000 datadog-cdk-constructs-v2-1.7.3/setup.py
-drwxr-xr-x   0 dylan.yang   (502) staff       (20)        0 2023-06-13 19:44:37.781059 datadog-cdk-constructs-v2-1.7.3/src/
-drwxr-xr-x   0 dylan.yang   (502) staff       (20)        0 2023-06-13 19:44:37.782222 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2/
--rw-r--r--   0 dylan.yang   (502) staff       (20)   113679 2023-06-13 19:44:33.000000 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2/__init__.py
-drwxr-xr-x   0 dylan.yang   (502) staff       (20)        0 2023-06-13 19:44:37.783186 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2/_jsii/
--rw-r--r--   0 dylan.yang   (502) staff       (20)      475 2023-06-13 19:44:33.000000 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2/_jsii/__init__.py
--rw-r--r--   0 dylan.yang   (502) staff       (20)  1307963 2023-06-13 19:44:33.000000 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2/_jsii/datadog-cdk-constructs-v2@1.7.3.jsii.tgz
--rw-r--r--   0 dylan.yang   (502) staff       (20)        1 2023-06-13 19:44:33.000000 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2/py.typed
-drwxr-xr-x   0 dylan.yang   (502) staff       (20)        0 2023-06-13 19:44:37.782902 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2.egg-info/
--rw-r--r--   0 dylan.yang   (502) staff       (20)    24060 2023-06-13 19:44:37.000000 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2.egg-info/PKG-INFO
--rw-r--r--   0 dylan.yang   (502) staff       (20)      523 2023-06-13 19:44:37.000000 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt
--rw-r--r--   0 dylan.yang   (502) staff       (20)        1 2023-06-13 19:44:37.000000 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2.egg-info/dependency_links.txt
--rw-r--r--   0 dylan.yang   (502) staff       (20)      161 2023-06-13 19:44:37.000000 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2.egg-info/requires.txt
--rw-r--r--   0 dylan.yang   (502) staff       (20)       26 2023-06-13 19:44:37.000000 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2.egg-info/top_level.txt
+drwxr-xr-x   0 stephen.firrincieli   (503) staff       (20)        0 2023-07-05 20:00:01.207850 datadog-cdk-constructs-v2-1.7.4/
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)    11358 2023-07-05 19:59:57.000000 datadog-cdk-constructs-v2-1.7.4/LICENSE
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)       23 2023-07-05 19:59:57.000000 datadog-cdk-constructs-v2-1.7.4/MANIFEST.in
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)    24060 2023-07-05 20:00:01.207687 datadog-cdk-constructs-v2-1.7.4/PKG-INFO
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)    23080 2023-07-05 19:59:57.000000 datadog-cdk-constructs-v2-1.7.4/README.md
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)      236 2023-07-05 19:59:57.000000 datadog-cdk-constructs-v2-1.7.4/pyproject.toml
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)       38 2023-07-05 20:00:01.207908 datadog-cdk-constructs-v2-1.7.4/setup.cfg
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)     1921 2023-07-05 19:59:57.000000 datadog-cdk-constructs-v2-1.7.4/setup.py
+drwxr-xr-x   0 stephen.firrincieli   (503) staff       (20)        0 2023-07-05 20:00:01.204037 datadog-cdk-constructs-v2-1.7.4/src/
+drwxr-xr-x   0 stephen.firrincieli   (503) staff       (20)        0 2023-07-05 20:00:01.205419 datadog-cdk-constructs-v2-1.7.4/src/datadog_cdk_constructs_v2/
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)   113679 2023-07-05 19:59:57.000000 datadog-cdk-constructs-v2-1.7.4/src/datadog_cdk_constructs_v2/__init__.py
+drwxr-xr-x   0 stephen.firrincieli   (503) staff       (20)        0 2023-07-05 20:00:01.206670 datadog-cdk-constructs-v2-1.7.4/src/datadog_cdk_constructs_v2/_jsii/
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)      475 2023-07-05 19:59:57.000000 datadog-cdk-constructs-v2-1.7.4/src/datadog_cdk_constructs_v2/_jsii/__init__.py
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)  1309027 2023-07-05 19:59:57.000000 datadog-cdk-constructs-v2-1.7.4/src/datadog_cdk_constructs_v2/_jsii/datadog-cdk-constructs-v2@1.7.4.jsii.tgz
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)        1 2023-07-05 19:59:57.000000 datadog-cdk-constructs-v2-1.7.4/src/datadog_cdk_constructs_v2/py.typed
+drwxr-xr-x   0 stephen.firrincieli   (503) staff       (20)        0 2023-07-05 20:00:01.206318 datadog-cdk-constructs-v2-1.7.4/src/datadog_cdk_constructs_v2.egg-info/
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)    24060 2023-07-05 20:00:00.000000 datadog-cdk-constructs-v2-1.7.4/src/datadog_cdk_constructs_v2.egg-info/PKG-INFO
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)      523 2023-07-05 20:00:01.000000 datadog-cdk-constructs-v2-1.7.4/src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)        1 2023-07-05 20:00:00.000000 datadog-cdk-constructs-v2-1.7.4/src/datadog_cdk_constructs_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)      161 2023-07-05 20:00:01.000000 datadog-cdk-constructs-v2-1.7.4/src/datadog_cdk_constructs_v2.egg-info/requires.txt
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)       26 2023-07-05 20:00:01.000000 datadog-cdk-constructs-v2-1.7.4/src/datadog_cdk_constructs_v2.egg-info/top_level.txt
```

### Comparing `datadog-cdk-constructs-v2-1.7.3/LICENSE` & `datadog-cdk-constructs-v2-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datadog-cdk-constructs-v2-1.7.3/PKG-INFO` & `datadog-cdk-constructs-v2-1.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog-cdk-constructs-v2
-Version: 1.7.3
+Version: 1.7.4
 Summary: CDK Construct Library to automatically instrument Python and Node Lambda functions with Datadog using AWS CDK v2
 Home-page: https://github.com/DataDog/datadog-cdk-constructs
 Author: Datadog
 License: Apache-2.0
 Project-URL: Source, https://github.com/DataDog/datadog-cdk-constructs
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `datadog-cdk-constructs-v2-1.7.3/README.md` & `datadog-cdk-constructs-v2-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `datadog-cdk-constructs-v2-1.7.3/setup.py` & `datadog-cdk-constructs-v2-1.7.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "datadog-cdk-constructs-v2",
-    "version": "1.7.3",
+    "version": "1.7.4",
     "description": "CDK Construct Library to automatically instrument Python and Node Lambda functions with Datadog using AWS CDK v2",
     "license": "Apache-2.0",
     "url": "https://github.com/DataDog/datadog-cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "Datadog",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "datadog_cdk_constructs_v2",
         "datadog_cdk_constructs_v2._jsii"
     ],
     "package_data": {
         "datadog_cdk_constructs_v2._jsii": [
-            "datadog-cdk-constructs-v2@1.7.3.jsii.tgz"
+            "datadog-cdk-constructs-v2@1.7.4.jsii.tgz"
         ],
         "datadog_cdk_constructs_v2": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2/__init__.py` & `datadog-cdk-constructs-v2-1.7.4/src/datadog_cdk_constructs_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2.egg-info/PKG-INFO` & `datadog-cdk-constructs-v2-1.7.4/src/datadog_cdk_constructs_v2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog-cdk-constructs-v2
-Version: 1.7.3
+Version: 1.7.4
 Summary: CDK Construct Library to automatically instrument Python and Node Lambda functions with Datadog using AWS CDK v2
 Home-page: https://github.com/DataDog/datadog-cdk-constructs
 Author: Datadog
 License: Apache-2.0
 Project-URL: Source, https://github.com/DataDog/datadog-cdk-constructs
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt` & `datadog-cdk-constructs-v2-1.7.4/src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/datadog_cdk_constructs_v2/py.typed
 src/datadog_cdk_constructs_v2.egg-info/PKG-INFO
 src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt
 src/datadog_cdk_constructs_v2.egg-info/dependency_links.txt
 src/datadog_cdk_constructs_v2.egg-info/requires.txt
 src/datadog_cdk_constructs_v2.egg-info/top_level.txt
 src/datadog_cdk_constructs_v2/_jsii/__init__.py
-src/datadog_cdk_constructs_v2/_jsii/datadog-cdk-constructs-v2@1.7.3.jsii.tgz
+src/datadog_cdk_constructs_v2/_jsii/datadog-cdk-constructs-v2@1.7.4.jsii.tgz
```

