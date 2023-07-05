# Comparing `tmp/ayon-python-api-0.3.1.tar.gz` & `tmp/ayon-python-api-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayon-python-api-0.3.1.tar", last modified: Thu Jun 29 15:14:29 2023, max compression
+gzip compressed data, was "ayon-python-api-0.3.2.tar", last modified: Wed Jul  5 12:10:01 2023, max compression
```

## Comparing `ayon-python-api-0.3.1.tar` & `ayon-python-api-0.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:29.800687 ayon-python-api-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-06-29 15:14:29.800687 ayon-python-api-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:29.796687 ayon-python-api-0.3.1/ayon_api/
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30325 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    59757 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/entity_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25639 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)    15583 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/graphql_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)   187387 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/server_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:29.796687 ayon-python-api-0.3.1/ayon_python_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-06-29 15:14:29.000000 ayon-python-api-0.3.1/ayon_python_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-29 15:14:29.000000 ayon-python-api-0.3.1/ayon_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:14:29.000000 ayon-python-api-0.3.1/ayon_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 15:14:29.000000 ayon-python-api-0.3.1/ayon_python_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 15:14:29.000000 ayon-python-api-0.3.1/ayon_python_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 15:14:29.800687 ayon-python-api-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:10:01.621467 ayon-python-api-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-07-05 12:10:01.621467 ayon-python-api-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:10:01.621467 ayon-python-api-0.3.2/ayon_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30325 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59757 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/entity_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25639 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15583 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/graphql_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   188014 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/server_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:10:01.621467 ayon-python-api-0.3.2/ayon_python_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-07-05 12:10:01.000000 ayon-python-api-0.3.2/ayon_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-05 12:10:01.000000 ayon-python-api-0.3.2/ayon_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 12:10:01.000000 ayon-python-api-0.3.2/ayon_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 12:10:01.000000 ayon-python-api-0.3.2/ayon_python_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 12:10:01.000000 ayon-python-api-0.3.2/ayon_python_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 12:10:01.621467 ayon-python-api-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/setup.py
```

### Comparing `ayon-python-api-0.3.1/LICENSE` & `ayon-python-api-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.1/PKG-INFO` & `ayon-python-api-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayon-python-api
-Version: 0.3.1
+Version: 0.3.2
 Summary: AYON Python API
 Home-page: https://github.com/ynput/ayon-python-api
 Author: ynput.io
 Author-email: "ynput.io" <info@ynput.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ayon-python-api-0.3.1/README.md` & `ayon-python-api-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.1/ayon_api/__init__.py` & `ayon-python-api-0.3.2/ayon_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from .version import __version__
 from .utils import (
     TransferProgress,
     slugify_string,
+    create_dependency_package_basename,
 )
 from .server_api import (
     ServerAPI,
 )
 
 from ._api import (
     GlobalServerAPI,
@@ -179,16 +181,19 @@
     get_representation_links,
 
     send_batch_operations,
 )
 
 
 __all__ = (
+    "__version__",
+
     "TransferProgress",
     "slugify_string",
+    "create_dependency_package_basename",
 
     "ServerAPI",
 
     "GlobalServerAPI",
     "ServiceContext",
 
     "init_service",
```

### Comparing `ayon-python-api-0.3.1/ayon_api/_api.py` & `ayon-python-api-0.3.2/ayon_api/_api.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.1/ayon_api/constants.py` & `ayon-python-api-0.3.2/ayon_api/constants.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.1/ayon_api/entity_hub.py` & `ayon-python-api-0.3.2/ayon_api/entity_hub.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.1/ayon_api/events.py` & `ayon-python-api-0.3.2/ayon_api/events.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.1/ayon_api/exceptions.py` & `ayon-python-api-0.3.2/ayon_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.1/ayon_api/graphql.py` & `ayon-python-api-0.3.2/ayon_api/graphql.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.1/ayon_api/graphql_queries.py` & `ayon-python-api-0.3.2/ayon_api/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.1/ayon_api/operations.py` & `ayon-python-api-0.3.2/ayon_api/operations.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.1/ayon_api/server_api.py` & `ayon-python-api-0.3.2/ayon_api/server_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     RepresentationParents,
     prepare_query_string,
     logout_from_server,
     create_entity_id,
     entity_data_json_default,
     failed_json_default,
     TransferProgress,
+    create_dependency_package_basename,
 )
 
 PatternType = type(re.compile(""))
 JSONDecodeError = getattr(json, "JSONDecodeError", ValueError)
 # This should be collected from server schema
 PROJECT_NAME_ALLOWED_SYMBOLS = "a-zA-Z0-9_"
 PROJECT_NAME_REGEX = re.compile(
@@ -111,14 +112,18 @@
         else:
             status_code = response.status_code
         self._response = response
         self.status = status_code
         self._data = data
 
     @property
+    def text(self):
+        return self._response.text
+
+    @property
     def orig_response(self):
         return self._response
 
     @property
     def headers(self):
         return self._response.headers
 
@@ -146,19 +151,21 @@
             return detail
         return _get_description(self)
 
     @property
     def status_code(self):
         return self.status
 
-    def raise_for_status(self):
+    def raise_for_status(self, message=None):
         try:
             self._response.raise_for_status()
         except requests.exceptions.HTTPError as exc:
-            raise HTTPRequestError(str(exc), exc.response)
+            if message is None:
+                message = str(exc)
+            raise HTTPRequestError(message, exc.response)
 
     def __enter__(self, *args, **kwargs):
         return self._response.__enter__(*args, **kwargs)
 
     def __contains__(self, key):
         return key in self.data
 
@@ -1299,42 +1306,48 @@
             progress.set_failed(str(exc))
             raise
 
         finally:
             progress.set_transfer_done()
         return progress
 
-    def _upload_file(self, url, filepath, progress):
+    def _upload_file(self, url, filepath, progress, request_type=None):
+        if request_type is None:
+            request_type = RequestTypes.put
         kwargs = {}
         if self._session is None:
             kwargs["headers"] = self.get_headers()
-            post_func = self._base_functions_mapping[RequestTypes.post]
+            post_func = self._base_functions_mapping[request_type]
         else:
-            post_func = self._session_functions_mapping[RequestTypes.post]
+            post_func = self._session_functions_mapping[request_type]
 
         with open(filepath, "rb") as stream:
             stream.seek(0, io.SEEK_END)
             size = stream.tell()
             stream.seek(0)
             progress.set_content_size(size)
             response = post_func(url, data=stream, **kwargs)
         response.raise_for_status()
         progress.set_transferred_size(size)
 
-    def upload_file(self, endpoint, filepath, progress=None):
+    def upload_file(
+        self, endpoint, filepath, progress=None, request_type=None
+    ):
         """Upload file to server.
 
         Todos:
             Uploading with more detailed progress.
 
         Args:
             endpoint (str): Endpoint or url where file will be uploaded.
             filepath (str): Source filepath.
             progress (Optional[TransferProgress]): Object that gives ability
                 to track upload progress.
+            request_type (Optional[RequestType]): Type of request that will
+                be used to upload file.
         """
 
         if endpoint.startswith(self._base_url):
             url = endpoint
         else:
             endpoint = endpoint.lstrip("/").rstrip("/")
             url = "{}/{}".format(self._rest_url, endpoint)
@@ -1345,15 +1358,15 @@
             progress = TransferProgress()
 
         progress.set_source_url(filepath)
         progress.set_destination_url(url)
         progress.set_started()
 
         try:
-            self._upload_file(url, filepath, progress)
+            self._upload_file(url, filepath, progress, request_type)
 
         except Exception as exc:
             progress.set_failed(str(exc))
             raise
 
         finally:
             progress.set_transfer_done()
@@ -1482,21 +1495,19 @@
         This can't be un-done, please use carefully.
 
         Args:
             attribute_name (str): Name of attribute to remove.
         """
 
         response = self.delete("attributes/{}".format(attribute_name))
-        if response.status_code != 204:
-            # TODO raise different exception
-            raise ValueError(
-                "Attribute \"{}\" was not created/updated. {}".format(
-                    attribute_name, response.detail
-                )
+        response.raise_for_status(
+            "Attribute \"{}\" was not created/updated. {}".format(
+                attribute_name, response.detail
             )
+        )
 
         self.reset_attributes_schema()
 
     def get_attributes_for_type(self, entity_type):
         """Get attribute schemas available for an entity type.
 
         ```
@@ -1728,46 +1739,54 @@
     def create_installer(
         self,
         filename,
         version,
         python_version,
         platform_name,
         python_modules,
+        runtime_python_modules,
         checksum,
-        checksum_type,
+        checksum_algorithm,
         file_size,
         sources=None,
     ):
         """Create new installer information on server.
 
         This step will create only metadata. Make sure to upload installer
             to the server using 'upload_installer' method.
 
+        Runtime python modules are modules that are required to run AYON
+            desktop application, but are not added to PYTHONPATH for any
+            subprocess.
+
         Args:
             filename (str): Installer filename.
             version (str): Version of installer.
             python_version (str): Version of Python.
             platform_name (str): Name of platform.
             python_modules (dict[str, str]): Python modules that are available
                 in installer.
+            runtime_python_modules (dict[str, str]): Runtime python modules
+                that are available in installer.
             checksum (str): Installer file checksum.
-            checksum_type (str): Type of checksum used to create checksum.
+            checksum_algorithm (str): Type of checksum used to create checksum.
             file_size (int): File size.
             sources (Optional[list[dict[str, Any]]]): List of sources that
                 can be used to download file.
         """
 
         body = {
             "filename": filename,
             "version": version,
             "pythonVersion": python_version,
             "platform": platform_name,
             "pythonModules": python_modules,
+            "runtimePythonModules": runtime_python_modules,
             "checksum": checksum,
-            "checksumType": checksum_type,
+            "checksumAlgorithm": checksum_algorithm,
             "size": file_size,
         }
         if sources:
             body["sources"] = sources
 
         response = self.post("desktop/installers", **body)
         response.raise_for_status()
@@ -1777,28 +1796,28 @@
 
         Args:
             filename (str): Installer filename.
             sources (list[dict[str, Any]]): List of sources that
                 can be used to download file. Fully replaces existing sources.
         """
 
-        response = self.post(
+        response = self.patch(
             "desktop/installers/{}".format(filename),
             sources=sources
         )
         response.raise_for_status()
 
     def delete_installer(self, filename):
         """Delete installer from server.
 
         Args:
             filename (str): Installer filename.
         """
 
-        response = self.delete("dekstop/installers/{}".format(filename))
+        response = self.delete("desktop/installers/{}".format(filename))
         response.raise_for_status()
 
     def download_installer(
         self,
         filename,
         dst_filepath,
         chunk_size=None,
@@ -1925,16 +1944,15 @@
             "dependencies",
             name=name,
             platform=platform_name,
             size=size,
             checksum=checksum,
             **kwargs
         )
-        if response.status not in (200, 201, 204):
-            raise ServerError("Failed to create/update dependency")
+        response.raise_for_status("Failed to create/update dependency")
         return response.data
 
     def get_dependency_packages(self):
         """Information about dependency packages on server.
 
         To download dependency package, use 'download_dependency_package'
         method and pass in 'filename'.
@@ -2061,16 +2079,15 @@
             platform_name (Optional[str]): Which platform of the package
                 should be removed. Current platform is used if not passed.
                 Deprecated since version 0.2.1
         """
 
         route = self._get_dependency_package_route(filename, platform_name)
         response = self.delete(route)
-        if response.status != 200:
-            raise ServerError("Failed to delete dependency file")
+        response.raise_for_status("Failed to delete dependency file")
         return response.data
 
     def download_dependency_package(
         self,
         src_filename,
         dst_directory,
         dst_filename,
@@ -2127,28 +2144,27 @@
 
         route = self._get_dependency_package_route(dst_filename, platform_name)
         self.upload_file(route, src_filepath, progress=progress)
 
     def create_dependency_package_basename(self, platform_name=None):
         """Create basename for dependency package file.
 
+        Deprecated:
+            Use 'create_dependency_package_basename' from `ayon_api` or
+                `ayon_api.utils` instead.
+
         Args:
             platform_name (Optional[str]): Name of platform for which the
                 bundle is targeted. Default value is current platform.
 
         Returns:
             str: Dependency package name with timestamp and platform.
         """
 
-        if platform_name is None:
-            platform_name = platform.system().lower()
-
-        now_date = datetime.datetime.now()
-        time_stamp = now_date.strftime("%y%m%d%H%M")
-        return "ayon_{}_{}".format(time_stamp, platform_name)
+        return create_dependency_package_basename(platform_name)
 
     def _get_bundles_route(self):
         major, minor, patch, _, _ = self.server_version_tuple
         # Backwards compatibility for AYON server 0.3.0
         # - first version where bundles were available
         if major == 0 and minor == 3 and patch == 0:
             return "desktop/bundles"
```

### Comparing `ayon-python-api-0.3.1/ayon_api/thumbnails.py` & `ayon-python-api-0.3.2/ayon_api/thumbnails.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.1/ayon_api/utils.py` & `ayon-python-api-0.3.2/ayon_api/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 import datetime
 import uuid
 import string
+import platform
 import collections
 try:
     # Python 3
     from urllib.parse import urlparse, urlencode
 except ImportError:
     # Python 2
     from urlparse import urlparse
@@ -445,7 +446,26 @@
     transfer_done = property(get_transfer_done)
     failed = property(get_failed)
     fail_reason = property(get_fail_reason)
     source_url = property(get_source_url, set_source_url)
     destination_url = property(get_destination_url, set_destination_url)
     content_size = property(get_content_size, set_content_size)
     transferred_size = property(get_transferred_size, set_transferred_size)
+
+
+def create_dependency_package_basename(platform_name=None):
+    """Create basename for dependency package file.
+
+    Args:
+        platform_name (Optional[str]): Name of platform for which the
+            bundle is targeted. Default value is current platform.
+
+    Returns:
+        str: Dependency package name with timestamp and platform.
+    """
+
+    if platform_name is None:
+        platform_name = platform.system().lower()
+
+    now_date = datetime.datetime.now()
+    time_stamp = now_date.strftime("%y%m%d%H%M")
+    return "ayon_{}_{}".format(time_stamp, platform_name)
```

### Comparing `ayon-python-api-0.3.1/ayon_python_api.egg-info/PKG-INFO` & `ayon-python-api-0.3.2/ayon_python_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayon-python-api
-Version: 0.3.1
+Version: 0.3.2
 Summary: AYON Python API
 Home-page: https://github.com/ynput/ayon-python-api
 Author: ynput.io
 Author-email: "ynput.io" <info@ynput.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ayon-python-api-0.3.1/ayon_python_api.egg-info/SOURCES.txt` & `ayon-python-api-0.3.2/ayon_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.1/pyproject.toml` & `ayon-python-api-0.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ayon-python-api"
-version = "0.3.1"
+version = "0.3.2"
 description = "AYON Python API"
 license = {file = "LICENSE"}
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     {name = "ynput.io", email = "info@ynput.io"}
 ]
 keywords = ["AYON", "ynput", "OpenPype", "vfx"]
```

### Comparing `ayon-python-api-0.3.1/setup.py` & `ayon-python-api-0.3.2/setup.py`

 * *Files identical despite different names*

