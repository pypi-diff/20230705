# Comparing `tmp/google-cloud-eventarc-publishing-0.6.2.tar.gz` & `tmp/google-cloud-eventarc-publishing-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-eventarc-publishing-0.6.2.tar", last modified: Mon Mar 27 14:57:26 2023, max compression
+gzip compressed data, was "google-cloud-eventarc-publishing-0.6.3.tar", last modified: Wed Jul  5 15:53:05 2023, max compression
```

## Comparing `google-cloud-eventarc-publishing-0.6.2.tar` & `google-cloud-eventarc-publishing-0.6.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:26.220987 google-cloud-eventarc-publishing-0.6.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4784 2023-03-27 14:57:26.220987 google-cloud-eventarc-publishing-0.6.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3845 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:26.212987 google-cloud-eventarc-publishing-0.6.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:26.212987 google-cloud-eventarc-publishing-0.6.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:26.212987 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing/
--rw-rw-r--   0 root         (0)     1003     1354 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:26.216987 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/
--rw-rw-r--   0 root         (0)     1003     1183 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1500 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:26.216987 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:26.216987 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/services/publisher/
--rw-rw-r--   0 root         (0)     1003      749 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/services/publisher/__init__.py
--rw-rw-r--   0 root         (0)     1003    16494 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/services/publisher/async_client.py
--rw-rw-r--   0 root         (0)     1003    25363 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/services/publisher/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:26.216987 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/services/publisher/transports/
--rw-rw-r--   0 root         (0)     1003     1330 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/services/publisher/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6639 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/services/publisher/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14221 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/services/publisher/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14457 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/services/publisher/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    18442 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/services/publisher/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:26.216987 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/types/
--rw-rw-r--   0 root         (0)     1003      930 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3960 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/types/publisher.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:26.216987 google-cloud-eventarc-publishing-0.6.2/google_cloud_eventarc_publishing.egg-info/
--rw-r--r--   0 root         (0)     1003     4784 2023-03-27 14:57:26.000000 google-cloud-eventarc-publishing-0.6.2/google_cloud_eventarc_publishing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1718 2023-03-27 14:57:26.000000 google-cloud-eventarc-publishing-0.6.2/google_cloud_eventarc_publishing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:57:26.000000 google-cloud-eventarc-publishing-0.6.2/google_cloud_eventarc_publishing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:57:26.000000 google-cloud-eventarc-publishing-0.6.2/google_cloud_eventarc_publishing.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:57:26.000000 google-cloud-eventarc-publishing-0.6.2/google_cloud_eventarc_publishing.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 14:57:26.000000 google-cloud-eventarc-publishing-0.6.2/google_cloud_eventarc_publishing.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:57:26.000000 google-cloud-eventarc-publishing-0.6.2/google_cloud_eventarc_publishing.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 14:57:26.220987 google-cloud-eventarc-publishing-0.6.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2975 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:26.220987 google-cloud-eventarc-publishing-0.6.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:26.220987 google-cloud-eventarc-publishing-0.6.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:26.220987 google-cloud-eventarc-publishing-0.6.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:26.220987 google-cloud-eventarc-publishing-0.6.2/tests/unit/gapic/eventarc_publishing_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/tests/unit/gapic/eventarc_publishing_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    71516 2023-03-27 14:54:45.000000 google-cloud-eventarc-publishing-0.6.2/tests/unit/gapic/eventarc_publishing_v1/test_publisher.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:05.929336 google-cloud-eventarc-publishing-0.6.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4741 2023-07-05 15:53:05.929336 google-cloud-eventarc-publishing-0.6.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3809 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:05.917336 google-cloud-eventarc-publishing-0.6.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:05.921336 google-cloud-eventarc-publishing-0.6.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:05.921336 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing/
+-rw-rw-r--   0 root         (0)     1003     1354 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:05.921336 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/
+-rw-rw-r--   0 root         (0)     1003     1183 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1500 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:05.921336 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:05.925336 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/services/publisher/
+-rw-rw-r--   0 root         (0)     1003      749 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/services/publisher/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16520 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/services/publisher/async_client.py
+-rw-rw-r--   0 root         (0)     1003    25363 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/services/publisher/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:05.925336 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/services/publisher/transports/
+-rw-rw-r--   0 root         (0)     1003     1330 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/services/publisher/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6639 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/services/publisher/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14221 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/services/publisher/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14457 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/services/publisher/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    18442 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/services/publisher/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:05.925336 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/types/
+-rw-rw-r--   0 root         (0)     1003      930 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3960 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/types/publisher.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:05.925336 google-cloud-eventarc-publishing-0.6.3/google_cloud_eventarc_publishing.egg-info/
+-rw-r--r--   0 root         (0)     1003     4741 2023-07-05 15:53:05.000000 google-cloud-eventarc-publishing-0.6.3/google_cloud_eventarc_publishing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1718 2023-07-05 15:53:05.000000 google-cloud-eventarc-publishing-0.6.3/google_cloud_eventarc_publishing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:05.000000 google-cloud-eventarc-publishing-0.6.3/google_cloud_eventarc_publishing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:53:05.000000 google-cloud-eventarc-publishing-0.6.3/google_cloud_eventarc_publishing.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:05.000000 google-cloud-eventarc-publishing-0.6.3/google_cloud_eventarc_publishing.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:53:05.000000 google-cloud-eventarc-publishing-0.6.3/google_cloud_eventarc_publishing.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:53:05.000000 google-cloud-eventarc-publishing-0.6.3/google_cloud_eventarc_publishing.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:53:05.929336 google-cloud-eventarc-publishing-0.6.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2968 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:05.925336 google-cloud-eventarc-publishing-0.6.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:05.925336 google-cloud-eventarc-publishing-0.6.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:05.925336 google-cloud-eventarc-publishing-0.6.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:05.929336 google-cloud-eventarc-publishing-0.6.3/tests/unit/gapic/eventarc_publishing_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/tests/unit/gapic/eventarc_publishing_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    71516 2023-07-05 15:46:58.000000 google-cloud-eventarc-publishing-0.6.3/tests/unit/gapic/eventarc_publishing_v1/test_publisher.py
```

### Comparing `google-cloud-eventarc-publishing-0.6.2/LICENSE` & `google-cloud-eventarc-publishing-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-publishing-0.6.2/MANIFEST.in` & `google-cloud-eventarc-publishing-0.6.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-publishing-0.6.2/PKG-INFO` & `google-cloud-eventarc-publishing-0.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-eventarc-publishing
-Version: 0.6.2
+Version: 0.6.3
 Summary: Google Cloud Eventarc Publishing API client library
-Home-page: https://github.com/googleapis/python-eventarc-publishing
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
 
-Python Client for Eventarc Publishing API
-=========================================
+Python Client for Eventarc Publishing
+=====================================
 
 |preview| |pypi| |versions|
 
-`Eventarc Publishing API`_: lets you asynchronously deliver events from Google services, SaaS, and your own apps using loosely coupled services that react to state changes.
+`Eventarc Publishing`_: lets you asynchronously deliver events from Google services, SaaS, and your own apps using loosely coupled services that react to state changes.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-eventarc-publishing.svg
    :target: https://pypi.org/project/google-cloud-eventarc-publishing/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-eventarc-publishing.svg
    :target: https://pypi.org/project/google-cloud-eventarc-publishing/
-.. _Eventarc Publishing API: https://cloud.google.com/eventarc/docs
+.. _Eventarc Publishing: https://cloud.google.com/eventarc/docs
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/eventarcpublishing/latest
 .. _Product Documentation:  https://cloud.google.com/eventarc/docs
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Eventarc Publishing API.`_
+3. `Enable the Eventarc Publishing.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Eventarc Publishing API.:  https://cloud.google.com/eventarc/docs
+.. _Enable the Eventarc Publishing.:  https://cloud.google.com/eventarc/docs
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-eventarc-publishing
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Eventarc Publishing API
+-  Read the `Client Library Documentation`_ for Eventarc Publishing
    to see other available methods on the client.
--  Read the `Eventarc Publishing API Product documentation`_ to learn
+-  Read the `Eventarc Publishing Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Eventarc Publishing API Product documentation:  https://cloud.google.com/eventarc/docs
+.. _Eventarc Publishing Product documentation:  https://cloud.google.com/eventarc/docs
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-eventarc-publishing-0.6.2/README.rst` & `google-cloud-eventarc-publishing-0.6.3/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Eventarc Publishing API
-=========================================
+Python Client for Eventarc Publishing
+=====================================
 
 |preview| |pypi| |versions|
 
-`Eventarc Publishing API`_: lets you asynchronously deliver events from Google services, SaaS, and your own apps using loosely coupled services that react to state changes.
+`Eventarc Publishing`_: lets you asynchronously deliver events from Google services, SaaS, and your own apps using loosely coupled services that react to state changes.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-eventarc-publishing.svg
    :target: https://pypi.org/project/google-cloud-eventarc-publishing/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-eventarc-publishing.svg
    :target: https://pypi.org/project/google-cloud-eventarc-publishing/
-.. _Eventarc Publishing API: https://cloud.google.com/eventarc/docs
+.. _Eventarc Publishing: https://cloud.google.com/eventarc/docs
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/eventarcpublishing/latest
 .. _Product Documentation:  https://cloud.google.com/eventarc/docs
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Eventarc Publishing API.`_
+3. `Enable the Eventarc Publishing.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Eventarc Publishing API.:  https://cloud.google.com/eventarc/docs
+.. _Enable the Eventarc Publishing.:  https://cloud.google.com/eventarc/docs
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-eventarc-publishing
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Eventarc Publishing API
+-  Read the `Client Library Documentation`_ for Eventarc Publishing
    to see other available methods on the client.
--  Read the `Eventarc Publishing API Product documentation`_ to learn
+-  Read the `Eventarc Publishing Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Eventarc Publishing API Product documentation:  https://cloud.google.com/eventarc/docs
+.. _Eventarc Publishing Product documentation:  https://cloud.google.com/eventarc/docs
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing/__init__.py` & `google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing/gapic_version.py` & `google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing/gapic_version.py`

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
-__version__ = "0.6.2"  # {x-release-please-version}
+__version__ = "0.6.3"  # {x-release-please-version}
```

### Comparing `google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/__init__.py` & `google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/gapic_metadata.json` & `google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/gapic_version.py` & `google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/gapic_version.py`

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
-__version__ = "0.6.2"  # {x-release-please-version}
+__version__ = "0.6.3"  # {x-release-please-version}
```

### Comparing `google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/services/__init__.py` & `google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/services/publisher/__init__.py` & `google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/services/publisher/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/services/publisher/async_client.py` & `google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/services/publisher/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,15 +388,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "PublisherAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/services/publisher/client.py` & `google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/services/publisher/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/services/publisher/transports/__init__.py` & `google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/services/publisher/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/services/publisher/transports/base.py` & `google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/services/publisher/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/services/publisher/transports/grpc.py` & `google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/services/publisher/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/services/publisher/transports/grpc_asyncio.py` & `google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/services/publisher/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/services/publisher/transports/rest.py` & `google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/services/publisher/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/types/__init__.py` & `google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-publishing-0.6.2/google/cloud/eventarc_publishing_v1/types/publisher.py` & `google-cloud-eventarc-publishing-0.6.3/google/cloud/eventarc_publishing_v1/types/publisher.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-publishing-0.6.2/google_cloud_eventarc_publishing.egg-info/PKG-INFO` & `google-cloud-eventarc-publishing-0.6.3/google_cloud_eventarc_publishing.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-eventarc-publishing
-Version: 0.6.2
+Version: 0.6.3
 Summary: Google Cloud Eventarc Publishing API client library
-Home-page: https://github.com/googleapis/python-eventarc-publishing
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
 
-Python Client for Eventarc Publishing API
-=========================================
+Python Client for Eventarc Publishing
+=====================================
 
 |preview| |pypi| |versions|
 
-`Eventarc Publishing API`_: lets you asynchronously deliver events from Google services, SaaS, and your own apps using loosely coupled services that react to state changes.
+`Eventarc Publishing`_: lets you asynchronously deliver events from Google services, SaaS, and your own apps using loosely coupled services that react to state changes.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-eventarc-publishing.svg
    :target: https://pypi.org/project/google-cloud-eventarc-publishing/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-eventarc-publishing.svg
    :target: https://pypi.org/project/google-cloud-eventarc-publishing/
-.. _Eventarc Publishing API: https://cloud.google.com/eventarc/docs
+.. _Eventarc Publishing: https://cloud.google.com/eventarc/docs
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/eventarcpublishing/latest
 .. _Product Documentation:  https://cloud.google.com/eventarc/docs
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Eventarc Publishing API.`_
+3. `Enable the Eventarc Publishing.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Eventarc Publishing API.:  https://cloud.google.com/eventarc/docs
+.. _Enable the Eventarc Publishing.:  https://cloud.google.com/eventarc/docs
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-eventarc-publishing
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Eventarc Publishing API
+-  Read the `Client Library Documentation`_ for Eventarc Publishing
    to see other available methods on the client.
--  Read the `Eventarc Publishing API Product documentation`_ to learn
+-  Read the `Eventarc Publishing Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Eventarc Publishing API Product documentation:  https://cloud.google.com/eventarc/docs
+.. _Eventarc Publishing Product documentation:  https://cloud.google.com/eventarc/docs
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-eventarc-publishing-0.6.2/google_cloud_eventarc_publishing.egg-info/SOURCES.txt` & `google-cloud-eventarc-publishing-0.6.3/google_cloud_eventarc_publishing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-publishing-0.6.2/setup.py` & `google-cloud-eventarc-publishing-0.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-eventarc-publishing"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-eventarc-publishing-0.6.2/tests/__init__.py` & `google-cloud-eventarc-publishing-0.6.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-publishing-0.6.2/tests/unit/__init__.py` & `google-cloud-eventarc-publishing-0.6.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-publishing-0.6.2/tests/unit/gapic/__init__.py` & `google-cloud-eventarc-publishing-0.6.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-publishing-0.6.2/tests/unit/gapic/eventarc_publishing_v1/__init__.py` & `google-cloud-eventarc-publishing-0.6.3/tests/unit/gapic/eventarc_publishing_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-publishing-0.6.2/tests/unit/gapic/eventarc_publishing_v1/test_publisher.py` & `google-cloud-eventarc-publishing-0.6.3/tests/unit/gapic/eventarc_publishing_v1/test_publisher.py`

 * *Files identical despite different names*

