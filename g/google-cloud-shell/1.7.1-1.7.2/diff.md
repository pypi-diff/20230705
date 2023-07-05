# Comparing `tmp/google-cloud-shell-1.7.1.tar.gz` & `tmp/google-cloud-shell-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-shell-1.7.1.tar", last modified: Mon Mar 27 16:03:37 2023, max compression
+gzip compressed data, was "google-cloud-shell-1.7.2.tar", last modified: Wed Jul  5 15:55:55 2023, max compression
```

## Comparing `google-cloud-shell-1.7.1.tar` & `google-cloud-shell-1.7.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:37.136672 google-cloud-shell-1.7.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4597 2023-03-27 16:03:37.136672 google-cloud-shell-1.7.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3687 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:37.124671 google-cloud-shell-1.7.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:37.124671 google-cloud-shell-1.7.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:37.128672 google-cloud-shell-1.7.1/google/cloud/shell/
--rw-rw-r--   0 root         (0)     1003     2071 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/google/cloud/shell/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/google/cloud/shell/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       79 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/google/cloud/shell/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:37.128672 google-cloud-shell-1.7.1/google/cloud/shell_v1/
--rw-rw-r--   0 root         (0)     1003     1945 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/google/cloud/shell_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2572 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/google/cloud/shell_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/google/cloud/shell_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       79 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/google/cloud/shell_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:37.128672 google-cloud-shell-1.7.1/google/cloud/shell_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/google/cloud/shell_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:37.132672 google-cloud-shell-1.7.1/google/cloud/shell_v1/services/cloud_shell_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/google/cloud/shell_v1/services/cloud_shell_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    30810 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/google/cloud/shell_v1/services/cloud_shell_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    39917 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/google/cloud/shell_v1/services/cloud_shell_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:37.132672 google-cloud-shell-1.7.1/google/cloud/shell_v1/services/cloud_shell_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/google/cloud/shell_v1/services/cloud_shell_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8403 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/google/cloud/shell_v1/services/cloud_shell_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18447 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/google/cloud/shell_v1/services/cloud_shell_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18858 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/google/cloud/shell_v1/services/cloud_shell_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    34009 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/google/cloud/shell_v1/services/cloud_shell_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:37.132672 google-cloud-shell-1.7.1/google/cloud/shell_v1/types/
--rw-rw-r--   0 root         (0)     1003     1651 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/google/cloud/shell_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    16170 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/google/cloud/shell_v1/types/cloudshell.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:37.132672 google-cloud-shell-1.7.1/google_cloud_shell.egg-info/
--rw-r--r--   0 root         (0)     1003     4597 2023-03-27 16:03:37.000000 google-cloud-shell-1.7.1/google_cloud_shell.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1431 2023-03-27 16:03:37.000000 google-cloud-shell-1.7.1/google_cloud_shell.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:03:37.000000 google-cloud-shell-1.7.1/google_cloud_shell.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 16:03:37.000000 google-cloud-shell-1.7.1/google_cloud_shell.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:03:37.000000 google-cloud-shell-1.7.1/google_cloud_shell.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 16:03:37.000000 google-cloud-shell-1.7.1/google_cloud_shell.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 16:03:37.000000 google-cloud-shell-1.7.1/google_cloud_shell.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 16:03:37.136672 google-cloud-shell-1.7.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2913 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:37.132672 google-cloud-shell-1.7.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:37.132672 google-cloud-shell-1.7.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:37.132672 google-cloud-shell-1.7.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:37.132672 google-cloud-shell-1.7.1/tests/unit/gapic/shell_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/tests/unit/gapic/shell_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   114991 2023-03-27 16:00:59.000000 google-cloud-shell-1.7.1/tests/unit/gapic/shell_v1/test_cloud_shell_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:55.409626 google-cloud-shell-1.7.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4568 2023-07-05 15:55:55.409626 google-cloud-shell-1.7.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3651 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:55.401627 google-cloud-shell-1.7.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:55.401627 google-cloud-shell-1.7.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:55.405626 google-cloud-shell-1.7.2/google/cloud/shell/
+-rw-rw-r--   0 root         (0)     1003     2071 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/google/cloud/shell/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/google/cloud/shell/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       79 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/google/cloud/shell/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:55.405626 google-cloud-shell-1.7.2/google/cloud/shell_v1/
+-rw-rw-r--   0 root         (0)     1003     1945 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/google/cloud/shell_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2572 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/google/cloud/shell_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/google/cloud/shell_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       79 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/google/cloud/shell_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:55.405626 google-cloud-shell-1.7.2/google/cloud/shell_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/google/cloud/shell_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:55.405626 google-cloud-shell-1.7.2/google/cloud/shell_v1/services/cloud_shell_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/google/cloud/shell_v1/services/cloud_shell_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    30844 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/google/cloud/shell_v1/services/cloud_shell_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    39917 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/google/cloud/shell_v1/services/cloud_shell_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:55.405626 google-cloud-shell-1.7.2/google/cloud/shell_v1/services/cloud_shell_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/google/cloud/shell_v1/services/cloud_shell_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8403 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/google/cloud/shell_v1/services/cloud_shell_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18447 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/google/cloud/shell_v1/services/cloud_shell_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18858 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/google/cloud/shell_v1/services/cloud_shell_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    34009 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/google/cloud/shell_v1/services/cloud_shell_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:55.405626 google-cloud-shell-1.7.2/google/cloud/shell_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1651 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/google/cloud/shell_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16170 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/google/cloud/shell_v1/types/cloudshell.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:55.409626 google-cloud-shell-1.7.2/google_cloud_shell.egg-info/
+-rw-r--r--   0 root         (0)     1003     4568 2023-07-05 15:55:55.000000 google-cloud-shell-1.7.2/google_cloud_shell.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1431 2023-07-05 15:55:55.000000 google-cloud-shell-1.7.2/google_cloud_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:55:55.000000 google-cloud-shell-1.7.2/google_cloud_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:55:55.000000 google-cloud-shell-1.7.2/google_cloud_shell.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:55:55.000000 google-cloud-shell-1.7.2/google_cloud_shell.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:55:55.000000 google-cloud-shell-1.7.2/google_cloud_shell.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:55:55.000000 google-cloud-shell-1.7.2/google_cloud_shell.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:55:55.409626 google-cloud-shell-1.7.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2920 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:55.409626 google-cloud-shell-1.7.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:55.409626 google-cloud-shell-1.7.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:55.409626 google-cloud-shell-1.7.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:55.409626 google-cloud-shell-1.7.2/tests/unit/gapic/shell_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/tests/unit/gapic/shell_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   114991 2023-07-05 15:46:59.000000 google-cloud-shell-1.7.2/tests/unit/gapic/shell_v1/test_cloud_shell_service.py
```

### Comparing `google-cloud-shell-1.7.1/LICENSE` & `google-cloud-shell-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-shell-1.7.1/MANIFEST.in` & `google-cloud-shell-1.7.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-shell-1.7.1/PKG-INFO` & `google-cloud-shell-1.7.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-shell
-Version: 1.7.1
+Version: 1.7.2
 Summary: Google Cloud Shell API client library
-Home-page: https://github.com/googleapis/python-shell
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
 
-Python Client for Cloud Shell API
-=================================
+Python Client for Cloud Shell
+=============================
 
 |stable| |pypi| |versions|
 
-`Cloud Shell API`_: is an interactive shell environment for Google Cloud that makes it easy for you to learn and experiment with Google Cloud and manage your projects and resources from your web browser.
+`Cloud Shell`_: is an interactive shell environment for Google Cloud that makes it easy for you to learn and experiment with Google Cloud and manage your projects and resources from your web browser.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-shell.svg
    :target: https://pypi.org/project/google-cloud-shell/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-shell.svg
    :target: https://pypi.org/project/google-cloud-shell/
-.. _Cloud Shell API: https://cloud.google.com/shell/
+.. _Cloud Shell: https://cloud.google.com/shell/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/cloudshell/latest
 .. _Product Documentation:  https://cloud.google.com/shell/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Shell API.`_
+3. `Enable the Cloud Shell.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Shell API.:  https://cloud.google.com/shell/
+.. _Enable the Cloud Shell.:  https://cloud.google.com/shell/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-shell
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Shell API
+-  Read the `Client Library Documentation`_ for Cloud Shell
    to see other available methods on the client.
--  Read the `Cloud Shell API Product documentation`_ to learn
+-  Read the `Cloud Shell Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Shell API Product documentation:  https://cloud.google.com/shell/
+.. _Cloud Shell Product documentation:  https://cloud.google.com/shell/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-shell-1.7.1/README.rst` & `google-cloud-shell-1.7.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Cloud Shell API
-=================================
+Python Client for Cloud Shell
+=============================
 
 |stable| |pypi| |versions|
 
-`Cloud Shell API`_: is an interactive shell environment for Google Cloud that makes it easy for you to learn and experiment with Google Cloud and manage your projects and resources from your web browser.
+`Cloud Shell`_: is an interactive shell environment for Google Cloud that makes it easy for you to learn and experiment with Google Cloud and manage your projects and resources from your web browser.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-shell.svg
    :target: https://pypi.org/project/google-cloud-shell/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-shell.svg
    :target: https://pypi.org/project/google-cloud-shell/
-.. _Cloud Shell API: https://cloud.google.com/shell/
+.. _Cloud Shell: https://cloud.google.com/shell/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/cloudshell/latest
 .. _Product Documentation:  https://cloud.google.com/shell/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Shell API.`_
+3. `Enable the Cloud Shell.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Shell API.:  https://cloud.google.com/shell/
+.. _Enable the Cloud Shell.:  https://cloud.google.com/shell/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-shell
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Shell API
+-  Read the `Client Library Documentation`_ for Cloud Shell
    to see other available methods on the client.
--  Read the `Cloud Shell API Product documentation`_ to learn
+-  Read the `Cloud Shell Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Shell API Product documentation:  https://cloud.google.com/shell/
+.. _Cloud Shell Product documentation:  https://cloud.google.com/shell/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-shell-1.7.1/google/cloud/shell/__init__.py` & `google-cloud-shell-1.7.2/google/cloud/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-shell-1.7.1/google/cloud/shell/gapic_version.py` & `google-cloud-shell-1.7.2/google/cloud/shell/gapic_version.py`

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

### Comparing `google-cloud-shell-1.7.1/google/cloud/shell_v1/__init__.py` & `google-cloud-shell-1.7.2/google/cloud/shell_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-shell-1.7.1/google/cloud/shell_v1/gapic_metadata.json` & `google-cloud-shell-1.7.2/google/cloud/shell_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-shell-1.7.1/google/cloud/shell_v1/gapic_version.py` & `google-cloud-shell-1.7.2/google/cloud/shell_v1/gapic_version.py`

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

### Comparing `google-cloud-shell-1.7.1/google/cloud/shell_v1/services/__init__.py` & `google-cloud-shell-1.7.2/google/cloud/shell_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-shell-1.7.1/google/cloud/shell_v1/services/cloud_shell_service/__init__.py` & `google-cloud-shell-1.7.2/google/cloud/shell_v1/services/cloud_shell_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-shell-1.7.1/google/cloud/shell_v1/services/cloud_shell_service/async_client.py` & `google-cloud-shell-1.7.2/google/cloud/shell_v1/services/cloud_shell_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -737,15 +737,15 @@
             cloudshell.RemovePublicKeyResponse,
             metadata_type=cloudshell.RemovePublicKeyMetadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "CloudShellServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-shell-1.7.1/google/cloud/shell_v1/services/cloud_shell_service/client.py` & `google-cloud-shell-1.7.2/google/cloud/shell_v1/services/cloud_shell_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-shell-1.7.1/google/cloud/shell_v1/services/cloud_shell_service/transports/__init__.py` & `google-cloud-shell-1.7.2/google/cloud/shell_v1/services/cloud_shell_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-shell-1.7.1/google/cloud/shell_v1/services/cloud_shell_service/transports/base.py` & `google-cloud-shell-1.7.2/google/cloud/shell_v1/services/cloud_shell_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-shell-1.7.1/google/cloud/shell_v1/services/cloud_shell_service/transports/grpc.py` & `google-cloud-shell-1.7.2/google/cloud/shell_v1/services/cloud_shell_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-shell-1.7.1/google/cloud/shell_v1/services/cloud_shell_service/transports/grpc_asyncio.py` & `google-cloud-shell-1.7.2/google/cloud/shell_v1/services/cloud_shell_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-shell-1.7.1/google/cloud/shell_v1/services/cloud_shell_service/transports/rest.py` & `google-cloud-shell-1.7.2/google/cloud/shell_v1/services/cloud_shell_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-shell-1.7.1/google/cloud/shell_v1/types/__init__.py` & `google-cloud-shell-1.7.2/google/cloud/shell_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-shell-1.7.1/google/cloud/shell_v1/types/cloudshell.py` & `google-cloud-shell-1.7.2/google/cloud/shell_v1/types/cloudshell.py`

 * *Files identical despite different names*

### Comparing `google-cloud-shell-1.7.1/google_cloud_shell.egg-info/PKG-INFO` & `google-cloud-shell-1.7.2/google_cloud_shell.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-shell
-Version: 1.7.1
+Version: 1.7.2
 Summary: Google Cloud Shell API client library
-Home-page: https://github.com/googleapis/python-shell
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
 
-Python Client for Cloud Shell API
-=================================
+Python Client for Cloud Shell
+=============================
 
 |stable| |pypi| |versions|
 
-`Cloud Shell API`_: is an interactive shell environment for Google Cloud that makes it easy for you to learn and experiment with Google Cloud and manage your projects and resources from your web browser.
+`Cloud Shell`_: is an interactive shell environment for Google Cloud that makes it easy for you to learn and experiment with Google Cloud and manage your projects and resources from your web browser.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-shell.svg
    :target: https://pypi.org/project/google-cloud-shell/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-shell.svg
    :target: https://pypi.org/project/google-cloud-shell/
-.. _Cloud Shell API: https://cloud.google.com/shell/
+.. _Cloud Shell: https://cloud.google.com/shell/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/cloudshell/latest
 .. _Product Documentation:  https://cloud.google.com/shell/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Shell API.`_
+3. `Enable the Cloud Shell.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Shell API.:  https://cloud.google.com/shell/
+.. _Enable the Cloud Shell.:  https://cloud.google.com/shell/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-shell
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Shell API
+-  Read the `Client Library Documentation`_ for Cloud Shell
    to see other available methods on the client.
--  Read the `Cloud Shell API Product documentation`_ to learn
+-  Read the `Cloud Shell Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Shell API Product documentation:  https://cloud.google.com/shell/
+.. _Cloud Shell Product documentation:  https://cloud.google.com/shell/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-shell-1.7.1/google_cloud_shell.egg-info/SOURCES.txt` & `google-cloud-shell-1.7.2/google_cloud_shell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-shell-1.7.1/setup.py` & `google-cloud-shell-1.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-shell"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-shell-1.7.1/tests/__init__.py` & `google-cloud-shell-1.7.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-shell-1.7.1/tests/unit/__init__.py` & `google-cloud-shell-1.7.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-shell-1.7.1/tests/unit/gapic/__init__.py` & `google-cloud-shell-1.7.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-shell-1.7.1/tests/unit/gapic/shell_v1/__init__.py` & `google-cloud-shell-1.7.2/tests/unit/gapic/shell_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-shell-1.7.1/tests/unit/gapic/shell_v1/test_cloud_shell_service.py` & `google-cloud-shell-1.7.2/tests/unit/gapic/shell_v1/test_cloud_shell_service.py`

 * *Files identical despite different names*

