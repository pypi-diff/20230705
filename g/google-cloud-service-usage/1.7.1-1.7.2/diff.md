# Comparing `tmp/google-cloud-service-usage-1.7.1.tar.gz` & `tmp/google-cloud-service-usage-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-service-usage-1.7.1.tar", last modified: Mon Mar 27 15:45:00 2023, max compression
+gzip compressed data, was "google-cloud-service-usage-1.7.2.tar", last modified: Wed Jul  5 15:55:50 2023, max compression
```

## Comparing `google-cloud-service-usage-1.7.1.tar` & `google-cloud-service-usage-1.7.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:45:00.296436 google-cloud-service-usage-1.7.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:42:02.000000 google-cloud-service-usage-1.7.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:42:02.000000 google-cloud-service-usage-1.7.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4656 2023-03-27 15:45:00.296436 google-cloud-service-usage-1.7.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3722 2023-03-27 15:42:02.000000 google-cloud-service-usage-1.7.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:45:00.284435 google-cloud-service-usage-1.7.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:45:00.284435 google-cloud-service-usage-1.7.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:45:00.288435 google-cloud-service-usage-1.7.1/google/cloud/service_usage/
--rw-rw-r--   0 root         (0)     1003     1901 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/google/cloud/service_usage/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/google/cloud/service_usage/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       87 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/google/cloud/service_usage/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:45:00.288435 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/
--rw-rw-r--   0 root         (0)     1003     1694 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2895 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       87 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:45:00.288435 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:45:00.292436 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/service_usage/
--rw-rw-r--   0 root         (0)     1003      761 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/service_usage/__init__.py
--rw-rw-r--   0 root         (0)     1003    31702 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/service_usage/async_client.py
--rw-rw-r--   0 root         (0)     1003    41010 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/service_usage/client.py
--rw-rw-r--   0 root         (0)     1003     5794 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/service_usage/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:45:00.292436 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/service_usage/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/service_usage/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8693 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/service_usage/transports/base.py
--rw-rw-r--   0 root         (0)     1003    19739 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/service_usage/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20148 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/service_usage/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    37246 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/service_usage/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:45:00.292436 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/types/
--rw-rw-r--   0 root         (0)     1003     1425 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     7066 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/types/resources.py
--rw-rw-r--   0 root         (0)     1003    11587 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/types/serviceusage.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:45:00.292436 google-cloud-service-usage-1.7.1/google_cloud_service_usage.egg-info/
--rw-r--r--   0 root         (0)     1003     4656 2023-03-27 15:45:00.000000 google-cloud-service-usage-1.7.1/google_cloud_service_usage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1707 2023-03-27 15:45:00.000000 google-cloud-service-usage-1.7.1/google_cloud_service_usage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:45:00.000000 google-cloud-service-usage-1.7.1/google_cloud_service_usage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:45:00.000000 google-cloud-service-usage-1.7.1/google_cloud_service_usage.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:45:00.000000 google-cloud-service-usage-1.7.1/google_cloud_service_usage.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 15:45:00.000000 google-cloud-service-usage-1.7.1/google_cloud_service_usage.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:45:00.000000 google-cloud-service-usage-1.7.1/google_cloud_service_usage.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:45:00.296436 google-cloud-service-usage-1.7.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2951 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:45:00.292436 google-cloud-service-usage-1.7.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:45:00.292436 google-cloud-service-usage-1.7.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:45:00.296436 google-cloud-service-usage-1.7.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:45:00.296436 google-cloud-service-usage-1.7.1/tests/unit/gapic/service_usage_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/tests/unit/gapic/service_usage_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   121617 2023-03-27 15:42:03.000000 google-cloud-service-usage-1.7.1/tests/unit/gapic/service_usage_v1/test_service_usage.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:50.669780 google-cloud-service-usage-1.7.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4619 2023-07-05 15:55:50.669780 google-cloud-service-usage-1.7.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3686 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:50.661780 google-cloud-service-usage-1.7.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:50.661780 google-cloud-service-usage-1.7.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:50.665780 google-cloud-service-usage-1.7.2/google/cloud/service_usage/
+-rw-rw-r--   0 root         (0)     1003     1901 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/google/cloud/service_usage/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/google/cloud/service_usage/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       87 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/google/cloud/service_usage/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:50.665780 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/
+-rw-rw-r--   0 root         (0)     1003     1694 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2895 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       87 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:50.665780 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:50.665780 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/service_usage/
+-rw-rw-r--   0 root         (0)     1003      761 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/service_usage/__init__.py
+-rw-rw-r--   0 root         (0)     1003    31731 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/service_usage/async_client.py
+-rw-rw-r--   0 root         (0)     1003    41010 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/service_usage/client.py
+-rw-rw-r--   0 root         (0)     1003     5794 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/service_usage/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:50.665780 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/service_usage/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/service_usage/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8693 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/service_usage/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    19739 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/service_usage/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    20148 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/service_usage/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    37246 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/service_usage/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:50.669780 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1425 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7066 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/types/resources.py
+-rw-rw-r--   0 root         (0)     1003    11587 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/types/serviceusage.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:50.669780 google-cloud-service-usage-1.7.2/google_cloud_service_usage.egg-info/
+-rw-r--r--   0 root         (0)     1003     4619 2023-07-05 15:55:50.000000 google-cloud-service-usage-1.7.2/google_cloud_service_usage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1707 2023-07-05 15:55:50.000000 google-cloud-service-usage-1.7.2/google_cloud_service_usage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:55:50.000000 google-cloud-service-usage-1.7.2/google_cloud_service_usage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:55:50.000000 google-cloud-service-usage-1.7.2/google_cloud_service_usage.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:55:50.000000 google-cloud-service-usage-1.7.2/google_cloud_service_usage.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:55:50.000000 google-cloud-service-usage-1.7.2/google_cloud_service_usage.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:55:50.000000 google-cloud-service-usage-1.7.2/google_cloud_service_usage.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:55:50.669780 google-cloud-service-usage-1.7.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2950 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:50.669780 google-cloud-service-usage-1.7.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:50.669780 google-cloud-service-usage-1.7.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:50.669780 google-cloud-service-usage-1.7.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:50.669780 google-cloud-service-usage-1.7.2/tests/unit/gapic/service_usage_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/tests/unit/gapic/service_usage_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   121816 2023-07-05 15:46:59.000000 google-cloud-service-usage-1.7.2/tests/unit/gapic/service_usage_v1/test_service_usage.py
```

### Comparing `google-cloud-service-usage-1.7.1/LICENSE` & `google-cloud-service-usage-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/MANIFEST.in` & `google-cloud-service-usage-1.7.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/PKG-INFO` & `google-cloud-service-usage-1.7.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-service-usage
-Version: 1.7.1
+Version: 1.7.2
 Summary: Google Cloud Service Usage API client library
-Home-page: https://github.com/googleapis/python-service-usage
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
 
-Python Client for Service Usage API
-===================================
+Python Client for Service Usage
+===============================
 
 |stable| |pypi| |versions|
 
-`Service Usage API`_: is an infrastructure service of Google Cloud that lets you list and manage other APIs and services in your Cloud projects.
+`Service Usage`_: is an infrastructure service of Google Cloud that lets you list and manage other APIs and services in your Cloud projects.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-service-usage.svg
    :target: https://pypi.org/project/google-cloud-service-usage/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-service-usage.svg
    :target: https://pypi.org/project/google-cloud-service-usage/
-.. _Service Usage API: https://cloud.google.com/service-usage
+.. _Service Usage: https://cloud.google.com/service-usage
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/serviceusage/latest
 .. _Product Documentation:  https://cloud.google.com/service-usage
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Service Usage API.`_
+3. `Enable the Service Usage.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Service Usage API.:  https://cloud.google.com/service-usage
+.. _Enable the Service Usage.:  https://cloud.google.com/service-usage
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-service-usage
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Service Usage API
+-  Read the `Client Library Documentation`_ for Service Usage
    to see other available methods on the client.
--  Read the `Service Usage API Product documentation`_ to learn
+-  Read the `Service Usage Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Service Usage API Product documentation:  https://cloud.google.com/service-usage
+.. _Service Usage Product documentation:  https://cloud.google.com/service-usage
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-service-usage-1.7.1/README.rst` & `google-cloud-service-usage-1.7.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Service Usage API
-===================================
+Python Client for Service Usage
+===============================
 
 |stable| |pypi| |versions|
 
-`Service Usage API`_: is an infrastructure service of Google Cloud that lets you list and manage other APIs and services in your Cloud projects.
+`Service Usage`_: is an infrastructure service of Google Cloud that lets you list and manage other APIs and services in your Cloud projects.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-service-usage.svg
    :target: https://pypi.org/project/google-cloud-service-usage/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-service-usage.svg
    :target: https://pypi.org/project/google-cloud-service-usage/
-.. _Service Usage API: https://cloud.google.com/service-usage
+.. _Service Usage: https://cloud.google.com/service-usage
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/serviceusage/latest
 .. _Product Documentation:  https://cloud.google.com/service-usage
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Service Usage API.`_
+3. `Enable the Service Usage.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Service Usage API.:  https://cloud.google.com/service-usage
+.. _Enable the Service Usage.:  https://cloud.google.com/service-usage
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-service-usage
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Service Usage API
+-  Read the `Client Library Documentation`_ for Service Usage
    to see other available methods on the client.
--  Read the `Service Usage API Product documentation`_ to learn
+-  Read the `Service Usage Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Service Usage API Product documentation:  https://cloud.google.com/service-usage
+.. _Service Usage Product documentation:  https://cloud.google.com/service-usage
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-service-usage-1.7.1/google/cloud/service_usage/__init__.py` & `google-cloud-service-usage-1.7.2/google/cloud/service_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/google/cloud/service_usage/gapic_version.py` & `google-cloud-service-usage-1.7.2/google/cloud/service_usage/gapic_version.py`

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
-__version__ = "1.7.1"  # {x-release-please-version}
+__version__ = "1.7.2"  # {x-release-please-version}
```

### Comparing `google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/__init__.py` & `google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/gapic_metadata.json` & `google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/gapic_version.py` & `google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/gapic_version.py`

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
-__version__ = "1.7.1"  # {x-release-please-version}
+__version__ = "1.7.2"  # {x-release-please-version}
```

### Comparing `google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/__init__.py` & `google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/service_usage/__init__.py` & `google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/service_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/service_usage/async_client.py` & `google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/service_usage/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -765,15 +765,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ServiceUsageAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/service_usage/client.py` & `google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/service_usage/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/service_usage/pagers.py` & `google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/service_usage/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/service_usage/transports/__init__.py` & `google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/service_usage/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/service_usage/transports/base.py` & `google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/service_usage/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/service_usage/transports/grpc.py` & `google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/service_usage/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/service_usage/transports/grpc_asyncio.py` & `google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/service_usage/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/services/service_usage/transports/rest.py` & `google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/services/service_usage/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/types/__init__.py` & `google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/types/resources.py` & `google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/types/resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/google/cloud/service_usage_v1/types/serviceusage.py` & `google-cloud-service-usage-1.7.2/google/cloud/service_usage_v1/types/serviceusage.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/google_cloud_service_usage.egg-info/PKG-INFO` & `google-cloud-service-usage-1.7.2/google_cloud_service_usage.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-service-usage
-Version: 1.7.1
+Version: 1.7.2
 Summary: Google Cloud Service Usage API client library
-Home-page: https://github.com/googleapis/python-service-usage
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
 
-Python Client for Service Usage API
-===================================
+Python Client for Service Usage
+===============================
 
 |stable| |pypi| |versions|
 
-`Service Usage API`_: is an infrastructure service of Google Cloud that lets you list and manage other APIs and services in your Cloud projects.
+`Service Usage`_: is an infrastructure service of Google Cloud that lets you list and manage other APIs and services in your Cloud projects.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-service-usage.svg
    :target: https://pypi.org/project/google-cloud-service-usage/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-service-usage.svg
    :target: https://pypi.org/project/google-cloud-service-usage/
-.. _Service Usage API: https://cloud.google.com/service-usage
+.. _Service Usage: https://cloud.google.com/service-usage
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/serviceusage/latest
 .. _Product Documentation:  https://cloud.google.com/service-usage
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Service Usage API.`_
+3. `Enable the Service Usage.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Service Usage API.:  https://cloud.google.com/service-usage
+.. _Enable the Service Usage.:  https://cloud.google.com/service-usage
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-service-usage
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Service Usage API
+-  Read the `Client Library Documentation`_ for Service Usage
    to see other available methods on the client.
--  Read the `Service Usage API Product documentation`_ to learn
+-  Read the `Service Usage Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Service Usage API Product documentation:  https://cloud.google.com/service-usage
+.. _Service Usage Product documentation:  https://cloud.google.com/service-usage
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-service-usage-1.7.1/google_cloud_service_usage.egg-info/SOURCES.txt` & `google-cloud-service-usage-1.7.2/google_cloud_service_usage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/setup.py` & `google-cloud-service-usage-1.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-service-usage"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-service-usage-1.7.1/tests/__init__.py` & `google-cloud-service-usage-1.7.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/tests/unit/__init__.py` & `google-cloud-service-usage-1.7.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/tests/unit/gapic/__init__.py` & `google-cloud-service-usage-1.7.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/tests/unit/gapic/service_usage_v1/__init__.py` & `google-cloud-service-usage-1.7.2/tests/unit/gapic/service_usage_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-usage-1.7.1/tests/unit/gapic/service_usage_v1/test_service_usage.py` & `google-cloud-service-usage-1.7.2/tests/unit/gapic/service_usage_v1/test_service_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1473,17 +1473,19 @@
                     resources.Service(),
                     resources.Service(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_services(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

