# Comparing `tmp/google-cloud-api-keys-0.5.2.tar.gz` & `tmp/google-cloud-api-keys-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-api-keys-0.5.2.tar", last modified: Mon Mar 27 15:52:17 2023, max compression
+gzip compressed data, was "google-cloud-api-keys-0.5.3.tar", last modified: Wed Jul  5 15:50:06 2023, max compression
```

## Comparing `google-cloud-api-keys-0.5.2.tar` & `google-cloud-api-keys-0.5.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:17.919017 google-cloud-api-keys-0.5.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4431 2023-03-27 15:52:17.919017 google-cloud-api-keys-0.5.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3525 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:17.911014 google-cloud-api-keys-0.5.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:17.911014 google-cloud-api-keys-0.5.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:17.911014 google-cloud-api-keys-0.5.2/google/cloud/api_keys/
--rw-rw-r--   0 root         (0)     1003     1929 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/google/cloud/api_keys/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/google/cloud/api_keys/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/google/cloud/api_keys/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:17.915016 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/
--rw-rw-r--   0 root         (0)     1003     1786 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     3372 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:17.915016 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:17.915016 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/api_keys/
--rw-rw-r--   0 root         (0)     1003      741 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/api_keys/__init__.py
--rw-rw-r--   0 root         (0)     1003    46724 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/api_keys/async_client.py
--rw-rw-r--   0 root         (0)     1003    56777 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/api_keys/client.py
--rw-rw-r--   0 root         (0)     1003     5566 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/api_keys/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:17.915016 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/api_keys/transports/
--rw-rw-r--   0 root         (0)     1003     1302 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/api_keys/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9384 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/api_keys/transports/base.py
--rw-rw-r--   0 root         (0)     1003    21761 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/api_keys/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    22172 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/api_keys/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    50938 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/api_keys/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:17.915016 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/types/
--rw-rw-r--   0 root         (0)     1003     1547 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     7812 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/types/apikeys.py
--rw-rw-r--   0 root         (0)     1003    10652 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/types/resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:17.919017 google-cloud-api-keys-0.5.2/google_cloud_api_keys.egg-info/
--rw-r--r--   0 root         (0)     1003     4431 2023-03-27 15:52:17.000000 google-cloud-api-keys-0.5.2/google_cloud_api_keys.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1507 2023-03-27 15:52:17.000000 google-cloud-api-keys-0.5.2/google_cloud_api_keys.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:52:17.000000 google-cloud-api-keys-0.5.2/google_cloud_api_keys.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:52:17.000000 google-cloud-api-keys-0.5.2/google_cloud_api_keys.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:52:17.000000 google-cloud-api-keys-0.5.2/google_cloud_api_keys.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 15:52:17.000000 google-cloud-api-keys-0.5.2/google_cloud_api_keys.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:52:17.000000 google-cloud-api-keys-0.5.2/google_cloud_api_keys.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:52:17.919017 google-cloud-api-keys-0.5.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2925 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:17.919017 google-cloud-api-keys-0.5.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:17.919017 google-cloud-api-keys-0.5.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:17.919017 google-cloud-api-keys-0.5.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:17.919017 google-cloud-api-keys-0.5.2/tests/unit/gapic/api_keys_v2/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/tests/unit/gapic/api_keys_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003   204812 2023-03-27 15:49:48.000000 google-cloud-api-keys-0.5.2/tests/unit/gapic/api_keys_v2/test_api_keys.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:06.774448 google-cloud-api-keys-0.5.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4399 2023-07-05 15:50:06.774448 google-cloud-api-keys-0.5.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3489 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:06.766447 google-cloud-api-keys-0.5.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:06.766447 google-cloud-api-keys-0.5.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:06.770448 google-cloud-api-keys-0.5.3/google/cloud/api_keys/
+-rw-rw-r--   0 root         (0)     1003     1929 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/google/cloud/api_keys/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/google/cloud/api_keys/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/google/cloud/api_keys/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:06.770448 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/
+-rw-rw-r--   0 root         (0)     1003     1786 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3372 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:06.770448 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:06.770448 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/api_keys/
+-rw-rw-r--   0 root         (0)     1003      741 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/api_keys/__init__.py
+-rw-rw-r--   0 root         (0)     1003    46748 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/api_keys/async_client.py
+-rw-rw-r--   0 root         (0)     1003    56777 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/api_keys/client.py
+-rw-rw-r--   0 root         (0)     1003     5566 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/api_keys/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:06.770448 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/api_keys/transports/
+-rw-rw-r--   0 root         (0)     1003     1302 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/api_keys/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9384 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/api_keys/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    21761 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/api_keys/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    22172 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/api_keys/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    50938 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/api_keys/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:06.770448 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/types/
+-rw-rw-r--   0 root         (0)     1003     1547 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7812 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/types/apikeys.py
+-rw-rw-r--   0 root         (0)     1003    10652 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/types/resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:06.774448 google-cloud-api-keys-0.5.3/google_cloud_api_keys.egg-info/
+-rw-r--r--   0 root         (0)     1003     4399 2023-07-05 15:50:06.000000 google-cloud-api-keys-0.5.3/google_cloud_api_keys.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1507 2023-07-05 15:50:06.000000 google-cloud-api-keys-0.5.3/google_cloud_api_keys.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:06.000000 google-cloud-api-keys-0.5.3/google_cloud_api_keys.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:50:06.000000 google-cloud-api-keys-0.5.3/google_cloud_api_keys.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:06.000000 google-cloud-api-keys-0.5.3/google_cloud_api_keys.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:50:06.000000 google-cloud-api-keys-0.5.3/google_cloud_api_keys.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:50:06.000000 google-cloud-api-keys-0.5.3/google_cloud_api_keys.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:50:06.774448 google-cloud-api-keys-0.5.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2929 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:06.774448 google-cloud-api-keys-0.5.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:06.774448 google-cloud-api-keys-0.5.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:06.774448 google-cloud-api-keys-0.5.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:06.774448 google-cloud-api-keys-0.5.3/tests/unit/gapic/api_keys_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/tests/unit/gapic/api_keys_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   205011 2023-07-05 15:46:58.000000 google-cloud-api-keys-0.5.3/tests/unit/gapic/api_keys_v2/test_api_keys.py
```

### Comparing `google-cloud-api-keys-0.5.2/LICENSE` & `google-cloud-api-keys-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/MANIFEST.in` & `google-cloud-api-keys-0.5.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/PKG-INFO` & `google-cloud-api-keys-0.5.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-api-keys
-Version: 0.5.2
+Version: 0.5.3
 Summary: Google Cloud Api Keys API client library
-Home-page: https://github.com/googleapis/python-api-keys
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for API Keys API
-==============================
+Python Client for API Keys
+==========================
 
 |preview| |pypi| |versions|
 
-`API Keys API`_: 
+`API Keys`_: 
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-api-keys.svg
    :target: https://pypi.org/project/google-cloud-api-keys/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-api-keys.svg
    :target: https://pypi.org/project/google-cloud-api-keys/
-.. _API Keys API: https://cloud.google.com/api-keys/docs
+.. _API Keys: https://cloud.google.com/api-keys/docs
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/apikeys/latest
 .. _Product Documentation:  https://cloud.google.com/api-keys/docs
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the API Keys API.`_
+3. `Enable the API Keys.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the API Keys API.:  https://cloud.google.com/api-keys/docs
+.. _Enable the API Keys.:  https://cloud.google.com/api-keys/docs
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-api-keys
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for API Keys API
+-  Read the `Client Library Documentation`_ for API Keys
    to see other available methods on the client.
--  Read the `API Keys API Product documentation`_ to learn
+-  Read the `API Keys Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _API Keys API Product documentation:  https://cloud.google.com/api-keys/docs
+.. _API Keys Product documentation:  https://cloud.google.com/api-keys/docs
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-api-keys-0.5.2/README.rst` & `google-cloud-api-keys-0.5.3/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for API Keys API
-==============================
+Python Client for API Keys
+==========================
 
 |preview| |pypi| |versions|
 
-`API Keys API`_: 
+`API Keys`_: 
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-api-keys.svg
    :target: https://pypi.org/project/google-cloud-api-keys/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-api-keys.svg
    :target: https://pypi.org/project/google-cloud-api-keys/
-.. _API Keys API: https://cloud.google.com/api-keys/docs
+.. _API Keys: https://cloud.google.com/api-keys/docs
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/apikeys/latest
 .. _Product Documentation:  https://cloud.google.com/api-keys/docs
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the API Keys API.`_
+3. `Enable the API Keys.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the API Keys API.:  https://cloud.google.com/api-keys/docs
+.. _Enable the API Keys.:  https://cloud.google.com/api-keys/docs
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-api-keys
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for API Keys API
+-  Read the `Client Library Documentation`_ for API Keys
    to see other available methods on the client.
--  Read the `API Keys API Product documentation`_ to learn
+-  Read the `API Keys Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _API Keys API Product documentation:  https://cloud.google.com/api-keys/docs
+.. _API Keys Product documentation:  https://cloud.google.com/api-keys/docs
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-api-keys-0.5.2/google/cloud/api_keys/__init__.py` & `google-cloud-api-keys-0.5.3/google/cloud/api_keys/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/google/cloud/api_keys/gapic_version.py` & `google-cloud-api-keys-0.5.3/google/cloud/api_keys/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.5.2"  # {x-release-please-version}
+__version__ = "0.5.3"  # {x-release-please-version}
```

### Comparing `google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/__init__.py` & `google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/gapic_metadata.json` & `google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/gapic_version.py` & `google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.5.2"  # {x-release-please-version}
+__version__ = "0.5.3"  # {x-release-please-version}
```

### Comparing `google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/__init__.py` & `google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/api_keys/__init__.py` & `google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/api_keys/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/api_keys/async_client.py` & `google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/api_keys/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1164,15 +1164,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ApiKeysAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/api_keys/client.py` & `google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/api_keys/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/api_keys/pagers.py` & `google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/api_keys/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/api_keys/transports/__init__.py` & `google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/api_keys/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/api_keys/transports/base.py` & `google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/api_keys/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/api_keys/transports/grpc.py` & `google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/api_keys/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/api_keys/transports/grpc_asyncio.py` & `google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/api_keys/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/services/api_keys/transports/rest.py` & `google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/services/api_keys/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/types/__init__.py` & `google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/types/apikeys.py` & `google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/types/apikeys.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/google/cloud/api_keys_v2/types/resources.py` & `google-cloud-api-keys-0.5.3/google/cloud/api_keys_v2/types/resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/google_cloud_api_keys.egg-info/PKG-INFO` & `google-cloud-api-keys-0.5.3/google_cloud_api_keys.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-api-keys
-Version: 0.5.2
+Version: 0.5.3
 Summary: Google Cloud Api Keys API client library
-Home-page: https://github.com/googleapis/python-api-keys
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for API Keys API
-==============================
+Python Client for API Keys
+==========================
 
 |preview| |pypi| |versions|
 
-`API Keys API`_: 
+`API Keys`_: 
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-api-keys.svg
    :target: https://pypi.org/project/google-cloud-api-keys/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-api-keys.svg
    :target: https://pypi.org/project/google-cloud-api-keys/
-.. _API Keys API: https://cloud.google.com/api-keys/docs
+.. _API Keys: https://cloud.google.com/api-keys/docs
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/apikeys/latest
 .. _Product Documentation:  https://cloud.google.com/api-keys/docs
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the API Keys API.`_
+3. `Enable the API Keys.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the API Keys API.:  https://cloud.google.com/api-keys/docs
+.. _Enable the API Keys.:  https://cloud.google.com/api-keys/docs
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-api-keys
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for API Keys API
+-  Read the `Client Library Documentation`_ for API Keys
    to see other available methods on the client.
--  Read the `API Keys API Product documentation`_ to learn
+-  Read the `API Keys Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _API Keys API Product documentation:  https://cloud.google.com/api-keys/docs
+.. _API Keys Product documentation:  https://cloud.google.com/api-keys/docs
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-api-keys-0.5.2/google_cloud_api_keys.egg-info/SOURCES.txt` & `google-cloud-api-keys-0.5.3/google_cloud_api_keys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/setup.py` & `google-cloud-api-keys-0.5.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-api-keys"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-api-keys-0.5.2/tests/__init__.py` & `google-cloud-api-keys-0.5.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/tests/unit/__init__.py` & `google-cloud-api-keys-0.5.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/tests/unit/gapic/__init__.py` & `google-cloud-api-keys-0.5.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/tests/unit/gapic/api_keys_v2/__init__.py` & `google-cloud-api-keys-0.5.3/tests/unit/gapic/api_keys_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-keys-0.5.2/tests/unit/gapic/api_keys_v2/test_api_keys.py` & `google-cloud-api-keys-0.5.3/tests/unit/gapic/api_keys_v2/test_api_keys.py`

 * *Files 0% similar despite different names*

```diff
@@ -1330,17 +1330,19 @@
                     resources.Key(),
                     resources.Key(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_keys(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

