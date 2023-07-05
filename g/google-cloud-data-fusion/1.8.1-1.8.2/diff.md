# Comparing `tmp/google-cloud-data-fusion-1.8.1.tar.gz` & `tmp/google-cloud-data-fusion-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-data-fusion-1.8.1.tar", last modified: Mon Mar 27 15:37:56 2023, max compression
+gzip compressed data, was "google-cloud-data-fusion-1.8.2.tar", last modified: Wed Jul  5 15:51:46 2023, max compression
```

## Comparing `google-cloud-data-fusion-1.8.1.tar` & `google-cloud-data-fusion-1.8.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:56.551154 google-cloud-data-fusion-1.8.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4661 2023-03-27 15:37:56.551154 google-cloud-data-fusion-1.8.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3733 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:56.543154 google-cloud-data-fusion-1.8.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:56.543154 google-cloud-data-fusion-1.8.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:56.543154 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion/
--rw-rw-r--   0 root         (0)     1003     1788 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       85 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:56.547154 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/
--rw-rw-r--   0 root         (0)     1003     1648 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3278 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       85 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:56.547154 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:56.547154 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/data_fusion/
--rw-rw-r--   0 root         (0)     1003      753 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/data_fusion/__init__.py
--rw-rw-r--   0 root         (0)     1003    41251 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/data_fusion/async_client.py
--rw-rw-r--   0 root         (0)     1003    51935 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/data_fusion/client.py
--rw-rw-r--   0 root         (0)     1003    11009 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/data_fusion/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:56.547154 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/data_fusion/transports/
--rw-rw-r--   0 root         (0)     1003     1344 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/data_fusion/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8966 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/data_fusion/transports/base.py
--rw-rw-r--   0 root         (0)     1003    19474 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/data_fusion/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19922 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/data_fusion/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    45446 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/data_fusion/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:56.547154 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/types/
--rw-rw-r--   0 root         (0)     1003     1397 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    27256 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/types/datafusion.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:56.551154 google-cloud-data-fusion-1.8.1/google_cloud_data_fusion.egg-info/
--rw-r--r--   0 root         (0)     1003     4661 2023-03-27 15:37:56.000000 google-cloud-data-fusion-1.8.1/google_cloud_data_fusion.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1580 2023-03-27 15:37:56.000000 google-cloud-data-fusion-1.8.1/google_cloud_data_fusion.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:37:56.000000 google-cloud-data-fusion-1.8.1/google_cloud_data_fusion.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:37:56.000000 google-cloud-data-fusion-1.8.1/google_cloud_data_fusion.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:37:56.000000 google-cloud-data-fusion-1.8.1/google_cloud_data_fusion.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 15:37:56.000000 google-cloud-data-fusion-1.8.1/google_cloud_data_fusion.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:37:56.000000 google-cloud-data-fusion-1.8.1/google_cloud_data_fusion.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:37:56.551154 google-cloud-data-fusion-1.8.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2943 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:56.551154 google-cloud-data-fusion-1.8.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:56.551154 google-cloud-data-fusion-1.8.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:56.551154 google-cloud-data-fusion-1.8.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:56.551154 google-cloud-data-fusion-1.8.1/tests/unit/gapic/data_fusion_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/tests/unit/gapic/data_fusion_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   199242 2023-03-27 15:35:07.000000 google-cloud-data-fusion-1.8.1/tests/unit/gapic/data_fusion_v1/test_data_fusion.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:46.004617 google-cloud-data-fusion-1.8.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4626 2023-07-05 15:51:46.004617 google-cloud-data-fusion-1.8.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3697 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:45.996617 google-cloud-data-fusion-1.8.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:45.996617 google-cloud-data-fusion-1.8.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:46.000617 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion/
+-rw-rw-r--   0 root         (0)     1003     1788 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       85 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:46.000617 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/
+-rw-rw-r--   0 root         (0)     1003     1648 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3278 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       85 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:46.000617 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:46.000617 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/data_fusion/
+-rw-rw-r--   0 root         (0)     1003      753 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/data_fusion/__init__.py
+-rw-rw-r--   0 root         (0)     1003    41278 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/data_fusion/async_client.py
+-rw-rw-r--   0 root         (0)     1003    51935 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/data_fusion/client.py
+-rw-rw-r--   0 root         (0)     1003    11009 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/data_fusion/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:46.000617 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/data_fusion/transports/
+-rw-rw-r--   0 root         (0)     1003     1344 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/data_fusion/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8966 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/data_fusion/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    19474 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/data_fusion/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19922 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/data_fusion/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    45446 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/data_fusion/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:46.000617 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1397 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27256 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/types/datafusion.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:46.004617 google-cloud-data-fusion-1.8.2/google_cloud_data_fusion.egg-info/
+-rw-r--r--   0 root         (0)     1003     4626 2023-07-05 15:51:45.000000 google-cloud-data-fusion-1.8.2/google_cloud_data_fusion.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1580 2023-07-05 15:51:45.000000 google-cloud-data-fusion-1.8.2/google_cloud_data_fusion.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:51:45.000000 google-cloud-data-fusion-1.8.2/google_cloud_data_fusion.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:51:45.000000 google-cloud-data-fusion-1.8.2/google_cloud_data_fusion.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:51:45.000000 google-cloud-data-fusion-1.8.2/google_cloud_data_fusion.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:51:45.000000 google-cloud-data-fusion-1.8.2/google_cloud_data_fusion.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:51:45.000000 google-cloud-data-fusion-1.8.2/google_cloud_data_fusion.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:51:46.004617 google-cloud-data-fusion-1.8.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2944 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:46.004617 google-cloud-data-fusion-1.8.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:46.004617 google-cloud-data-fusion-1.8.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:46.004617 google-cloud-data-fusion-1.8.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:46.004617 google-cloud-data-fusion-1.8.2/tests/unit/gapic/data_fusion_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/tests/unit/gapic/data_fusion_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   199640 2023-07-05 15:46:58.000000 google-cloud-data-fusion-1.8.2/tests/unit/gapic/data_fusion_v1/test_data_fusion.py
```

### Comparing `google-cloud-data-fusion-1.8.1/LICENSE` & `google-cloud-data-fusion-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-data-fusion-1.8.1/MANIFEST.in` & `google-cloud-data-fusion-1.8.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-data-fusion-1.8.1/PKG-INFO` & `google-cloud-data-fusion-1.8.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-data-fusion
-Version: 1.8.1
+Version: 1.8.2
 Summary: Google Cloud Data Fusion API client library
-Home-page: https://github.com/googleapis/python-data-fusion
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for Cloud Data Fusion API
-=======================================
+Python Client for Cloud Data Fusion
+===================================
 
 |stable| |pypi| |versions|
 
-`Cloud Data Fusion API`_: is a fully managed, cloud-native, enterprise data integration service for quickly building and managing data pipelines.
+`Cloud Data Fusion`_: is a fully managed, cloud-native, enterprise data integration service for quickly building and managing data pipelines.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-data-fusion.svg
    :target: https://pypi.org/project/google-cloud-data-fusion/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-data-fusion.svg
    :target: https://pypi.org/project/google-cloud-data-fusion/
-.. _Cloud Data Fusion API: https://cloud.google.com/data-fusion
+.. _Cloud Data Fusion: https://cloud.google.com/data-fusion
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/datafusion/latest
 .. _Product Documentation:  https://cloud.google.com/data-fusion
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Data Fusion API.`_
+3. `Enable the Cloud Data Fusion.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Data Fusion API.:  https://cloud.google.com/data-fusion
+.. _Enable the Cloud Data Fusion.:  https://cloud.google.com/data-fusion
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-data-fusion
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Data Fusion API
+-  Read the `Client Library Documentation`_ for Cloud Data Fusion
    to see other available methods on the client.
--  Read the `Cloud Data Fusion API Product documentation`_ to learn
+-  Read the `Cloud Data Fusion Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Data Fusion API Product documentation:  https://cloud.google.com/data-fusion
+.. _Cloud Data Fusion Product documentation:  https://cloud.google.com/data-fusion
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-data-fusion-1.8.1/README.rst` & `google-cloud-data-fusion-1.8.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Cloud Data Fusion API
-=======================================
+Python Client for Cloud Data Fusion
+===================================
 
 |stable| |pypi| |versions|
 
-`Cloud Data Fusion API`_: is a fully managed, cloud-native, enterprise data integration service for quickly building and managing data pipelines.
+`Cloud Data Fusion`_: is a fully managed, cloud-native, enterprise data integration service for quickly building and managing data pipelines.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-data-fusion.svg
    :target: https://pypi.org/project/google-cloud-data-fusion/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-data-fusion.svg
    :target: https://pypi.org/project/google-cloud-data-fusion/
-.. _Cloud Data Fusion API: https://cloud.google.com/data-fusion
+.. _Cloud Data Fusion: https://cloud.google.com/data-fusion
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/datafusion/latest
 .. _Product Documentation:  https://cloud.google.com/data-fusion
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Data Fusion API.`_
+3. `Enable the Cloud Data Fusion.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Data Fusion API.:  https://cloud.google.com/data-fusion
+.. _Enable the Cloud Data Fusion.:  https://cloud.google.com/data-fusion
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-data-fusion
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Data Fusion API
+-  Read the `Client Library Documentation`_ for Cloud Data Fusion
    to see other available methods on the client.
--  Read the `Cloud Data Fusion API Product documentation`_ to learn
+-  Read the `Cloud Data Fusion Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Data Fusion API Product documentation:  https://cloud.google.com/data-fusion
+.. _Cloud Data Fusion Product documentation:  https://cloud.google.com/data-fusion
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-data-fusion-1.8.1/google/cloud/data_fusion/__init__.py` & `google-cloud-data-fusion-1.8.2/google/cloud/data_fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-fusion-1.8.1/google/cloud/data_fusion/gapic_version.py` & `google-cloud-data-fusion-1.8.2/google/cloud/data_fusion/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.1"  # {x-release-please-version}
+__version__ = "1.8.2"  # {x-release-please-version}
```

### Comparing `google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/__init__.py` & `google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/gapic_metadata.json` & `google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/gapic_version.py` & `google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.1"  # {x-release-please-version}
+__version__ = "1.8.2"  # {x-release-please-version}
```

### Comparing `google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/__init__.py` & `google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/data_fusion/__init__.py` & `google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/data_fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/data_fusion/async_client.py` & `google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/data_fusion/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1008,15 +1008,15 @@
             datafusion.Instance,
             metadata_type=datafusion.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "DataFusionAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/data_fusion/client.py` & `google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/data_fusion/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/data_fusion/pagers.py` & `google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/data_fusion/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/data_fusion/transports/__init__.py` & `google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/data_fusion/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/data_fusion/transports/base.py` & `google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/data_fusion/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/data_fusion/transports/grpc.py` & `google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/data_fusion/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/data_fusion/transports/grpc_asyncio.py` & `google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/data_fusion/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/services/data_fusion/transports/rest.py` & `google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/services/data_fusion/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/types/__init__.py` & `google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-fusion-1.8.1/google/cloud/data_fusion_v1/types/datafusion.py` & `google-cloud-data-fusion-1.8.2/google/cloud/data_fusion_v1/types/datafusion.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-fusion-1.8.1/google_cloud_data_fusion.egg-info/PKG-INFO` & `google-cloud-data-fusion-1.8.2/google_cloud_data_fusion.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-data-fusion
-Version: 1.8.1
+Version: 1.8.2
 Summary: Google Cloud Data Fusion API client library
-Home-page: https://github.com/googleapis/python-data-fusion
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for Cloud Data Fusion API
-=======================================
+Python Client for Cloud Data Fusion
+===================================
 
 |stable| |pypi| |versions|
 
-`Cloud Data Fusion API`_: is a fully managed, cloud-native, enterprise data integration service for quickly building and managing data pipelines.
+`Cloud Data Fusion`_: is a fully managed, cloud-native, enterprise data integration service for quickly building and managing data pipelines.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-data-fusion.svg
    :target: https://pypi.org/project/google-cloud-data-fusion/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-data-fusion.svg
    :target: https://pypi.org/project/google-cloud-data-fusion/
-.. _Cloud Data Fusion API: https://cloud.google.com/data-fusion
+.. _Cloud Data Fusion: https://cloud.google.com/data-fusion
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/datafusion/latest
 .. _Product Documentation:  https://cloud.google.com/data-fusion
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Data Fusion API.`_
+3. `Enable the Cloud Data Fusion.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Data Fusion API.:  https://cloud.google.com/data-fusion
+.. _Enable the Cloud Data Fusion.:  https://cloud.google.com/data-fusion
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-data-fusion
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Data Fusion API
+-  Read the `Client Library Documentation`_ for Cloud Data Fusion
    to see other available methods on the client.
--  Read the `Cloud Data Fusion API Product documentation`_ to learn
+-  Read the `Cloud Data Fusion Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Data Fusion API Product documentation:  https://cloud.google.com/data-fusion
+.. _Cloud Data Fusion Product documentation:  https://cloud.google.com/data-fusion
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-data-fusion-1.8.1/google_cloud_data_fusion.egg-info/SOURCES.txt` & `google-cloud-data-fusion-1.8.2/google_cloud_data_fusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-data-fusion-1.8.1/setup.py` & `google-cloud-data-fusion-1.8.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-data-fusion"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-data-fusion-1.8.1/tests/__init__.py` & `google-cloud-data-fusion-1.8.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-fusion-1.8.1/tests/unit/__init__.py` & `google-cloud-data-fusion-1.8.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-fusion-1.8.1/tests/unit/gapic/__init__.py` & `google-cloud-data-fusion-1.8.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-fusion-1.8.1/tests/unit/gapic/data_fusion_v1/__init__.py` & `google-cloud-data-fusion-1.8.2/tests/unit/gapic/data_fusion_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-fusion-1.8.1/tests/unit/gapic/data_fusion_v1/test_data_fusion.py` & `google-cloud-data-fusion-1.8.2/tests/unit/gapic/data_fusion_v1/test_data_fusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1123,17 +1123,19 @@
                     datafusion.Version(),
                     datafusion.Version(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_available_versions(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1465,17 +1467,19 @@
                     datafusion.Instance(),
                     datafusion.Instance(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_instances(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

