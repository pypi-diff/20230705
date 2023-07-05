# Comparing `tmp/google-cloud-appengine-logging-1.3.0.tar.gz` & `tmp/google-cloud-appengine-logging-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-appengine-logging-1.3.0.tar", last modified: Wed Jan 11 15:33:39 2023, max compression
+gzip compressed data, was "google-cloud-appengine-logging-1.3.1.tar", last modified: Wed Jul  5 15:50:19 2023, max compression
```

## Comparing `google-cloud-appengine-logging-1.3.0.tar` & `google-cloud-appengine-logging-1.3.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:33:39.013227 google-cloud-appengine-logging-1.3.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-11 15:30:22.000000 google-cloud-appengine-logging-1.3.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-11 15:30:22.000000 google-cloud-appengine-logging-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4858 2023-01-11 15:33:39.013227 google-cloud-appengine-logging-1.3.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3912 2023-01-11 15:30:22.000000 google-cloud-appengine-logging-1.3.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:33:39.009227 google-cloud-appengine-logging-1.3.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:33:39.009227 google-cloud-appengine-logging-1.3.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:33:39.009227 google-cloud-appengine-logging-1.3.0/google/cloud/appengine_logging/
--rw-rw-r--   0 root         (0)     1003      952 2023-01-11 15:30:22.000000 google-cloud-appengine-logging-1.3.0/google/cloud/appengine_logging/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-11 15:30:22.000000 google-cloud-appengine-logging-1.3.0/google/cloud/appengine_logging/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-01-11 15:30:22.000000 google-cloud-appengine-logging-1.3.0/google/cloud/appengine_logging/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:33:39.013227 google-cloud-appengine-logging-1.3.0/google/cloud/appengine_logging_v1/
--rw-rw-r--   0 root         (0)     1003      898 2023-01-11 15:30:22.000000 google-cloud-appengine-logging-1.3.0/google/cloud/appengine_logging_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      249 2023-01-11 15:30:22.000000 google-cloud-appengine-logging-1.3.0/google/cloud/appengine_logging_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       91 2023-01-11 15:30:22.000000 google-cloud-appengine-logging-1.3.0/google/cloud/appengine_logging_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:33:39.013227 google-cloud-appengine-logging-1.3.0/google/cloud/appengine_logging_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:30:22.000000 google-cloud-appengine-logging-1.3.0/google/cloud/appengine_logging_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:33:39.013227 google-cloud-appengine-logging-1.3.0/google/cloud/appengine_logging_v1/types/
--rw-rw-r--   0 root         (0)     1003      771 2023-01-11 15:30:22.000000 google-cloud-appengine-logging-1.3.0/google/cloud/appengine_logging_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    11823 2023-01-11 15:30:22.000000 google-cloud-appengine-logging-1.3.0/google/cloud/appengine_logging_v1/types/request_log.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:33:39.013227 google-cloud-appengine-logging-1.3.0/google_cloud_appengine_logging.egg-info/
--rw-r--r--   0 root         (0)     1003     4858 2023-01-11 15:33:38.000000 google-cloud-appengine-logging-1.3.0/google_cloud_appengine_logging.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1057 2023-01-11 15:33:38.000000 google-cloud-appengine-logging-1.3.0/google_cloud_appengine_logging.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-11 15:33:38.000000 google-cloud-appengine-logging-1.3.0/google_cloud_appengine_logging.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-11 15:33:38.000000 google-cloud-appengine-logging-1.3.0/google_cloud_appengine_logging.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-11 15:33:38.000000 google-cloud-appengine-logging-1.3.0/google_cloud_appengine_logging.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-01-11 15:33:38.000000 google-cloud-appengine-logging-1.3.0/google_cloud_appengine_logging.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-11 15:33:38.000000 google-cloud-appengine-logging-1.3.0/google_cloud_appengine_logging.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-01-11 15:33:39.013227 google-cloud-appengine-logging-1.3.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3020 2023-01-11 15:30:22.000000 google-cloud-appengine-logging-1.3.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:33:39.013227 google-cloud-appengine-logging-1.3.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:30:22.000000 google-cloud-appengine-logging-1.3.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:33:39.013227 google-cloud-appengine-logging-1.3.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:30:22.000000 google-cloud-appengine-logging-1.3.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:33:39.013227 google-cloud-appengine-logging-1.3.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:30:22.000000 google-cloud-appengine-logging-1.3.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:33:39.013227 google-cloud-appengine-logging-1.3.0/tests/unit/gapic/appengine_logging_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:30:22.000000 google-cloud-appengine-logging-1.3.0/tests/unit/gapic/appengine_logging_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1023 2023-01-11 15:30:22.000000 google-cloud-appengine-logging-1.3.0/tests/unit/gapic/appengine_logging_v1/test_appengine_logging_v1.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:19.547735 google-cloud-appengine-logging-1.3.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-appengine-logging-1.3.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-appengine-logging-1.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4817 2023-07-05 15:50:19.547735 google-cloud-appengine-logging-1.3.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3876 2023-07-05 15:46:58.000000 google-cloud-appengine-logging-1.3.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:19.543735 google-cloud-appengine-logging-1.3.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:19.543735 google-cloud-appengine-logging-1.3.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:19.543735 google-cloud-appengine-logging-1.3.1/google/cloud/appengine_logging/
+-rw-rw-r--   0 root         (0)     1003      952 2023-07-05 15:46:58.000000 google-cloud-appengine-logging-1.3.1/google/cloud/appengine_logging/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-appengine-logging-1.3.1/google/cloud/appengine_logging/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-07-05 15:46:58.000000 google-cloud-appengine-logging-1.3.1/google/cloud/appengine_logging/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:19.547735 google-cloud-appengine-logging-1.3.1/google/cloud/appengine_logging_v1/
+-rw-rw-r--   0 root         (0)     1003      901 2023-07-05 15:46:58.000000 google-cloud-appengine-logging-1.3.1/google/cloud/appengine_logging_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      249 2023-07-05 15:46:58.000000 google-cloud-appengine-logging-1.3.1/google/cloud/appengine_logging_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-appengine-logging-1.3.1/google/cloud/appengine_logging_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-07-05 15:46:58.000000 google-cloud-appengine-logging-1.3.1/google/cloud/appengine_logging_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:19.547735 google-cloud-appengine-logging-1.3.1/google/cloud/appengine_logging_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-appengine-logging-1.3.1/google/cloud/appengine_logging_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:19.547735 google-cloud-appengine-logging-1.3.1/google/cloud/appengine_logging_v1/types/
+-rw-rw-r--   0 root         (0)     1003      771 2023-07-05 15:46:58.000000 google-cloud-appengine-logging-1.3.1/google/cloud/appengine_logging_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11859 2023-07-05 15:46:58.000000 google-cloud-appengine-logging-1.3.1/google/cloud/appengine_logging_v1/types/request_log.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:19.547735 google-cloud-appengine-logging-1.3.1/google_cloud_appengine_logging.egg-info/
+-rw-r--r--   0 root         (0)     1003     4817 2023-07-05 15:50:19.000000 google-cloud-appengine-logging-1.3.1/google_cloud_appengine_logging.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1108 2023-07-05 15:50:19.000000 google-cloud-appengine-logging-1.3.1/google_cloud_appengine_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:19.000000 google-cloud-appengine-logging-1.3.1/google_cloud_appengine_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:50:19.000000 google-cloud-appengine-logging-1.3.1/google_cloud_appengine_logging.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:19.000000 google-cloud-appengine-logging-1.3.1/google_cloud_appengine_logging.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:50:19.000000 google-cloud-appengine-logging-1.3.1/google_cloud_appengine_logging.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:50:19.000000 google-cloud-appengine-logging-1.3.1/google_cloud_appengine_logging.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:50:19.547735 google-cloud-appengine-logging-1.3.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2962 2023-07-05 15:46:58.000000 google-cloud-appengine-logging-1.3.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:19.547735 google-cloud-appengine-logging-1.3.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-appengine-logging-1.3.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:19.547735 google-cloud-appengine-logging-1.3.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-appengine-logging-1.3.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:19.547735 google-cloud-appengine-logging-1.3.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-appengine-logging-1.3.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:19.547735 google-cloud-appengine-logging-1.3.1/tests/unit/gapic/appengine_logging_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-appengine-logging-1.3.1/tests/unit/gapic/appengine_logging_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1023 2023-07-05 15:46:58.000000 google-cloud-appengine-logging-1.3.1/tests/unit/gapic/appengine_logging_v1/test_appengine_logging_v1.py
```

### Comparing `google-cloud-appengine-logging-1.3.0/LICENSE` & `google-cloud-appengine-logging-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-logging-1.3.0/MANIFEST.in` & `google-cloud-appengine-logging-1.3.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-logging-1.3.0/PKG-INFO` & `google-cloud-appengine-logging-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-appengine-logging
-Version: 1.3.0
+Version: 1.3.1
 Summary: Google Cloud Appengine Logging API client library
-Home-page: https://github.com/googleapis/python-appengine-logging
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
 
-Python Client for App Engine Logging Protos API
-===============================================
+Python Client for App Engine Logging Protos
+===========================================
 
 |stable| |pypi| |versions|
 
-`App Engine Logging Protos API`_: 
+`App Engine Logging Protos`_: 
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-appengine-logging.svg
    :target: https://pypi.org/project/google-cloud-appengine-logging/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-appengine-logging.svg
    :target: https://pypi.org/project/google-cloud-appengine-logging/
-.. _App Engine Logging Protos API: https://cloud.google.com/logging/docs/reference/v2/rpc/google.appengine.logging.v1
+.. _App Engine Logging Protos: https://cloud.google.com/logging/docs/reference/v2/rpc/google.appengine.logging.v1
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/appenginelogging/latest
 .. _Product Documentation:  https://cloud.google.com/logging/docs/reference/v2/rpc/google.appengine.logging.v1
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the App Engine Logging Protos API.`_
+3. `Enable the App Engine Logging Protos.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the App Engine Logging Protos API.:  https://cloud.google.com/logging/docs/reference/v2/rpc/google.appengine.logging.v1
+.. _Enable the App Engine Logging Protos.:  https://cloud.google.com/logging/docs/reference/v2/rpc/google.appengine.logging.v1
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-appengine-logging
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for App Engine Logging Protos API
+-  Read the `Client Library Documentation`_ for App Engine Logging Protos
    to see other available methods on the client.
--  Read the `App Engine Logging Protos API Product documentation`_ to learn
+-  Read the `App Engine Logging Protos Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _App Engine Logging Protos API Product documentation:  https://cloud.google.com/logging/docs/reference/v2/rpc/google.appengine.logging.v1
+.. _App Engine Logging Protos Product documentation:  https://cloud.google.com/logging/docs/reference/v2/rpc/google.appengine.logging.v1
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-appengine-logging-1.3.0/README.rst` & `google-cloud-appengine-logging-1.3.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for App Engine Logging Protos API
-===============================================
+Python Client for App Engine Logging Protos
+===========================================
 
 |stable| |pypi| |versions|
 
-`App Engine Logging Protos API`_: 
+`App Engine Logging Protos`_: 
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-appengine-logging.svg
    :target: https://pypi.org/project/google-cloud-appengine-logging/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-appengine-logging.svg
    :target: https://pypi.org/project/google-cloud-appengine-logging/
-.. _App Engine Logging Protos API: https://cloud.google.com/logging/docs/reference/v2/rpc/google.appengine.logging.v1
+.. _App Engine Logging Protos: https://cloud.google.com/logging/docs/reference/v2/rpc/google.appengine.logging.v1
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/appenginelogging/latest
 .. _Product Documentation:  https://cloud.google.com/logging/docs/reference/v2/rpc/google.appengine.logging.v1
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the App Engine Logging Protos API.`_
+3. `Enable the App Engine Logging Protos.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the App Engine Logging Protos API.:  https://cloud.google.com/logging/docs/reference/v2/rpc/google.appengine.logging.v1
+.. _Enable the App Engine Logging Protos.:  https://cloud.google.com/logging/docs/reference/v2/rpc/google.appengine.logging.v1
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-appengine-logging
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for App Engine Logging Protos API
+-  Read the `Client Library Documentation`_ for App Engine Logging Protos
    to see other available methods on the client.
--  Read the `App Engine Logging Protos API Product documentation`_ to learn
+-  Read the `App Engine Logging Protos Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _App Engine Logging Protos API Product documentation:  https://cloud.google.com/logging/docs/reference/v2/rpc/google.appengine.logging.v1
+.. _App Engine Logging Protos Product documentation:  https://cloud.google.com/logging/docs/reference/v2/rpc/google.appengine.logging.v1
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-appengine-logging-1.3.0/google/cloud/appengine_logging/__init__.py` & `google-cloud-appengine-logging-1.3.1/google/cloud/appengine_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-logging-1.3.0/google/cloud/appengine_logging/gapic_version.py` & `google-cloud-appengine-logging-1.3.1/google/cloud/appengine_logging/gapic_version.py`

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
-__version__ = "1.3.0"  # {x-release-please-version}
+__version__ = "1.3.1"  # {x-release-please-version}
```

### Comparing `google-cloud-appengine-logging-1.3.0/google/cloud/appengine_logging_v1/__init__.py` & `google-cloud-appengine-logging-1.3.1/google/cloud/appengine_logging_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.appengine_logging import gapic_version as package_version
+from google.cloud.appengine_logging_v1 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
 from .types.request_log import LogLine, RequestLog, SourceLocation, SourceReference
 
 __all__ = (
```

### Comparing `google-cloud-appengine-logging-1.3.0/google/cloud/appengine_logging_v1/services/__init__.py` & `google-cloud-appengine-logging-1.3.1/google/cloud/appengine_logging_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-logging-1.3.0/google/cloud/appengine_logging_v1/types/__init__.py` & `google-cloud-appengine-logging-1.3.1/google/cloud/appengine_logging_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-logging-1.3.0/google/cloud/appengine_logging_v1/types/request_log.py` & `google-cloud-appengine-logging-1.3.1/google/cloud/appengine_logging_v1/types/request_log.py`

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
 
 from google.logging.type import log_severity_pb2  # type: ignore
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
```

### Comparing `google-cloud-appengine-logging-1.3.0/google_cloud_appengine_logging.egg-info/PKG-INFO` & `google-cloud-appengine-logging-1.3.1/google_cloud_appengine_logging.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-appengine-logging
-Version: 1.3.0
+Version: 1.3.1
 Summary: Google Cloud Appengine Logging API client library
-Home-page: https://github.com/googleapis/python-appengine-logging
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
 
-Python Client for App Engine Logging Protos API
-===============================================
+Python Client for App Engine Logging Protos
+===========================================
 
 |stable| |pypi| |versions|
 
-`App Engine Logging Protos API`_: 
+`App Engine Logging Protos`_: 
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-appengine-logging.svg
    :target: https://pypi.org/project/google-cloud-appengine-logging/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-appengine-logging.svg
    :target: https://pypi.org/project/google-cloud-appengine-logging/
-.. _App Engine Logging Protos API: https://cloud.google.com/logging/docs/reference/v2/rpc/google.appengine.logging.v1
+.. _App Engine Logging Protos: https://cloud.google.com/logging/docs/reference/v2/rpc/google.appengine.logging.v1
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/appenginelogging/latest
 .. _Product Documentation:  https://cloud.google.com/logging/docs/reference/v2/rpc/google.appengine.logging.v1
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the App Engine Logging Protos API.`_
+3. `Enable the App Engine Logging Protos.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the App Engine Logging Protos API.:  https://cloud.google.com/logging/docs/reference/v2/rpc/google.appengine.logging.v1
+.. _Enable the App Engine Logging Protos.:  https://cloud.google.com/logging/docs/reference/v2/rpc/google.appengine.logging.v1
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-appengine-logging
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for App Engine Logging Protos API
+-  Read the `Client Library Documentation`_ for App Engine Logging Protos
    to see other available methods on the client.
--  Read the `App Engine Logging Protos API Product documentation`_ to learn
+-  Read the `App Engine Logging Protos Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _App Engine Logging Protos API Product documentation:  https://cloud.google.com/logging/docs/reference/v2/rpc/google.appengine.logging.v1
+.. _App Engine Logging Protos Product documentation:  https://cloud.google.com/logging/docs/reference/v2/rpc/google.appengine.logging.v1
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-appengine-logging-1.3.0/google_cloud_appengine_logging.egg-info/SOURCES.txt` & `google-cloud-appengine-logging-1.3.1/google_cloud_appengine_logging.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.cfg
 setup.py
 google/cloud/appengine_logging/__init__.py
 google/cloud/appengine_logging/gapic_version.py
 google/cloud/appengine_logging/py.typed
 google/cloud/appengine_logging_v1/__init__.py
 google/cloud/appengine_logging_v1/gapic_metadata.json
+google/cloud/appengine_logging_v1/gapic_version.py
 google/cloud/appengine_logging_v1/py.typed
 google/cloud/appengine_logging_v1/services/__init__.py
 google/cloud/appengine_logging_v1/types/__init__.py
 google/cloud/appengine_logging_v1/types/request_log.py
 google_cloud_appengine_logging.egg-info/PKG-INFO
 google_cloud_appengine_logging.egg-info/SOURCES.txt
 google_cloud_appengine_logging.egg-info/dependency_links.txt
```

### Comparing `google-cloud-appengine-logging-1.3.0/setup.py` & `google-cloud-appengine-logging-1.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,31 +39,29 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-appengine-logging"
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

### Comparing `google-cloud-appengine-logging-1.3.0/tests/__init__.py` & `google-cloud-appengine-logging-1.3.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-logging-1.3.0/tests/unit/__init__.py` & `google-cloud-appengine-logging-1.3.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-logging-1.3.0/tests/unit/gapic/__init__.py` & `google-cloud-appengine-logging-1.3.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-logging-1.3.0/tests/unit/gapic/appengine_logging_v1/__init__.py` & `google-cloud-appengine-logging-1.3.1/tests/unit/gapic/appengine_logging_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-logging-1.3.0/tests/unit/gapic/appengine_logging_v1/test_appengine_logging_v1.py` & `google-cloud-appengine-logging-1.3.1/tests/unit/gapic/appengine_logging_v1/test_appengine_logging_v1.py`

 * *Files identical despite different names*

