# Comparing `tmp/google-cloud-dataform-0.5.1.tar.gz` & `tmp/google-cloud-dataform-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-dataform-0.5.1.tar", last modified: Mon Mar 27 15:52:29 2023, max compression
+gzip compressed data, was "google-cloud-dataform-0.5.2.tar", last modified: Wed Jul  5 15:52:03 2023, max compression
```

## Comparing `google-cloud-dataform-0.5.1.tar` & `google-cloud-dataform-0.5.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:29.127484 google-cloud-dataform-0.5.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:49:49.000000 google-cloud-dataform-0.5.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:49:49.000000 google-cloud-dataform-0.5.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4430 2023-03-27 15:52:29.127484 google-cloud-dataform-0.5.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3524 2023-03-27 15:49:49.000000 google-cloud-dataform-0.5.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:29.115477 google-cloud-dataform-0.5.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:29.115477 google-cloud-dataform-0.5.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:29.119479 google-cloud-dataform-0.5.1/google/cloud/dataform/
--rw-rw-r--   0 root         (0)     1003     4793 2023-03-27 15:49:49.000000 google-cloud-dataform-0.5.1/google/cloud/dataform/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:49:49.000000 google-cloud-dataform-0.5.1/google/cloud/dataform/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-03-27 15:49:49.000000 google-cloud-dataform-0.5.1/google/cloud/dataform/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:29.119479 google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/
--rw-rw-r--   0 root         (0)     1003     4655 2023-03-27 15:49:49.000000 google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    14870 2023-03-27 15:49:50.000000 google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:49:50.000000 google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-03-27 15:49:50.000000 google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:29.119479 google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:50.000000 google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:29.119479 google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/dataform/
--rw-rw-r--   0 root         (0)     1003      745 2023-03-27 15:49:50.000000 google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/dataform/__init__.py
--rw-rw-r--   0 root         (0)     1003   144720 2023-03-27 15:49:50.000000 google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/dataform/async_client.py
--rw-rw-r--   0 root         (0)     1003   162534 2023-03-27 15:49:50.000000 google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/dataform/client.py
--rw-rw-r--   0 root         (0)     1003    37903 2023-03-27 15:49:50.000000 google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/dataform/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:29.123482 google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/dataform/transports/
--rw-rw-r--   0 root         (0)     1003     1316 2023-03-27 15:49:50.000000 google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/dataform/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    22984 2023-03-27 15:49:50.000000 google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/dataform/transports/base.py
--rw-rw-r--   0 root         (0)     1003    54507 2023-03-27 15:49:50.000000 google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/dataform/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    55648 2023-03-27 15:49:50.000000 google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/dataform/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   191467 2023-03-27 15:49:50.000000 google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/dataform/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:29.123482 google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     4413 2023-03-27 15:49:50.000000 google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    72889 2023-03-27 15:49:50.000000 google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/types/dataform.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:29.123482 google-cloud-dataform-0.5.1/google_cloud_dataform.egg-info/
--rw-r--r--   0 root         (0)     1003     4430 2023-03-27 15:52:29.000000 google-cloud-dataform-0.5.1/google_cloud_dataform.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1554 2023-03-27 15:52:29.000000 google-cloud-dataform-0.5.1/google_cloud_dataform.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:52:29.000000 google-cloud-dataform-0.5.1/google_cloud_dataform.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:52:29.000000 google-cloud-dataform-0.5.1/google_cloud_dataform.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:52:29.000000 google-cloud-dataform-0.5.1/google_cloud_dataform.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 15:52:29.000000 google-cloud-dataform-0.5.1/google_cloud_dataform.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:52:29.000000 google-cloud-dataform-0.5.1/google_cloud_dataform.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:52:29.127484 google-cloud-dataform-0.5.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2972 2023-03-27 15:49:50.000000 google-cloud-dataform-0.5.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:29.123482 google-cloud-dataform-0.5.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:50.000000 google-cloud-dataform-0.5.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:29.123482 google-cloud-dataform-0.5.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:50.000000 google-cloud-dataform-0.5.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:29.123482 google-cloud-dataform-0.5.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:50.000000 google-cloud-dataform-0.5.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:29.123482 google-cloud-dataform-0.5.1/tests/unit/gapic/dataform_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:50.000000 google-cloud-dataform-0.5.1/tests/unit/gapic/dataform_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   703045 2023-03-27 15:49:50.000000 google-cloud-dataform-0.5.1/tests/unit/gapic/dataform_v1beta1/test_dataform.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:03.481005 google-cloud-dataform-0.5.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4398 2023-07-05 15:52:03.481005 google-cloud-dataform-0.5.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3488 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:03.473005 google-cloud-dataform-0.5.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:03.473005 google-cloud-dataform-0.5.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:03.473005 google-cloud-dataform-0.5.2/google/cloud/dataform/
+-rw-rw-r--   0 root         (0)     1003     4793 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/google/cloud/dataform/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/google/cloud/dataform/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/google/cloud/dataform/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:03.477005 google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     4655 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14870 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:03.477005 google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:03.477005 google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/dataform/
+-rw-rw-r--   0 root         (0)     1003      745 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/dataform/__init__.py
+-rw-rw-r--   0 root         (0)     1003   144745 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/dataform/async_client.py
+-rw-rw-r--   0 root         (0)     1003   162534 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/dataform/client.py
+-rw-rw-r--   0 root         (0)     1003    37903 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/dataform/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:03.477005 google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/dataform/transports/
+-rw-rw-r--   0 root         (0)     1003     1316 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/dataform/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22984 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/dataform/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    54507 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/dataform/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    55648 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/dataform/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   191467 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/dataform/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:03.477005 google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     4413 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    72889 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/types/dataform.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:03.481005 google-cloud-dataform-0.5.2/google_cloud_dataform.egg-info/
+-rw-r--r--   0 root         (0)     1003     4398 2023-07-05 15:52:03.000000 google-cloud-dataform-0.5.2/google_cloud_dataform.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1554 2023-07-05 15:52:03.000000 google-cloud-dataform-0.5.2/google_cloud_dataform.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:03.000000 google-cloud-dataform-0.5.2/google_cloud_dataform.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:52:03.000000 google-cloud-dataform-0.5.2/google_cloud_dataform.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:03.000000 google-cloud-dataform-0.5.2/google_cloud_dataform.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:52:03.000000 google-cloud-dataform-0.5.2/google_cloud_dataform.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:52:03.000000 google-cloud-dataform-0.5.2/google_cloud_dataform.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:52:03.481005 google-cloud-dataform-0.5.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2976 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:03.481005 google-cloud-dataform-0.5.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:03.481005 google-cloud-dataform-0.5.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:03.481005 google-cloud-dataform-0.5.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:03.481005 google-cloud-dataform-0.5.2/tests/unit/gapic/dataform_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/tests/unit/gapic/dataform_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   704438 2023-07-05 15:46:58.000000 google-cloud-dataform-0.5.2/tests/unit/gapic/dataform_v1beta1/test_dataform.py
```

### Comparing `google-cloud-dataform-0.5.1/LICENSE` & `google-cloud-dataform-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-dataform-0.5.1/MANIFEST.in` & `google-cloud-dataform-0.5.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-dataform-0.5.1/PKG-INFO` & `google-cloud-dataform-0.5.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-dataform
-Version: 0.5.1
+Version: 0.5.2
 Summary: Google Cloud Dataform API client library
-Home-page: https://github.com/googleapis/python-dataform
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
 
-Python Client for Cloud Dataform API
-====================================
+Python Client for Cloud Dataform
+================================
 
 |preview| |pypi| |versions|
 
-`Cloud Dataform API`_: 
+`Cloud Dataform`_: 
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-dataform.svg
    :target: https://pypi.org/project/google-cloud-dataform/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-dataform.svg
    :target: https://pypi.org/project/google-cloud-dataform/
-.. _Cloud Dataform API: https://cloud.google.com
+.. _Cloud Dataform: https://cloud.google.com
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/dataform/latest
 .. _Product Documentation:  https://cloud.google.com
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Dataform API.`_
+3. `Enable the Cloud Dataform.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Dataform API.:  https://cloud.google.com
+.. _Enable the Cloud Dataform.:  https://cloud.google.com
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-dataform
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Dataform API
+-  Read the `Client Library Documentation`_ for Cloud Dataform
    to see other available methods on the client.
--  Read the `Cloud Dataform API Product documentation`_ to learn
+-  Read the `Cloud Dataform Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Dataform API Product documentation:  https://cloud.google.com
+.. _Cloud Dataform Product documentation:  https://cloud.google.com
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-dataform-0.5.1/README.rst` & `google-cloud-dataform-0.5.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Cloud Dataform API
-====================================
+Python Client for Cloud Dataform
+================================
 
 |preview| |pypi| |versions|
 
-`Cloud Dataform API`_: 
+`Cloud Dataform`_: 
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-dataform.svg
    :target: https://pypi.org/project/google-cloud-dataform/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-dataform.svg
    :target: https://pypi.org/project/google-cloud-dataform/
-.. _Cloud Dataform API: https://cloud.google.com
+.. _Cloud Dataform: https://cloud.google.com
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/dataform/latest
 .. _Product Documentation:  https://cloud.google.com
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Dataform API.`_
+3. `Enable the Cloud Dataform.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Dataform API.:  https://cloud.google.com
+.. _Enable the Cloud Dataform.:  https://cloud.google.com
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-dataform
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Dataform API
+-  Read the `Client Library Documentation`_ for Cloud Dataform
    to see other available methods on the client.
--  Read the `Cloud Dataform API Product documentation`_ to learn
+-  Read the `Cloud Dataform Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Dataform API Product documentation:  https://cloud.google.com
+.. _Cloud Dataform Product documentation:  https://cloud.google.com
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-dataform-0.5.1/google/cloud/dataform/__init__.py` & `google-cloud-dataform-0.5.2/google/cloud/dataform/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataform-0.5.1/google/cloud/dataform/gapic_version.py` & `google-cloud-dataform-0.5.2/google/cloud/dataform/gapic_version.py`

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
-__version__ = "0.5.1"  # {x-release-please-version}
+__version__ = "0.5.2"  # {x-release-please-version}
```

### Comparing `google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/__init__.py` & `google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/gapic_metadata.json` & `google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/gapic_version.py` & `google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/gapic_version.py`

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
-__version__ = "0.5.1"  # {x-release-please-version}
+__version__ = "0.5.2"  # {x-release-please-version}
```

### Comparing `google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/__init__.py` & `google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/dataform/__init__.py` & `google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/dataform/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/dataform/async_client.py` & `google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/dataform/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3596,15 +3596,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "DataformAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/dataform/client.py` & `google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/dataform/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/dataform/pagers.py` & `google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/dataform/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/dataform/transports/__init__.py` & `google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/dataform/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/dataform/transports/base.py` & `google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/dataform/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/dataform/transports/grpc.py` & `google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/dataform/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/dataform/transports/grpc_asyncio.py` & `google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/dataform/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/services/dataform/transports/rest.py` & `google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/services/dataform/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/types/__init__.py` & `google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataform-0.5.1/google/cloud/dataform_v1beta1/types/dataform.py` & `google-cloud-dataform-0.5.2/google/cloud/dataform_v1beta1/types/dataform.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataform-0.5.1/google_cloud_dataform.egg-info/PKG-INFO` & `google-cloud-dataform-0.5.2/google_cloud_dataform.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-dataform
-Version: 0.5.1
+Version: 0.5.2
 Summary: Google Cloud Dataform API client library
-Home-page: https://github.com/googleapis/python-dataform
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
 
-Python Client for Cloud Dataform API
-====================================
+Python Client for Cloud Dataform
+================================
 
 |preview| |pypi| |versions|
 
-`Cloud Dataform API`_: 
+`Cloud Dataform`_: 
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-dataform.svg
    :target: https://pypi.org/project/google-cloud-dataform/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-dataform.svg
    :target: https://pypi.org/project/google-cloud-dataform/
-.. _Cloud Dataform API: https://cloud.google.com
+.. _Cloud Dataform: https://cloud.google.com
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/dataform/latest
 .. _Product Documentation:  https://cloud.google.com
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Dataform API.`_
+3. `Enable the Cloud Dataform.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Dataform API.:  https://cloud.google.com
+.. _Enable the Cloud Dataform.:  https://cloud.google.com
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-dataform
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Dataform API
+-  Read the `Client Library Documentation`_ for Cloud Dataform
    to see other available methods on the client.
--  Read the `Cloud Dataform API Product documentation`_ to learn
+-  Read the `Cloud Dataform Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Dataform API Product documentation:  https://cloud.google.com
+.. _Cloud Dataform Product documentation:  https://cloud.google.com
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-dataform-0.5.1/google_cloud_dataform.egg-info/SOURCES.txt` & `google-cloud-dataform-0.5.2/google_cloud_dataform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-dataform-0.5.1/setup.py` & `google-cloud-dataform-0.5.2/setup.py`

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
-url = "https://github.com/googleapis/python-dataform"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-dataform-0.5.1/tests/__init__.py` & `google-cloud-dataform-0.5.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataform-0.5.1/tests/unit/__init__.py` & `google-cloud-dataform-0.5.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataform-0.5.1/tests/unit/gapic/__init__.py` & `google-cloud-dataform-0.5.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataform-0.5.1/tests/unit/gapic/dataform_v1beta1/__init__.py` & `google-cloud-dataform-0.5.2/tests/unit/gapic/dataform_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataform-0.5.1/tests/unit/gapic/dataform_v1beta1/test_dataform.py` & `google-cloud-dataform-0.5.2/tests/unit/gapic/dataform_v1beta1/test_dataform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1108,17 +1108,19 @@
                     dataform.Repository(),
                     dataform.Repository(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_repositories(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2668,17 +2670,19 @@
                     dataform.Workspace(),
                     dataform.Workspace(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_workspaces(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4928,17 +4932,19 @@
                     dataform.QueryDirectoryContentsResponse.DirectoryEntry(),
                     dataform.QueryDirectoryContentsResponse.DirectoryEntry(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.query_directory_contents(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -6380,17 +6386,19 @@
                     dataform.CompilationResult(),
                     dataform.CompilationResult(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_compilation_results(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -7250,17 +7258,19 @@
                     dataform.CompilationResultAction(),
                     dataform.CompilationResultAction(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.query_compilation_result_actions(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -7697,17 +7707,19 @@
                     dataform.WorkflowInvocation(),
                     dataform.WorkflowInvocation(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_workflow_invocations(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -8959,17 +8971,19 @@
                     dataform.WorkflowInvocationAction(),
                     dataform.WorkflowInvocationAction(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.query_workflow_invocation_actions(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

