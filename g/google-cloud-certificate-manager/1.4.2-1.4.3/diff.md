# Comparing `tmp/google-cloud-certificate-manager-1.4.2.tar.gz` & `tmp/google-cloud-certificate-manager-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-certificate-manager-1.4.2.tar", last modified: Mon Mar 27 15:52:21 2023, max compression
+gzip compressed data, was "google-cloud-certificate-manager-1.4.3.tar", last modified: Wed Jul  5 15:51:23 2023, max compression
```

## Comparing `google-cloud-certificate-manager-1.4.2.tar` & `google-cloud-certificate-manager-1.4.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:21.559856 google-cloud-certificate-manager-1.4.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4869 2023-03-27 15:52:21.559856 google-cloud-certificate-manager-1.4.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3917 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:21.551854 google-cloud-certificate-manager-1.4.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:21.551854 google-cloud-certificate-manager-1.4.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:21.555855 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager/
--rw-rw-r--   0 root         (0)     1003     3638 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:21.555855 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/
--rw-rw-r--   0 root         (0)     1003     3435 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    10841 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:21.555855 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:21.555855 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/certificate_manager/
--rw-rw-r--   0 root         (0)     1003      785 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/certificate_manager/__init__.py
--rw-rw-r--   0 root         (0)     1003   156139 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/certificate_manager/async_client.py
--rw-rw-r--   0 root         (0)     1003   165453 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/certificate_manager/client.py
--rw-rw-r--   0 root         (0)     1003    28589 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/certificate_manager/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:21.555855 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/certificate_manager/transports/
--rw-rw-r--   0 root         (0)     1003     1464 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/certificate_manager/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    28004 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/certificate_manager/transports/base.py
--rw-rw-r--   0 root         (0)     1003    48442 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/certificate_manager/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    49319 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/certificate_manager/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   163560 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/certificate_manager/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:21.559856 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/types/
--rw-rw-r--   0 root         (0)     1003     3117 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    10825 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/types/certificate_issuance_config.py
--rw-rw-r--   0 root         (0)     1003    51498 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/types/certificate_manager.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:21.559856 google-cloud-certificate-manager-1.4.2/google_cloud_certificate_manager.egg-info/
--rw-r--r--   0 root         (0)     1003     4869 2023-03-27 15:52:21.000000 google-cloud-certificate-manager-1.4.2/google_cloud_certificate_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1966 2023-03-27 15:52:21.000000 google-cloud-certificate-manager-1.4.2/google_cloud_certificate_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:52:21.000000 google-cloud-certificate-manager-1.4.2/google_cloud_certificate_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:52:21.000000 google-cloud-certificate-manager-1.4.2/google_cloud_certificate_manager.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:52:21.000000 google-cloud-certificate-manager-1.4.2/google_cloud_certificate_manager.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 15:52:21.000000 google-cloud-certificate-manager-1.4.2/google_cloud_certificate_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:52:21.000000 google-cloud-certificate-manager-1.4.2/google_cloud_certificate_manager.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:52:21.559856 google-cloud-certificate-manager-1.4.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2975 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:21.559856 google-cloud-certificate-manager-1.4.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:21.559856 google-cloud-certificate-manager-1.4.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:21.559856 google-cloud-certificate-manager-1.4.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:21.559856 google-cloud-certificate-manager-1.4.2/tests/unit/gapic/certificate_manager_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/tests/unit/gapic/certificate_manager_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   649703 2023-03-27 15:49:44.000000 google-cloud-certificate-manager-1.4.2/tests/unit/gapic/certificate_manager_v1/test_certificate_manager.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:23.163856 google-cloud-certificate-manager-1.4.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4826 2023-07-05 15:51:23.163856 google-cloud-certificate-manager-1.4.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3881 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:23.155856 google-cloud-certificate-manager-1.4.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:23.155856 google-cloud-certificate-manager-1.4.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:23.159856 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager/
+-rw-rw-r--   0 root         (0)     1003     3638 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:23.159856 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/
+-rw-rw-r--   0 root         (0)     1003     3435 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10841 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:23.159856 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:23.159856 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/certificate_manager/
+-rw-rw-r--   0 root         (0)     1003      785 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/certificate_manager/__init__.py
+-rw-rw-r--   0 root         (0)     1003   156174 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/certificate_manager/async_client.py
+-rw-rw-r--   0 root         (0)     1003   165453 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/certificate_manager/client.py
+-rw-rw-r--   0 root         (0)     1003    28589 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/certificate_manager/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:23.159856 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/certificate_manager/transports/
+-rw-rw-r--   0 root         (0)     1003     1464 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/certificate_manager/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    28004 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/certificate_manager/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    48442 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/certificate_manager/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    49319 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/certificate_manager/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   163548 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/certificate_manager/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:23.163856 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3117 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10825 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/types/certificate_issuance_config.py
+-rw-rw-r--   0 root         (0)     1003    51498 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/types/certificate_manager.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:23.163856 google-cloud-certificate-manager-1.4.3/google_cloud_certificate_manager.egg-info/
+-rw-r--r--   0 root         (0)     1003     4826 2023-07-05 15:51:23.000000 google-cloud-certificate-manager-1.4.3/google_cloud_certificate_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1966 2023-07-05 15:51:23.000000 google-cloud-certificate-manager-1.4.3/google_cloud_certificate_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:51:23.000000 google-cloud-certificate-manager-1.4.3/google_cloud_certificate_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:51:23.000000 google-cloud-certificate-manager-1.4.3/google_cloud_certificate_manager.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:51:23.000000 google-cloud-certificate-manager-1.4.3/google_cloud_certificate_manager.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:51:23.000000 google-cloud-certificate-manager-1.4.3/google_cloud_certificate_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:51:23.000000 google-cloud-certificate-manager-1.4.3/google_cloud_certificate_manager.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:51:23.167856 google-cloud-certificate-manager-1.4.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2968 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:23.163856 google-cloud-certificate-manager-1.4.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:23.163856 google-cloud-certificate-manager-1.4.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:23.163856 google-cloud-certificate-manager-1.4.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:23.163856 google-cloud-certificate-manager-1.4.3/tests/unit/gapic/certificate_manager_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/tests/unit/gapic/certificate_manager_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   650394 2023-07-05 15:46:58.000000 google-cloud-certificate-manager-1.4.3/tests/unit/gapic/certificate_manager_v1/test_certificate_manager.py
```

### Comparing `google-cloud-certificate-manager-1.4.2/LICENSE` & `google-cloud-certificate-manager-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-certificate-manager-1.4.2/MANIFEST.in` & `google-cloud-certificate-manager-1.4.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-certificate-manager-1.4.2/PKG-INFO` & `google-cloud-certificate-manager-1.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-certificate-manager
-Version: 1.4.2
+Version: 1.4.3
 Summary: Google Cloud Certificate Manager API client library
-Home-page: https://github.com/googleapis/python-certificate-manager
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
 
-Python Client for Certificate Manager API
-=========================================
+Python Client for Certificate Manager
+=====================================
 
 |stable| |pypi| |versions|
 
-`Certificate Manager API`_: lets you acquire and manage TLS (SSL) certificates for use with Cloud Load Balancing.
+`Certificate Manager`_: lets you acquire and manage TLS (SSL) certificates for use with Cloud Load Balancing.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-certificate-manager.svg
    :target: https://pypi.org/project/google-cloud-certificate-manager/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-certificate-manager.svg
    :target: https://pypi.org/project/google-cloud-certificate-manager/
-.. _Certificate Manager API: https://cloud.google.com/python/docs/reference/certificatemanager/latest
+.. _Certificate Manager: https://cloud.google.com/python/docs/reference/certificatemanager/latest
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/certificatemanager/latest
 .. _Product Documentation:  https://cloud.google.com/python/docs/reference/certificatemanager/latest
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Certificate Manager API.`_
+3. `Enable the Certificate Manager.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Certificate Manager API.:  https://cloud.google.com/python/docs/reference/certificatemanager/latest
+.. _Enable the Certificate Manager.:  https://cloud.google.com/python/docs/reference/certificatemanager/latest
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-certificate-manager
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Certificate Manager API
+-  Read the `Client Library Documentation`_ for Certificate Manager
    to see other available methods on the client.
--  Read the `Certificate Manager API Product documentation`_ to learn
+-  Read the `Certificate Manager Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Certificate Manager API Product documentation:  https://cloud.google.com/python/docs/reference/certificatemanager/latest
+.. _Certificate Manager Product documentation:  https://cloud.google.com/python/docs/reference/certificatemanager/latest
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-certificate-manager-1.4.2/README.rst` & `google-cloud-certificate-manager-1.4.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Certificate Manager API
-=========================================
+Python Client for Certificate Manager
+=====================================
 
 |stable| |pypi| |versions|
 
-`Certificate Manager API`_: lets you acquire and manage TLS (SSL) certificates for use with Cloud Load Balancing.
+`Certificate Manager`_: lets you acquire and manage TLS (SSL) certificates for use with Cloud Load Balancing.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-certificate-manager.svg
    :target: https://pypi.org/project/google-cloud-certificate-manager/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-certificate-manager.svg
    :target: https://pypi.org/project/google-cloud-certificate-manager/
-.. _Certificate Manager API: https://cloud.google.com/python/docs/reference/certificatemanager/latest
+.. _Certificate Manager: https://cloud.google.com/python/docs/reference/certificatemanager/latest
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/certificatemanager/latest
 .. _Product Documentation:  https://cloud.google.com/python/docs/reference/certificatemanager/latest
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Certificate Manager API.`_
+3. `Enable the Certificate Manager.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Certificate Manager API.:  https://cloud.google.com/python/docs/reference/certificatemanager/latest
+.. _Enable the Certificate Manager.:  https://cloud.google.com/python/docs/reference/certificatemanager/latest
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-certificate-manager
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Certificate Manager API
+-  Read the `Client Library Documentation`_ for Certificate Manager
    to see other available methods on the client.
--  Read the `Certificate Manager API Product documentation`_ to learn
+-  Read the `Certificate Manager Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Certificate Manager API Product documentation:  https://cloud.google.com/python/docs/reference/certificatemanager/latest
+.. _Certificate Manager Product documentation:  https://cloud.google.com/python/docs/reference/certificatemanager/latest
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager/__init__.py` & `google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager/gapic_version.py` & `google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.4.2"  # {x-release-please-version}
+__version__ = "1.4.3"  # {x-release-please-version}
```

### Comparing `google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/__init__.py` & `google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/gapic_metadata.json` & `google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/gapic_version.py` & `google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.4.2"  # {x-release-please-version}
+__version__ = "1.4.3"  # {x-release-please-version}
```

### Comparing `google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/__init__.py` & `google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/certificate_manager/__init__.py` & `google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/certificate_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/certificate_manager/async_client.py` & `google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/certificate_manager/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3822,15 +3822,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "CertificateManagerAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/certificate_manager/client.py` & `google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/certificate_manager/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/certificate_manager/pagers.py` & `google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/certificate_manager/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/certificate_manager/transports/__init__.py` & `google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/certificate_manager/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/certificate_manager/transports/base.py` & `google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/certificate_manager/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/certificate_manager/transports/grpc.py` & `google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/certificate_manager/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/certificate_manager/transports/grpc_asyncio.py` & `google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/certificate_manager/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/services/certificate_manager/transports/rest.py` & `google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/services/certificate_manager/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -3876,15 +3876,15 @@
 
             request, metadata = self._interceptor.pre_cancel_operation(
                 request, metadata
             )
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
```

### Comparing `google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/types/__init__.py` & `google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/types/certificate_issuance_config.py` & `google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/types/certificate_issuance_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-certificate-manager-1.4.2/google/cloud/certificate_manager_v1/types/certificate_manager.py` & `google-cloud-certificate-manager-1.4.3/google/cloud/certificate_manager_v1/types/certificate_manager.py`

 * *Files identical despite different names*

### Comparing `google-cloud-certificate-manager-1.4.2/google_cloud_certificate_manager.egg-info/PKG-INFO` & `google-cloud-certificate-manager-1.4.3/google_cloud_certificate_manager.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-certificate-manager
-Version: 1.4.2
+Version: 1.4.3
 Summary: Google Cloud Certificate Manager API client library
-Home-page: https://github.com/googleapis/python-certificate-manager
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
 
-Python Client for Certificate Manager API
-=========================================
+Python Client for Certificate Manager
+=====================================
 
 |stable| |pypi| |versions|
 
-`Certificate Manager API`_: lets you acquire and manage TLS (SSL) certificates for use with Cloud Load Balancing.
+`Certificate Manager`_: lets you acquire and manage TLS (SSL) certificates for use with Cloud Load Balancing.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-certificate-manager.svg
    :target: https://pypi.org/project/google-cloud-certificate-manager/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-certificate-manager.svg
    :target: https://pypi.org/project/google-cloud-certificate-manager/
-.. _Certificate Manager API: https://cloud.google.com/python/docs/reference/certificatemanager/latest
+.. _Certificate Manager: https://cloud.google.com/python/docs/reference/certificatemanager/latest
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/certificatemanager/latest
 .. _Product Documentation:  https://cloud.google.com/python/docs/reference/certificatemanager/latest
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Certificate Manager API.`_
+3. `Enable the Certificate Manager.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Certificate Manager API.:  https://cloud.google.com/python/docs/reference/certificatemanager/latest
+.. _Enable the Certificate Manager.:  https://cloud.google.com/python/docs/reference/certificatemanager/latest
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-certificate-manager
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Certificate Manager API
+-  Read the `Client Library Documentation`_ for Certificate Manager
    to see other available methods on the client.
--  Read the `Certificate Manager API Product documentation`_ to learn
+-  Read the `Certificate Manager Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Certificate Manager API Product documentation:  https://cloud.google.com/python/docs/reference/certificatemanager/latest
+.. _Certificate Manager Product documentation:  https://cloud.google.com/python/docs/reference/certificatemanager/latest
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-certificate-manager-1.4.2/google_cloud_certificate_manager.egg-info/SOURCES.txt` & `google-cloud-certificate-manager-1.4.3/google_cloud_certificate_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-certificate-manager-1.4.2/setup.py` & `google-cloud-certificate-manager-1.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-certificate-manager"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-certificate-manager-1.4.2/tests/__init__.py` & `google-cloud-certificate-manager-1.4.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-certificate-manager-1.4.2/tests/unit/__init__.py` & `google-cloud-certificate-manager-1.4.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-certificate-manager-1.4.2/tests/unit/gapic/__init__.py` & `google-cloud-certificate-manager-1.4.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-certificate-manager-1.4.2/tests/unit/gapic/certificate_manager_v1/__init__.py` & `google-cloud-certificate-manager-1.4.3/tests/unit/gapic/certificate_manager_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-certificate-manager-1.4.2/tests/unit/gapic/certificate_manager_v1/test_certificate_manager.py` & `google-cloud-certificate-manager-1.4.3/tests/unit/gapic/certificate_manager_v1/test_certificate_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1186,17 +1186,19 @@
                     certificate_manager.Certificate(),
                     certificate_manager.Certificate(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_certificates(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1220,17 +1222,14 @@
         # Designate an appropriate return value for the call.
         call.return_value = certificate_manager.Certificate(
             name="name_value",
             description="description_value",
             san_dnsnames=["san_dnsnames_value"],
             pem_certificate="pem_certificate_value",
             scope=certificate_manager.Certificate.Scope.EDGE_CACHE,
-            self_managed=certificate_manager.Certificate.SelfManagedCertificate(
-                pem_certificate="pem_certificate_value"
-            ),
         )
         response = client.get_certificate(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == certificate_manager.GetCertificateRequest()
@@ -2638,17 +2637,19 @@
                     certificate_manager.CertificateMap(),
                     certificate_manager.CertificateMap(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_certificate_maps(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4093,17 +4094,19 @@
                     certificate_manager.CertificateMapEntry(),
                     certificate_manager.CertificateMapEntry(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_certificate_map_entries(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5571,17 +5574,19 @@
                     certificate_manager.DnsAuthorization(),
                     certificate_manager.DnsAuthorization(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_dns_authorizations(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -7049,17 +7054,19 @@
                     certificate_issuance_config.CertificateIssuanceConfig(),
                     certificate_issuance_config.CertificateIssuanceConfig(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_certificate_issuance_configs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -8236,17 +8243,14 @@
         # Designate an appropriate value for the returned response.
         return_value = certificate_manager.Certificate(
             name="name_value",
             description="description_value",
             san_dnsnames=["san_dnsnames_value"],
             pem_certificate="pem_certificate_value",
             scope=certificate_manager.Certificate.Scope.EDGE_CACHE,
-            self_managed=certificate_manager.Certificate.SelfManagedCertificate(
-                pem_certificate="pem_certificate_value"
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = certificate_manager.Certificate.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

