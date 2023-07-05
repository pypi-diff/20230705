# Comparing `tmp/talk_codebase-0.1.41.tar.gz` & `tmp/talk_codebase-0.1.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.41.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.42.tar", max compression
```

## Comparing `talk_codebase-0.1.41.tar` & `talk_codebase-0.1.42.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3183 2023-07-05 02:23:05.047333 talk_codebase-0.1.41/README.md
--rw-r--r--   0        0        0      986 2023-07-05 02:23:05.047333 talk_codebase-0.1.41/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-05 02:23:05.047333 talk_codebase-0.1.41/talk_codebase/__init__.py
--rw-r--r--   0        0        0     1353 2023-07-05 02:23:05.047333 talk_codebase-0.1.41/talk_codebase/cli.py
--rw-r--r--   0        0        0     2250 2023-07-05 02:23:05.047333 talk_codebase-0.1.41/talk_codebase/config.py
--rw-r--r--   0        0        0     1926 2023-07-05 02:23:05.047333 talk_codebase-0.1.41/talk_codebase/consts.py
--rw-r--r--   0        0        0     5695 2023-07-05 02:23:05.047333 talk_codebase-0.1.41/talk_codebase/llm.py
--rw-r--r--   0        0        0     2256 2023-07-05 02:23:05.047333 talk_codebase-0.1.41/talk_codebase/utils.py
--rw-r--r--   0        0        0     4237 1970-01-01 00:00:00.000000 talk_codebase-0.1.41/PKG-INFO
+-rw-r--r--   0        0        0     3183 2023-07-05 11:00:37.949703 talk_codebase-0.1.42/README.md
+-rw-r--r--   0        0        0      984 2023-07-05 11:00:37.953703 talk_codebase-0.1.42/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-05 11:00:37.953703 talk_codebase-0.1.42/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     1353 2023-07-05 11:00:37.953703 talk_codebase-0.1.42/talk_codebase/cli.py
+-rw-r--r--   0        0        0     2250 2023-07-05 11:00:37.953703 talk_codebase-0.1.42/talk_codebase/config.py
+-rw-r--r--   0        0        0     1946 2023-07-05 11:00:37.953703 talk_codebase-0.1.42/talk_codebase/consts.py
+-rw-r--r--   0        0        0     4921 2023-07-05 11:00:37.953703 talk_codebase-0.1.42/talk_codebase/llm.py
+-rw-r--r--   0        0        0     2256 2023-07-05 11:00:37.953703 talk_codebase-0.1.42/talk_codebase/utils.py
+-rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 talk_codebase-0.1.42/PKG-INFO
```

### Comparing `talk_codebase-0.1.41/README.md` & `talk_codebase-0.1.42/README.md`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.41/pyproject.toml` & `talk_codebase-0.1.42/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.41"
+version = "0.1.42"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
@@ -17,16 +17,15 @@
 urllib3 = "1.26.6"
 gitpython = "^3.1.31"
 questionary = "^1.10.0"
 sentence-transformers = "^2.2.2"
 unstructured = "^0.6.10"
 gpt4all = "^1.0.1"
 langchain = "^0.0.223"
-llama-cpp-python = "^0.1.67"
-
+llama-cpp-python = "0.1.68"
 
 [tool.poetry.group.dev.dependencies]
 setuptools = "^68.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `talk_codebase-0.1.41/talk_codebase/cli.py` & `talk_codebase-0.1.42/talk_codebase/cli.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.41/talk_codebase/config.py` & `talk_codebase-0.1.42/talk_codebase/config.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.41/talk_codebase/consts.py` & `talk_codebase-0.1.42/talk_codebase/consts.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "chunk_size": "2056",
     "chunk_overlap": "256",
     "k": "1",
     "temperature": "0.7",
     "openai_model_name": DEFAULT_OPENAI_MODEL,
     "local_model_name": DEFAULT_LOCAL_MODEL,
     "model_path": DEFAULT_MODEL_DIRECTORY,
+    "n_batch": "8",
 }
 
 LOADER_MAPPING = {
     ".csv": {
         "loader": CSVLoader,
         "args": {}
     },
```

### Comparing `talk_codebase-0.1.41/talk_codebase/utils.py` & `talk_codebase-0.1.42/talk_codebase/utils.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.41/PKG-INFO` & `talk_codebase-0.1.42/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.41
+Version: 0.1.42
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: gpt4all (>=1.0.1,<2.0.0)
 Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: langchain (>=0.0.223,<0.0.224)
-Requires-Dist: llama-cpp-python (>=0.1.67,<0.2.0)
+Requires-Dist: llama-cpp-python (==0.1.68)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Requires-Dist: unstructured (>=0.6.10,<0.7.0)
 Requires-Dist: urllib3 (==1.26.6)
 Description-Content-Type: text/markdown
```

