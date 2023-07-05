# Comparing `tmp/qdrant_haystack-1.0.4.tar.gz` & `tmp/qdrant_haystack-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdrant_haystack-1.0.4.tar", max compression
+gzip compressed data, was "qdrant_haystack-1.0.5.tar", max compression
```

## Comparing `qdrant_haystack-1.0.4.tar` & `qdrant_haystack-1.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-06-26 16:33:42.874713 qdrant_haystack-1.0.4/LICENSE
--rw-r--r--   0        0        0     3160 2023-06-26 16:33:42.874713 qdrant_haystack-1.0.4/README.md
--rw-r--r--   0        0        0      764 2023-06-26 16:33:42.874713 qdrant_haystack-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      100 2023-06-26 16:33:42.874713 qdrant_haystack-1.0.4/src/qdrant_haystack/__init__.py
--rw-r--r--   0        0        0      107 2023-06-26 16:33:42.874713 qdrant_haystack-1.0.4/src/qdrant_haystack/document_stores/__init__.py
--rw-r--r--   0        0        0     2291 2023-06-26 16:33:42.874713 qdrant_haystack-1.0.4/src/qdrant_haystack/document_stores/converters.py
--rw-r--r--   0        0        0     8295 2023-06-26 16:33:42.874713 qdrant_haystack-1.0.4/src/qdrant_haystack/document_stores/filters.py
--rw-r--r--   0        0        0    20377 2023-06-26 16:33:42.874713 qdrant_haystack-1.0.4/src/qdrant_haystack/document_stores/qdrant.py
--rw-r--r--   0        0        0        0 2023-06-26 16:33:42.874713 qdrant_haystack-1.0.4/src/qdrant_haystack/utils.py
--rw-r--r--   0        0        0     3828 1970-01-01 00:00:00.000000 qdrant_haystack-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-05 10:15:50.719409 qdrant_haystack-1.0.5/LICENSE
+-rw-r--r--   0        0        0     3160 2023-07-05 10:15:50.719409 qdrant_haystack-1.0.5/README.md
+-rw-r--r--   0        0        0      864 2023-07-05 10:15:50.723409 qdrant_haystack-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-07-05 10:15:50.723409 qdrant_haystack-1.0.5/src/qdrant_haystack/__init__.py
+-rw-r--r--   0        0        0      107 2023-07-05 10:15:50.723409 qdrant_haystack-1.0.5/src/qdrant_haystack/document_stores/__init__.py
+-rw-r--r--   0        0        0     2291 2023-07-05 10:15:50.723409 qdrant_haystack-1.0.5/src/qdrant_haystack/document_stores/converters.py
+-rw-r--r--   0        0        0     8295 2023-07-05 10:15:50.723409 qdrant_haystack-1.0.5/src/qdrant_haystack/document_stores/filters.py
+-rw-r--r--   0        0        0    20475 2023-07-05 10:15:50.723409 qdrant_haystack-1.0.5/src/qdrant_haystack/document_stores/qdrant.py
+-rw-r--r--   0        0        0        0 2023-07-05 10:15:50.723409 qdrant_haystack-1.0.5/src/qdrant_haystack/utils.py
+-rw-r--r--   0        0        0     3828 1970-01-01 00:00:00.000000 qdrant_haystack-1.0.5/PKG-INFO
```

### Comparing `qdrant_haystack-1.0.4/LICENSE` & `qdrant_haystack-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-1.0.4/README.md` & `qdrant_haystack-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-1.0.4/pyproject.toml` & `qdrant_haystack-1.0.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qdrant-haystack"
-version = "1.0.4"
+version = "1.0.5"
 description = "An integration of Qdrant ANN vector database backend with Haystack"
 authors = ["Kacper Łukawski <kacper.lukawski@qdrant.com>"]
 packages = [
     {include = "qdrant_haystack", from = "src"}
 ]
 readme = "README.md"
 license = "Apache 2.0"
@@ -19,14 +19,17 @@
 pytest = "^7.1"
 pre-commit = "^3.1.0"
 black = "^23.1.0"
 isort = "^5.12.0"
 mypy = "^1.0.1"
 flake8 = "^6.0.0"
 
+[tool.poetry.group.dev.dependencies]
+farm-haystack = {extras = ["inference"], version = "^1.18.1"}
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 minversion = "7.1"
 pythonpath = [
```

### Comparing `qdrant_haystack-1.0.4/src/qdrant_haystack/document_stores/converters.py` & `qdrant_haystack-1.0.5/src/qdrant_haystack/document_stores/converters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-1.0.4/src/qdrant_haystack/document_stores/filters.py` & `qdrant_haystack-1.0.5/src/qdrant_haystack/document_stores/filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-1.0.4/src/qdrant_haystack/document_stores/qdrant.py` & `qdrant_haystack-1.0.5/src/qdrant_haystack/document_stores/qdrant.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 from typing import Any, Dict, Generator, List, Optional, Union, cast
 
 import numpy as np
 import qdrant_client
 from grpc import RpcError
 from haystack import Document, Label
 from haystack.document_stores import BaseDocumentStore
-from haystack.document_stores.base import get_batches_from_generator
+
+try:
+    from haystack.utils.batching import get_batches_from_generator
+except ImportError:
+    from haystack.document_stores.base import get_batches_from_generator
+
 from haystack.errors import DocumentStoreError
 from haystack.nodes import DenseRetriever
 from haystack.schema import FilterType
 from qdrant_client import grpc
 from qdrant_client.http import models as rest
 from qdrant_client.http.exceptions import UnexpectedResponse
 from tqdm import tqdm
```

### Comparing `qdrant_haystack-1.0.4/PKG-INFO` & `qdrant_haystack-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdrant-haystack
-Version: 1.0.4
+Version: 1.0.5
 Summary: An integration of Qdrant ANN vector database backend with Haystack
 License: Apache 2.0
 Author: Kacper Łukawski
 Author-email: kacper.lukawski@qdrant.com
 Requires-Python: >=3.8.1,<=3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

