# Comparing `tmp/google-cloud-vm-migration-1.6.1.tar.gz` & `tmp/google-cloud-vm-migration-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-vm-migration-1.6.1.tar", last modified: Mon Mar 27 15:52:05 2023, max compression
+gzip compressed data, was "google-cloud-vm-migration-1.6.2.tar", last modified: Wed Jul  5 15:56:26 2023, max compression
```

## Comparing `google-cloud-vm-migration-1.6.1.tar` & `google-cloud-vm-migration-1.6.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:05.440505 google-cloud-vm-migration-1.6.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4712 2023-03-27 15:52:05.440505 google-cloud-vm-migration-1.6.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3781 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:05.432502 google-cloud-vm-migration-1.6.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:05.432502 google-cloud-vm-migration-1.6.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:05.432502 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration/
--rw-rw-r--   0 root         (0)     1003     7199 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:05.436504 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/
--rw-rw-r--   0 root         (0)     1003     7058 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    18442 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:05.436504 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:05.436504 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/vm_migration/
--rw-rw-r--   0 root         (0)     1003      757 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/vm_migration/__init__.py
--rw-rw-r--   0 root         (0)     1003   243361 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/vm_migration/async_client.py
--rw-rw-r--   0 root         (0)     1003   264674 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/vm_migration/client.py
--rw-rw-r--   0 root         (0)     1003    46901 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/vm_migration/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:05.436504 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/vm_migration/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/vm_migration/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    28408 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/vm_migration/transports/base.py
--rw-rw-r--   0 root         (0)     1003    70819 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/vm_migration/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    72562 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/vm_migration/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   272305 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/vm_migration/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:05.436504 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/types/
--rw-rw-r--   0 root         (0)     1003     6802 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003   157158 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/types/vmmigration.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:05.440505 google-cloud-vm-migration-1.6.1/google_cloud_vm_migration.egg-info/
--rw-r--r--   0 root         (0)     1003     4712 2023-03-27 15:52:05.000000 google-cloud-vm-migration-1.6.1/google_cloud_vm_migration.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1598 2023-03-27 15:52:05.000000 google-cloud-vm-migration-1.6.1/google_cloud_vm_migration.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:52:05.000000 google-cloud-vm-migration-1.6.1/google_cloud_vm_migration.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:52:05.000000 google-cloud-vm-migration-1.6.1/google_cloud_vm_migration.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:52:05.000000 google-cloud-vm-migration-1.6.1/google_cloud_vm_migration.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 15:52:05.000000 google-cloud-vm-migration-1.6.1/google_cloud_vm_migration.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:52:05.000000 google-cloud-vm-migration-1.6.1/google_cloud_vm_migration.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:52:05.440505 google-cloud-vm-migration-1.6.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2993 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:05.440505 google-cloud-vm-migration-1.6.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:05.440505 google-cloud-vm-migration-1.6.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:05.440505 google-cloud-vm-migration-1.6.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:05.440505 google-cloud-vm-migration-1.6.1/tests/unit/gapic/vmmigration_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/tests/unit/gapic/vmmigration_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003  1105392 2023-03-27 15:49:52.000000 google-cloud-vm-migration-1.6.1/tests/unit/gapic/vmmigration_v1/test_vm_migration.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:26.740573 google-cloud-vm-migration-1.6.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4676 2023-07-05 15:56:26.740573 google-cloud-vm-migration-1.6.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3745 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:26.732573 google-cloud-vm-migration-1.6.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:26.732573 google-cloud-vm-migration-1.6.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:26.732573 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration/
+-rw-rw-r--   0 root         (0)     1003     7199 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:26.732573 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/
+-rw-rw-r--   0 root         (0)     1003     7058 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18442 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:26.732573 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:26.736573 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/vm_migration/
+-rw-rw-r--   0 root         (0)     1003      757 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/vm_migration/__init__.py
+-rw-rw-r--   0 root         (0)     1003   243389 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/vm_migration/async_client.py
+-rw-rw-r--   0 root         (0)     1003   264674 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/vm_migration/client.py
+-rw-rw-r--   0 root         (0)     1003    46901 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/vm_migration/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:26.736573 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/vm_migration/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/vm_migration/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    28408 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/vm_migration/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    70819 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/vm_migration/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    72562 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/vm_migration/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   272293 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/vm_migration/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:26.736573 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/types/
+-rw-rw-r--   0 root         (0)     1003     6802 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003   157158 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/types/vmmigration.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:26.740573 google-cloud-vm-migration-1.6.2/google_cloud_vm_migration.egg-info/
+-rw-r--r--   0 root         (0)     1003     4676 2023-07-05 15:56:26.000000 google-cloud-vm-migration-1.6.2/google_cloud_vm_migration.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1598 2023-07-05 15:56:26.000000 google-cloud-vm-migration-1.6.2/google_cloud_vm_migration.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:56:26.000000 google-cloud-vm-migration-1.6.2/google_cloud_vm_migration.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:56:26.000000 google-cloud-vm-migration-1.6.2/google_cloud_vm_migration.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:56:26.000000 google-cloud-vm-migration-1.6.2/google_cloud_vm_migration.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:56:26.000000 google-cloud-vm-migration-1.6.2/google_cloud_vm_migration.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:56:26.000000 google-cloud-vm-migration-1.6.2/google_cloud_vm_migration.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:56:26.740573 google-cloud-vm-migration-1.6.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2993 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:26.740573 google-cloud-vm-migration-1.6.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:26.740573 google-cloud-vm-migration-1.6.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:26.740573 google-cloud-vm-migration-1.6.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:26.740573 google-cloud-vm-migration-1.6.2/tests/unit/gapic/vmmigration_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/tests/unit/gapic/vmmigration_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003  1105595 2023-07-05 15:46:59.000000 google-cloud-vm-migration-1.6.2/tests/unit/gapic/vmmigration_v1/test_vm_migration.py
```

### Comparing `google-cloud-vm-migration-1.6.1/LICENSE` & `google-cloud-vm-migration-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-vm-migration-1.6.1/MANIFEST.in` & `google-cloud-vm-migration-1.6.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-vm-migration-1.6.1/PKG-INFO` & `google-cloud-vm-migration-1.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-vm-migration
-Version: 1.6.1
+Version: 1.6.2
 Summary: Google Cloud Vm Migration API client library
-Home-page: https://github.com/googleapis/python-vm-migration
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
 
-Python Client for Cloud VM Migration API
-========================================
+Python Client for Cloud VM Migration
+====================================
 
 |stable| |pypi| |versions|
 
-`Cloud VM Migration API`_:  for Compute Engine migrates VMs from your on-premises data center into Compute Engine.
+`Cloud VM Migration`_:  for Compute Engine migrates VMs from your on-premises data center into Compute Engine.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-vm-migration.svg
    :target: https://pypi.org/project/google-cloud-vm-migration/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-vm-migration.svg
    :target: https://pypi.org/project/google-cloud-vm-migration/
-.. _Cloud VM Migration API: https://cloud.google.com/migrate/compute-engine/docs
+.. _Cloud VM Migration: https://cloud.google.com/migrate/compute-engine/docs
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/vmmigration/latest
 .. _Product Documentation:  https://cloud.google.com/migrate/compute-engine/docs
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud VM Migration API.`_
+3. `Enable the Cloud VM Migration.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud VM Migration API.:  https://cloud.google.com/migrate/compute-engine/docs
+.. _Enable the Cloud VM Migration.:  https://cloud.google.com/migrate/compute-engine/docs
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-vm-migration
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud VM Migration API
+-  Read the `Client Library Documentation`_ for Cloud VM Migration
    to see other available methods on the client.
--  Read the `Cloud VM Migration API Product documentation`_ to learn
+-  Read the `Cloud VM Migration Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud VM Migration API Product documentation:  https://cloud.google.com/migrate/compute-engine/docs
+.. _Cloud VM Migration Product documentation:  https://cloud.google.com/migrate/compute-engine/docs
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-vm-migration-1.6.1/README.rst` & `google-cloud-vm-migration-1.6.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Cloud VM Migration API
-========================================
+Python Client for Cloud VM Migration
+====================================
 
 |stable| |pypi| |versions|
 
-`Cloud VM Migration API`_:  for Compute Engine migrates VMs from your on-premises data center into Compute Engine.
+`Cloud VM Migration`_:  for Compute Engine migrates VMs from your on-premises data center into Compute Engine.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-vm-migration.svg
    :target: https://pypi.org/project/google-cloud-vm-migration/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-vm-migration.svg
    :target: https://pypi.org/project/google-cloud-vm-migration/
-.. _Cloud VM Migration API: https://cloud.google.com/migrate/compute-engine/docs
+.. _Cloud VM Migration: https://cloud.google.com/migrate/compute-engine/docs
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/vmmigration/latest
 .. _Product Documentation:  https://cloud.google.com/migrate/compute-engine/docs
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud VM Migration API.`_
+3. `Enable the Cloud VM Migration.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud VM Migration API.:  https://cloud.google.com/migrate/compute-engine/docs
+.. _Enable the Cloud VM Migration.:  https://cloud.google.com/migrate/compute-engine/docs
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-vm-migration
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud VM Migration API
+-  Read the `Client Library Documentation`_ for Cloud VM Migration
    to see other available methods on the client.
--  Read the `Cloud VM Migration API Product documentation`_ to learn
+-  Read the `Cloud VM Migration Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud VM Migration API Product documentation:  https://cloud.google.com/migrate/compute-engine/docs
+.. _Cloud VM Migration Product documentation:  https://cloud.google.com/migrate/compute-engine/docs
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-vm-migration-1.6.1/google/cloud/vmmigration/__init__.py` & `google-cloud-vm-migration-1.6.2/google/cloud/vmmigration/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vm-migration-1.6.1/google/cloud/vmmigration/gapic_version.py` & `google-cloud-vm-migration-1.6.2/google/cloud/vmmigration/gapic_version.py`

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
-__version__ = "1.6.1"  # {x-release-please-version}
+__version__ = "1.6.2"  # {x-release-please-version}
```

### Comparing `google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/__init__.py` & `google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/gapic_metadata.json` & `google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/gapic_version.py` & `google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/gapic_version.py`

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
-__version__ = "1.6.1"  # {x-release-please-version}
+__version__ = "1.6.2"  # {x-release-please-version}
```

### Comparing `google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/__init__.py` & `google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/vm_migration/__init__.py` & `google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/vm_migration/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/vm_migration/async_client.py` & `google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/vm_migration/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -6026,15 +6026,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "VmMigrationAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/vm_migration/client.py` & `google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/vm_migration/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/vm_migration/pagers.py` & `google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/vm_migration/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/vm_migration/transports/__init__.py` & `google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/vm_migration/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/vm_migration/transports/base.py` & `google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/vm_migration/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/vm_migration/transports/grpc.py` & `google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/vm_migration/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/vm_migration/transports/grpc_asyncio.py` & `google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/vm_migration/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/services/vm_migration/transports/rest.py` & `google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/services/vm_migration/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -6733,15 +6733,15 @@
 
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

### Comparing `google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/types/__init__.py` & `google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vm-migration-1.6.1/google/cloud/vmmigration_v1/types/vmmigration.py` & `google-cloud-vm-migration-1.6.2/google/cloud/vmmigration_v1/types/vmmigration.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vm-migration-1.6.1/google_cloud_vm_migration.egg-info/PKG-INFO` & `google-cloud-vm-migration-1.6.2/google_cloud_vm_migration.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-vm-migration
-Version: 1.6.1
+Version: 1.6.2
 Summary: Google Cloud Vm Migration API client library
-Home-page: https://github.com/googleapis/python-vm-migration
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
 
-Python Client for Cloud VM Migration API
-========================================
+Python Client for Cloud VM Migration
+====================================
 
 |stable| |pypi| |versions|
 
-`Cloud VM Migration API`_:  for Compute Engine migrates VMs from your on-premises data center into Compute Engine.
+`Cloud VM Migration`_:  for Compute Engine migrates VMs from your on-premises data center into Compute Engine.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-vm-migration.svg
    :target: https://pypi.org/project/google-cloud-vm-migration/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-vm-migration.svg
    :target: https://pypi.org/project/google-cloud-vm-migration/
-.. _Cloud VM Migration API: https://cloud.google.com/migrate/compute-engine/docs
+.. _Cloud VM Migration: https://cloud.google.com/migrate/compute-engine/docs
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/vmmigration/latest
 .. _Product Documentation:  https://cloud.google.com/migrate/compute-engine/docs
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud VM Migration API.`_
+3. `Enable the Cloud VM Migration.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud VM Migration API.:  https://cloud.google.com/migrate/compute-engine/docs
+.. _Enable the Cloud VM Migration.:  https://cloud.google.com/migrate/compute-engine/docs
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-vm-migration
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud VM Migration API
+-  Read the `Client Library Documentation`_ for Cloud VM Migration
    to see other available methods on the client.
--  Read the `Cloud VM Migration API Product documentation`_ to learn
+-  Read the `Cloud VM Migration Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud VM Migration API Product documentation:  https://cloud.google.com/migrate/compute-engine/docs
+.. _Cloud VM Migration Product documentation:  https://cloud.google.com/migrate/compute-engine/docs
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-vm-migration-1.6.1/google_cloud_vm_migration.egg-info/SOURCES.txt` & `google-cloud-vm-migration-1.6.2/google_cloud_vm_migration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-vm-migration-1.6.1/setup.py` & `google-cloud-vm-migration-1.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
-url = "https://github.com/googleapis/python-vm-migration"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-vm-migration-1.6.1/tests/__init__.py` & `google-cloud-vm-migration-1.6.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vm-migration-1.6.1/tests/unit/__init__.py` & `google-cloud-vm-migration-1.6.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vm-migration-1.6.1/tests/unit/gapic/__init__.py` & `google-cloud-vm-migration-1.6.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vm-migration-1.6.1/tests/unit/gapic/vmmigration_v1/__init__.py` & `google-cloud-vm-migration-1.6.2/tests/unit/gapic/vmmigration_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vm-migration-1.6.1/tests/unit/gapic/vmmigration_v1/test_vm_migration.py` & `google-cloud-vm-migration-1.6.2/tests/unit/gapic/vmmigration_v1/test_vm_migration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1111,17 +1111,19 @@
                     vmmigration.Source(),
                     vmmigration.Source(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_sources(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1142,15 +1144,14 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_source), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = vmmigration.Source(
             name="name_value",
             description="description_value",
-            vmware=vmmigration.VmwareSourceDetails(username="username_value"),
         )
         response = client.get_source(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == vmmigration.GetSourceRequest()
@@ -2104,19 +2105,15 @@
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.fetch_inventory), "__call__") as call:
         # Designate an appropriate return value for the call.
-        call.return_value = vmmigration.FetchInventoryResponse(
-            vmware_vms=vmmigration.VmwareVmsDetails(
-                details=[vmmigration.VmwareVmDetails(vm_id="vm_id_value")]
-            ),
-        )
+        call.return_value = vmmigration.FetchInventoryResponse()
         response = client.fetch_inventory(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == vmmigration.FetchInventoryRequest()
 
@@ -2753,17 +2750,19 @@
                     vmmigration.UtilizationReport(),
                     vmmigration.UtilizationReport(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_utilization_reports(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3965,17 +3964,19 @@
                     vmmigration.DatacenterConnector(),
                     vmmigration.DatacenterConnector(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_datacenter_connectors(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5644,17 +5645,19 @@
                     vmmigration.MigratingVm(),
                     vmmigration.MigratingVm(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_migrating_vms(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5679,20 +5682,14 @@
         call.return_value = vmmigration.MigratingVm(
             name="name_value",
             source_vm_id="source_vm_id_value",
             display_name="display_name_value",
             description="description_value",
             state=vmmigration.MigratingVm.State.PENDING,
             group="group_value",
-            compute_engine_target_defaults=vmmigration.ComputeEngineTargetDefaults(
-                vm_name="vm_name_value"
-            ),
-            aws_source_vm_details=vmmigration.AwsSourceVmDetails(
-                firmware=vmmigration.AwsSourceVmDetails.Firmware.EFI
-            ),
         )
         response = client.get_migrating_vm(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == vmmigration.GetMigratingVmRequest()
@@ -8090,17 +8087,19 @@
                     vmmigration.CloneJob(),
                     vmmigration.CloneJob(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_clone_jobs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -8121,17 +8120,14 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_clone_job), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = vmmigration.CloneJob(
             name="name_value",
             state=vmmigration.CloneJob.State.PENDING,
-            compute_engine_target_details=vmmigration.ComputeEngineTargetDetails(
-                vm_name="vm_name_value"
-            ),
         )
         response = client.get_clone_job(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == vmmigration.GetCloneJobRequest()
@@ -9299,17 +9295,19 @@
                     vmmigration.CutoverJob(),
                     vmmigration.CutoverJob(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_cutover_jobs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -9332,17 +9330,14 @@
     with mock.patch.object(type(client.transport.get_cutover_job), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = vmmigration.CutoverJob(
             name="name_value",
             state=vmmigration.CutoverJob.State.PENDING,
             progress_percent=1733,
             state_message="state_message_value",
-            compute_engine_target_details=vmmigration.ComputeEngineTargetDetails(
-                vm_name="vm_name_value"
-            ),
         )
         response = client.get_cutover_job(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == vmmigration.GetCutoverJobRequest()
@@ -9970,17 +9965,19 @@
                     vmmigration.Group(),
                     vmmigration.Group(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_groups(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -11841,17 +11838,19 @@
                     vmmigration.TargetProject(),
                     vmmigration.TargetProject(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_target_projects(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -13292,17 +13291,19 @@
                     vmmigration.ReplicationCycle(),
                     vmmigration.ReplicationCycle(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_replication_cycles(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -13938,15 +13939,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = vmmigration.Source(
             name="name_value",
             description="description_value",
-            vmware=vmmigration.VmwareSourceDetails(username="username_value"),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = vmmigration.Source.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -15206,19 +15206,15 @@
     # send a request that will satisfy transcoding
     request_init = {"source": "projects/sample1/locations/sample2/sources/sample3"}
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
-        return_value = vmmigration.FetchInventoryResponse(
-            vmware_vms=vmmigration.VmwareVmsDetails(
-                details=[vmmigration.VmwareVmDetails(vm_id="vm_id_value")]
-            ),
-        )
+        return_value = vmmigration.FetchInventoryResponse()
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = vmmigration.FetchInventoryResponse.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
 
@@ -19356,20 +19352,14 @@
         return_value = vmmigration.MigratingVm(
             name="name_value",
             source_vm_id="source_vm_id_value",
             display_name="display_name_value",
             description="description_value",
             state=vmmigration.MigratingVm.State.PENDING,
             group="group_value",
-            compute_engine_target_defaults=vmmigration.ComputeEngineTargetDefaults(
-                vm_name="vm_name_value"
-            ),
-            aws_source_vm_details=vmmigration.AwsSourceVmDetails(
-                firmware=vmmigration.AwsSourceVmDetails.Firmware.EFI
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = vmmigration.MigratingVm.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -22583,17 +22573,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = vmmigration.CloneJob(
             name="name_value",
             state=vmmigration.CloneJob.State.PENDING,
-            compute_engine_target_details=vmmigration.ComputeEngineTargetDetails(
-                vm_name="vm_name_value"
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = vmmigration.CloneJob.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -24006,17 +23993,14 @@
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = vmmigration.CutoverJob(
             name="name_value",
             state=vmmigration.CutoverJob.State.PENDING,
             progress_percent=1733,
             state_message="state_message_value",
-            compute_engine_target_details=vmmigration.ComputeEngineTargetDetails(
-                vm_name="vm_name_value"
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = vmmigration.CutoverJob.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

