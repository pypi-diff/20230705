# Comparing `tmp/vectordb-0.0.3.dev4.tar.gz` & `tmp/vectordb-0.0.3.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectordb-0.0.3.dev4.tar", last modified: Wed Jul  5 12:41:35 2023, max compression
+gzip compressed data, was "vectordb-0.0.3.dev5.tar", last modified: Wed Jul  5 12:41:51 2023, max compression
```

## Comparing `vectordb-0.0.3.dev4.tar` & `vectordb-0.0.3.dev5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:35.858640 vectordb-0.0.3.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-05 12:41:35.854640 vectordb-0.0.3.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 12:41:35.858640 vectordb-0.0.3.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:35.850640 vectordb-0.0.3.dev4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:35.850640 vectordb-0.0.3.dev4/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/tests/integration/test_hnswlib_vectordb_serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/tests/integration/test_inmemory_vectordb_serve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:35.854640 vectordb-0.0.3.dev4/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/tests/unit/test_hnswlib_vectordb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/tests/unit/test_inmemory_vectordb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:35.854640 vectordb-0.0.3.dev4/vectordb/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-05 12:41:35.000000 vectordb-0.0.3.dev4/vectordb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/vectordb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:35.854640 vectordb-0.0.3.dev4/vectordb/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/vectordb/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/vectordb/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:35.854640 vectordb-0.0.3.dev4/vectordb/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/vectordb/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/vectordb/db/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:35.854640 vectordb-0.0.3.dev4/vectordb/db/executors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/vectordb/db/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/vectordb/db/executors/hnsw_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/vectordb/db/executors/inmemory_exact_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/vectordb/db/executors/typed_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/vectordb/db/hnsw_vectordb.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/vectordb/db/inmemory_exact_vectordb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/vectordb/db/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:35.854640 vectordb-0.0.3.dev4/vectordb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/vectordb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/vectordb/utils/create_doc_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/vectordb/utils/pass_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/vectordb/utils/push_to_hubble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/vectordb/utils/sort_matches_by_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-05 12:41:30.000000 vectordb-0.0.3.dev4/vectordb/utils/unify_input_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:35.854640 vectordb-0.0.3.dev4/vectordb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-05 12:41:35.000000 vectordb-0.0.3.dev4/vectordb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-05 12:41:35.000000 vectordb-0.0.3.dev4/vectordb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 12:41:35.000000 vectordb-0.0.3.dev4/vectordb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-05 12:41:35.000000 vectordb-0.0.3.dev4/vectordb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 12:41:35.000000 vectordb-0.0.3.dev4/vectordb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 12:41:35.000000 vectordb-0.0.3.dev4/vectordb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:51.091257 vectordb-0.0.3.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-05 12:41:51.091257 vectordb-0.0.3.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13202 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 12:41:51.091257 vectordb-0.0.3.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:51.087257 vectordb-0.0.3.dev5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:51.087257 vectordb-0.0.3.dev5/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/tests/integration/test_hnswlib_vectordb_serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/tests/integration/test_inmemory_vectordb_serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:51.087257 vectordb-0.0.3.dev5/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/tests/unit/test_hnswlib_vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/tests/unit/test_inmemory_vectordb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:51.087257 vectordb-0.0.3.dev5/vectordb/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-05 12:41:50.000000 vectordb-0.0.3.dev5/vectordb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:51.087257 vectordb-0.0.3.dev5/vectordb/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:51.087257 vectordb-0.0.3.dev5/vectordb/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/db/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:51.087257 vectordb-0.0.3.dev5/vectordb/db/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/db/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/db/executors/hnsw_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/db/executors/inmemory_exact_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/db/executors/typed_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/db/hnsw_vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/db/inmemory_exact_vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/db/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:51.091257 vectordb-0.0.3.dev5/vectordb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/utils/create_doc_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/utils/pass_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/utils/push_to_hubble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/utils/sort_matches_by_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/utils/unify_input_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:51.087257 vectordb-0.0.3.dev5/vectordb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-05 12:41:51.000000 vectordb-0.0.3.dev5/vectordb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-05 12:41:51.000000 vectordb-0.0.3.dev5/vectordb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 12:41:51.000000 vectordb-0.0.3.dev5/vectordb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-05 12:41:51.000000 vectordb-0.0.3.dev5/vectordb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 12:41:51.000000 vectordb-0.0.3.dev5/vectordb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 12:41:51.000000 vectordb-0.0.3.dev5/vectordb.egg-info/top_level.txt
```

### Comparing `vectordb-0.0.3.dev4/LICENSE` & `vectordb-0.0.3.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev4/PKG-INFO` & `vectordb-0.0.3.dev5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectordb
-Version: 0.0.3.dev4
+Version: 0.0.3.dev5
 Summary: The Python VectorDB. Build your vector database from working as a library to scaling as a database in the cloud
 Home-page: https://github.com/jina-ai/vectordb/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/vectordb/tags
 Platform: UNKNOWN
```

### Comparing `vectordb-0.0.3.dev4/README.md` & `vectordb-0.0.3.dev5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     embedding: NdArray[128]
 
 
 db = InMemoryExactNNVectorDB[MyDoc](workspace='./vectordb') # notice how `db` is the instance that we want to serve
 
 if __name__ == '__main__':
     # make sure to protect this part of the code
-    with app.serve() as service:
+    with db.serve() as service:
         service.block()
 ```
 
 
 | Description | Command | 
 | --- | ---: |
 | Serve your app locally | `vectordb serve --db example:db` |
```

### Comparing `vectordb-0.0.3.dev4/setup.py` & `vectordb-0.0.3.dev5/setup.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev4/tests/integration/test_hnswlib_vectordb_serve.py` & `vectordb-0.0.3.dev5/tests/integration/test_hnswlib_vectordb_serve.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev4/tests/integration/test_inmemory_vectordb_serve.py` & `vectordb-0.0.3.dev5/tests/integration/test_inmemory_vectordb_serve.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev4/tests/unit/test_hnswlib_vectordb.py` & `vectordb-0.0.3.dev5/tests/unit/test_hnswlib_vectordb.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev4/tests/unit/test_inmemory_vectordb.py` & `vectordb-0.0.3.dev5/tests/unit/test_inmemory_vectordb.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev4/vectordb/__main__.py` & `vectordb-0.0.3.dev5/vectordb/__main__.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev4/vectordb/client/client.py` & `vectordb-0.0.3.dev5/vectordb/client/client.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev4/vectordb/db/base.py` & `vectordb-0.0.3.dev5/vectordb/db/base.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev4/vectordb/db/executors/hnsw_indexer.py` & `vectordb-0.0.3.dev5/vectordb/db/executors/hnsw_indexer.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev4/vectordb/db/executors/inmemory_exact_indexer.py` & `vectordb-0.0.3.dev5/vectordb/db/executors/inmemory_exact_indexer.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev4/vectordb/db/executors/typed_executor.py` & `vectordb-0.0.3.dev5/vectordb/db/executors/typed_executor.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev4/vectordb/db/service.py` & `vectordb-0.0.3.dev5/vectordb/db/service.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev4/vectordb/utils/create_doc_type.py` & `vectordb-0.0.3.dev5/vectordb/utils/create_doc_type.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev4/vectordb/utils/pass_parameters.py` & `vectordb-0.0.3.dev5/vectordb/utils/pass_parameters.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev4/vectordb/utils/push_to_hubble.py` & `vectordb-0.0.3.dev5/vectordb/utils/push_to_hubble.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev4/vectordb/utils/sort_matches_by_score.py` & `vectordb-0.0.3.dev5/vectordb/utils/sort_matches_by_score.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev4/vectordb/utils/unify_input_output.py` & `vectordb-0.0.3.dev5/vectordb/utils/unify_input_output.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev4/vectordb.egg-info/PKG-INFO` & `vectordb-0.0.3.dev5/vectordb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectordb
-Version: 0.0.3.dev4
+Version: 0.0.3.dev5
 Summary: The Python VectorDB. Build your vector database from working as a library to scaling as a database in the cloud
 Home-page: https://github.com/jina-ai/vectordb/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/vectordb/tags
 Platform: UNKNOWN
```

### Comparing `vectordb-0.0.3.dev4/vectordb.egg-info/SOURCES.txt` & `vectordb-0.0.3.dev5/vectordb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

