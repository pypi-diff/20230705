# Comparing `tmp/planetary-computer-0.5.1.tar.gz` & `tmp/planetary-computer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetary-computer-0.5.1.tar", last modified: Fri Apr 14 19:27:57 2023, max compression
+gzip compressed data, was "planetary-computer-1.0.0.tar", last modified: Wed Jul  5 13:06:47 2023, max compression
```

## Comparing `planetary-computer-0.5.1.tar` & `planetary-computer-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:27:57.537193 planetary-computer-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-04-14 19:27:57.537193 planetary-computer-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:27:57.537193 planetary-computer-0.5.1/planetary_computer/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/planetary_computer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/planetary_computer/_adlfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15166 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/planetary_computer/sas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:27:57.537193 planetary-computer-0.5.1/planetary_computer/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/planetary_computer/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/planetary_computer/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/planetary_computer/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/planetary_computer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/planetary_computer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:27:57.537193 planetary-computer-0.5.1/planetary_computer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-04-14 19:27:57.000000 planetary-computer-0.5.1/planetary_computer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-14 19:27:57.000000 planetary-computer-0.5.1/planetary_computer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:27:57.000000 planetary-computer-0.5.1/planetary_computer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 19:27:57.000000 planetary-computer-0.5.1/planetary_computer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-14 19:27:57.000000 planetary-computer-0.5.1/planetary_computer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-14 19:27:57.000000 planetary-computer-0.5.1/planetary_computer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-14 19:27:57.537193 planetary-computer-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:27:57.537193 planetary-computer-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/tests/test_adlfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    13627 2023-04-14 19:27:48.000000 planetary-computer-0.5.1/tests/test_signing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:06:47.140867 planetary-computer-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-05 13:06:25.000000 planetary-computer-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-07-05 13:06:47.140867 planetary-computer-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-05 13:06:25.000000 planetary-computer-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:06:47.136867 planetary-computer-1.0.0/planetary_computer/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-05 13:06:25.000000 planetary-computer-1.0.0/planetary_computer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-05 13:06:25.000000 planetary-computer-1.0.0/planetary_computer/_adlfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15396 2023-07-05 13:06:25.000000 planetary-computer-1.0.0/planetary_computer/sas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:06:47.140867 planetary-computer-1.0.0/planetary_computer/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:06:25.000000 planetary-computer-1.0.0/planetary_computer/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-05 13:06:25.000000 planetary-computer-1.0.0/planetary_computer/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-05 13:06:25.000000 planetary-computer-1.0.0/planetary_computer/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-05 13:06:25.000000 planetary-computer-1.0.0/planetary_computer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 13:06:25.000000 planetary-computer-1.0.0/planetary_computer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:06:47.140867 planetary-computer-1.0.0/planetary_computer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-07-05 13:06:47.000000 planetary-computer-1.0.0/planetary_computer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-05 13:06:47.000000 planetary-computer-1.0.0/planetary_computer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 13:06:47.000000 planetary-computer-1.0.0/planetary_computer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-05 13:06:47.000000 planetary-computer-1.0.0/planetary_computer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-05 13:06:47.000000 planetary-computer-1.0.0/planetary_computer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 13:06:47.000000 planetary-computer-1.0.0/planetary_computer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-05 13:06:25.000000 planetary-computer-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 13:06:47.140867 planetary-computer-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:06:47.140867 planetary-computer-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-05 13:06:25.000000 planetary-computer-1.0.0/tests/test_adlfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-05 13:06:25.000000 planetary-computer-1.0.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13673 2023-07-05 13:06:25.000000 planetary-computer-1.0.0/tests/test_signing.py
```

### Comparing `planetary-computer-0.5.1/LICENSE` & `planetary-computer-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `planetary-computer-0.5.1/PKG-INFO` & `planetary-computer-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: planetary-computer
-Version: 0.5.1
-Summary: Planetary Computer SDK for Python
-Author: microsoft
-Author-email: planetarycomputer@microsoft.com
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: adlfs
-Provides-Extra: azure
-Provides-Extra: dev
-License-File: LICENSE
-
 # Planetary Computer SDK for Python
 
 Python library for interacting with the Microsoft Planetary Computer.
 
 For general questions or discussions about the Planetary Computer, use the [microsoft/PlanetaryComputer](http://github.com/microsoft/PlanetaryComputer) repository.
 
 ## Installation
```

### Comparing `planetary-computer-0.5.1/README.md` & `planetary-computer-1.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,41 @@
+Metadata-Version: 2.1
+Name: planetary-computer
+Version: 1.0.0
+Summary: Planetary Computer SDK for Python
+Author-email: microsoft <planetarycomputer@microsoft.com>
+License:     MIT License
+        
+            Copyright (c) Microsoft Corporation.
+        
+            Permission is hereby granted, free of charge, to any person obtaining a copy
+            of this software and associated documentation files (the "Software"), to deal
+            in the Software without restriction, including without limitation the rights
+            to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+            copies of the Software, and to permit persons to whom the Software is
+            furnished to do so, subject to the following conditions:
+        
+            The above copyright notice and this permission notice shall be included in all
+            copies or substantial portions of the Software.
+        
+            THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+            IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+            FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+            AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+            LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+            OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+            SOFTWARE
+        
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: adlfs
+Provides-Extra: azure
+Provides-Extra: dev
+License-File: LICENSE
+
 # Planetary Computer SDK for Python
 
 Python library for interacting with the Microsoft Planetary Computer.
 
 For general questions or discussions about the Planetary Computer, use the [microsoft/PlanetaryComputer](http://github.com/microsoft/PlanetaryComputer) repository.
 
 ## Installation
```

### Comparing `planetary-computer-0.5.1/planetary_computer/__init__.py` & `planetary-computer-1.0.0/planetary_computer/__init__.py`

 * *Files identical despite different names*

### Comparing `planetary-computer-0.5.1/planetary_computer/_adlfs.py` & `planetary-computer-1.0.0/planetary_computer/_adlfs.py`

 * *Files identical despite different names*

### Comparing `planetary-computer-0.5.1/planetary_computer/sas.py` & `planetary-computer-1.0.0/planetary_computer/sas.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from copy import deepcopy
 import warnings
 
 from functools import singledispatch
 from urllib.parse import urlparse, parse_qs
 import requests
 import requests.adapters
+import packaging.version
+import pydantic
 from pydantic import BaseModel, Field
 from pystac import Asset, Item, ItemCollection, STACObjectType, Collection
 from pystac.utils import datetime_to_str
 from pystac.serialization.identify import identify_stac_object_type
 from pystac_client import ItemSearch
 import pystac_client
 import urllib3.util.retry
@@ -22,28 +24,35 @@
     parse_blob_url,
     parse_adlfs_url,
     is_fsspec_asset,
     is_vrt_string,
     asset_xpr,
 )
 
+_PYDANTIC_2_0 = packaging.version.parse(
+    pydantic.__version__
+) >= packaging.version.parse("2.0.0")
+
 
 BLOB_STORAGE_DOMAIN = ".blob.core.windows.net"
 AssetLike = TypeVar("AssetLike", Asset, Dict[str, Any])
 
 
 class SASBase(BaseModel):
     """Base model for responses."""
 
     expiry: datetime = Field(alias="msft:expiry")
     """RFC339 datetime format of the time this token will expire"""
 
     class Config:
-        json_encoders = {datetime: datetime_to_str}
-        allow_population_by_field_name = True
+        if _PYDANTIC_2_0:
+            populate_by_name = True
+        else:
+            allow_population_by_field_name = True
+            json_encoders = {datetime: datetime_to_str}
 
 
 class SignedLink(SASBase):
     """Signed SAS URL response"""
 
     href: str
     """The HREF in the format of a URL that can be used in HTTP GET operations"""
```

### Comparing `planetary-computer-0.5.1/planetary_computer/scripts/cli.py` & `planetary-computer-1.0.0/planetary_computer/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `planetary-computer-0.5.1/planetary_computer/utils.py` & `planetary-computer-1.0.0/planetary_computer/utils.py`

 * *Files identical despite different names*

### Comparing `planetary-computer-0.5.1/planetary_computer.egg-info/PKG-INFO` & `planetary-computer-1.0.0/planetary_computer.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,34 @@
 Metadata-Version: 2.1
 Name: planetary-computer
-Version: 0.5.1
+Version: 1.0.0
 Summary: Planetary Computer SDK for Python
-Author: microsoft
-Author-email: planetarycomputer@microsoft.com
+Author-email: microsoft <planetarycomputer@microsoft.com>
+License:     MIT License
+        
+            Copyright (c) Microsoft Corporation.
+        
+            Permission is hereby granted, free of charge, to any person obtaining a copy
+            of this software and associated documentation files (the "Software"), to deal
+            in the Software without restriction, including without limitation the rights
+            to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+            copies of the Software, and to permit persons to whom the Software is
+            furnished to do so, subject to the following conditions:
+        
+            The above copyright notice and this permission notice shall be included in all
+            copies or substantial portions of the Software.
+        
+            THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+            IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+            FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+            AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+            LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+            OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+            SOFTWARE
+        
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: adlfs
 Provides-Extra: azure
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `planetary-computer-0.5.1/planetary_computer.egg-info/SOURCES.txt` & `planetary-computer-1.0.0/planetary_computer.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
-setup.py
 planetary_computer/__init__.py
 planetary_computer/_adlfs.py
 planetary_computer/sas.py
 planetary_computer/settings.py
 planetary_computer/utils.py
 planetary_computer/version.py
 planetary_computer.egg-info/PKG-INFO
 planetary_computer.egg-info/SOURCES.txt
 planetary_computer.egg-info/dependency_links.txt
 planetary_computer.egg-info/entry_points.txt
 planetary_computer.egg-info/requires.txt
 planetary_computer.egg-info/top_level.txt
 planetary_computer/scripts/__init__.py
 planetary_computer/scripts/cli.py
-tests/__init__.py
 tests/test_adlfs.py
 tests/test_settings.py
 tests/test_signing.py
```

### Comparing `planetary-computer-0.5.1/tests/test_adlfs.py` & `planetary-computer-1.0.0/tests/test_adlfs.py`

 * *Files identical despite different names*

### Comparing `planetary-computer-0.5.1/tests/test_settings.py` & `planetary-computer-1.0.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `planetary-computer-0.5.1/tests/test_signing.py` & `planetary-computer-1.0.0/tests/test_signing.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,14 +144,15 @@
 
         search = ItemSearch(
             url=PC_SEARCH_URL,
             bbox=(-73.21, 43.99, -73.12, 44.05),
             collections=CONTAINER_NAME,
             limit=1,
             max_items=1,
+            datetime="2018-01-01/2018-12-31",
         )
         signed_item_collection = pc.sign(search)
         self.assertEqual(len(list(signed_item_collection)), 1)
         for signed_item in signed_item_collection:
             self.verify_signed_urls_in_item(signed_item)
 
     def test_sign_assets_deprecated(self) -> None:
```

