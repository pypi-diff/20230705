# Comparing `tmp/google-cloud-dms-1.7.0.tar.gz` & `tmp/google-cloud-dms-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-dms-1.7.0.tar", last modified: Wed May 31 20:49:48 2023, max compression
+gzip compressed data, was "google-cloud-dms-1.7.1.tar", last modified: Wed Jul  5 15:52:37 2023, max compression
```

## Comparing `google-cloud-dms-1.7.0.tar` & `google-cloud-dms-1.7.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.869138 google-cloud-dms-1.7.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4791 2023-05-31 20:49:48.869138 google-cloud-dms-1.7.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3887 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.861137 google-cloud-dms-1.7.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.861137 google-cloud-dms-1.7.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.865137 google-cloud-dms-1.7.0/google/cloud/clouddms/
--rw-rw-r--   0 root         (0)     1003     6922 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.865137 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/
--rw-rw-r--   0 root         (0)     1003     6736 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    10619 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.865137 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.865137 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/
--rw-rw-r--   0 root         (0)     1003      793 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   196914 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   213369 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/client.py
--rw-rw-r--   0 root         (0)     1003    32059 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.865137 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/transports/
--rw-rw-r--   0 root         (0)     1003     1255 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    25648 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    65408 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    66754 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.869138 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/types/
--rw-rw-r--   0 root         (0)     1003     6412 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    53494 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/types/clouddms.py
--rw-rw-r--   0 root         (0)     1003    68164 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/types/clouddms_resources.py
--rw-rw-r--   0 root         (0)     1003    37330 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/types/conversionworkspace_resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.869138 google-cloud-dms-1.7.0/google_cloud_dms.egg-info/
--rw-r--r--   0 root         (0)     1003     4791 2023-05-31 20:49:48.000000 google-cloud-dms-1.7.0/google_cloud_dms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1610 2023-05-31 20:49:48.000000 google-cloud-dms-1.7.0/google_cloud_dms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-31 20:49:48.000000 google-cloud-dms-1.7.0/google_cloud_dms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-05-31 20:49:48.000000 google-cloud-dms-1.7.0/google_cloud_dms.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-31 20:49:48.000000 google-cloud-dms-1.7.0/google_cloud_dms.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-05-31 20:49:48.000000 google-cloud-dms-1.7.0/google_cloud_dms.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-05-31 20:49:48.000000 google-cloud-dms-1.7.0/google_cloud_dms.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-05-31 20:49:48.869138 google-cloud-dms-1.7.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2957 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.869138 google-cloud-dms-1.7.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.869138 google-cloud-dms-1.7.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.869138 google-cloud-dms-1.7.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.869138 google-cloud-dms-1.7.0/tests/unit/gapic/clouddms_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/tests/unit/gapic/clouddms_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   425567 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/tests/unit/gapic/clouddms_v1/test_data_migration_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:37.645364 google-cloud-dms-1.7.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4764 2023-07-05 15:52:37.645364 google-cloud-dms-1.7.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3851 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:37.637364 google-cloud-dms-1.7.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:37.637364 google-cloud-dms-1.7.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:37.641364 google-cloud-dms-1.7.1/google/cloud/clouddms/
+-rw-rw-r--   0 root         (0)     1003     6922 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/google/cloud/clouddms/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/google/cloud/clouddms/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/google/cloud/clouddms/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:37.641364 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/
+-rw-rw-r--   0 root         (0)     1003     6736 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10619 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:37.641364 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:37.641364 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/services/data_migration_service/
+-rw-rw-r--   0 root         (0)     1003      793 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/services/data_migration_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   196951 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/services/data_migration_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   213369 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/services/data_migration_service/client.py
+-rw-rw-r--   0 root         (0)     1003    32059 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/services/data_migration_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:37.645364 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/services/data_migration_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1255 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/services/data_migration_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25648 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/services/data_migration_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    65408 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/services/data_migration_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    66754 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/services/data_migration_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:37.645364 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/types/
+-rw-rw-r--   0 root         (0)     1003     6412 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    53494 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/types/clouddms.py
+-rw-rw-r--   0 root         (0)     1003    68164 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/types/clouddms_resources.py
+-rw-rw-r--   0 root         (0)     1003    37330 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/google/cloud/clouddms_v1/types/conversionworkspace_resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:37.645364 google-cloud-dms-1.7.1/google_cloud_dms.egg-info/
+-rw-r--r--   0 root         (0)     1003     4764 2023-07-05 15:52:37.000000 google-cloud-dms-1.7.1/google_cloud_dms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1610 2023-07-05 15:52:37.000000 google-cloud-dms-1.7.1/google_cloud_dms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:37.000000 google-cloud-dms-1.7.1/google_cloud_dms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:52:37.000000 google-cloud-dms-1.7.1/google_cloud_dms.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:37.000000 google-cloud-dms-1.7.1/google_cloud_dms.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:52:37.000000 google-cloud-dms-1.7.1/google_cloud_dms.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:52:37.000000 google-cloud-dms-1.7.1/google_cloud_dms.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:52:37.645364 google-cloud-dms-1.7.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2966 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:37.645364 google-cloud-dms-1.7.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:37.645364 google-cloud-dms-1.7.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:37.645364 google-cloud-dms-1.7.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:37.645364 google-cloud-dms-1.7.1/tests/unit/gapic/clouddms_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/tests/unit/gapic/clouddms_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   426425 2023-07-05 15:46:58.000000 google-cloud-dms-1.7.1/tests/unit/gapic/clouddms_v1/test_data_migration_service.py
```

### Comparing `google-cloud-dms-1.7.0/LICENSE` & `google-cloud-dms-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/MANIFEST.in` & `google-cloud-dms-1.7.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/PKG-INFO` & `google-cloud-dms-1.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-dms
-Version: 1.7.0
+Version: 1.7.1
 Summary: Google Cloud Dms API client library
-Home-page: https://github.com/googleapis/python-dms
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
 
-Python Client for Cloud Database Migration Service API
-======================================================
+Python Client for Cloud Database Migration Service
+==================================================
 
 |stable| |pypi| |versions|
 
-`Cloud Database Migration Service API`_: makes it easier for you to migrate your data to Google Cloud. This service helps you lift and shift your MySQL and PostgreSQL workloads into Cloud SQL.
+`Cloud Database Migration Service`_: makes it easier for you to migrate your data to Google Cloud. This service helps you lift and shift your MySQL and PostgreSQL workloads into Cloud SQL.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-dms.svg
    :target: https://pypi.org/project/google-cloud-dms/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-dms.svg
    :target: https://pypi.org/project/google-cloud-dms/
-.. _Cloud Database Migration Service API: https://cloud.google.com/database-migration/
+.. _Cloud Database Migration Service: https://cloud.google.com/database-migration/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/datamigration/latest
 .. _Product Documentation:  https://cloud.google.com/database-migration/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Database Migration Service API.`_
+3. `Enable the Cloud Database Migration Service.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Database Migration Service API.:  https://cloud.google.com/database-migration/
+.. _Enable the Cloud Database Migration Service.:  https://cloud.google.com/database-migration/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-dms
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Database Migration Service API
+-  Read the `Client Library Documentation`_ for Cloud Database Migration Service
    to see other available methods on the client.
--  Read the `Cloud Database Migration Service API Product documentation`_ to learn
+-  Read the `Cloud Database Migration Service Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Database Migration Service API Product documentation:  https://cloud.google.com/database-migration/
+.. _Cloud Database Migration Service Product documentation:  https://cloud.google.com/database-migration/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-dms-1.7.0/README.rst` & `google-cloud-dms-1.7.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Cloud Database Migration Service API
-======================================================
+Python Client for Cloud Database Migration Service
+==================================================
 
 |stable| |pypi| |versions|
 
-`Cloud Database Migration Service API`_: makes it easier for you to migrate your data to Google Cloud. This service helps you lift and shift your MySQL and PostgreSQL workloads into Cloud SQL.
+`Cloud Database Migration Service`_: makes it easier for you to migrate your data to Google Cloud. This service helps you lift and shift your MySQL and PostgreSQL workloads into Cloud SQL.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-dms.svg
    :target: https://pypi.org/project/google-cloud-dms/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-dms.svg
    :target: https://pypi.org/project/google-cloud-dms/
-.. _Cloud Database Migration Service API: https://cloud.google.com/database-migration/
+.. _Cloud Database Migration Service: https://cloud.google.com/database-migration/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/datamigration/latest
 .. _Product Documentation:  https://cloud.google.com/database-migration/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Database Migration Service API.`_
+3. `Enable the Cloud Database Migration Service.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Database Migration Service API.:  https://cloud.google.com/database-migration/
+.. _Enable the Cloud Database Migration Service.:  https://cloud.google.com/database-migration/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-dms
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Database Migration Service API
+-  Read the `Client Library Documentation`_ for Cloud Database Migration Service
    to see other available methods on the client.
--  Read the `Cloud Database Migration Service API Product documentation`_ to learn
+-  Read the `Cloud Database Migration Service Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Database Migration Service API Product documentation:  https://cloud.google.com/database-migration/
+.. _Cloud Database Migration Service Product documentation:  https://cloud.google.com/database-migration/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-dms-1.7.0/google/cloud/clouddms/__init__.py` & `google-cloud-dms-1.7.1/google/cloud/clouddms/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/google/cloud/clouddms/gapic_version.py` & `google-cloud-dms-1.7.1/google/cloud/clouddms/gapic_version.py`

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
-__version__ = "1.7.0"  # {x-release-please-version}
+__version__ = "1.7.1"  # {x-release-please-version}
```

### Comparing `google-cloud-dms-1.7.0/google/cloud/clouddms_v1/__init__.py` & `google-cloud-dms-1.7.1/google/cloud/clouddms_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/google/cloud/clouddms_v1/gapic_metadata.json` & `google-cloud-dms-1.7.1/google/cloud/clouddms_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/google/cloud/clouddms_v1/gapic_version.py` & `google-cloud-dms-1.7.1/google/cloud/clouddms_v1/gapic_version.py`

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
-__version__ = "1.7.0"  # {x-release-please-version}
+__version__ = "1.7.1"  # {x-release-please-version}
```

### Comparing `google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/__init__.py` & `google-cloud-dms-1.7.1/google/cloud/clouddms_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/__init__.py` & `google-cloud-dms-1.7.1/google/cloud/clouddms_v1/services/data_migration_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/async_client.py` & `google-cloud-dms-1.7.1/google/cloud/clouddms_v1/services/data_migration_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4901,15 +4901,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "DataMigrationServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/client.py` & `google-cloud-dms-1.7.1/google/cloud/clouddms_v1/services/data_migration_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/pagers.py` & `google-cloud-dms-1.7.1/google/cloud/clouddms_v1/services/data_migration_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/transports/__init__.py` & `google-cloud-dms-1.7.1/google/cloud/clouddms_v1/services/data_migration_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/transports/base.py` & `google-cloud-dms-1.7.1/google/cloud/clouddms_v1/services/data_migration_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/transports/grpc.py` & `google-cloud-dms-1.7.1/google/cloud/clouddms_v1/services/data_migration_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/transports/grpc_asyncio.py` & `google-cloud-dms-1.7.1/google/cloud/clouddms_v1/services/data_migration_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/google/cloud/clouddms_v1/types/__init__.py` & `google-cloud-dms-1.7.1/google/cloud/clouddms_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/google/cloud/clouddms_v1/types/clouddms.py` & `google-cloud-dms-1.7.1/google/cloud/clouddms_v1/types/clouddms.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/google/cloud/clouddms_v1/types/clouddms_resources.py` & `google-cloud-dms-1.7.1/google/cloud/clouddms_v1/types/clouddms_resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/google/cloud/clouddms_v1/types/conversionworkspace_resources.py` & `google-cloud-dms-1.7.1/google/cloud/clouddms_v1/types/conversionworkspace_resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/google_cloud_dms.egg-info/PKG-INFO` & `google-cloud-dms-1.7.1/google_cloud_dms.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-dms
-Version: 1.7.0
+Version: 1.7.1
 Summary: Google Cloud Dms API client library
-Home-page: https://github.com/googleapis/python-dms
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
 
-Python Client for Cloud Database Migration Service API
-======================================================
+Python Client for Cloud Database Migration Service
+==================================================
 
 |stable| |pypi| |versions|
 
-`Cloud Database Migration Service API`_: makes it easier for you to migrate your data to Google Cloud. This service helps you lift and shift your MySQL and PostgreSQL workloads into Cloud SQL.
+`Cloud Database Migration Service`_: makes it easier for you to migrate your data to Google Cloud. This service helps you lift and shift your MySQL and PostgreSQL workloads into Cloud SQL.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-dms.svg
    :target: https://pypi.org/project/google-cloud-dms/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-dms.svg
    :target: https://pypi.org/project/google-cloud-dms/
-.. _Cloud Database Migration Service API: https://cloud.google.com/database-migration/
+.. _Cloud Database Migration Service: https://cloud.google.com/database-migration/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/datamigration/latest
 .. _Product Documentation:  https://cloud.google.com/database-migration/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Database Migration Service API.`_
+3. `Enable the Cloud Database Migration Service.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Database Migration Service API.:  https://cloud.google.com/database-migration/
+.. _Enable the Cloud Database Migration Service.:  https://cloud.google.com/database-migration/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-dms
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Database Migration Service API
+-  Read the `Client Library Documentation`_ for Cloud Database Migration Service
    to see other available methods on the client.
--  Read the `Cloud Database Migration Service API Product documentation`_ to learn
+-  Read the `Cloud Database Migration Service Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Database Migration Service API Product documentation:  https://cloud.google.com/database-migration/
+.. _Cloud Database Migration Service Product documentation:  https://cloud.google.com/database-migration/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-dms-1.7.0/google_cloud_dms.egg-info/SOURCES.txt` & `google-cloud-dms-1.7.1/google_cloud_dms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/setup.py` & `google-cloud-dms-1.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
-url = "https://github.com/googleapis/python-dms"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-dms-1.7.0/tests/__init__.py` & `google-cloud-dms-1.7.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/tests/unit/__init__.py` & `google-cloud-dms-1.7.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/tests/unit/gapic/__init__.py` & `google-cloud-dms-1.7.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/tests/unit/gapic/clouddms_v1/__init__.py` & `google-cloud-dms-1.7.1/tests/unit/gapic/clouddms_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.7.0/tests/unit/gapic/clouddms_v1/test_data_migration_service.py` & `google-cloud-dms-1.7.1/tests/unit/gapic/clouddms_v1/test_data_migration_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1162,17 +1162,19 @@
                     clouddms_resources.MigrationJob(),
                     clouddms_resources.MigrationJob(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_migration_jobs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1203,17 +1205,14 @@
             phase=clouddms_resources.MigrationJob.Phase.FULL_DUMP,
             type_=clouddms_resources.MigrationJob.Type.ONE_TIME,
             dump_path="dump_path_value",
             source="source_value",
             destination="destination_value",
             filter="filter_value",
             cmek_key_name="cmek_key_name_value",
-            reverse_ssh_connectivity=clouddms_resources.ReverseSshConnectivity(
-                vm_ip="vm_ip_value"
-            ),
         )
         response = client.get_migration_job(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == clouddms.GetMigrationJobRequest()
@@ -3727,17 +3726,19 @@
                     clouddms_resources.ConnectionProfile(),
                     clouddms_resources.ConnectionProfile(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_connection_profiles(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3762,15 +3763,14 @@
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = clouddms_resources.ConnectionProfile(
             name="name_value",
             state=clouddms_resources.ConnectionProfile.State.DRAFT,
             display_name="display_name_value",
             provider=clouddms_resources.DatabaseProvider.CLOUDSQL,
-            mysql=clouddms_resources.MySqlConnectionProfile(host="host_value"),
         )
         response = client.get_connection_profile(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == clouddms.GetConnectionProfileRequest()
@@ -5034,17 +5034,14 @@
         type(client.transport.get_private_connection), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = clouddms_resources.PrivateConnection(
             name="name_value",
             display_name="display_name_value",
             state=clouddms_resources.PrivateConnection.State.CREATING,
-            vpc_peering_config=clouddms_resources.VpcPeeringConfig(
-                vpc_name="vpc_name_value"
-            ),
         )
         response = client.get_private_connection(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == clouddms.GetPrivateConnectionRequest()
@@ -5705,17 +5702,19 @@
                     clouddms_resources.PrivateConnection(),
                     clouddms_resources.PrivateConnection(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_private_connections(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -6657,17 +6656,19 @@
                     conversionworkspace_resources.ConversionWorkspace(),
                     conversionworkspace_resources.ConversionWorkspace(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_conversion_workspaces(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -8717,17 +8718,19 @@
                     conversionworkspace_resources.DatabaseEntity(),
                     conversionworkspace_resources.DatabaseEntity(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.describe_database_entities(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -9450,17 +9453,19 @@
                     str(),
                     str(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.fetch_static_ips(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
```

