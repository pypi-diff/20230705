# Comparing `tmp/retake-0.1.1.dev0.tar.gz` & `tmp/retake-0.1.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retake-0.1.1.dev0.tar", max compression
+gzip compressed data, was "retake-0.1.2.dev0.tar", max compression
```

## Comparing `retake-0.1.1.dev0.tar` & `retake-0.1.2.dev0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1454 2023-07-05 01:31:03.009679 retake-0.1.1.dev0/README.md
--rw-r--r--   0        0        0        0 2023-07-05 01:31:03.011094 retake-0.1.1.dev0/core/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 01:31:03.011248 retake-0.1.1.dev0/core/extract/__init__.py
--rw-r--r--   0        0        0     1494 2023-07-05 01:31:03.011534 retake-0.1.1.dev0/core/extract/postgres.py
--rw-r--r--   0        0        0        0 2023-07-05 01:31:03.011590 retake-0.1.1.dev0/core/load/__init__.py
--rw-r--r--   0        0        0     5122 2023-07-05 14:30:44.151482 retake-0.1.1.dev0/core/load/elasticsearch.py
--rw-r--r--   0        0        0      225 2023-07-05 01:31:03.012046 retake-0.1.1.dev0/core/load/opensearch.py
--rw-r--r--   0        0        0        0 2023-07-05 01:31:03.012095 retake-0.1.1.dev0/core/transform/__init__.py
--rw-r--r--   0        0        0      263 2023-07-05 01:31:03.012356 retake-0.1.1.dev0/core/transform/embedding.py
--rw-r--r--   0        0        0      425 2023-07-05 17:32:23.323421 retake-0.1.1.dev0/pyproject.toml
--rw-r--r--   0        0        0      288 2023-07-05 17:32:03.435359 retake-0.1.1.dev0/retake/__init__.py
--rw-r--r--   0        0        0      235 2023-07-03 18:27:13.908241 retake-0.1.1.dev0/retake/embedding.py
--rw-r--r--   0        0        0     2060 2023-07-05 17:32:03.434299 retake-0.1.1.dev0/retake/pipeline.py
--rw-r--r--   0        0        0      662 2023-07-05 14:43:12.228036 retake-0.1.1.dev0/retake/sink.py
--rw-r--r--   0        0        0      384 2023-07-03 18:27:13.908355 retake-0.1.1.dev0/retake/source.py
--rw-r--r--   0        0        0      356 2023-07-05 14:43:12.224740 retake-0.1.1.dev0/retake/target.py
--rw-r--r--   0        0        0      752 2023-07-05 01:31:03.011031 retake-0.1.1.dev0/retake/transform.py
--rw-r--r--   0        0        0     1876 1970-01-01 00:00:00.000000 retake-0.1.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1454 2023-07-05 01:31:03.009679 retake-0.1.2.dev0/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 01:31:03.011094 retake-0.1.2.dev0/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 01:31:03.011248 retake-0.1.2.dev0/core/extract/__init__.py
+-rw-r--r--   0        0        0     1494 2023-07-05 01:31:03.011534 retake-0.1.2.dev0/core/extract/postgres.py
+-rw-r--r--   0        0        0        0 2023-07-05 01:31:03.011590 retake-0.1.2.dev0/core/load/__init__.py
+-rw-r--r--   0        0        0     5122 2023-07-05 14:30:44.151482 retake-0.1.2.dev0/core/load/elasticsearch.py
+-rw-r--r--   0        0        0      225 2023-07-05 01:31:03.012046 retake-0.1.2.dev0/core/load/opensearch.py
+-rw-r--r--   0        0        0        0 2023-07-05 01:31:03.012095 retake-0.1.2.dev0/core/transform/__init__.py
+-rw-r--r--   0        0        0      263 2023-07-05 01:31:03.012356 retake-0.1.2.dev0/core/transform/embedding.py
+-rw-r--r--   0        0        0      425 2023-07-05 17:32:53.070339 retake-0.1.2.dev0/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-07-05 17:32:03.435359 retake-0.1.2.dev0/retake/__init__.py
+-rw-r--r--   0        0        0      235 2023-07-03 18:27:13.908241 retake-0.1.2.dev0/retake/embedding.py
+-rw-r--r--   0        0        0     2067 2023-07-05 17:32:47.123824 retake-0.1.2.dev0/retake/pipeline.py
+-rw-r--r--   0        0        0      662 2023-07-05 14:43:12.228036 retake-0.1.2.dev0/retake/sink.py
+-rw-r--r--   0        0        0      384 2023-07-03 18:27:13.908355 retake-0.1.2.dev0/retake/source.py
+-rw-r--r--   0        0        0      356 2023-07-05 14:43:12.224740 retake-0.1.2.dev0/retake/target.py
+-rw-r--r--   0        0        0      752 2023-07-05 01:31:03.011031 retake-0.1.2.dev0/retake/transform.py
+-rw-r--r--   0        0        0     1876 1970-01-01 00:00:00.000000 retake-0.1.2.dev0/PKG-INFO
```

### Comparing `retake-0.1.1.dev0/README.md` & `retake-0.1.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `retake-0.1.1.dev0/core/extract/postgres.py` & `retake-0.1.2.dev0/core/extract/postgres.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.1.dev0/core/load/elasticsearch.py` & `retake-0.1.2.dev0/core/load/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.1.dev0/retake/pipeline.py` & `retake-0.1.2.dev0/retake/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union
+from typing import Union, Tuple
 
 from retake.embedding import OpenAI
 from retake.source import PostgresSource
 from retake.transform import PostgresTransform
 from retake.sink import ElasticSearchSink
 from retake.target import ElasticSearchTarget
 from core.load.elasticsearch import ElasticSearchLoader
```

### Comparing `retake-0.1.1.dev0/retake/sink.py` & `retake-0.1.2.dev0/retake/sink.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.1.dev0/retake/transform.py` & `retake-0.1.2.dev0/retake/transform.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.1.dev0/PKG-INFO` & `retake-0.1.2.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retake
-Version: 0.1.1.dev0
+Version: 0.1.2.dev0
 Summary: Real-time pipelines for vectors
 Author: Ming Ying
 Author-email: ming.ying.nyc@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

