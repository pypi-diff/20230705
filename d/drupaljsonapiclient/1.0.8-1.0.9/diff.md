# Comparing `tmp/drupaljsonapiclient-1.0.8.tar.gz` & `tmp/drupaljsonapiclient-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drupaljsonapiclient-1.0.8.tar", max compression
+gzip compressed data, was "drupaljsonapiclient-1.0.9.tar", max compression
```

## Comparing `drupaljsonapiclient-1.0.8.tar` & `drupaljsonapiclient-1.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1690 2023-06-27 02:06:45.257616 drupaljsonapiclient-1.0.8/LICENSE
--rw-r--r--   0        0        0     1244 2023-06-27 02:06:45.257616 drupaljsonapiclient-1.0.8/README.md
--rw-r--r--   0        0        0      156 2023-06-27 02:06:45.257616 drupaljsonapiclient-1.0.8/drupaljsonapiclient/__init__.py
--rw-r--r--   0        0        0     3605 2023-06-27 02:06:45.257616 drupaljsonapiclient-1.0.8/drupaljsonapiclient/common.py
--rw-r--r--   0        0        0     4383 2023-06-27 02:06:45.257616 drupaljsonapiclient-1.0.8/drupaljsonapiclient/document.py
--rw-r--r--   0        0        0      620 2023-06-27 02:06:45.257616 drupaljsonapiclient-1.0.8/drupaljsonapiclient/exceptions.py
--rw-r--r--   0        0        0     3145 2023-06-27 02:06:45.257616 drupaljsonapiclient-1.0.8/drupaljsonapiclient/filter.py
--rw-r--r--   0        0        0     4283 2023-06-27 02:06:45.258616 drupaljsonapiclient-1.0.8/drupaljsonapiclient/objects.py
--rw-r--r--   0        0        0    14266 2023-06-27 02:06:45.258616 drupaljsonapiclient-1.0.8/drupaljsonapiclient/relationships.py
--rw-r--r--   0        0        0    26615 2023-06-27 02:06:45.258616 drupaljsonapiclient-1.0.8/drupaljsonapiclient/resourceobject.py
--rw-r--r--   0        0        0    28112 2023-06-27 02:06:45.258616 drupaljsonapiclient-1.0.8/drupaljsonapiclient/session.py
--rw-r--r--   0        0        0     1008 2023-06-27 02:06:45.259616 drupaljsonapiclient-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     2206 1970-01-01 00:00:00.000000 drupaljsonapiclient-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1690 2023-07-03 15:57:46.902012 drupaljsonapiclient-1.0.9/LICENSE
+-rw-r--r--   0        0        0     1244 2023-07-03 15:57:46.902012 drupaljsonapiclient-1.0.9/README.md
+-rw-r--r--   0        0        0      156 2023-07-03 15:57:46.902012 drupaljsonapiclient-1.0.9/drupaljsonapiclient/__init__.py
+-rw-r--r--   0        0        0     3605 2023-07-03 15:57:46.902012 drupaljsonapiclient-1.0.9/drupaljsonapiclient/common.py
+-rw-r--r--   0        0        0     4383 2023-07-03 15:57:46.902012 drupaljsonapiclient-1.0.9/drupaljsonapiclient/document.py
+-rw-r--r--   0        0        0      620 2023-07-03 15:57:46.902012 drupaljsonapiclient-1.0.9/drupaljsonapiclient/exceptions.py
+-rw-r--r--   0        0        0     3145 2023-07-03 15:57:46.902012 drupaljsonapiclient-1.0.9/drupaljsonapiclient/filter.py
+-rw-r--r--   0        0        0     4283 2023-07-03 15:57:46.902012 drupaljsonapiclient-1.0.9/drupaljsonapiclient/objects.py
+-rw-r--r--   0        0        0    14266 2023-07-03 15:57:46.902012 drupaljsonapiclient-1.0.9/drupaljsonapiclient/relationships.py
+-rw-r--r--   0        0        0    26615 2023-07-03 15:57:46.902012 drupaljsonapiclient-1.0.9/drupaljsonapiclient/resourceobject.py
+-rw-r--r--   0        0        0    28123 2023-07-03 15:57:46.903012 drupaljsonapiclient-1.0.9/drupaljsonapiclient/session.py
+-rw-r--r--   0        0        0     1066 2023-07-03 15:57:46.904012 drupaljsonapiclient-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2164 1970-01-01 00:00:00.000000 drupaljsonapiclient-1.0.9/PKG-INFO
```

### Comparing `drupaljsonapiclient-1.0.8/LICENSE` & `drupaljsonapiclient-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.8/README.md` & `drupaljsonapiclient-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.8/drupaljsonapiclient/common.py` & `drupaljsonapiclient-1.0.9/drupaljsonapiclient/common.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.8/drupaljsonapiclient/document.py` & `drupaljsonapiclient-1.0.9/drupaljsonapiclient/document.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.8/drupaljsonapiclient/exceptions.py` & `drupaljsonapiclient-1.0.9/drupaljsonapiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.8/drupaljsonapiclient/filter.py` & `drupaljsonapiclient-1.0.9/drupaljsonapiclient/filter.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.8/drupaljsonapiclient/objects.py` & `drupaljsonapiclient-1.0.9/drupaljsonapiclient/objects.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.8/drupaljsonapiclient/relationships.py` & `drupaljsonapiclient-1.0.9/drupaljsonapiclient/relationships.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.8/drupaljsonapiclient/resourceobject.py` & `drupaljsonapiclient-1.0.9/drupaljsonapiclient/resourceobject.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.8/drupaljsonapiclient/session.py` & `drupaljsonapiclient-1.0.9/drupaljsonapiclient/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,14 @@
     TYPE_CHECKING, Set, Optional, Tuple, Dict, Union, Iterable,
     AsyncIterable, Awaitable, AsyncIterator, Iterator, List, IO
 )
 from urllib.parse import ParseResult, urlparse
 
 from pathlib import Path
 
-import aiofiles
-
 import jsonschema
 
 from .common import jsonify_attribute_name, error_from_response, \
     HttpStatus, HttpMethod
 from .exceptions import DocumentError, AsyncError
 
 if TYPE_CHECKING:
@@ -114,14 +112,15 @@
         self.resources_by_resource_identifier: \
             'Dict[Tuple[str, str], ResourceObject]' = {}
         self.resources_by_link: 'Dict[str, ResourceObject]' = {}
         self.documents_by_link: 'Dict[str, Document]' = {}
         self.schema: Schema = Schema(schema)
         if enable_async:
             import aiohttp
+            import aiofiles
             self._aiohttp_session = aiohttp.ClientSession(loop=loop)
         self.use_relationship_iterator = use_relationship_iterator
 
     def add_resources(self, *resources: 'ResourceObject') -> None:
         """
         Add resources to session cache.
         """
```

### Comparing `drupaljsonapiclient-1.0.8/pyproject.toml` & `drupaljsonapiclient-1.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "drupaljsonapiclient"
-version = "1.0.8"
+version = "1.0.9"
 description = "Drupal CMS JSON:API client for Python."
 authors = ["Martins Bruvelis <martins.bruvelis@gmail.com>"]
 readme = "README.md"
 packages = [{include = "drupaljsonapiclient"}]
 repository = "https://gitlab.com/martins-bruvelis/drupaljsonapiclient"
 documentation = "https://gitlab.com/martins-bruvelis/drupaljsonapiclient/-/blob/main/README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.31.0"
-aiohttp = "^3.8.4"
-jsonmerge = "^1.9.0"
-aiofiles = "^23.1.0"
 jsonschema = "^4.17.3"
+aiohttp = {version = "^3.8.4", optional = true}
+aiofiles = {version = "^23.1.0", optional = true}
 
 
 [tool.poetry.group.dev.dependencies]
 jupyterlab = "^4.0.2"
 ipywidgets = "^8.0.6"
 plotly = "^5.15.0"
 jupyter-dash = "^0.4.2"
@@ -29,11 +28,12 @@
 matplotlib = "^3.7.1"
 tabulate = "^0.9.0"
 flatjsondict = "^1.0.3"
 pandas = "^2.0.2"
 pyjanitor = "^0.24.0"
 gspread = "^5.9.0"
 gspread-pandas = "^3.2.2"
+jsonmerge = "^1.9.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `drupaljsonapiclient-1.0.8/PKG-INFO` & `drupaljsonapiclient-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: drupaljsonapiclient
-Version: 1.0.8
+Version: 1.0.9
 Summary: Drupal CMS JSON:API client for Python.
 Home-page: https://gitlab.com/martins-bruvelis/drupaljsonapiclient
 Author: Martins Bruvelis
 Author-email: martins.bruvelis@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: jsonmerge (>=1.9.0,<2.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Documentation, https://gitlab.com/martins-bruvelis/drupaljsonapiclient/-/blob/main/README.md
 Project-URL: Repository, https://gitlab.com/martins-bruvelis/drupaljsonapiclient
 Description-Content-Type: text/markdown
 
 # drupaljsonapiclient: Drupal CMS JSON:API client for Python
```

