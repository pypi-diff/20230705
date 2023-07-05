# Comparing `tmp/google-cloud-private-catalog-0.9.2.tar.gz` & `tmp/google-cloud-private-catalog-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-private-catalog-0.9.2.tar", last modified: Mon Mar 27 14:57:57 2023, max compression
+gzip compressed data, was "google-cloud-private-catalog-0.9.3.tar", last modified: Wed Jul  5 15:54:45 2023, max compression
```

## Comparing `google-cloud-private-catalog-0.9.2.tar` & `google-cloud-private-catalog-0.9.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:57.320046 google-cloud-private-catalog-0.9.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4793 2023-03-27 14:57:57.320046 google-cloud-private-catalog-0.9.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3866 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:57.312048 google-cloud-private-catalog-0.9.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:57.312048 google-cloud-private-catalog-0.9.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:57.316047 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog/
--rw-rw-r--   0 root         (0)     1003     1657 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:57.316047 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/
--rw-rw-r--   0 root         (0)     1003     1485 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1796 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:57.316047 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:57.316047 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/private_catalog/
--rw-rw-r--   0 root         (0)     1003      769 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/private_catalog/__init__.py
--rw-rw-r--   0 root         (0)     1003    22688 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/private_catalog/async_client.py
--rw-rw-r--   0 root         (0)     1003    32744 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/private_catalog/client.py
--rw-rw-r--   0 root         (0)     1003    16182 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/private_catalog/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:57.320046 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/
--rw-rw-r--   0 root         (0)     1003     1400 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7115 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15775 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16051 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    24885 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:57.320046 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1206 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    25467 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/types/private_catalog.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:57.320046 google-cloud-private-catalog-0.9.2/google_cloud_private_catalog.egg-info/
--rw-r--r--   0 root         (0)     1003     4793 2023-03-27 14:57:57.000000 google-cloud-private-catalog-0.9.2/google_cloud_private_catalog.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1806 2023-03-27 14:57:57.000000 google-cloud-private-catalog-0.9.2/google_cloud_private_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:57:57.000000 google-cloud-private-catalog-0.9.2/google_cloud_private_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:57:57.000000 google-cloud-private-catalog-0.9.2/google_cloud_private_catalog.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:57:57.000000 google-cloud-private-catalog-0.9.2/google_cloud_private_catalog.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 14:57:57.000000 google-cloud-private-catalog-0.9.2/google_cloud_private_catalog.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:57:57.000000 google-cloud-private-catalog-0.9.2/google_cloud_private_catalog.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 14:57:57.320046 google-cloud-private-catalog-0.9.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2958 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:57.320046 google-cloud-private-catalog-0.9.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:57.320046 google-cloud-private-catalog-0.9.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:57.320046 google-cloud-private-catalog-0.9.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:57.320046 google-cloud-private-catalog-0.9.2/tests/unit/gapic/privatecatalog_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/tests/unit/gapic/privatecatalog_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   121988 2023-03-27 14:55:27.000000 google-cloud-private-catalog-0.9.2/tests/unit/gapic/privatecatalog_v1beta1/test_private_catalog.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:45.671670 google-cloud-private-catalog-0.9.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4754 2023-07-05 15:54:45.671670 google-cloud-private-catalog-0.9.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3830 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:45.663670 google-cloud-private-catalog-0.9.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:45.663670 google-cloud-private-catalog-0.9.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:45.667670 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog/
+-rw-rw-r--   0 root         (0)     1003     1657 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:45.667670 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     1485 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1796 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:45.667670 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:45.667670 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/private_catalog/
+-rw-rw-r--   0 root         (0)     1003      769 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/private_catalog/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22719 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/private_catalog/async_client.py
+-rw-rw-r--   0 root         (0)     1003    32744 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/private_catalog/client.py
+-rw-rw-r--   0 root         (0)     1003    16182 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/private_catalog/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:45.667670 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/
+-rw-rw-r--   0 root         (0)     1003     1400 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7115 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15775 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16051 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    24885 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:45.667670 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1206 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25467 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/types/private_catalog.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:45.671670 google-cloud-private-catalog-0.9.3/google_cloud_private_catalog.egg-info/
+-rw-r--r--   0 root         (0)     1003     4754 2023-07-05 15:54:45.000000 google-cloud-private-catalog-0.9.3/google_cloud_private_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1806 2023-07-05 15:54:45.000000 google-cloud-private-catalog-0.9.3/google_cloud_private_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:45.000000 google-cloud-private-catalog-0.9.3/google_cloud_private_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:54:45.000000 google-cloud-private-catalog-0.9.3/google_cloud_private_catalog.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:45.000000 google-cloud-private-catalog-0.9.3/google_cloud_private_catalog.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:54:45.000000 google-cloud-private-catalog-0.9.3/google_cloud_private_catalog.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:54:45.000000 google-cloud-private-catalog-0.9.3/google_cloud_private_catalog.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:54:45.671670 google-cloud-private-catalog-0.9.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2955 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:45.671670 google-cloud-private-catalog-0.9.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:45.671670 google-cloud-private-catalog-0.9.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:45.671670 google-cloud-private-catalog-0.9.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:45.671670 google-cloud-private-catalog-0.9.3/tests/unit/gapic/privatecatalog_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/tests/unit/gapic/privatecatalog_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   122585 2023-07-05 15:46:59.000000 google-cloud-private-catalog-0.9.3/tests/unit/gapic/privatecatalog_v1beta1/test_private_catalog.py
```

### Comparing `google-cloud-private-catalog-0.9.2/LICENSE` & `google-cloud-private-catalog-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-private-catalog-0.9.2/MANIFEST.in` & `google-cloud-private-catalog-0.9.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-private-catalog-0.9.2/PKG-INFO` & `google-cloud-private-catalog-0.9.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-private-catalog
-Version: 0.9.2
+Version: 0.9.3
 Summary: Google Cloud Private Catalog API client library
-Home-page: https://github.com/googleapis/python-private-catalog
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
 
-Python Client for Private Catalog API
-=====================================
+Python Client for Private Catalog
+=================================
 
 |preview| |pypi| |versions|
 
-`Private Catalog API`_: allows developers and cloud admins to make their solutions discoverable to their internal enterprise users. Cloud admins can manage their solutions and ensure their users are always launching the latest versions.
+`Private Catalog`_: allows developers and cloud admins to make their solutions discoverable to their internal enterprise users. Cloud admins can manage their solutions and ensure their users are always launching the latest versions.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-private-catalog.svg
    :target: https://pypi.org/project/google-cloud-private-catalog/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-private-catalog.svg
    :target: https://pypi.org/project/google-cloud-private-catalog/
-.. _Private Catalog API: https://cloud.google.com/private-catalog/
+.. _Private Catalog: https://cloud.google.com/private-catalog/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/cloudprivatecatalog/latest
 .. _Product Documentation:  https://cloud.google.com/private-catalog/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Private Catalog API.`_
+3. `Enable the Private Catalog.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Private Catalog API.:  https://cloud.google.com/private-catalog/
+.. _Enable the Private Catalog.:  https://cloud.google.com/private-catalog/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-private-catalog
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Private Catalog API
+-  Read the `Client Library Documentation`_ for Private Catalog
    to see other available methods on the client.
--  Read the `Private Catalog API Product documentation`_ to learn
+-  Read the `Private Catalog Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Private Catalog API Product documentation:  https://cloud.google.com/private-catalog/
+.. _Private Catalog Product documentation:  https://cloud.google.com/private-catalog/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-private-catalog-0.9.2/README.rst` & `google-cloud-private-catalog-0.9.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Private Catalog API
-=====================================
+Python Client for Private Catalog
+=================================
 
 |preview| |pypi| |versions|
 
-`Private Catalog API`_: allows developers and cloud admins to make their solutions discoverable to their internal enterprise users. Cloud admins can manage their solutions and ensure their users are always launching the latest versions.
+`Private Catalog`_: allows developers and cloud admins to make their solutions discoverable to their internal enterprise users. Cloud admins can manage their solutions and ensure their users are always launching the latest versions.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-private-catalog.svg
    :target: https://pypi.org/project/google-cloud-private-catalog/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-private-catalog.svg
    :target: https://pypi.org/project/google-cloud-private-catalog/
-.. _Private Catalog API: https://cloud.google.com/private-catalog/
+.. _Private Catalog: https://cloud.google.com/private-catalog/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/cloudprivatecatalog/latest
 .. _Product Documentation:  https://cloud.google.com/private-catalog/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Private Catalog API.`_
+3. `Enable the Private Catalog.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Private Catalog API.:  https://cloud.google.com/private-catalog/
+.. _Enable the Private Catalog.:  https://cloud.google.com/private-catalog/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-private-catalog
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Private Catalog API
+-  Read the `Client Library Documentation`_ for Private Catalog
    to see other available methods on the client.
--  Read the `Private Catalog API Product documentation`_ to learn
+-  Read the `Private Catalog Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Private Catalog API Product documentation:  https://cloud.google.com/private-catalog/
+.. _Private Catalog Product documentation:  https://cloud.google.com/private-catalog/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog/__init__.py` & `google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog/gapic_version.py` & `google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog/gapic_version.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.9.2"  # {x-release-please-version}
+__version__ = "0.9.3"  # {x-release-please-version}
```

### Comparing `google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/__init__.py` & `google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/gapic_metadata.json` & `google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/gapic_version.py` & `google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/gapic_version.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.9.2"  # {x-release-please-version}
+__version__ = "0.9.3"  # {x-release-please-version}
```

### Comparing `google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/__init__.py` & `google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/private_catalog/__init__.py` & `google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/private_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/private_catalog/async_client.py` & `google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/private_catalog/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -522,15 +522,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "PrivateCatalogAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/private_catalog/client.py` & `google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/private_catalog/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/private_catalog/pagers.py` & `google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/private_catalog/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/__init__.py` & `google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/base.py` & `google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/grpc.py` & `google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/grpc_asyncio.py` & `google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/rest.py` & `google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/services/private_catalog/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/types/__init__.py` & `google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-catalog-0.9.2/google/cloud/privatecatalog_v1beta1/types/private_catalog.py` & `google-cloud-private-catalog-0.9.3/google/cloud/privatecatalog_v1beta1/types/private_catalog.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-catalog-0.9.2/google_cloud_private_catalog.egg-info/PKG-INFO` & `google-cloud-private-catalog-0.9.3/google_cloud_private_catalog.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-private-catalog
-Version: 0.9.2
+Version: 0.9.3
 Summary: Google Cloud Private Catalog API client library
-Home-page: https://github.com/googleapis/python-private-catalog
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
 
-Python Client for Private Catalog API
-=====================================
+Python Client for Private Catalog
+=================================
 
 |preview| |pypi| |versions|
 
-`Private Catalog API`_: allows developers and cloud admins to make their solutions discoverable to their internal enterprise users. Cloud admins can manage their solutions and ensure their users are always launching the latest versions.
+`Private Catalog`_: allows developers and cloud admins to make their solutions discoverable to their internal enterprise users. Cloud admins can manage their solutions and ensure their users are always launching the latest versions.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-private-catalog.svg
    :target: https://pypi.org/project/google-cloud-private-catalog/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-private-catalog.svg
    :target: https://pypi.org/project/google-cloud-private-catalog/
-.. _Private Catalog API: https://cloud.google.com/private-catalog/
+.. _Private Catalog: https://cloud.google.com/private-catalog/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/cloudprivatecatalog/latest
 .. _Product Documentation:  https://cloud.google.com/private-catalog/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Private Catalog API.`_
+3. `Enable the Private Catalog.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Private Catalog API.:  https://cloud.google.com/private-catalog/
+.. _Enable the Private Catalog.:  https://cloud.google.com/private-catalog/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-private-catalog
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Private Catalog API
+-  Read the `Client Library Documentation`_ for Private Catalog
    to see other available methods on the client.
--  Read the `Private Catalog API Product documentation`_ to learn
+-  Read the `Private Catalog Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Private Catalog API Product documentation:  https://cloud.google.com/private-catalog/
+.. _Private Catalog Product documentation:  https://cloud.google.com/private-catalog/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-private-catalog-0.9.2/google_cloud_private_catalog.egg-info/SOURCES.txt` & `google-cloud-private-catalog-0.9.3/google_cloud_private_catalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-private-catalog-0.9.2/setup.py` & `google-cloud-private-catalog-0.9.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-private-catalog"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-private-catalog-0.9.2/tests/__init__.py` & `google-cloud-private-catalog-0.9.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-catalog-0.9.2/tests/unit/__init__.py` & `google-cloud-private-catalog-0.9.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-catalog-0.9.2/tests/unit/gapic/__init__.py` & `google-cloud-private-catalog-0.9.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-catalog-0.9.2/tests/unit/gapic/privatecatalog_v1beta1/__init__.py` & `google-cloud-private-catalog-0.9.3/tests/unit/gapic/privatecatalog_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-catalog-0.9.2/tests/unit/gapic/privatecatalog_v1beta1/test_private_catalog.py` & `google-cloud-private-catalog-0.9.3/tests/unit/gapic/privatecatalog_v1beta1/test_private_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1028,17 +1028,19 @@
                     private_catalog.Catalog(),
                     private_catalog.Catalog(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.search_catalogs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1366,17 +1368,19 @@
                     private_catalog.Product(),
                     private_catalog.Product(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.search_products(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1704,17 +1708,19 @@
                     private_catalog.Version(),
                     private_catalog.Version(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.search_versions(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

