# Comparing `tmp/hydrus_api-5.0.0.tar.gz` & `tmp/hydrus_api-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrus_api-5.0.0.tar", max compression
+gzip compressed data, was "hydrus_api-5.0.1.tar", max compression
```

## Comparing `hydrus_api-5.0.0.tar` & `hydrus_api-5.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34519 2022-08-24 12:02:10.016675 hydrus_api-5.0.0/LICENSE
--rw-r--r--   0        0        0     3743 2023-02-26 15:04:30.873837 hydrus_api-5.0.0/README.md
--rw-r--r--   0        0        0    36574 2023-02-26 14:50:11.217357 hydrus_api-5.0.0/hydrus_api/__init__.py
--rw-r--r--   0        0        0     5237 2023-02-26 14:28:02.015850 hydrus_api-5.0.0/hydrus_api/utils.py
--rw-r--r--   0        0        0      773 2023-02-26 14:38:29.942340 hydrus_api-5.0.0/pyproject.toml
--rw-r--r--   0        0        0     4464 1970-01-01 00:00:00.000000 hydrus_api-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0    34519 2022-08-24 12:02:10.016675 hydrus_api-5.0.1/LICENSE
+-rw-r--r--   0        0        0     3743 2023-02-26 15:04:30.873837 hydrus_api-5.0.1/README.md
+-rw-r--r--   0        0        0    36520 2023-07-05 19:46:34.566755 hydrus_api-5.0.1/hydrus_api/__init__.py
+-rw-r--r--   0        0        0     5237 2023-02-26 14:28:02.015850 hydrus_api-5.0.1/hydrus_api/utils.py
+-rw-r--r--   0        0        0      784 2023-07-05 19:46:22.496884 hydrus_api-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4464 1970-01-01 00:00:00.000000 hydrus_api-5.0.1/PKG-INFO
```

### Comparing `hydrus_api-5.0.0/LICENSE` & `hydrus_api-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrus_api-5.0.0/README.md` & `hydrus_api-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hydrus_api-5.0.0/hydrus_api/__init__.py` & `hydrus_api-5.0.1/hydrus_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import json
 import os
 import typing as T
 import collections.abc as abc
 
 import requests
 
-__version__ = "5.0.0"
+__version__ = "5.0.1"
 
 DEFAULT_API_URL = "http://127.0.0.1:45869/"
 HYDRUS_METADATA_ENCODING = "utf-8"
 AUTHENTICATION_TIMEOUT_CODE = 419
 
 
 # Customize IntEnum, so we can just do str(Enum.member) to get the string representation of its value unmodified,
@@ -834,18 +834,17 @@
             params["pixel_duplicates"] = pixel_duplicates
         if max_hamming_distance is not None:
             params["max_hamming_distance"] = max_hamming_distance
 
         response = self._api_request("GET", self._GET_RANDOM_POTENTIALS_PATH, params=params)
         return response.json()
 
-    def set_file_relationships(self, relationships: abc.Iterable[abc.Mapping[str, T.Any]]) -> dict[str, T.Any]:
+    def set_file_relationships(self, relationships: abc.Iterable[abc.Mapping[str, T.Any]]) -> None:
         payload = {"relationships": relationships}
-        response = self._api_request("POST", self._SET_FILE_RELATIONSHIPS_PATH, json=payload)
-        return response.json()
+        self._api_request("POST", self._SET_FILE_RELATIONSHIPS_PATH, json=payload)
 
     def set_kings(
         self, file_ids: T.Optional[abc.Iterable[int]] = None, hashes: T.Optional[abc.Iterable[str]] = None
     ) -> dict[str, T.Any]:
         if file_ids is None and hashes is None:
             raise ValueError("At least one of file_ids, hashes is required")
```

### Comparing `hydrus_api-5.0.0/hydrus_api/utils.py` & `hydrus_api-5.0.1/hydrus_api/utils.py`

 * *Files identical despite different names*

### Comparing `hydrus_api-5.0.0/pyproject.toml` & `hydrus_api-5.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hydrus-api"
-version = "5.0.0"
+version = "5.0.1"
 description = "Python module implementing the Hydrus API"
 authors = ["cryzed <cryzed@googlemail.com>"]
 
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://gitlab.com/cryzed/hydrus-api"
 repository = "https://gitlab.com/cryzed/hydrus-api"
@@ -28,9 +28,9 @@
 line-length = 120
 
 [tool.isort]
 profile = "black"
 line_length = 120
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `hydrus_api-5.0.0/PKG-INFO` & `hydrus_api-5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrus-api
-Version: 5.0.0
+Version: 5.0.1
 Summary: Python module implementing the Hydrus API
 Home-page: https://gitlab.com/cryzed/hydrus-api
 License: AGPL-3.0-or-later
 Keywords: hydrus,api
 Author: cryzed
 Author-email: cryzed@googlemail.com
 Requires-Python: >=3.9,<4.0
```

