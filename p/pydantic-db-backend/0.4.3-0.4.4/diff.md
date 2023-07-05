# Comparing `tmp/pydantic_db_backend-0.4.3.tar.gz` & `tmp/pydantic_db_backend-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_db_backend-0.4.3.tar", max compression
+gzip compressed data, was "pydantic_db_backend-0.4.4.tar", max compression
```

## Comparing `pydantic_db_backend-0.4.3.tar` & `pydantic_db_backend-0.4.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       87 2023-06-14 17:15:43.151729 pydantic_db_backend-0.4.3/README.md
--rw-r--r--   0        0        0        0 2023-05-11 08:45:17.171212 pydantic_db_backend-0.4.3/pydantic_db_backend/__init__.py
--rw-r--r--   0        0        0     6222 2023-06-28 07:49:52.142216 pydantic_db_backend-0.4.3/pydantic_db_backend/backend.py
--rw-r--r--   0        0        0        0 2023-05-13 10:06:57.338481 pydantic_db_backend-0.4.3/pydantic_db_backend/backends/__init__.py
--rw-r--r--   0        0        0     6047 2023-06-28 09:24:42.810581 pydantic_db_backend-0.4.3/pydantic_db_backend/backends/couchdb.py
--rw-r--r--   0        0        0      100 2023-06-14 12:06:00.522425 pydantic_db_backend-0.4.3/pydantic_db_backend/backends/json_files.py
--rw-r--r--   0        0        0      701 2023-06-20 16:53:47.237618 pydantic_db_backend-0.4.3/pydantic_db_backend/exceptions/__init__.py
--rw-r--r--   0        0        0     1192 2023-06-28 08:36:47.839745 pydantic_db_backend-0.4.3/pydantic_db_backend/utils.py
--rw-r--r--   0        0        0      996 2023-07-03 14:21:11.829497 pydantic_db_backend-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 pydantic_db_backend-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-06-14 17:15:43.151729 pydantic_db_backend-0.4.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 08:45:17.171212 pydantic_db_backend-0.4.4/pydantic_db_backend/__init__.py
+-rw-r--r--   0        0        0     6182 2023-07-05 12:04:36.107157 pydantic_db_backend-0.4.4/pydantic_db_backend/backend.py
+-rw-r--r--   0        0        0        0 2023-05-13 10:06:57.338481 pydantic_db_backend-0.4.4/pydantic_db_backend/backends/__init__.py
+-rw-r--r--   0        0        0     6047 2023-06-28 09:24:42.810581 pydantic_db_backend-0.4.4/pydantic_db_backend/backends/couchdb.py
+-rw-r--r--   0        0        0      100 2023-06-14 12:06:00.522425 pydantic_db_backend-0.4.4/pydantic_db_backend/backends/json_files.py
+-rw-r--r--   0        0        0      701 2023-06-20 16:53:47.237618 pydantic_db_backend-0.4.4/pydantic_db_backend/exceptions/__init__.py
+-rw-r--r--   0        0        0     1192 2023-06-28 08:36:47.839745 pydantic_db_backend-0.4.4/pydantic_db_backend/utils.py
+-rw-r--r--   0        0        0      996 2023-07-05 12:05:58.214172 pydantic_db_backend-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 pydantic_db_backend-0.4.4/PKG-INFO
```

### Comparing `pydantic_db_backend-0.4.3/pydantic_db_backend/backend.py` & `pydantic_db_backend-0.4.4/pydantic_db_backend/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from __future__ import annotations
 
 import contextlib
 import datetime
 import json
+import logging
 import re
 from contextvars import ContextVar
 from typing import Type, Dict, List
 
 from dotenv import load_dotenv
-import logging
-
-from freezegun.api import FakeDatetime
 from pydantic import BaseModel, Field
 
 from pydantic_db_backend.utils import uid, utcnow, str_to_datetime_if_parseable
 
 log = logging.getLogger(__name__)
 
 backend_context_var = ContextVar('backend_context_var')
```

### Comparing `pydantic_db_backend-0.4.3/pydantic_db_backend/backends/couchdb.py` & `pydantic_db_backend-0.4.4/pydantic_db_backend/backends/couchdb.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.4.3/pydantic_db_backend/exceptions/__init__.py` & `pydantic_db_backend-0.4.4/pydantic_db_backend/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.4.3/pydantic_db_backend/utils.py` & `pydantic_db_backend-0.4.4/pydantic_db_backend/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.4.3/pyproject.toml` & `pydantic_db_backend-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-db-backend"
-version = "0.4.3"
+version = "0.4.4"
 description = ""
 authors = ["Marco Bartel <bsimpson888@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-dotenv = "^0.15.0"
```

### Comparing `pydantic_db_backend-0.4.3/PKG-INFO` & `pydantic_db_backend-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-db-backend
-Version: 0.4.3
+Version: 0.4.4
 Summary: 
 Author: Marco Bartel
 Author-email: bsimpson888@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: couchdb
```

