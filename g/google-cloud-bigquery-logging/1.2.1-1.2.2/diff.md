# Comparing `tmp/google-cloud-bigquery-logging-1.2.1.tar.gz` & `tmp/google-cloud-bigquery-logging-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-bigquery-logging-1.2.1.tar", last modified: Mon Apr  3 13:59:16 2023, max compression
+gzip compressed data, was "google-cloud-bigquery-logging-1.2.2.tar", last modified: Wed Jul  5 15:51:10 2023, max compression
```

## Comparing `google-cloud-bigquery-logging-1.2.1.tar` & `google-cloud-bigquery-logging-1.2.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:16.210765 google-cloud-bigquery-logging-1.2.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-03 13:56:13.000000 google-cloud-bigquery-logging-1.2.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-04-03 13:56:13.000000 google-cloud-bigquery-logging-1.2.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4734 2023-04-03 13:59:16.210765 google-cloud-bigquery-logging-1.2.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3791 2023-04-03 13:56:13.000000 google-cloud-bigquery-logging-1.2.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:16.206766 google-cloud-bigquery-logging-1.2.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:16.206766 google-cloud-bigquery-logging-1.2.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:16.206766 google-cloud-bigquery-logging-1.2.1/google/cloud/bigquery_logging/
--rw-rw-r--   0 root         (0)     1003     2355 2023-04-03 13:56:13.000000 google-cloud-bigquery-logging-1.2.1/google/cloud/bigquery_logging/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-04-03 13:56:13.000000 google-cloud-bigquery-logging-1.2.1/google/cloud/bigquery_logging/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-04-03 13:56:13.000000 google-cloud-bigquery-logging-1.2.1/google/cloud/bigquery_logging/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:16.206766 google-cloud-bigquery-logging-1.2.1/google/cloud/bigquery_logging_v1/
--rw-rw-r--   0 root         (0)     1003     2326 2023-04-03 13:56:13.000000 google-cloud-bigquery-logging-1.2.1/google/cloud/bigquery_logging_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      253 2023-04-03 13:56:13.000000 google-cloud-bigquery-logging-1.2.1/google/cloud/bigquery_logging_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-04-03 13:56:13.000000 google-cloud-bigquery-logging-1.2.1/google/cloud/bigquery_logging_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-04-03 13:56:13.000000 google-cloud-bigquery-logging-1.2.1/google/cloud/bigquery_logging_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:16.210765 google-cloud-bigquery-logging-1.2.1/google/cloud/bigquery_logging_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-03 13:56:13.000000 google-cloud-bigquery-logging-1.2.1/google/cloud/bigquery_logging_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:16.210765 google-cloud-bigquery-logging-1.2.1/google/cloud/bigquery_logging_v1/types/
--rw-rw-r--   0 root         (0)     1003     2197 2023-04-03 13:56:13.000000 google-cloud-bigquery-logging-1.2.1/google/cloud/bigquery_logging_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    44917 2023-04-03 13:56:13.000000 google-cloud-bigquery-logging-1.2.1/google/cloud/bigquery_logging_v1/types/audit_data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:16.210765 google-cloud-bigquery-logging-1.2.1/google_cloud_bigquery_logging.egg-info/
--rw-r--r--   0 root         (0)     1003     4734 2023-04-03 13:59:16.000000 google-cloud-bigquery-logging-1.2.1/google_cloud_bigquery_logging.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1087 2023-04-03 13:59:16.000000 google-cloud-bigquery-logging-1.2.1/google_cloud_bigquery_logging.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-03 13:59:16.000000 google-cloud-bigquery-logging-1.2.1/google_cloud_bigquery_logging.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-04-03 13:59:16.000000 google-cloud-bigquery-logging-1.2.1/google_cloud_bigquery_logging.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-03 13:59:16.000000 google-cloud-bigquery-logging-1.2.1/google_cloud_bigquery_logging.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-04-03 13:59:16.000000 google-cloud-bigquery-logging-1.2.1/google_cloud_bigquery_logging.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-03 13:59:16.000000 google-cloud-bigquery-logging-1.2.1/google_cloud_bigquery_logging.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-04-03 13:59:16.210765 google-cloud-bigquery-logging-1.2.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3010 2023-04-03 13:56:13.000000 google-cloud-bigquery-logging-1.2.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:16.210765 google-cloud-bigquery-logging-1.2.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-03 13:56:13.000000 google-cloud-bigquery-logging-1.2.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:16.210765 google-cloud-bigquery-logging-1.2.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-03 13:56:13.000000 google-cloud-bigquery-logging-1.2.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:16.210765 google-cloud-bigquery-logging-1.2.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-03 13:56:13.000000 google-cloud-bigquery-logging-1.2.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:16.210765 google-cloud-bigquery-logging-1.2.1/tests/unit/gapic/bigquery_logging_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-03 13:56:13.000000 google-cloud-bigquery-logging-1.2.1/tests/unit/gapic/bigquery_logging_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      814 2023-04-03 13:56:13.000000 google-cloud-bigquery-logging-1.2.1/tests/unit/gapic/bigquery_logging_v1/test_bigquery_logging_v1.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:10.487292 google-cloud-bigquery-logging-1.2.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-bigquery-logging-1.2.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-bigquery-logging-1.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4694 2023-07-05 15:51:10.487292 google-cloud-bigquery-logging-1.2.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3755 2023-07-05 15:46:58.000000 google-cloud-bigquery-logging-1.2.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:10.483291 google-cloud-bigquery-logging-1.2.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:10.483291 google-cloud-bigquery-logging-1.2.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:10.483291 google-cloud-bigquery-logging-1.2.2/google/cloud/bigquery_logging/
+-rw-rw-r--   0 root         (0)     1003     2355 2023-07-05 15:46:58.000000 google-cloud-bigquery-logging-1.2.2/google/cloud/bigquery_logging/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-bigquery-logging-1.2.2/google/cloud/bigquery_logging/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-07-05 15:46:58.000000 google-cloud-bigquery-logging-1.2.2/google/cloud/bigquery_logging/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:10.483291 google-cloud-bigquery-logging-1.2.2/google/cloud/bigquery_logging_v1/
+-rw-rw-r--   0 root         (0)     1003     2326 2023-07-05 15:46:58.000000 google-cloud-bigquery-logging-1.2.2/google/cloud/bigquery_logging_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      253 2023-07-05 15:46:58.000000 google-cloud-bigquery-logging-1.2.2/google/cloud/bigquery_logging_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-bigquery-logging-1.2.2/google/cloud/bigquery_logging_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-07-05 15:46:58.000000 google-cloud-bigquery-logging-1.2.2/google/cloud/bigquery_logging_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:10.483291 google-cloud-bigquery-logging-1.2.2/google/cloud/bigquery_logging_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-logging-1.2.2/google/cloud/bigquery_logging_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:10.483291 google-cloud-bigquery-logging-1.2.2/google/cloud/bigquery_logging_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2197 2023-07-05 15:46:58.000000 google-cloud-bigquery-logging-1.2.2/google/cloud/bigquery_logging_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    44917 2023-07-05 15:46:58.000000 google-cloud-bigquery-logging-1.2.2/google/cloud/bigquery_logging_v1/types/audit_data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:10.487292 google-cloud-bigquery-logging-1.2.2/google_cloud_bigquery_logging.egg-info/
+-rw-r--r--   0 root         (0)     1003     4694 2023-07-05 15:51:10.000000 google-cloud-bigquery-logging-1.2.2/google_cloud_bigquery_logging.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1087 2023-07-05 15:51:10.000000 google-cloud-bigquery-logging-1.2.2/google_cloud_bigquery_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:51:10.000000 google-cloud-bigquery-logging-1.2.2/google_cloud_bigquery_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:51:10.000000 google-cloud-bigquery-logging-1.2.2/google_cloud_bigquery_logging.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:51:10.000000 google-cloud-bigquery-logging-1.2.2/google_cloud_bigquery_logging.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:51:10.000000 google-cloud-bigquery-logging-1.2.2/google_cloud_bigquery_logging.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:51:10.000000 google-cloud-bigquery-logging-1.2.2/google_cloud_bigquery_logging.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:51:10.487292 google-cloud-bigquery-logging-1.2.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3006 2023-07-05 15:46:58.000000 google-cloud-bigquery-logging-1.2.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:10.487292 google-cloud-bigquery-logging-1.2.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-logging-1.2.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:10.487292 google-cloud-bigquery-logging-1.2.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-logging-1.2.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:10.487292 google-cloud-bigquery-logging-1.2.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-logging-1.2.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:10.487292 google-cloud-bigquery-logging-1.2.2/tests/unit/gapic/bigquery_logging_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-logging-1.2.2/tests/unit/gapic/bigquery_logging_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      814 2023-07-05 15:46:58.000000 google-cloud-bigquery-logging-1.2.2/tests/unit/gapic/bigquery_logging_v1/test_bigquery_logging_v1.py
```

### Comparing `google-cloud-bigquery-logging-1.2.1/LICENSE` & `google-cloud-bigquery-logging-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-logging-1.2.1/MANIFEST.in` & `google-cloud-bigquery-logging-1.2.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-logging-1.2.1/PKG-INFO` & `google-cloud-bigquery-logging-1.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-logging
-Version: 1.2.1
+Version: 1.2.2
 Summary: Google Cloud Bigquery Logging API client library
-Home-page: https://github.com/googleapis/python-bigquery-logging
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
 
-Python Client for BigQuery Logging Protos API
-=============================================
+Python Client for BigQuery Logging Protos
+=========================================
 
 |stable| |pypi| |versions|
 
-`BigQuery Logging Protos API`_: 
+`BigQuery Logging Protos`_: 
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-logging.svg
    :target: https://pypi.org/project/google-cloud-bigquery-logging/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-bigquery-logging.svg
    :target: https://pypi.org/project/google-cloud-bigquery-logging/
-.. _BigQuery Logging Protos API: https://cloud.google.com/bigquery/docs/reference/auditlogs
+.. _BigQuery Logging Protos: https://cloud.google.com/bigquery/docs/reference/auditlogs
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/bigquerylogging/latest
 .. _Product Documentation:  https://cloud.google.com/bigquery/docs/reference/auditlogs
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the BigQuery Logging Protos API.`_
+3. `Enable the BigQuery Logging Protos.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the BigQuery Logging Protos API.:  https://cloud.google.com/bigquery/docs/reference/auditlogs
+.. _Enable the BigQuery Logging Protos.:  https://cloud.google.com/bigquery/docs/reference/auditlogs
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-bigquery-logging
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for BigQuery Logging Protos API
+-  Read the `Client Library Documentation`_ for BigQuery Logging Protos
    to see other available methods on the client.
--  Read the `BigQuery Logging Protos API Product documentation`_ to learn
+-  Read the `BigQuery Logging Protos Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _BigQuery Logging Protos API Product documentation:  https://cloud.google.com/bigquery/docs/reference/auditlogs
+.. _BigQuery Logging Protos Product documentation:  https://cloud.google.com/bigquery/docs/reference/auditlogs
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-bigquery-logging-1.2.1/README.rst` & `google-cloud-bigquery-logging-1.2.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for BigQuery Logging Protos API
-=============================================
+Python Client for BigQuery Logging Protos
+=========================================
 
 |stable| |pypi| |versions|
 
-`BigQuery Logging Protos API`_: 
+`BigQuery Logging Protos`_: 
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-logging.svg
    :target: https://pypi.org/project/google-cloud-bigquery-logging/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-bigquery-logging.svg
    :target: https://pypi.org/project/google-cloud-bigquery-logging/
-.. _BigQuery Logging Protos API: https://cloud.google.com/bigquery/docs/reference/auditlogs
+.. _BigQuery Logging Protos: https://cloud.google.com/bigquery/docs/reference/auditlogs
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/bigquerylogging/latest
 .. _Product Documentation:  https://cloud.google.com/bigquery/docs/reference/auditlogs
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the BigQuery Logging Protos API.`_
+3. `Enable the BigQuery Logging Protos.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the BigQuery Logging Protos API.:  https://cloud.google.com/bigquery/docs/reference/auditlogs
+.. _Enable the BigQuery Logging Protos.:  https://cloud.google.com/bigquery/docs/reference/auditlogs
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-bigquery-logging
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for BigQuery Logging Protos API
+-  Read the `Client Library Documentation`_ for BigQuery Logging Protos
    to see other available methods on the client.
--  Read the `BigQuery Logging Protos API Product documentation`_ to learn
+-  Read the `BigQuery Logging Protos Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _BigQuery Logging Protos API Product documentation:  https://cloud.google.com/bigquery/docs/reference/auditlogs
+.. _BigQuery Logging Protos Product documentation:  https://cloud.google.com/bigquery/docs/reference/auditlogs
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-bigquery-logging-1.2.1/google/cloud/bigquery_logging/__init__.py` & `google-cloud-bigquery-logging-1.2.2/google/cloud/bigquery_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-logging-1.2.1/google/cloud/bigquery_logging/gapic_version.py` & `google-cloud-bigquery-logging-1.2.2/google/cloud/bigquery_logging/gapic_version.py`

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
-__version__ = "1.2.1"  # {x-release-please-version}
+__version__ = "1.2.2"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-logging-1.2.1/google/cloud/bigquery_logging_v1/__init__.py` & `google-cloud-bigquery-logging-1.2.2/google/cloud/bigquery_logging_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-logging-1.2.1/google/cloud/bigquery_logging_v1/gapic_version.py` & `google-cloud-bigquery-logging-1.2.2/google/cloud/bigquery_logging_v1/gapic_version.py`

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
-__version__ = "1.2.1"  # {x-release-please-version}
+__version__ = "1.2.2"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-logging-1.2.1/google/cloud/bigquery_logging_v1/services/__init__.py` & `google-cloud-bigquery-logging-1.2.2/google/cloud/bigquery_logging_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-logging-1.2.1/google/cloud/bigquery_logging_v1/types/__init__.py` & `google-cloud-bigquery-logging-1.2.2/google/cloud/bigquery_logging_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-logging-1.2.1/google/cloud/bigquery_logging_v1/types/audit_data.py` & `google-cloud-bigquery-logging-1.2.2/google/cloud/bigquery_logging_v1/types/audit_data.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-logging-1.2.1/google_cloud_bigquery_logging.egg-info/PKG-INFO` & `google-cloud-bigquery-logging-1.2.2/google_cloud_bigquery_logging.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-logging
-Version: 1.2.1
+Version: 1.2.2
 Summary: Google Cloud Bigquery Logging API client library
-Home-page: https://github.com/googleapis/python-bigquery-logging
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
 
-Python Client for BigQuery Logging Protos API
-=============================================
+Python Client for BigQuery Logging Protos
+=========================================
 
 |stable| |pypi| |versions|
 
-`BigQuery Logging Protos API`_: 
+`BigQuery Logging Protos`_: 
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-logging.svg
    :target: https://pypi.org/project/google-cloud-bigquery-logging/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-bigquery-logging.svg
    :target: https://pypi.org/project/google-cloud-bigquery-logging/
-.. _BigQuery Logging Protos API: https://cloud.google.com/bigquery/docs/reference/auditlogs
+.. _BigQuery Logging Protos: https://cloud.google.com/bigquery/docs/reference/auditlogs
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/bigquerylogging/latest
 .. _Product Documentation:  https://cloud.google.com/bigquery/docs/reference/auditlogs
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the BigQuery Logging Protos API.`_
+3. `Enable the BigQuery Logging Protos.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the BigQuery Logging Protos API.:  https://cloud.google.com/bigquery/docs/reference/auditlogs
+.. _Enable the BigQuery Logging Protos.:  https://cloud.google.com/bigquery/docs/reference/auditlogs
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-bigquery-logging
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for BigQuery Logging Protos API
+-  Read the `Client Library Documentation`_ for BigQuery Logging Protos
    to see other available methods on the client.
--  Read the `BigQuery Logging Protos API Product documentation`_ to learn
+-  Read the `BigQuery Logging Protos Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _BigQuery Logging Protos API Product documentation:  https://cloud.google.com/bigquery/docs/reference/auditlogs
+.. _BigQuery Logging Protos Product documentation:  https://cloud.google.com/bigquery/docs/reference/auditlogs
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-bigquery-logging-1.2.1/google_cloud_bigquery_logging.egg-info/SOURCES.txt` & `google-cloud-bigquery-logging-1.2.2/google_cloud_bigquery_logging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-logging-1.2.1/setup.py` & `google-cloud-bigquery-logging-1.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
-url = "https://github.com/googleapis/python-bigquery-logging"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-bigquery-logging-1.2.1/tests/__init__.py` & `google-cloud-bigquery-logging-1.2.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-logging-1.2.1/tests/unit/__init__.py` & `google-cloud-bigquery-logging-1.2.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-logging-1.2.1/tests/unit/gapic/__init__.py` & `google-cloud-bigquery-logging-1.2.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-logging-1.2.1/tests/unit/gapic/bigquery_logging_v1/__init__.py` & `google-cloud-bigquery-logging-1.2.2/tests/unit/gapic/bigquery_logging_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-logging-1.2.1/tests/unit/gapic/bigquery_logging_v1/test_bigquery_logging_v1.py` & `google-cloud-bigquery-logging-1.2.2/tests/unit/gapic/bigquery_logging_v1/test_bigquery_logging_v1.py`

 * *Files identical despite different names*

