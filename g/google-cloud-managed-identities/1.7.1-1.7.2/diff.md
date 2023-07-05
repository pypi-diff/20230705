# Comparing `tmp/google-cloud-managed-identities-1.7.1.tar.gz` & `tmp/google-cloud-managed-identities-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-managed-identities-1.7.1.tar", last modified: Mon Jan 23 15:49:54 2023, max compression
+gzip compressed data, was "google-cloud-managed-identities-1.7.2.tar", last modified: Wed Jul  5 15:53:47 2023, max compression
```

## Comparing `google-cloud-managed-identities-1.7.1.tar` & `google-cloud-managed-identities-1.7.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:49:54.505500 google-cloud-managed-identities-1.7.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5198 2023-01-23 15:49:54.505500 google-cloud-managed-identities-1.7.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4249 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:49:54.497498 google-cloud-managed-identities-1.7.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:49:54.497498 google-cloud-managed-identities-1.7.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:49:54.497498 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities/
--rw-rw-r--   0 root         (0)     1003     1975 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       92 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:49:54.497498 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/
--rw-rw-r--   0 root         (0)     1003     1770 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3065 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       92 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:49:54.497498 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:49:54.501499 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/services/managed_identities_service/
--rw-rw-r--   0 root         (0)     1003      809 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/services/managed_identities_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    64953 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/services/managed_identities_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    75389 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/services/managed_identities_service/client.py
--rw-rw-r--   0 root         (0)     1003     5986 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/services/managed_identities_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:49:54.501499 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/services/managed_identities_service/transports/
--rw-rw-r--   0 root         (0)     1003     1291 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/services/managed_identities_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10532 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/services/managed_identities_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    24490 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/services/managed_identities_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    25016 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/services/managed_identities_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:49:54.501499 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/types/
--rw-rw-r--   0 root         (0)     1003     1426 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    13039 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/types/managed_identities_service.py
--rw-rw-r--   0 root         (0)     1003    11193 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/types/resource.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:49:54.501499 google-cloud-managed-identities-1.7.1/google_cloud_managed_identities.egg-info/
--rw-r--r--   0 root         (0)     1003     5198 2023-01-23 15:49:54.000000 google-cloud-managed-identities-1.7.1/google_cloud_managed_identities.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1884 2023-01-23 15:49:54.000000 google-cloud-managed-identities-1.7.1/google_cloud_managed_identities.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-23 15:49:54.000000 google-cloud-managed-identities-1.7.1/google_cloud_managed_identities.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-23 15:49:54.000000 google-cloud-managed-identities-1.7.1/google_cloud_managed_identities.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-23 15:49:54.000000 google-cloud-managed-identities-1.7.1/google_cloud_managed_identities.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-01-23 15:49:54.000000 google-cloud-managed-identities-1.7.1/google_cloud_managed_identities.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-23 15:49:54.000000 google-cloud-managed-identities-1.7.1/google_cloud_managed_identities.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-01-23 15:49:54.505500 google-cloud-managed-identities-1.7.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3023 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:49:54.501499 google-cloud-managed-identities-1.7.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:49:54.501499 google-cloud-managed-identities-1.7.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:49:54.501499 google-cloud-managed-identities-1.7.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:49:54.505500 google-cloud-managed-identities-1.7.1/tests/unit/gapic/managedidentities_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/tests/unit/gapic/managedidentities_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   150989 2023-01-23 15:46:37.000000 google-cloud-managed-identities-1.7.1/tests/unit/gapic/managedidentities_v1/test_managed_identities_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:47.256890 google-cloud-managed-identities-1.7.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5156 2023-07-05 15:53:47.256890 google-cloud-managed-identities-1.7.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4213 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:47.248890 google-cloud-managed-identities-1.7.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:47.248890 google-cloud-managed-identities-1.7.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:47.248890 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities/
+-rw-rw-r--   0 root         (0)     1003     1975 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       92 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:47.248890 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/
+-rw-rw-r--   0 root         (0)     1003     1773 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3065 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       92 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:47.248890 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:47.252890 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/services/managed_identities_service/
+-rw-rw-r--   0 root         (0)     1003      809 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/services/managed_identities_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    64994 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/services/managed_identities_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    75389 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/services/managed_identities_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5986 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/services/managed_identities_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:47.252890 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/services/managed_identities_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1291 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/services/managed_identities_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10532 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/services/managed_identities_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    24490 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/services/managed_identities_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    25016 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/services/managed_identities_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:47.252890 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1426 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13075 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/types/managed_identities_service.py
+-rw-rw-r--   0 root         (0)     1003    11229 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/types/resource.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:47.252890 google-cloud-managed-identities-1.7.2/google_cloud_managed_identities.egg-info/
+-rw-r--r--   0 root         (0)     1003     5156 2023-07-05 15:53:47.000000 google-cloud-managed-identities-1.7.2/google_cloud_managed_identities.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1884 2023-07-05 15:53:47.000000 google-cloud-managed-identities-1.7.2/google_cloud_managed_identities.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:47.000000 google-cloud-managed-identities-1.7.2/google_cloud_managed_identities.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:53:47.000000 google-cloud-managed-identities-1.7.2/google_cloud_managed_identities.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:47.000000 google-cloud-managed-identities-1.7.2/google_cloud_managed_identities.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:53:47.000000 google-cloud-managed-identities-1.7.2/google_cloud_managed_identities.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:53:47.000000 google-cloud-managed-identities-1.7.2/google_cloud_managed_identities.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:53:47.256890 google-cloud-managed-identities-1.7.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2964 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:47.252890 google-cloud-managed-identities-1.7.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:47.252890 google-cloud-managed-identities-1.7.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:47.252890 google-cloud-managed-identities-1.7.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:47.252890 google-cloud-managed-identities-1.7.2/tests/unit/gapic/managedidentities_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/tests/unit/gapic/managedidentities_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   151188 2023-07-05 15:46:59.000000 google-cloud-managed-identities-1.7.2/tests/unit/gapic/managedidentities_v1/test_managed_identities_service.py
```

### Comparing `google-cloud-managed-identities-1.7.1/LICENSE` & `google-cloud-managed-identities-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-managed-identities-1.7.1/MANIFEST.in` & `google-cloud-managed-identities-1.7.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-managed-identities-1.7.1/PKG-INFO` & `google-cloud-managed-identities-1.7.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-managed-identities
-Version: 1.7.1
+Version: 1.7.2
 Summary: Google Cloud Managed Identities API client library
-Home-page: https://github.com/googleapis/python-managed-identities
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
 
-Python Client for Managed Service for Microsoft Active Directory API
-====================================================================
+Python Client for Managed Service for Microsoft Active Directory
+================================================================
 
 |stable| |pypi| |versions|
 
-`Managed Service for Microsoft Active Directory API`_: is a highly available, hardened Google Cloud service running actual Microsoft AD that enables you to manage authentication and authorization for your AD-dependent workloads, automate AD server maintenance and security configuration, and connect your on-premises AD domain to the cloud.
+`Managed Service for Microsoft Active Directory`_: is a highly available, hardened Google Cloud service running actual Microsoft AD that enables you to manage authentication and authorization for your AD-dependent workloads, automate AD server maintenance and security configuration, and connect your on-premises AD domain to the cloud.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-managed-identities.svg
    :target: https://pypi.org/project/google-cloud-managed-identities/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-managed-identities.svg
    :target: https://pypi.org/project/google-cloud-managed-identities/
-.. _Managed Service for Microsoft Active Directory API: https://cloud.google.com/managed-microsoft-ad/
+.. _Managed Service for Microsoft Active Directory: https://cloud.google.com/managed-microsoft-ad/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/managedidentities/latest
 .. _Product Documentation:  https://cloud.google.com/managed-microsoft-ad/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Managed Service for Microsoft Active Directory API.`_
+3. `Enable the Managed Service for Microsoft Active Directory.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Managed Service for Microsoft Active Directory API.:  https://cloud.google.com/managed-microsoft-ad/
+.. _Enable the Managed Service for Microsoft Active Directory.:  https://cloud.google.com/managed-microsoft-ad/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-managed-identities
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Managed Service for Microsoft Active Directory API
+-  Read the `Client Library Documentation`_ for Managed Service for Microsoft Active Directory
    to see other available methods on the client.
--  Read the `Managed Service for Microsoft Active Directory API Product documentation`_ to learn
+-  Read the `Managed Service for Microsoft Active Directory Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Managed Service for Microsoft Active Directory API Product documentation:  https://cloud.google.com/managed-microsoft-ad/
+.. _Managed Service for Microsoft Active Directory Product documentation:  https://cloud.google.com/managed-microsoft-ad/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-managed-identities-1.7.1/README.rst` & `google-cloud-managed-identities-1.7.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Managed Service for Microsoft Active Directory API
-====================================================================
+Python Client for Managed Service for Microsoft Active Directory
+================================================================
 
 |stable| |pypi| |versions|
 
-`Managed Service for Microsoft Active Directory API`_: is a highly available, hardened Google Cloud service running actual Microsoft AD that enables you to manage authentication and authorization for your AD-dependent workloads, automate AD server maintenance and security configuration, and connect your on-premises AD domain to the cloud.
+`Managed Service for Microsoft Active Directory`_: is a highly available, hardened Google Cloud service running actual Microsoft AD that enables you to manage authentication and authorization for your AD-dependent workloads, automate AD server maintenance and security configuration, and connect your on-premises AD domain to the cloud.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-managed-identities.svg
    :target: https://pypi.org/project/google-cloud-managed-identities/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-managed-identities.svg
    :target: https://pypi.org/project/google-cloud-managed-identities/
-.. _Managed Service for Microsoft Active Directory API: https://cloud.google.com/managed-microsoft-ad/
+.. _Managed Service for Microsoft Active Directory: https://cloud.google.com/managed-microsoft-ad/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/managedidentities/latest
 .. _Product Documentation:  https://cloud.google.com/managed-microsoft-ad/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Managed Service for Microsoft Active Directory API.`_
+3. `Enable the Managed Service for Microsoft Active Directory.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Managed Service for Microsoft Active Directory API.:  https://cloud.google.com/managed-microsoft-ad/
+.. _Enable the Managed Service for Microsoft Active Directory.:  https://cloud.google.com/managed-microsoft-ad/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-managed-identities
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Managed Service for Microsoft Active Directory API
+-  Read the `Client Library Documentation`_ for Managed Service for Microsoft Active Directory
    to see other available methods on the client.
--  Read the `Managed Service for Microsoft Active Directory API Product documentation`_ to learn
+-  Read the `Managed Service for Microsoft Active Directory Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Managed Service for Microsoft Active Directory API Product documentation:  https://cloud.google.com/managed-microsoft-ad/
+.. _Managed Service for Microsoft Active Directory Product documentation:  https://cloud.google.com/managed-microsoft-ad/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-managed-identities-1.7.1/google/cloud/managedidentities/__init__.py` & `google-cloud-managed-identities-1.7.2/google/cloud/managedidentities/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-managed-identities-1.7.1/google/cloud/managedidentities/gapic_version.py` & `google-cloud-managed-identities-1.7.2/google/cloud/managedidentities/gapic_version.py`

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

### Comparing `google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/__init__.py` & `google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.managedidentities import gapic_version as package_version
+from google.cloud.managedidentities_v1 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
 from .services.managed_identities_service import (
     ManagedIdentitiesServiceAsyncClient,
     ManagedIdentitiesServiceClient,
```

### Comparing `google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/gapic_metadata.json` & `google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/gapic_version.py` & `google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/gapic_version.py`

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

### Comparing `google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/services/__init__.py` & `google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/services/managed_identities_service/__init__.py` & `google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/services/managed_identities_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/services/managed_identities_service/async_client.py` & `google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/services/managed_identities_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1565,15 +1565,15 @@
             resource.Domain,
             metadata_type=managed_identities_service.OpMetadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ManagedIdentitiesServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/services/managed_identities_service/client.py` & `google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/services/managed_identities_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/services/managed_identities_service/pagers.py` & `google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/services/managed_identities_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/services/managed_identities_service/transports/__init__.py` & `google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/services/managed_identities_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/services/managed_identities_service/transports/base.py` & `google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/services/managed_identities_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/services/managed_identities_service/transports/grpc.py` & `google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/services/managed_identities_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/services/managed_identities_service/transports/grpc_asyncio.py` & `google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/services/managed_identities_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/types/__init__.py` & `google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/types/managed_identities_service.py` & `google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/types/managed_identities_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 from google.cloud.managedidentities_v1.types import resource
```

### Comparing `google-cloud-managed-identities-1.7.1/google/cloud/managedidentities_v1/types/resource.py` & `google-cloud-managed-identities-1.7.2/google/cloud/managedidentities_v1/types/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.managedidentities.v1",
```

### Comparing `google-cloud-managed-identities-1.7.1/google_cloud_managed_identities.egg-info/PKG-INFO` & `google-cloud-managed-identities-1.7.2/google_cloud_managed_identities.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-managed-identities
-Version: 1.7.1
+Version: 1.7.2
 Summary: Google Cloud Managed Identities API client library
-Home-page: https://github.com/googleapis/python-managed-identities
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
 
-Python Client for Managed Service for Microsoft Active Directory API
-====================================================================
+Python Client for Managed Service for Microsoft Active Directory
+================================================================
 
 |stable| |pypi| |versions|
 
-`Managed Service for Microsoft Active Directory API`_: is a highly available, hardened Google Cloud service running actual Microsoft AD that enables you to manage authentication and authorization for your AD-dependent workloads, automate AD server maintenance and security configuration, and connect your on-premises AD domain to the cloud.
+`Managed Service for Microsoft Active Directory`_: is a highly available, hardened Google Cloud service running actual Microsoft AD that enables you to manage authentication and authorization for your AD-dependent workloads, automate AD server maintenance and security configuration, and connect your on-premises AD domain to the cloud.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-managed-identities.svg
    :target: https://pypi.org/project/google-cloud-managed-identities/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-managed-identities.svg
    :target: https://pypi.org/project/google-cloud-managed-identities/
-.. _Managed Service for Microsoft Active Directory API: https://cloud.google.com/managed-microsoft-ad/
+.. _Managed Service for Microsoft Active Directory: https://cloud.google.com/managed-microsoft-ad/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/managedidentities/latest
 .. _Product Documentation:  https://cloud.google.com/managed-microsoft-ad/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Managed Service for Microsoft Active Directory API.`_
+3. `Enable the Managed Service for Microsoft Active Directory.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Managed Service for Microsoft Active Directory API.:  https://cloud.google.com/managed-microsoft-ad/
+.. _Enable the Managed Service for Microsoft Active Directory.:  https://cloud.google.com/managed-microsoft-ad/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-managed-identities
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Managed Service for Microsoft Active Directory API
+-  Read the `Client Library Documentation`_ for Managed Service for Microsoft Active Directory
    to see other available methods on the client.
--  Read the `Managed Service for Microsoft Active Directory API Product documentation`_ to learn
+-  Read the `Managed Service for Microsoft Active Directory Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Managed Service for Microsoft Active Directory API Product documentation:  https://cloud.google.com/managed-microsoft-ad/
+.. _Managed Service for Microsoft Active Directory Product documentation:  https://cloud.google.com/managed-microsoft-ad/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-managed-identities-1.7.1/google_cloud_managed_identities.egg-info/SOURCES.txt` & `google-cloud-managed-identities-1.7.2/google_cloud_managed_identities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-managed-identities-1.7.1/setup.py` & `google-cloud-managed-identities-1.7.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,31 +39,29 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-managed-identities"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 packages = [
     package
     for package in setuptools.PEP420PackageFinder.find()
     if package.startswith("google")
 ]
 
-namespaces = ["google"]
-if "google.cloud" in packages:
-    namespaces.append("google.cloud")
+namespaces = ["google", "google.cloud"]
 
 setuptools.setup(
     name=name,
     version=version,
     description=description,
     long_description=readme,
     author="Google LLC",
```

### Comparing `google-cloud-managed-identities-1.7.1/tests/__init__.py` & `google-cloud-managed-identities-1.7.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-managed-identities-1.7.1/tests/unit/__init__.py` & `google-cloud-managed-identities-1.7.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-managed-identities-1.7.1/tests/unit/gapic/__init__.py` & `google-cloud-managed-identities-1.7.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-managed-identities-1.7.1/tests/unit/gapic/managedidentities_v1/__init__.py` & `google-cloud-managed-identities-1.7.2/tests/unit/gapic/managedidentities_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-managed-identities-1.7.1/tests/unit/gapic/managedidentities_v1/test_managed_identities_service.py` & `google-cloud-managed-identities-1.7.2/tests/unit/gapic/managedidentities_v1/test_managed_identities_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1644,17 +1644,19 @@
                     resource.Domain(),
                     resource.Domain(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_domains(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

