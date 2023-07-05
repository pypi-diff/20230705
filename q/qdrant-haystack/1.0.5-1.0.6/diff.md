# Comparing `tmp/qdrant_haystack-1.0.5.tar.gz` & `tmp/qdrant_haystack-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdrant_haystack-1.0.5.tar", max compression
+gzip compressed data, was "qdrant_haystack-1.0.6.tar", max compression
```

## Comparing `qdrant_haystack-1.0.5.tar` & `qdrant_haystack-1.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-07-05 10:15:50.719409 qdrant_haystack-1.0.5/LICENSE
--rw-r--r--   0        0        0     3160 2023-07-05 10:15:50.719409 qdrant_haystack-1.0.5/README.md
--rw-r--r--   0        0        0      864 2023-07-05 10:15:50.723409 qdrant_haystack-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      100 2023-07-05 10:15:50.723409 qdrant_haystack-1.0.5/src/qdrant_haystack/__init__.py
--rw-r--r--   0        0        0      107 2023-07-05 10:15:50.723409 qdrant_haystack-1.0.5/src/qdrant_haystack/document_stores/__init__.py
--rw-r--r--   0        0        0     2291 2023-07-05 10:15:50.723409 qdrant_haystack-1.0.5/src/qdrant_haystack/document_stores/converters.py
--rw-r--r--   0        0        0     8295 2023-07-05 10:15:50.723409 qdrant_haystack-1.0.5/src/qdrant_haystack/document_stores/filters.py
--rw-r--r--   0        0        0    20475 2023-07-05 10:15:50.723409 qdrant_haystack-1.0.5/src/qdrant_haystack/document_stores/qdrant.py
--rw-r--r--   0        0        0        0 2023-07-05 10:15:50.723409 qdrant_haystack-1.0.5/src/qdrant_haystack/utils.py
--rw-r--r--   0        0        0     3828 1970-01-01 00:00:00.000000 qdrant_haystack-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-05 13:13:09.946870 qdrant_haystack-1.0.6/LICENSE
+-rw-r--r--   0        0        0     3160 2023-07-05 13:13:09.946870 qdrant_haystack-1.0.6/README.md
+-rw-r--r--   0        0        0      863 2023-07-05 13:13:09.946870 qdrant_haystack-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-07-05 13:13:09.946870 qdrant_haystack-1.0.6/src/qdrant_haystack/__init__.py
+-rw-r--r--   0        0        0      107 2023-07-05 13:13:09.946870 qdrant_haystack-1.0.6/src/qdrant_haystack/document_stores/__init__.py
+-rw-r--r--   0        0        0     2291 2023-07-05 13:13:09.946870 qdrant_haystack-1.0.6/src/qdrant_haystack/document_stores/converters.py
+-rw-r--r--   0        0        0     8295 2023-07-05 13:13:09.950870 qdrant_haystack-1.0.6/src/qdrant_haystack/document_stores/filters.py
+-rw-r--r--   0        0        0    20475 2023-07-05 13:13:09.950870 qdrant_haystack-1.0.6/src/qdrant_haystack/document_stores/qdrant.py
+-rw-r--r--   0        0        0        0 2023-07-05 13:13:09.950870 qdrant_haystack-1.0.6/src/qdrant_haystack/utils.py
+-rw-r--r--   0        0        0     3827 1970-01-01 00:00:00.000000 qdrant_haystack-1.0.6/PKG-INFO
```

### Comparing `qdrant_haystack-1.0.5/LICENSE` & `qdrant_haystack-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-1.0.5/README.md` & `qdrant_haystack-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-1.0.5/pyproject.toml` & `qdrant_haystack-1.0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "qdrant-haystack"
-version = "1.0.5"
+version = "1.0.6"
 description = "An integration of Qdrant ANN vector database backend with Haystack"
 authors = ["Kacper Łukawski <kacper.lukawski@qdrant.com>"]
 packages = [
     {include = "qdrant_haystack", from = "src"}
 ]
 readme = "README.md"
 license = "Apache 2.0"
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<=3.11"
+python = ">=3.8.1,<3.12"
 qdrant-client = "^1.1.4"
 farm-haystack = "^1.13.0"
 torch = "<=2.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1"
 pre-commit = "^3.1.0"
```

### Comparing `qdrant_haystack-1.0.5/src/qdrant_haystack/document_stores/converters.py` & `qdrant_haystack-1.0.6/src/qdrant_haystack/document_stores/converters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-1.0.5/src/qdrant_haystack/document_stores/filters.py` & `qdrant_haystack-1.0.6/src/qdrant_haystack/document_stores/filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-1.0.5/src/qdrant_haystack/document_stores/qdrant.py` & `qdrant_haystack-1.0.6/src/qdrant_haystack/document_stores/qdrant.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-1.0.5/PKG-INFO` & `qdrant_haystack-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: qdrant-haystack
-Version: 1.0.5
+Version: 1.0.6
 Summary: An integration of Qdrant ANN vector database backend with Haystack
 License: Apache 2.0
 Author: Kacper Łukawski
 Author-email: kacper.lukawski@qdrant.com
-Requires-Python: >=3.8.1,<=3.11
+Requires-Python: >=3.8.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: farm-haystack (>=1.13.0,<2.0.0)
 Requires-Dist: qdrant-client (>=1.1.4,<2.0.0)
```

