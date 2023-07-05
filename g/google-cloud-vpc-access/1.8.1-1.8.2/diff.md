# Comparing `tmp/google-cloud-vpc-access-1.8.1.tar.gz` & `tmp/google-cloud-vpc-access-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-vpc-access-1.8.1.tar", last modified: Mon Mar 27 15:57:35 2023, max compression
+gzip compressed data, was "google-cloud-vpc-access-1.8.2.tar", last modified: Wed Jul  5 15:56:38 2023, max compression
```

## Comparing `google-cloud-vpc-access-1.8.1.tar` & `google-cloud-vpc-access-1.8.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:57:35.412579 google-cloud-vpc-access-1.8.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4801 2023-03-27 15:57:35.412579 google-cloud-vpc-access-1.8.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3876 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:57:35.404578 google-cloud-vpc-access-1.8.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:57:35.404578 google-cloud-vpc-access-1.8.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:57:35.408579 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess/
--rw-rw-r--   0 root         (0)     1003     1435 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:57:35.408579 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/
--rw-rw-r--   0 root         (0)     1003     1298 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2156 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:57:35.408579 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:57:35.408579 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/vpc_access_service/
--rw-rw-r--   0 root         (0)     1003      777 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/vpc_access_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    35191 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/vpc_access_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    44660 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/vpc_access_service/client.py
--rw-rw-r--   0 root         (0)     1003     5791 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/vpc_access_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:57:35.408579 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8499 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18737 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19083 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    39970 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:57:35.412579 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/types/
--rw-rw-r--   0 root         (0)     1003     1005 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     9174 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/types/vpc_access.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:57:35.412579 google-cloud-vpc-access-1.8.1/google_cloud_vpc_access.egg-info/
--rw-r--r--   0 root         (0)     1003     4801 2023-03-27 15:57:35.000000 google-cloud-vpc-access-1.8.1/google_cloud_vpc_access.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1601 2023-03-27 15:57:35.000000 google-cloud-vpc-access-1.8.1/google_cloud_vpc_access.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:57:35.000000 google-cloud-vpc-access-1.8.1/google_cloud_vpc_access.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:57:35.000000 google-cloud-vpc-access-1.8.1/google_cloud_vpc_access.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:57:35.000000 google-cloud-vpc-access-1.8.1/google_cloud_vpc_access.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 15:57:35.000000 google-cloud-vpc-access-1.8.1/google_cloud_vpc_access.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:57:35.000000 google-cloud-vpc-access-1.8.1/google_cloud_vpc_access.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:57:35.412579 google-cloud-vpc-access-1.8.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2932 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:57:35.412579 google-cloud-vpc-access-1.8.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:57:35.412579 google-cloud-vpc-access-1.8.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:57:35.412579 google-cloud-vpc-access-1.8.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:57:35.412579 google-cloud-vpc-access-1.8.1/tests/unit/gapic/vpcaccess_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/tests/unit/gapic/vpcaccess_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   164010 2023-03-27 15:54:59.000000 google-cloud-vpc-access-1.8.1/tests/unit/gapic/vpcaccess_v1/test_vpc_access_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:38.668155 google-cloud-vpc-access-1.8.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4767 2023-07-05 15:56:38.668155 google-cloud-vpc-access-1.8.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3840 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:38.660155 google-cloud-vpc-access-1.8.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:38.660155 google-cloud-vpc-access-1.8.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:38.660155 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess/
+-rw-rw-r--   0 root         (0)     1003     1435 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:38.664155 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/
+-rw-rw-r--   0 root         (0)     1003     1298 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2156 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:38.664155 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:38.664155 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/vpc_access_service/
+-rw-rw-r--   0 root         (0)     1003      777 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/vpc_access_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    35224 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/vpc_access_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    44660 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/vpc_access_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5791 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/vpc_access_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:38.664155 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8499 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18737 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19083 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    39970 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:38.664155 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1005 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9174 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/types/vpc_access.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:38.668155 google-cloud-vpc-access-1.8.2/google_cloud_vpc_access.egg-info/
+-rw-r--r--   0 root         (0)     1003     4767 2023-07-05 15:56:38.000000 google-cloud-vpc-access-1.8.2/google_cloud_vpc_access.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1601 2023-07-05 15:56:38.000000 google-cloud-vpc-access-1.8.2/google_cloud_vpc_access.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:56:38.000000 google-cloud-vpc-access-1.8.2/google_cloud_vpc_access.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:56:38.000000 google-cloud-vpc-access-1.8.2/google_cloud_vpc_access.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:56:38.000000 google-cloud-vpc-access-1.8.2/google_cloud_vpc_access.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:56:38.000000 google-cloud-vpc-access-1.8.2/google_cloud_vpc_access.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:56:38.000000 google-cloud-vpc-access-1.8.2/google_cloud_vpc_access.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:56:38.668155 google-cloud-vpc-access-1.8.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2934 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:38.668155 google-cloud-vpc-access-1.8.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:38.668155 google-cloud-vpc-access-1.8.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:38.668155 google-cloud-vpc-access-1.8.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:38.668155 google-cloud-vpc-access-1.8.2/tests/unit/gapic/vpcaccess_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/tests/unit/gapic/vpcaccess_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   164209 2023-07-05 15:46:59.000000 google-cloud-vpc-access-1.8.2/tests/unit/gapic/vpcaccess_v1/test_vpc_access_service.py
```

### Comparing `google-cloud-vpc-access-1.8.1/LICENSE` & `google-cloud-vpc-access-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-vpc-access-1.8.1/MANIFEST.in` & `google-cloud-vpc-access-1.8.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-vpc-access-1.8.1/PKG-INFO` & `google-cloud-vpc-access-1.8.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-vpc-access
-Version: 1.8.1
+Version: 1.8.2
 Summary: Google Cloud Vpc Access API client library
-Home-page: https://github.com/googleapis/python-vpc-access
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
 
-Python Client for Virtual Private Cloud API
-===========================================
+Python Client for Virtual Private Cloud
+=======================================
 
 |stable| |pypi| |versions|
 
-`Virtual Private Cloud API`_: provides networking functionality to Compute Engine virtual machine (VM) instances, Google Kubernetes Engine (GKE) containers, and the App Engine flexible environment. VPC provides networking for your cloud-based services that is global, scalable, and flexible.
+`Virtual Private Cloud`_: provides networking functionality to Compute Engine virtual machine (VM) instances, Google Kubernetes Engine (GKE) containers, and the App Engine flexible environment. VPC provides networking for your cloud-based services that is global, scalable, and flexible.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-vpc-access.svg
    :target: https://pypi.org/project/google-cloud-vpc-access/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-vpc-access.svg
    :target: https://pypi.org/project/google-cloud-vpc-access/
-.. _Virtual Private Cloud API: https://cloud.google.com/vpc/
+.. _Virtual Private Cloud: https://cloud.google.com/vpc/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/vpcaccess/latest
 .. _Product Documentation:  https://cloud.google.com/vpc/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Virtual Private Cloud API.`_
+3. `Enable the Virtual Private Cloud.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Virtual Private Cloud API.:  https://cloud.google.com/vpc/
+.. _Enable the Virtual Private Cloud.:  https://cloud.google.com/vpc/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-vpc-access
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Virtual Private Cloud API
+-  Read the `Client Library Documentation`_ for Virtual Private Cloud
    to see other available methods on the client.
--  Read the `Virtual Private Cloud API Product documentation`_ to learn
+-  Read the `Virtual Private Cloud Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Virtual Private Cloud API Product documentation:  https://cloud.google.com/vpc/
+.. _Virtual Private Cloud Product documentation:  https://cloud.google.com/vpc/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-vpc-access-1.8.1/README.rst` & `google-cloud-vpc-access-1.8.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Virtual Private Cloud API
-===========================================
+Python Client for Virtual Private Cloud
+=======================================
 
 |stable| |pypi| |versions|
 
-`Virtual Private Cloud API`_: provides networking functionality to Compute Engine virtual machine (VM) instances, Google Kubernetes Engine (GKE) containers, and the App Engine flexible environment. VPC provides networking for your cloud-based services that is global, scalable, and flexible.
+`Virtual Private Cloud`_: provides networking functionality to Compute Engine virtual machine (VM) instances, Google Kubernetes Engine (GKE) containers, and the App Engine flexible environment. VPC provides networking for your cloud-based services that is global, scalable, and flexible.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-vpc-access.svg
    :target: https://pypi.org/project/google-cloud-vpc-access/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-vpc-access.svg
    :target: https://pypi.org/project/google-cloud-vpc-access/
-.. _Virtual Private Cloud API: https://cloud.google.com/vpc/
+.. _Virtual Private Cloud: https://cloud.google.com/vpc/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/vpcaccess/latest
 .. _Product Documentation:  https://cloud.google.com/vpc/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Virtual Private Cloud API.`_
+3. `Enable the Virtual Private Cloud.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Virtual Private Cloud API.:  https://cloud.google.com/vpc/
+.. _Enable the Virtual Private Cloud.:  https://cloud.google.com/vpc/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-vpc-access
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Virtual Private Cloud API
+-  Read the `Client Library Documentation`_ for Virtual Private Cloud
    to see other available methods on the client.
--  Read the `Virtual Private Cloud API Product documentation`_ to learn
+-  Read the `Virtual Private Cloud Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Virtual Private Cloud API Product documentation:  https://cloud.google.com/vpc/
+.. _Virtual Private Cloud Product documentation:  https://cloud.google.com/vpc/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess/__init__.py` & `google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess/gapic_version.py` & `google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess/gapic_version.py`

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

### Comparing `google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/__init__.py` & `google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/gapic_metadata.json` & `google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/gapic_version.py` & `google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/gapic_version.py`

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

### Comparing `google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/__init__.py` & `google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/vpc_access_service/__init__.py` & `google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/vpc_access_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/vpc_access_service/async_client.py` & `google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/vpc_access_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -862,15 +862,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "VpcAccessServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/vpc_access_service/client.py` & `google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/vpc_access_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/vpc_access_service/pagers.py` & `google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/vpc_access_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/__init__.py` & `google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/base.py` & `google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/grpc.py` & `google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/grpc_asyncio.py` & `google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/rest.py` & `google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/services/vpc_access_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/types/__init__.py` & `google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vpc-access-1.8.1/google/cloud/vpcaccess_v1/types/vpc_access.py` & `google-cloud-vpc-access-1.8.2/google/cloud/vpcaccess_v1/types/vpc_access.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vpc-access-1.8.1/google_cloud_vpc_access.egg-info/PKG-INFO` & `google-cloud-vpc-access-1.8.2/google_cloud_vpc_access.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-vpc-access
-Version: 1.8.1
+Version: 1.8.2
 Summary: Google Cloud Vpc Access API client library
-Home-page: https://github.com/googleapis/python-vpc-access
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
 
-Python Client for Virtual Private Cloud API
-===========================================
+Python Client for Virtual Private Cloud
+=======================================
 
 |stable| |pypi| |versions|
 
-`Virtual Private Cloud API`_: provides networking functionality to Compute Engine virtual machine (VM) instances, Google Kubernetes Engine (GKE) containers, and the App Engine flexible environment. VPC provides networking for your cloud-based services that is global, scalable, and flexible.
+`Virtual Private Cloud`_: provides networking functionality to Compute Engine virtual machine (VM) instances, Google Kubernetes Engine (GKE) containers, and the App Engine flexible environment. VPC provides networking for your cloud-based services that is global, scalable, and flexible.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-vpc-access.svg
    :target: https://pypi.org/project/google-cloud-vpc-access/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-vpc-access.svg
    :target: https://pypi.org/project/google-cloud-vpc-access/
-.. _Virtual Private Cloud API: https://cloud.google.com/vpc/
+.. _Virtual Private Cloud: https://cloud.google.com/vpc/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/vpcaccess/latest
 .. _Product Documentation:  https://cloud.google.com/vpc/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Virtual Private Cloud API.`_
+3. `Enable the Virtual Private Cloud.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Virtual Private Cloud API.:  https://cloud.google.com/vpc/
+.. _Enable the Virtual Private Cloud.:  https://cloud.google.com/vpc/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-vpc-access
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Virtual Private Cloud API
+-  Read the `Client Library Documentation`_ for Virtual Private Cloud
    to see other available methods on the client.
--  Read the `Virtual Private Cloud API Product documentation`_ to learn
+-  Read the `Virtual Private Cloud Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Virtual Private Cloud API Product documentation:  https://cloud.google.com/vpc/
+.. _Virtual Private Cloud Product documentation:  https://cloud.google.com/vpc/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-vpc-access-1.8.1/google_cloud_vpc_access.egg-info/SOURCES.txt` & `google-cloud-vpc-access-1.8.2/google_cloud_vpc_access.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-vpc-access-1.8.1/setup.py` & `google-cloud-vpc-access-1.8.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-vpc-access"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-vpc-access-1.8.1/tests/__init__.py` & `google-cloud-vpc-access-1.8.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vpc-access-1.8.1/tests/unit/__init__.py` & `google-cloud-vpc-access-1.8.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vpc-access-1.8.1/tests/unit/gapic/__init__.py` & `google-cloud-vpc-access-1.8.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vpc-access-1.8.1/tests/unit/gapic/vpcaccess_v1/__init__.py` & `google-cloud-vpc-access-1.8.2/tests/unit/gapic/vpcaccess_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vpc-access-1.8.1/tests/unit/gapic/vpcaccess_v1/test_vpc_access_service.py` & `google-cloud-vpc-access-1.8.2/tests/unit/gapic/vpcaccess_v1/test_vpc_access_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1666,17 +1666,19 @@
                     vpc_access.Connector(),
                     vpc_access.Connector(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_connectors(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

