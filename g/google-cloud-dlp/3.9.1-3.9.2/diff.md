# Comparing `tmp/google-cloud-dlp-3.9.1.tar.gz` & `tmp/google-cloud-dlp-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-dlp-3.9.1.tar", last modified: Tue Oct  4 01:12:35 2022, max compression
+gzip compressed data, was "google-cloud-dlp-3.9.2.tar", last modified: Mon Oct 10 16:31:28 2022, max compression
```

## Comparing `google-cloud-dlp-3.9.1.tar` & `google-cloud-dlp-3.9.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 01:12:35.870453 google-cloud-dlp-3.9.1/
--rw-rw-r--   0 root         (0)     1003    11358 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4719 2022-10-04 01:12:35.870453 google-cloud-dlp-3.9.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3823 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 01:12:35.858455 google-cloud-dlp-3.9.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 01:12:35.858455 google-cloud-dlp-3.9.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 01:12:35.862454 google-cloud-dlp-3.9.1/google/cloud/dlp/
--rw-rw-r--   0 root         (0)     1003    10088 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/google/cloud/dlp/__init__.py
--rw-rw-r--   0 root         (0)     1003       77 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/google/cloud/dlp/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 01:12:35.862454 google-cloud-dlp-3.9.1/google/cloud/dlp_v2/
--rw-rw-r--   0 root         (0)     1003     9959 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/google/cloud/dlp_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     9485 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/google/cloud/dlp_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       77 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/google/cloud/dlp_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 01:12:35.862454 google-cloud-dlp-3.9.1/google/cloud/dlp_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/google/cloud/dlp_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 01:12:35.866453 google-cloud-dlp-3.9.1/google/cloud/dlp_v2/services/dlp_service/
--rw-rw-r--   0 root         (0)     1003      753 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/google/cloud/dlp_v2/services/dlp_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   168525 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/google/cloud/dlp_v2/services/dlp_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   178631 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/google/cloud/dlp_v2/services/dlp_service/client.py
--rw-rw-r--   0 root         (0)     1003    25726 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/google/cloud/dlp_v2/services/dlp_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 01:12:35.866453 google-cloud-dlp-3.9.1/google/cloud/dlp_v2/services/dlp_service/transports/
--rw-rw-r--   0 root         (0)     1003     1157 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/google/cloud/dlp_v2/services/dlp_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    28535 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/google/cloud/dlp_v2/services/dlp_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    54429 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/google/cloud/dlp_v2/services/dlp_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    55579 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/google/cloud/dlp_v2/services/dlp_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 01:12:35.866453 google-cloud-dlp-3.9.1/google/cloud/dlp_v2/types/
--rw-rw-r--   0 root         (0)     1003     9819 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/google/cloud/dlp_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003   277666 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/google/cloud/dlp_v2/types/dlp.py
--rw-rw-r--   0 root         (0)     1003    47922 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/google/cloud/dlp_v2/types/storage.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 01:12:35.866453 google-cloud-dlp-3.9.1/google_cloud_dlp.egg-info/
--rw-r--r--   0 root         (0)     1003     4719 2022-10-04 01:12:35.000000 google-cloud-dlp-3.9.1/google_cloud_dlp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1398 2022-10-04 01:12:35.000000 google-cloud-dlp-3.9.1/google_cloud_dlp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-04 01:12:35.000000 google-cloud-dlp-3.9.1/google_cloud_dlp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-10-04 01:12:35.000000 google-cloud-dlp-3.9.1/google_cloud_dlp.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-04 01:12:35.000000 google-cloud-dlp-3.9.1/google_cloud_dlp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      184 2022-10-04 01:12:35.000000 google-cloud-dlp-3.9.1/google_cloud_dlp.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-10-04 01:12:35.000000 google-cloud-dlp-3.9.1/google_cloud_dlp.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 01:12:35.866453 google-cloud-dlp-3.9.1/scripts/
--rw-rw-r--   0 root         (0)     1003     8539 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/scripts/fixup_dlp_v2_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-10-04 01:12:35.870453 google-cloud-dlp-3.9.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2575 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 01:12:35.866453 google-cloud-dlp-3.9.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 01:12:35.862454 google-cloud-dlp-3.9.1/tests/system/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 01:12:35.862454 google-cloud-dlp-3.9.1/tests/system/gapic/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 01:12:35.866453 google-cloud-dlp-3.9.1/tests/system/gapic/v2/
--rw-rw-r--   0 root         (0)     1003     1500 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/tests/system/gapic/v2/test_system_dlp_service_v2.py
--rw-rw-r--   0 root         (0)     1003    21026 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/tests/system/gapic/v2/test_system_dlp_service_v2_vpcsc.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 01:12:35.870453 google-cloud-dlp-3.9.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 01:12:35.870453 google-cloud-dlp-3.9.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 01:12:35.870453 google-cloud-dlp-3.9.1/tests/unit/gapic/dlp_v2/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/tests/unit/gapic/dlp_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003   359309 2022-10-04 01:09:13.000000 google-cloud-dlp-3.9.1/tests/unit/gapic/dlp_v2/test_dlp_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:31:28.721619 google-cloud-dlp-3.9.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4719 2022-10-10 16:31:28.721619 google-cloud-dlp-3.9.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3823 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:31:28.709622 google-cloud-dlp-3.9.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:31:28.709622 google-cloud-dlp-3.9.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:31:28.713621 google-cloud-dlp-3.9.2/google/cloud/dlp/
+-rw-rw-r--   0 root         (0)     1003    10088 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/google/cloud/dlp/__init__.py
+-rw-rw-r--   0 root         (0)     1003       77 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/google/cloud/dlp/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:31:28.713621 google-cloud-dlp-3.9.2/google/cloud/dlp_v2/
+-rw-rw-r--   0 root         (0)     1003     9959 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/google/cloud/dlp_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9485 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/google/cloud/dlp_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       77 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/google/cloud/dlp_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:31:28.713621 google-cloud-dlp-3.9.2/google/cloud/dlp_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/google/cloud/dlp_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:31:28.713621 google-cloud-dlp-3.9.2/google/cloud/dlp_v2/services/dlp_service/
+-rw-rw-r--   0 root         (0)     1003      753 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/google/cloud/dlp_v2/services/dlp_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   168525 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/google/cloud/dlp_v2/services/dlp_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   178631 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/google/cloud/dlp_v2/services/dlp_service/client.py
+-rw-rw-r--   0 root         (0)     1003    25726 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/google/cloud/dlp_v2/services/dlp_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:31:28.717620 google-cloud-dlp-3.9.2/google/cloud/dlp_v2/services/dlp_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1157 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/google/cloud/dlp_v2/services/dlp_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    28535 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/google/cloud/dlp_v2/services/dlp_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    54429 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/google/cloud/dlp_v2/services/dlp_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    55579 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/google/cloud/dlp_v2/services/dlp_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:31:28.717620 google-cloud-dlp-3.9.2/google/cloud/dlp_v2/types/
+-rw-rw-r--   0 root         (0)     1003     9819 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/google/cloud/dlp_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003   277666 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/google/cloud/dlp_v2/types/dlp.py
+-rw-rw-r--   0 root         (0)     1003    47922 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/google/cloud/dlp_v2/types/storage.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:31:28.717620 google-cloud-dlp-3.9.2/google_cloud_dlp.egg-info/
+-rw-r--r--   0 root         (0)     1003     4719 2022-10-10 16:31:28.000000 google-cloud-dlp-3.9.2/google_cloud_dlp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1398 2022-10-10 16:31:28.000000 google-cloud-dlp-3.9.2/google_cloud_dlp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:31:28.000000 google-cloud-dlp-3.9.2/google_cloud_dlp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-10-10 16:31:28.000000 google-cloud-dlp-3.9.2/google_cloud_dlp.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:31:28.000000 google-cloud-dlp-3.9.2/google_cloud_dlp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      256 2022-10-10 16:31:28.000000 google-cloud-dlp-3.9.2/google_cloud_dlp.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-10-10 16:31:28.000000 google-cloud-dlp-3.9.2/google_cloud_dlp.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:31:28.717620 google-cloud-dlp-3.9.2/scripts/
+-rw-rw-r--   0 root         (0)     1003     8539 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/scripts/fixup_dlp_v2_keywords.py
+-rw-rw-r--   0 root         (0)     1003       67 2022-10-10 16:31:28.721619 google-cloud-dlp-3.9.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2644 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:31:28.717620 google-cloud-dlp-3.9.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:31:28.709622 google-cloud-dlp-3.9.2/tests/system/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:31:28.709622 google-cloud-dlp-3.9.2/tests/system/gapic/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:31:28.717620 google-cloud-dlp-3.9.2/tests/system/gapic/v2/
+-rw-rw-r--   0 root         (0)     1003     1500 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/tests/system/gapic/v2/test_system_dlp_service_v2.py
+-rw-rw-r--   0 root         (0)     1003    21026 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/tests/system/gapic/v2/test_system_dlp_service_v2_vpcsc.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:31:28.721619 google-cloud-dlp-3.9.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:31:28.721619 google-cloud-dlp-3.9.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:31:28.721619 google-cloud-dlp-3.9.2/tests/unit/gapic/dlp_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/tests/unit/gapic/dlp_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   359309 2022-10-10 16:28:08.000000 google-cloud-dlp-3.9.2/tests/unit/gapic/dlp_v2/test_dlp_service.py
```

### Comparing `google-cloud-dlp-3.9.1/LICENSE` & `google-cloud-dlp-3.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/MANIFEST.in` & `google-cloud-dlp-3.9.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/PKG-INFO` & `google-cloud-dlp-3.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-dlp
-Version: 3.9.1
+Version: 3.9.2
 Summary: Cloud Data Loss Prevention (DLP) API API client library
 Home-page: https://github.com/googleapis/python-dlp
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-dlp-3.9.1/README.rst` & `google-cloud-dlp-3.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/google/cloud/dlp/__init__.py` & `google-cloud-dlp-3.9.2/google/cloud/dlp/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/google/cloud/dlp_v2/__init__.py` & `google-cloud-dlp-3.9.2/google/cloud/dlp_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/google/cloud/dlp_v2/gapic_metadata.json` & `google-cloud-dlp-3.9.2/google/cloud/dlp_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/google/cloud/dlp_v2/services/__init__.py` & `google-cloud-dlp-3.9.2/google/cloud/dlp_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/google/cloud/dlp_v2/services/dlp_service/__init__.py` & `google-cloud-dlp-3.9.2/google/cloud/dlp_v2/services/dlp_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/google/cloud/dlp_v2/services/dlp_service/async_client.py` & `google-cloud-dlp-3.9.2/google/cloud/dlp_v2/services/dlp_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/google/cloud/dlp_v2/services/dlp_service/client.py` & `google-cloud-dlp-3.9.2/google/cloud/dlp_v2/services/dlp_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/google/cloud/dlp_v2/services/dlp_service/pagers.py` & `google-cloud-dlp-3.9.2/google/cloud/dlp_v2/services/dlp_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/google/cloud/dlp_v2/services/dlp_service/transports/__init__.py` & `google-cloud-dlp-3.9.2/google/cloud/dlp_v2/services/dlp_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/google/cloud/dlp_v2/services/dlp_service/transports/base.py` & `google-cloud-dlp-3.9.2/google/cloud/dlp_v2/services/dlp_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/google/cloud/dlp_v2/services/dlp_service/transports/grpc.py` & `google-cloud-dlp-3.9.2/google/cloud/dlp_v2/services/dlp_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/google/cloud/dlp_v2/services/dlp_service/transports/grpc_asyncio.py` & `google-cloud-dlp-3.9.2/google/cloud/dlp_v2/services/dlp_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/google/cloud/dlp_v2/types/__init__.py` & `google-cloud-dlp-3.9.2/google/cloud/dlp_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/google/cloud/dlp_v2/types/dlp.py` & `google-cloud-dlp-3.9.2/google/cloud/dlp_v2/types/dlp.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/google/cloud/dlp_v2/types/storage.py` & `google-cloud-dlp-3.9.2/google/cloud/dlp_v2/types/storage.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/google_cloud_dlp.egg-info/PKG-INFO` & `google-cloud-dlp-3.9.2/google_cloud_dlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-dlp
-Version: 3.9.1
+Version: 3.9.2
 Summary: Cloud Data Loss Prevention (DLP) API API client library
 Home-page: https://github.com/googleapis/python-dlp
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-dlp-3.9.1/google_cloud_dlp.egg-info/SOURCES.txt` & `google-cloud-dlp-3.9.2/google_cloud_dlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/scripts/fixup_dlp_v2_keywords.py` & `google-cloud-dlp-3.9.2/scripts/fixup_dlp_v2_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/setup.py` & `google-cloud-dlp-3.9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 import io
 import os
 
 import setuptools
 
 name = "google-cloud-dlp"
 description = "Cloud Data Loss Prevention (DLP) API API client library"
-version = "3.9.1"
+version = "3.9.2"
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     "google-api-core[grpc] >= 1.32.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
-    "protobuf >= 3.20.2, <5.0.0dev",
+    "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
 
 extras = {"libcst": "libcst >= 0.2.5"}
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
```

### Comparing `google-cloud-dlp-3.9.1/tests/__init__.py` & `google-cloud-dlp-3.9.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/tests/system/gapic/v2/test_system_dlp_service_v2.py` & `google-cloud-dlp-3.9.2/tests/system/gapic/v2/test_system_dlp_service_v2.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/tests/system/gapic/v2/test_system_dlp_service_v2_vpcsc.py` & `google-cloud-dlp-3.9.2/tests/system/gapic/v2/test_system_dlp_service_v2_vpcsc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/tests/unit/__init__.py` & `google-cloud-dlp-3.9.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/tests/unit/gapic/__init__.py` & `google-cloud-dlp-3.9.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/tests/unit/gapic/dlp_v2/__init__.py` & `google-cloud-dlp-3.9.2/tests/unit/gapic/dlp_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dlp-3.9.1/tests/unit/gapic/dlp_v2/test_dlp_service.py` & `google-cloud-dlp-3.9.2/tests/unit/gapic/dlp_v2/test_dlp_service.py`

 * *Files identical despite different names*

