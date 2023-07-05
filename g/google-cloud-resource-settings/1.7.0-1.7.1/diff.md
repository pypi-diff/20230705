# Comparing `tmp/google-cloud-resource-settings-1.7.0.tar.gz` & `tmp/google-cloud-resource-settings-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-resource-settings-1.7.0.tar", last modified: Fri Feb 24 00:04:11 2023, max compression
+gzip compressed data, was "google-cloud-resource-settings-1.7.1.tar", last modified: Wed Jul  5 15:55:21 2023, max compression
```

## Comparing `google-cloud-resource-settings-1.7.0.tar` & `google-cloud-resource-settings-1.7.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:04:11.697017 google-cloud-resource-settings-1.7.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4917 2023-02-24 00:04:11.697017 google-cloud-resource-settings-1.7.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3971 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:04:11.689019 google-cloud-resource-settings-1.7.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:04:11.689019 google-cloud-resource-settings-1.7.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:04:11.689019 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings/
--rw-rw-r--   0 root         (0)     1003     1490 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:04:11.693018 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/
--rw-rw-r--   0 root         (0)     1003     1325 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1784 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:04:11.693018 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:04:11.693018 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/resource_settings_service/
--rw-rw-r--   0 root         (0)     1003      805 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/resource_settings_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    24004 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/resource_settings_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    32210 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/resource_settings_service/client.py
--rw-rw-r--   0 root         (0)     1003     5881 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/resource_settings_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:04:11.693018 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/
--rw-rw-r--   0 root         (0)     1003     1547 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8191 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15525 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15820 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    23872 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:04:11.693018 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/types/
--rw-rw-r--   0 root         (0)     1003      990 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    12342 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/types/resource_settings.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:04:11.697017 google-cloud-resource-settings-1.7.0/google_cloud_resource_settings.egg-info/
--rw-r--r--   0 root         (0)     1003     4917 2023-02-24 00:04:11.000000 google-cloud-resource-settings-1.7.0/google_cloud_resource_settings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1874 2023-02-24 00:04:11.000000 google-cloud-resource-settings-1.7.0/google_cloud_resource_settings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-02-24 00:04:11.000000 google-cloud-resource-settings-1.7.0/google_cloud_resource_settings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-02-24 00:04:11.000000 google-cloud-resource-settings-1.7.0/google_cloud_resource_settings.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-02-24 00:04:11.000000 google-cloud-resource-settings-1.7.0/google_cloud_resource_settings.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-02-24 00:04:11.000000 google-cloud-resource-settings-1.7.0/google_cloud_resource_settings.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-02-24 00:04:11.000000 google-cloud-resource-settings-1.7.0/google_cloud_resource_settings.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-02-24 00:04:11.697017 google-cloud-resource-settings-1.7.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2966 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:04:11.697017 google-cloud-resource-settings-1.7.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:04:11.697017 google-cloud-resource-settings-1.7.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:04:11.697017 google-cloud-resource-settings-1.7.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:04:11.697017 google-cloud-resource-settings-1.7.0/tests/unit/gapic/resourcesettings_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/tests/unit/gapic/resourcesettings_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   115599 2023-02-24 00:01:49.000000 google-cloud-resource-settings-1.7.0/tests/unit/gapic/resourcesettings_v1/test_resource_settings_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:21.262688 google-cloud-resource-settings-1.7.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4876 2023-07-05 15:55:21.262688 google-cloud-resource-settings-1.7.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3935 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:21.254689 google-cloud-resource-settings-1.7.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:21.254689 google-cloud-resource-settings-1.7.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:21.258688 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings/
+-rw-rw-r--   0 root         (0)     1003     1490 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:21.258688 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/
+-rw-rw-r--   0 root         (0)     1003     1325 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1784 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:21.258688 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:21.258688 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/resource_settings_service/
+-rw-rw-r--   0 root         (0)     1003      805 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/resource_settings_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24044 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/resource_settings_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    32210 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/resource_settings_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5881 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/resource_settings_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:21.258688 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1547 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8191 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15525 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15820 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    23877 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:21.258688 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/types/
+-rw-rw-r--   0 root         (0)     1003      990 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12378 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/types/resource_settings.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:21.262688 google-cloud-resource-settings-1.7.1/google_cloud_resource_settings.egg-info/
+-rw-r--r--   0 root         (0)     1003     4876 2023-07-05 15:55:21.000000 google-cloud-resource-settings-1.7.1/google_cloud_resource_settings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1874 2023-07-05 15:55:21.000000 google-cloud-resource-settings-1.7.1/google_cloud_resource_settings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:55:21.000000 google-cloud-resource-settings-1.7.1/google_cloud_resource_settings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:55:21.000000 google-cloud-resource-settings-1.7.1/google_cloud_resource_settings.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:55:21.000000 google-cloud-resource-settings-1.7.1/google_cloud_resource_settings.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:55:21.000000 google-cloud-resource-settings-1.7.1/google_cloud_resource_settings.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:55:21.000000 google-cloud-resource-settings-1.7.1/google_cloud_resource_settings.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:55:21.262688 google-cloud-resource-settings-1.7.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2961 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:21.262688 google-cloud-resource-settings-1.7.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:21.262688 google-cloud-resource-settings-1.7.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:21.262688 google-cloud-resource-settings-1.7.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:21.262688 google-cloud-resource-settings-1.7.1/tests/unit/gapic/resourcesettings_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/tests/unit/gapic/resourcesettings_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   115798 2023-07-05 15:46:59.000000 google-cloud-resource-settings-1.7.1/tests/unit/gapic/resourcesettings_v1/test_resource_settings_service.py
```

### Comparing `google-cloud-resource-settings-1.7.0/LICENSE` & `google-cloud-resource-settings-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-settings-1.7.0/MANIFEST.in` & `google-cloud-resource-settings-1.7.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-settings-1.7.0/PKG-INFO` & `google-cloud-resource-settings-1.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-resource-settings
-Version: 1.7.0
+Version: 1.7.1
 Summary: Google Cloud Resource Settings API client library
-Home-page: https://github.com/googleapis/python-resource-settings
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
 
-Python Client for Resource Settings API
-=======================================
+Python Client for Resource Settings
+===================================
 
 |stable| |pypi| |versions|
 
-`Resource Settings API`_: allows users to control and modify the behavior of their GCP resources (e.g., VM, firewall, Project, etc.) across the Cloud Resource Hierarchy.
+`Resource Settings`_: allows users to control and modify the behavior of their GCP resources (e.g., VM, firewall, Project, etc.) across the Cloud Resource Hierarchy.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-resource-settings.svg
    :target: https://pypi.org/project/google-cloud-resource-settings/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-resource-settings.svg
    :target: https://pypi.org/project/google-cloud-resource-settings/
-.. _Resource Settings API: https://cloud.google.com/resource-manager/docs/reference/resource-settings/rest
+.. _Resource Settings: https://cloud.google.com/resource-manager/docs/reference/resource-settings/rest
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/resourcesettings/latest
 .. _Product Documentation:  https://cloud.google.com/resource-manager/docs/reference/resource-settings/rest
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Resource Settings API.`_
+3. `Enable the Resource Settings.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Resource Settings API.:  https://cloud.google.com/resource-manager/docs/reference/resource-settings/rest
+.. _Enable the Resource Settings.:  https://cloud.google.com/resource-manager/docs/reference/resource-settings/rest
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-resource-settings
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Resource Settings API
+-  Read the `Client Library Documentation`_ for Resource Settings
    to see other available methods on the client.
--  Read the `Resource Settings API Product documentation`_ to learn
+-  Read the `Resource Settings Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Resource Settings API Product documentation:  https://cloud.google.com/resource-manager/docs/reference/resource-settings/rest
+.. _Resource Settings Product documentation:  https://cloud.google.com/resource-manager/docs/reference/resource-settings/rest
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-resource-settings-1.7.0/README.rst` & `google-cloud-resource-settings-1.7.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Resource Settings API
-=======================================
+Python Client for Resource Settings
+===================================
 
 |stable| |pypi| |versions|
 
-`Resource Settings API`_: allows users to control and modify the behavior of their GCP resources (e.g., VM, firewall, Project, etc.) across the Cloud Resource Hierarchy.
+`Resource Settings`_: allows users to control and modify the behavior of their GCP resources (e.g., VM, firewall, Project, etc.) across the Cloud Resource Hierarchy.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-resource-settings.svg
    :target: https://pypi.org/project/google-cloud-resource-settings/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-resource-settings.svg
    :target: https://pypi.org/project/google-cloud-resource-settings/
-.. _Resource Settings API: https://cloud.google.com/resource-manager/docs/reference/resource-settings/rest
+.. _Resource Settings: https://cloud.google.com/resource-manager/docs/reference/resource-settings/rest
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/resourcesettings/latest
 .. _Product Documentation:  https://cloud.google.com/resource-manager/docs/reference/resource-settings/rest
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Resource Settings API.`_
+3. `Enable the Resource Settings.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Resource Settings API.:  https://cloud.google.com/resource-manager/docs/reference/resource-settings/rest
+.. _Enable the Resource Settings.:  https://cloud.google.com/resource-manager/docs/reference/resource-settings/rest
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-resource-settings
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Resource Settings API
+-  Read the `Client Library Documentation`_ for Resource Settings
    to see other available methods on the client.
--  Read the `Resource Settings API Product documentation`_ to learn
+-  Read the `Resource Settings Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Resource Settings API Product documentation:  https://cloud.google.com/resource-manager/docs/reference/resource-settings/rest
+.. _Resource Settings Product documentation:  https://cloud.google.com/resource-manager/docs/reference/resource-settings/rest
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings/__init__.py` & `google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings/gapic_version.py` & `google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings/gapic_version.py`

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

### Comparing `google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/__init__.py` & `google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/gapic_metadata.json` & `google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/gapic_version.py` & `google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/gapic_version.py`

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

### Comparing `google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/__init__.py` & `google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/resource_settings_service/__init__.py` & `google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/resource_settings_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/resource_settings_service/async_client.py` & `google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/resource_settings_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -573,15 +573,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ResourceSettingsServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/resource_settings_service/client.py` & `google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/resource_settings_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/resource_settings_service/pagers.py` & `google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/resource_settings_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/__init__.py` & `google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/base.py` & `google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/grpc.py` & `google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/grpc_asyncio.py` & `google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/rest.py` & `google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/services/resource_settings_service/transports/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import dataclasses
 import json  # type: ignore
 import re
-from typing import Callable, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
 import warnings
 
 from google.api_core import gapic_v1, path_template, rest_helpers, rest_streaming
 from google.api_core import exceptions as core_exceptions
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
@@ -271,15 +271,15 @@
         self._interceptor = interceptor or ResourceSettingsServiceRestInterceptor()
         self._prep_wrapped_messages(client_info)
 
     class _GetSetting(ResourceSettingsServiceRestStub):
         def __hash__(self):
             return hash("GetSetting")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -365,15 +365,15 @@
             resp = self._interceptor.post_get_setting(resp)
             return resp
 
     class _ListSettings(ResourceSettingsServiceRestStub):
         def __hash__(self):
             return hash("ListSettings")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -459,15 +459,15 @@
             resp = self._interceptor.post_list_settings(resp)
             return resp
 
     class _UpdateSetting(ResourceSettingsServiceRestStub):
         def __hash__(self):
             return hash("UpdateSetting")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
```

### Comparing `google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/types/__init__.py` & `google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-settings-1.7.0/google/cloud/resourcesettings_v1/types/resource_settings.py` & `google-cloud-resource-settings-1.7.1/google/cloud/resourcesettings_v1/types/resource_settings.py`

 * *Files 0% similar despite different names*

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
 
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.resourcesettings.v1",
     manifest={
```

### Comparing `google-cloud-resource-settings-1.7.0/google_cloud_resource_settings.egg-info/PKG-INFO` & `google-cloud-resource-settings-1.7.1/google_cloud_resource_settings.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-resource-settings
-Version: 1.7.0
+Version: 1.7.1
 Summary: Google Cloud Resource Settings API client library
-Home-page: https://github.com/googleapis/python-resource-settings
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
 
-Python Client for Resource Settings API
-=======================================
+Python Client for Resource Settings
+===================================
 
 |stable| |pypi| |versions|
 
-`Resource Settings API`_: allows users to control and modify the behavior of their GCP resources (e.g., VM, firewall, Project, etc.) across the Cloud Resource Hierarchy.
+`Resource Settings`_: allows users to control and modify the behavior of their GCP resources (e.g., VM, firewall, Project, etc.) across the Cloud Resource Hierarchy.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-resource-settings.svg
    :target: https://pypi.org/project/google-cloud-resource-settings/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-resource-settings.svg
    :target: https://pypi.org/project/google-cloud-resource-settings/
-.. _Resource Settings API: https://cloud.google.com/resource-manager/docs/reference/resource-settings/rest
+.. _Resource Settings: https://cloud.google.com/resource-manager/docs/reference/resource-settings/rest
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/resourcesettings/latest
 .. _Product Documentation:  https://cloud.google.com/resource-manager/docs/reference/resource-settings/rest
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Resource Settings API.`_
+3. `Enable the Resource Settings.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Resource Settings API.:  https://cloud.google.com/resource-manager/docs/reference/resource-settings/rest
+.. _Enable the Resource Settings.:  https://cloud.google.com/resource-manager/docs/reference/resource-settings/rest
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-resource-settings
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Resource Settings API
+-  Read the `Client Library Documentation`_ for Resource Settings
    to see other available methods on the client.
--  Read the `Resource Settings API Product documentation`_ to learn
+-  Read the `Resource Settings Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Resource Settings API Product documentation:  https://cloud.google.com/resource-manager/docs/reference/resource-settings/rest
+.. _Resource Settings Product documentation:  https://cloud.google.com/resource-manager/docs/reference/resource-settings/rest
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-resource-settings-1.7.0/google_cloud_resource_settings.egg-info/SOURCES.txt` & `google-cloud-resource-settings-1.7.1/google_cloud_resource_settings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-settings-1.7.0/setup.py` & `google-cloud-resource-settings-1.7.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-resource-settings"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-resource-settings-1.7.0/tests/__init__.py` & `google-cloud-resource-settings-1.7.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-settings-1.7.0/tests/unit/__init__.py` & `google-cloud-resource-settings-1.7.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-settings-1.7.0/tests/unit/gapic/__init__.py` & `google-cloud-resource-settings-1.7.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-settings-1.7.0/tests/unit/gapic/resourcesettings_v1/__init__.py` & `google-cloud-resource-settings-1.7.1/tests/unit/gapic/resourcesettings_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-settings-1.7.0/tests/unit/gapic/resourcesettings_v1/test_resource_settings_service.py` & `google-cloud-resource-settings-1.7.1/tests/unit/gapic/resourcesettings_v1/test_resource_settings_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1158,17 +1158,19 @@
                     resource_settings.Setting(),
                     resource_settings.Setting(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_settings(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

