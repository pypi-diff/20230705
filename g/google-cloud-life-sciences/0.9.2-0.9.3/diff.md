# Comparing `tmp/google-cloud-life-sciences-0.9.2.tar.gz` & `tmp/google-cloud-life-sciences-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-life-sciences-0.9.2.tar", last modified: Mon Mar 27 15:55:00 2023, max compression
+gzip compressed data, was "google-cloud-life-sciences-0.9.3.tar", last modified: Wed Jul  5 15:53:42 2023, max compression
```

## Comparing `google-cloud-life-sciences-0.9.2.tar` & `google-cloud-life-sciences-0.9.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:55:00.248562 google-cloud-life-sciences-0.9.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4679 2023-03-27 15:55:00.248562 google-cloud-life-sciences-0.9.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3758 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:55:00.240563 google-cloud-life-sciences-0.9.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:55:00.240563 google-cloud-life-sciences-0.9.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:55:00.244563 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences/
--rw-rw-r--   0 root         (0)     1003     2234 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       87 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:55:00.244563 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/
--rw-rw-r--   0 root         (0)     1003     2073 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     1060 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       87 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:55:00.244563 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:55:00.244563 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/
--rw-rw-r--   0 root         (0)     1003      801 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/__init__.py
--rw-rw-r--   0 root         (0)     1003    24929 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/async_client.py
--rw-rw-r--   0 root         (0)     1003    33272 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:55:00.248562 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/
--rw-rw-r--   0 root         (0)     1003     1533 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7565 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17802 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18060 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    32210 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:55:00.248562 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/types/
--rw-rw-r--   0 root         (0)     1003     1742 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    51024 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/types/workflows.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:55:00.248562 google-cloud-life-sciences-0.9.2/google_cloud_life_sciences.egg-info/
--rw-r--r--   0 root         (0)     1003     4679 2023-03-27 15:55:00.000000 google-cloud-life-sciences-0.9.2/google_cloud_life_sciences.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1748 2023-03-27 15:55:00.000000 google-cloud-life-sciences-0.9.2/google_cloud_life_sciences.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:55:00.000000 google-cloud-life-sciences-0.9.2/google_cloud_life_sciences.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:55:00.000000 google-cloud-life-sciences-0.9.2/google_cloud_life_sciences.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:55:00.000000 google-cloud-life-sciences-0.9.2/google_cloud_life_sciences.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 15:55:00.000000 google-cloud-life-sciences-0.9.2/google_cloud_life_sciences.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:55:00.000000 google-cloud-life-sciences-0.9.2/google_cloud_life_sciences.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:55:00.252562 google-cloud-life-sciences-0.9.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2950 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:55:00.248562 google-cloud-life-sciences-0.9.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:55:00.248562 google-cloud-life-sciences-0.9.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:55:00.248562 google-cloud-life-sciences-0.9.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:55:00.248562 google-cloud-life-sciences-0.9.2/tests/unit/gapic/lifesciences_v2beta/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/tests/unit/gapic/lifesciences_v2beta/__init__.py
--rw-rw-r--   0 root         (0)     1003   106474 2023-03-27 15:52:26.000000 google-cloud-life-sciences-0.9.2/tests/unit/gapic/lifesciences_v2beta/test_workflows_service_v2_beta.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:42.224966 google-cloud-life-sciences-0.9.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4642 2023-07-05 15:53:42.224966 google-cloud-life-sciences-0.9.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3722 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:42.220966 google-cloud-life-sciences-0.9.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:42.220966 google-cloud-life-sciences-0.9.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:42.220966 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences/
+-rw-rw-r--   0 root         (0)     1003     2234 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       87 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:42.220966 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/
+-rw-rw-r--   0 root         (0)     1003     2073 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1060 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       87 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:42.220966 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:42.224966 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/
+-rw-rw-r--   0 root         (0)     1003      801 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24968 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/async_client.py
+-rw-rw-r--   0 root         (0)     1003    33272 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:42.224966 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/
+-rw-rw-r--   0 root         (0)     1003     1533 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7565 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17802 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18060 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    32198 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:42.224966 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/types/
+-rw-rw-r--   0 root         (0)     1003     1742 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    51024 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/types/workflows.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:42.224966 google-cloud-life-sciences-0.9.3/google_cloud_life_sciences.egg-info/
+-rw-r--r--   0 root         (0)     1003     4642 2023-07-05 15:53:42.000000 google-cloud-life-sciences-0.9.3/google_cloud_life_sciences.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1748 2023-07-05 15:53:42.000000 google-cloud-life-sciences-0.9.3/google_cloud_life_sciences.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:42.000000 google-cloud-life-sciences-0.9.3/google_cloud_life_sciences.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:53:42.000000 google-cloud-life-sciences-0.9.3/google_cloud_life_sciences.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:42.000000 google-cloud-life-sciences-0.9.3/google_cloud_life_sciences.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:53:42.000000 google-cloud-life-sciences-0.9.3/google_cloud_life_sciences.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:53:42.000000 google-cloud-life-sciences-0.9.3/google_cloud_life_sciences.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:53:42.228966 google-cloud-life-sciences-0.9.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2949 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:42.224966 google-cloud-life-sciences-0.9.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:42.224966 google-cloud-life-sciences-0.9.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:42.224966 google-cloud-life-sciences-0.9.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:42.224966 google-cloud-life-sciences-0.9.3/tests/unit/gapic/lifesciences_v2beta/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/tests/unit/gapic/lifesciences_v2beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003   106474 2023-07-05 15:46:59.000000 google-cloud-life-sciences-0.9.3/tests/unit/gapic/lifesciences_v2beta/test_workflows_service_v2_beta.py
```

### Comparing `google-cloud-life-sciences-0.9.2/LICENSE` & `google-cloud-life-sciences-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-life-sciences-0.9.2/MANIFEST.in` & `google-cloud-life-sciences-0.9.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-life-sciences-0.9.2/PKG-INFO` & `google-cloud-life-sciences-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-life-sciences
-Version: 0.9.2
+Version: 0.9.3
 Summary: Google Cloud Life Sciences API client library
-Home-page: https://github.com/googleapis/python-life-sciences
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
 
-Python Client for Cloud Life Sciences API
-=========================================
+Python Client for Cloud Life Sciences
+=====================================
 
 |preview| |pypi| |versions|
 
-`Cloud Life Sciences API`_: is a suite of services and tools for managing, processing, and transforming life sciences data.
+`Cloud Life Sciences`_: is a suite of services and tools for managing, processing, and transforming life sciences data.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-life-sciences.svg
    :target: https://pypi.org/project/google-cloud-life-sciences/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-life-sciences.svg
    :target: https://pypi.org/project/google-cloud-life-sciences/
-.. _Cloud Life Sciences API: https://cloud.google.com/life-sciences/
+.. _Cloud Life Sciences: https://cloud.google.com/life-sciences/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/lifesciences/latest
 .. _Product Documentation:  https://cloud.google.com/life-sciences/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Life Sciences API.`_
+3. `Enable the Cloud Life Sciences.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Life Sciences API.:  https://cloud.google.com/life-sciences/
+.. _Enable the Cloud Life Sciences.:  https://cloud.google.com/life-sciences/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-life-sciences
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Life Sciences API
+-  Read the `Client Library Documentation`_ for Cloud Life Sciences
    to see other available methods on the client.
--  Read the `Cloud Life Sciences API Product documentation`_ to learn
+-  Read the `Cloud Life Sciences Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Life Sciences API Product documentation:  https://cloud.google.com/life-sciences/
+.. _Cloud Life Sciences Product documentation:  https://cloud.google.com/life-sciences/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-life-sciences-0.9.2/README.rst` & `google-cloud-life-sciences-0.9.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Cloud Life Sciences API
-=========================================
+Python Client for Cloud Life Sciences
+=====================================
 
 |preview| |pypi| |versions|
 
-`Cloud Life Sciences API`_: is a suite of services and tools for managing, processing, and transforming life sciences data.
+`Cloud Life Sciences`_: is a suite of services and tools for managing, processing, and transforming life sciences data.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-life-sciences.svg
    :target: https://pypi.org/project/google-cloud-life-sciences/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-life-sciences.svg
    :target: https://pypi.org/project/google-cloud-life-sciences/
-.. _Cloud Life Sciences API: https://cloud.google.com/life-sciences/
+.. _Cloud Life Sciences: https://cloud.google.com/life-sciences/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/lifesciences/latest
 .. _Product Documentation:  https://cloud.google.com/life-sciences/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Life Sciences API.`_
+3. `Enable the Cloud Life Sciences.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Life Sciences API.:  https://cloud.google.com/life-sciences/
+.. _Enable the Cloud Life Sciences.:  https://cloud.google.com/life-sciences/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-life-sciences
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Life Sciences API
+-  Read the `Client Library Documentation`_ for Cloud Life Sciences
    to see other available methods on the client.
--  Read the `Cloud Life Sciences API Product documentation`_ to learn
+-  Read the `Cloud Life Sciences Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Life Sciences API Product documentation:  https://cloud.google.com/life-sciences/
+.. _Cloud Life Sciences Product documentation:  https://cloud.google.com/life-sciences/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-life-sciences-0.9.2/google/cloud/lifesciences/__init__.py` & `google-cloud-life-sciences-0.9.3/google/cloud/lifesciences/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-life-sciences-0.9.2/google/cloud/lifesciences/gapic_version.py` & `google-cloud-life-sciences-0.9.3/google/cloud/lifesciences/gapic_version.py`

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

### Comparing `google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/__init__.py` & `google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/gapic_metadata.json` & `google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/gapic_version.py` & `google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/gapic_version.py`

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

### Comparing `google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/services/__init__.py` & `google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/__init__.py` & `google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/async_client.py` & `google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -599,15 +599,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "WorkflowsServiceV2BetaAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/client.py` & `google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/__init__.py` & `google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/base.py` & `google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/grpc.py` & `google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/grpc_asyncio.py` & `google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/rest.py` & `google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/services/workflows_service_v2_beta/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -644,15 +644,15 @@
 
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

### Comparing `google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/types/__init__.py` & `google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-life-sciences-0.9.2/google/cloud/lifesciences_v2beta/types/workflows.py` & `google-cloud-life-sciences-0.9.3/google/cloud/lifesciences_v2beta/types/workflows.py`

 * *Files identical despite different names*

### Comparing `google-cloud-life-sciences-0.9.2/google_cloud_life_sciences.egg-info/PKG-INFO` & `google-cloud-life-sciences-0.9.3/google_cloud_life_sciences.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-life-sciences
-Version: 0.9.2
+Version: 0.9.3
 Summary: Google Cloud Life Sciences API client library
-Home-page: https://github.com/googleapis/python-life-sciences
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
 
-Python Client for Cloud Life Sciences API
-=========================================
+Python Client for Cloud Life Sciences
+=====================================
 
 |preview| |pypi| |versions|
 
-`Cloud Life Sciences API`_: is a suite of services and tools for managing, processing, and transforming life sciences data.
+`Cloud Life Sciences`_: is a suite of services and tools for managing, processing, and transforming life sciences data.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-life-sciences.svg
    :target: https://pypi.org/project/google-cloud-life-sciences/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-life-sciences.svg
    :target: https://pypi.org/project/google-cloud-life-sciences/
-.. _Cloud Life Sciences API: https://cloud.google.com/life-sciences/
+.. _Cloud Life Sciences: https://cloud.google.com/life-sciences/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/lifesciences/latest
 .. _Product Documentation:  https://cloud.google.com/life-sciences/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Life Sciences API.`_
+3. `Enable the Cloud Life Sciences.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Life Sciences API.:  https://cloud.google.com/life-sciences/
+.. _Enable the Cloud Life Sciences.:  https://cloud.google.com/life-sciences/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-life-sciences
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Life Sciences API
+-  Read the `Client Library Documentation`_ for Cloud Life Sciences
    to see other available methods on the client.
--  Read the `Cloud Life Sciences API Product documentation`_ to learn
+-  Read the `Cloud Life Sciences Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Life Sciences API Product documentation:  https://cloud.google.com/life-sciences/
+.. _Cloud Life Sciences Product documentation:  https://cloud.google.com/life-sciences/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-life-sciences-0.9.2/google_cloud_life_sciences.egg-info/SOURCES.txt` & `google-cloud-life-sciences-0.9.3/google_cloud_life_sciences.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-life-sciences-0.9.2/setup.py` & `google-cloud-life-sciences-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-life-sciences"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-life-sciences-0.9.2/tests/__init__.py` & `google-cloud-life-sciences-0.9.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-life-sciences-0.9.2/tests/unit/__init__.py` & `google-cloud-life-sciences-0.9.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-life-sciences-0.9.2/tests/unit/gapic/__init__.py` & `google-cloud-life-sciences-0.9.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-life-sciences-0.9.2/tests/unit/gapic/lifesciences_v2beta/__init__.py` & `google-cloud-life-sciences-0.9.3/tests/unit/gapic/lifesciences_v2beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-life-sciences-0.9.2/tests/unit/gapic/lifesciences_v2beta/test_workflows_service_v2_beta.py` & `google-cloud-life-sciences-0.9.3/tests/unit/gapic/lifesciences_v2beta/test_workflows_service_v2_beta.py`

 * *Files identical despite different names*

