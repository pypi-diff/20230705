# Comparing `tmp/powerdns-secondary-cleaner-1.0.1.tar.gz` & `tmp/powerdns-secondary-cleaner-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerdns-secondary-cleaner-1.0.1.tar", last modified: Sun Jul  2 15:51:37 2023, max compression
+gzip compressed data, was "powerdns-secondary-cleaner-1.0.2.tar", last modified: Wed Jul  5 16:35:33 2023, max compression
```

## Comparing `powerdns-secondary-cleaner-1.0.1.tar` & `powerdns-secondary-cleaner-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:51:37.170128 powerdns-secondary-cleaner-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1972 2023-07-02 15:51:37.170128 powerdns-secondary-cleaner-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1345 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:51:37.170128 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner/
--rw-rw-rw-   0 root         (0) root         (0)     1947 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner/CLI.py
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1532 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner/powerdns_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:51:37.170128 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1972 2023-07-02 15:51:37.000000 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      469 2023-07-02 15:51:37.000000 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 15:51:37.000000 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-07-02 15:51:37.000000 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-07-02 15:51:37.000000 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-02 15:51:37.000000 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-07-02 15:51:37.170128 powerdns-secondary-cleaner-1.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1286 2023-07-02 15:50:24.000000 powerdns-secondary-cleaner-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:35:33.538658 powerdns-secondary-cleaner-1.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1972 2023-07-05 16:35:33.538658 powerdns-secondary-cleaner-1.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2023-07-04 13:54:36.000000 powerdns-secondary-cleaner-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:35:33.538658 powerdns-secondary-cleaner-1.0.2/powerdns_secondary_cleaner/
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0.2/powerdns_secondary_cleaner/CLI.py
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0.2/powerdns_secondary_cleaner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1556 2023-07-05 16:33:39.000000 powerdns-secondary-cleaner-1.0.2/powerdns_secondary_cleaner/powerdns_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:35:33.538658 powerdns-secondary-cleaner-1.0.2/powerdns_secondary_cleaner.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1972 2023-07-05 16:35:33.000000 powerdns-secondary-cleaner-1.0.2/powerdns_secondary_cleaner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      469 2023-07-05 16:35:33.000000 powerdns-secondary-cleaner-1.0.2/powerdns_secondary_cleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:35:33.000000 powerdns-secondary-cleaner-1.0.2/powerdns_secondary_cleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-05 16:35:33.000000 powerdns-secondary-cleaner-1.0.2/powerdns_secondary_cleaner.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-07-05 16:35:33.000000 powerdns-secondary-cleaner-1.0.2/powerdns_secondary_cleaner.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-05 16:35:33.000000 powerdns-secondary-cleaner-1.0.2/powerdns_secondary_cleaner.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-07-05 16:35:33.538658 powerdns-secondary-cleaner-1.0.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1286 2023-07-05 16:33:39.000000 powerdns-secondary-cleaner-1.0.2/setup.py
```

### Comparing `powerdns-secondary-cleaner-1.0.1/LICENSE` & `powerdns-secondary-cleaner-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `powerdns-secondary-cleaner-1.0.1/PKG-INFO` & `powerdns-secondary-cleaner-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerdns-secondary-cleaner
-Version: 1.0.1
+Version: 1.0.2
 Summary: Use powerdns-secondary-cleaner to delete zones on secondary PowerDNS server that were deleted on primary PowerDNS server.
 Home-page: https://github.com/CyberfusionIO/powerdns-secondary-cleaner
 Author: William Edwards
 Author-email: support@cyberfusion.nl
 License: MIT
 Keywords: cyberfusion,powerdns
 Platform: linux
@@ -47,15 +47,15 @@
 
 Example when running on primary:
 
     powerdns-secondary-cleaner --primary-api-url=http://localhost:8081 --primary-api-key=example --secondary-api-url=http://secondary.test:8081 --secondary-api-key=example
 
 Example when running on secondary:
 
-    powerdns-secondary-cleaner --secondary-api-url=http://primary.test:8081 --primary-api-key=example --primary-api-url=http://localhost:8081 --secondary-api-key=example
+    powerdns-secondary-cleaner --secondary-api-url=http://localhost:8081 --secondary-api-key=example --primary-api-url=http://primary.test:8081 --primary-api-key=example
 
 Only show which zones would be deleted on secondary:
 
     powerdns-secondary-cleaner ... --dry-run
 
 # Tests
```

### Comparing `powerdns-secondary-cleaner-1.0.1/README.md` & `powerdns-secondary-cleaner-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 Example when running on primary:
 
     powerdns-secondary-cleaner --primary-api-url=http://localhost:8081 --primary-api-key=example --secondary-api-url=http://secondary.test:8081 --secondary-api-key=example
 
 Example when running on secondary:
 
-    powerdns-secondary-cleaner --secondary-api-url=http://primary.test:8081 --primary-api-key=example --primary-api-url=http://localhost:8081 --secondary-api-key=example
+    powerdns-secondary-cleaner --secondary-api-url=http://localhost:8081 --secondary-api-key=example --primary-api-url=http://primary.test:8081 --primary-api-key=example
 
 Only show which zones would be deleted on secondary:
 
     powerdns-secondary-cleaner ... --dry-run
 
 # Tests
```

### Comparing `powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner/CLI.py` & `powerdns-secondary-cleaner-1.0.2/powerdns_secondary_cleaner/CLI.py`

 * *Files identical despite different names*

### Comparing `powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner/powerdns_api.py` & `powerdns-secondary-cleaner-1.0.2/powerdns_secondary_cleaner/powerdns_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Classes to use PowerDNS API."""
 
 from dataclasses import dataclass
 from typing import List
 
 import requests
 
+TIMEOUT = 60
+
 
 @dataclass
 class Zone:
     """Represents PowerDNS zone."""
 
     id_: str
 
@@ -26,26 +28,26 @@
         self.api_url = api_url
         self.api_key = api_key
 
     def _execute_get_request(self, endpoint: str) -> dict:
         """Execute GET request and get response."""
         request = requests.get(
             f"{self.api_url}/api/v1/servers/localhost/{endpoint}",
-            timeout=10,
+            timeout=TIMEOUT,
             headers={"X-API-Key": self.api_key},
         )
         request.raise_for_status()
 
         return request.json()
 
     def _execute_delete_request(self, endpoint: str) -> None:
         """Execute DELETE request."""
         request = requests.delete(
             f"{self.api_url}/api/v1/servers/localhost/{endpoint}",
-            timeout=10,
+            timeout=TIMEOUT,
             headers={"X-API-Key": self.api_key},
         )
         request.raise_for_status()
 
     def get_zones(self) -> List[Zone]:
         """Get zones."""
         zones = self._execute_get_request("zones")
```

### Comparing `powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner.egg-info/PKG-INFO` & `powerdns-secondary-cleaner-1.0.2/powerdns_secondary_cleaner.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerdns-secondary-cleaner
-Version: 1.0.1
+Version: 1.0.2
 Summary: Use powerdns-secondary-cleaner to delete zones on secondary PowerDNS server that were deleted on primary PowerDNS server.
 Home-page: https://github.com/CyberfusionIO/powerdns-secondary-cleaner
 Author: William Edwards
 Author-email: support@cyberfusion.nl
 License: MIT
 Keywords: cyberfusion,powerdns
 Platform: linux
@@ -47,15 +47,15 @@
 
 Example when running on primary:
 
     powerdns-secondary-cleaner --primary-api-url=http://localhost:8081 --primary-api-key=example --secondary-api-url=http://secondary.test:8081 --secondary-api-key=example
 
 Example when running on secondary:
 
-    powerdns-secondary-cleaner --secondary-api-url=http://primary.test:8081 --primary-api-key=example --primary-api-url=http://localhost:8081 --secondary-api-key=example
+    powerdns-secondary-cleaner --secondary-api-url=http://localhost:8081 --secondary-api-key=example --primary-api-url=http://primary.test:8081 --primary-api-key=example
 
 Only show which zones would be deleted on secondary:
 
     powerdns-secondary-cleaner ... --dry-run
 
 # Tests
```

### Comparing `powerdns-secondary-cleaner-1.0.1/setup.py` & `powerdns-secondary-cleaner-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="powerdns-secondary-cleaner",
-    version="1.0.1",
+    version="1.0.2",
     description="Use powerdns-secondary-cleaner to delete zones on secondary PowerDNS server that were deleted on primary PowerDNS server.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.6",
     author="William Edwards",
     author_email="support@cyberfusion.nl",
     url="https://github.com/CyberfusionIO/powerdns-secondary-cleaner",
```

