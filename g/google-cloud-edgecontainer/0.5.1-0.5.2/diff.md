# Comparing `tmp/google-cloud-edgecontainer-0.5.1.tar.gz` & `tmp/google-cloud-edgecontainer-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-edgecontainer-0.5.1.tar", last modified: Mon Mar 27 15:54:39 2023, max compression
+gzip compressed data, was "google-cloud-edgecontainer-0.5.2.tar", last modified: Wed Jul  5 15:52:52 2023, max compression
```

## Comparing `google-cloud-edgecontainer-0.5.1.tar` & `google-cloud-edgecontainer-0.5.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:39.572547 google-cloud-edgecontainer-0.5.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4909 2023-03-27 15:54:39.572547 google-cloud-edgecontainer-0.5.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3988 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:39.564547 google-cloud-edgecontainer-0.5.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:39.564547 google-cloud-edgecontainer-0.5.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:39.564547 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer/
--rw-rw-r--   0 root         (0)     1003     3030 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       87 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:39.564547 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/
--rw-rw-r--   0 root         (0)     1003     2843 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     7030 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       87 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:39.564547 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:39.568547 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/edge_container/
--rw-rw-r--   0 root         (0)     1003      765 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/edge_container/__init__.py
--rw-rw-r--   0 root         (0)     1003   105329 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/edge_container/async_client.py
--rw-rw-r--   0 root         (0)     1003   117351 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/edge_container/client.py
--rw-rw-r--   0 root         (0)     1003    20793 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/edge_container/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:39.568547 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/edge_container/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/edge_container/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    17460 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/edge_container/transports/base.py
--rw-rw-r--   0 root         (0)     1003    35431 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/edge_container/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    36164 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/edge_container/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   114568 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/edge_container/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:39.568547 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/types/
--rw-rw-r--   0 root         (0)     1003     2569 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    24450 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/types/resources.py
--rw-rw-r--   0 root         (0)     1003    20145 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:39.568547 google-cloud-edgecontainer-0.5.1/google_cloud_edgecontainer.egg-info/
--rw-r--r--   0 root         (0)     1003     4909 2023-03-27 15:54:39.000000 google-cloud-edgecontainer-0.5.1/google_cloud_edgecontainer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1712 2023-03-27 15:54:39.000000 google-cloud-edgecontainer-0.5.1/google_cloud_edgecontainer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:54:39.000000 google-cloud-edgecontainer-0.5.1/google_cloud_edgecontainer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:54:39.000000 google-cloud-edgecontainer-0.5.1/google_cloud_edgecontainer.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:54:39.000000 google-cloud-edgecontainer-0.5.1/google_cloud_edgecontainer.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 15:54:39.000000 google-cloud-edgecontainer-0.5.1/google_cloud_edgecontainer.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:54:39.000000 google-cloud-edgecontainer-0.5.1/google_cloud_edgecontainer.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:54:39.572547 google-cloud-edgecontainer-0.5.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2951 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:39.568547 google-cloud-edgecontainer-0.5.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:39.568547 google-cloud-edgecontainer-0.5.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:39.572547 google-cloud-edgecontainer-0.5.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:39.572547 google-cloud-edgecontainer-0.5.1/tests/unit/gapic/edgecontainer_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/tests/unit/gapic/edgecontainer_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   458689 2023-03-27 15:52:05.000000 google-cloud-edgecontainer-0.5.1/tests/unit/gapic/edgecontainer_v1/test_edge_container.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:52.957381 google-cloud-edgecontainer-0.5.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4872 2023-07-05 15:52:52.957381 google-cloud-edgecontainer-0.5.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3952 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:52.945381 google-cloud-edgecontainer-0.5.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:52.945381 google-cloud-edgecontainer-0.5.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:52.949381 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer/
+-rw-rw-r--   0 root         (0)     1003     3030 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       87 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:52.949381 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/
+-rw-rw-r--   0 root         (0)     1003     2843 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7030 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       87 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:52.949381 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:52.949381 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/edge_container/
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/edge_container/__init__.py
+-rw-rw-r--   0 root         (0)     1003   105359 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/edge_container/async_client.py
+-rw-rw-r--   0 root         (0)     1003   117351 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/edge_container/client.py
+-rw-rw-r--   0 root         (0)     1003    20793 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/edge_container/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:52.953381 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/edge_container/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/edge_container/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17460 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/edge_container/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    35431 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/edge_container/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    36164 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/edge_container/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   114556 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/edge_container/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:52.953381 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2569 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24450 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/types/resources.py
+-rw-rw-r--   0 root         (0)     1003    20145 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:52.953381 google-cloud-edgecontainer-0.5.2/google_cloud_edgecontainer.egg-info/
+-rw-r--r--   0 root         (0)     1003     4872 2023-07-05 15:52:52.000000 google-cloud-edgecontainer-0.5.2/google_cloud_edgecontainer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1712 2023-07-05 15:52:52.000000 google-cloud-edgecontainer-0.5.2/google_cloud_edgecontainer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:52.000000 google-cloud-edgecontainer-0.5.2/google_cloud_edgecontainer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:52:52.000000 google-cloud-edgecontainer-0.5.2/google_cloud_edgecontainer.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:52.000000 google-cloud-edgecontainer-0.5.2/google_cloud_edgecontainer.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:52:52.000000 google-cloud-edgecontainer-0.5.2/google_cloud_edgecontainer.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:52:52.000000 google-cloud-edgecontainer-0.5.2/google_cloud_edgecontainer.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:52:52.957381 google-cloud-edgecontainer-0.5.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2950 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:52.953381 google-cloud-edgecontainer-0.5.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:52.953381 google-cloud-edgecontainer-0.5.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:52.953381 google-cloud-edgecontainer-0.5.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:52.953381 google-cloud-edgecontainer-0.5.2/tests/unit/gapic/edgecontainer_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/tests/unit/gapic/edgecontainer_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   459485 2023-07-05 15:46:58.000000 google-cloud-edgecontainer-0.5.2/tests/unit/gapic/edgecontainer_v1/test_edge_container.py
```

### Comparing `google-cloud-edgecontainer-0.5.1/LICENSE` & `google-cloud-edgecontainer-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-edgecontainer-0.5.1/MANIFEST.in` & `google-cloud-edgecontainer-0.5.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-edgecontainer-0.5.1/PKG-INFO` & `google-cloud-edgecontainer-0.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-edgecontainer
-Version: 0.5.1
+Version: 0.5.2
 Summary: Google Cloud Edgecontainer API client library
-Home-page: https://github.com/googleapis/python-edgecontainer
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
 
-Python Client for Distributed Cloud Edge Container API
-======================================================
+Python Client for Distributed Cloud Edge Container
+==================================================
 
 |preview| |pypi| |versions|
 
-`Distributed Cloud Edge Container API`_: Google Distributed Cloud Edge allows you to run Kubernetes clusters on dedicated hardware provided and maintained by Google that is separate from the Google Cloud data center.
+`Distributed Cloud Edge Container`_: Google Distributed Cloud Edge allows you to run Kubernetes clusters on dedicated hardware provided and maintained by Google that is separate from the Google Cloud data center.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-edgecontainer.svg
    :target: https://pypi.org/project/google-cloud-edgecontainer/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-edgecontainer.svg
    :target: https://pypi.org/project/google-cloud-edgecontainer/
-.. _Distributed Cloud Edge Container API: https://cloud.google.com/distributed-cloud/edge
+.. _Distributed Cloud Edge Container: https://cloud.google.com/distributed-cloud/edge
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/edgecontainer/latest
 .. _Product Documentation:  https://cloud.google.com/distributed-cloud/edge
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Distributed Cloud Edge Container API.`_
+3. `Enable the Distributed Cloud Edge Container.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Distributed Cloud Edge Container API.:  https://cloud.google.com/distributed-cloud/edge
+.. _Enable the Distributed Cloud Edge Container.:  https://cloud.google.com/distributed-cloud/edge
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-edgecontainer
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Distributed Cloud Edge Container API
+-  Read the `Client Library Documentation`_ for Distributed Cloud Edge Container
    to see other available methods on the client.
--  Read the `Distributed Cloud Edge Container API Product documentation`_ to learn
+-  Read the `Distributed Cloud Edge Container Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Distributed Cloud Edge Container API Product documentation:  https://cloud.google.com/distributed-cloud/edge
+.. _Distributed Cloud Edge Container Product documentation:  https://cloud.google.com/distributed-cloud/edge
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-edgecontainer-0.5.1/README.rst` & `google-cloud-edgecontainer-0.5.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Distributed Cloud Edge Container API
-======================================================
+Python Client for Distributed Cloud Edge Container
+==================================================
 
 |preview| |pypi| |versions|
 
-`Distributed Cloud Edge Container API`_: Google Distributed Cloud Edge allows you to run Kubernetes clusters on dedicated hardware provided and maintained by Google that is separate from the Google Cloud data center.
+`Distributed Cloud Edge Container`_: Google Distributed Cloud Edge allows you to run Kubernetes clusters on dedicated hardware provided and maintained by Google that is separate from the Google Cloud data center.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-edgecontainer.svg
    :target: https://pypi.org/project/google-cloud-edgecontainer/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-edgecontainer.svg
    :target: https://pypi.org/project/google-cloud-edgecontainer/
-.. _Distributed Cloud Edge Container API: https://cloud.google.com/distributed-cloud/edge
+.. _Distributed Cloud Edge Container: https://cloud.google.com/distributed-cloud/edge
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/edgecontainer/latest
 .. _Product Documentation:  https://cloud.google.com/distributed-cloud/edge
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Distributed Cloud Edge Container API.`_
+3. `Enable the Distributed Cloud Edge Container.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Distributed Cloud Edge Container API.:  https://cloud.google.com/distributed-cloud/edge
+.. _Enable the Distributed Cloud Edge Container.:  https://cloud.google.com/distributed-cloud/edge
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-edgecontainer
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Distributed Cloud Edge Container API
+-  Read the `Client Library Documentation`_ for Distributed Cloud Edge Container
    to see other available methods on the client.
--  Read the `Distributed Cloud Edge Container API Product documentation`_ to learn
+-  Read the `Distributed Cloud Edge Container Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Distributed Cloud Edge Container API Product documentation:  https://cloud.google.com/distributed-cloud/edge
+.. _Distributed Cloud Edge Container Product documentation:  https://cloud.google.com/distributed-cloud/edge
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer/__init__.py` & `google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer/gapic_version.py` & `google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer/gapic_version.py`

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

### Comparing `google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/__init__.py` & `google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/gapic_metadata.json` & `google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/gapic_version.py` & `google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/gapic_version.py`

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

### Comparing `google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/__init__.py` & `google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/edge_container/__init__.py` & `google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/edge_container/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/edge_container/async_client.py` & `google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/edge_container/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2640,15 +2640,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "EdgeContainerAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/edge_container/client.py` & `google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/edge_container/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/edge_container/pagers.py` & `google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/edge_container/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/edge_container/transports/__init__.py` & `google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/edge_container/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/edge_container/transports/base.py` & `google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/edge_container/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/edge_container/transports/grpc.py` & `google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/edge_container/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/edge_container/transports/grpc_asyncio.py` & `google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/edge_container/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/services/edge_container/transports/rest.py` & `google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/services/edge_container/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -2700,15 +2700,15 @@
 
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

### Comparing `google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/types/__init__.py` & `google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/types/resources.py` & `google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/types/resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-edgecontainer-0.5.1/google/cloud/edgecontainer_v1/types/service.py` & `google-cloud-edgecontainer-0.5.2/google/cloud/edgecontainer_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-edgecontainer-0.5.1/google_cloud_edgecontainer.egg-info/PKG-INFO` & `google-cloud-edgecontainer-0.5.2/google_cloud_edgecontainer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-edgecontainer
-Version: 0.5.1
+Version: 0.5.2
 Summary: Google Cloud Edgecontainer API client library
-Home-page: https://github.com/googleapis/python-edgecontainer
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
 
-Python Client for Distributed Cloud Edge Container API
-======================================================
+Python Client for Distributed Cloud Edge Container
+==================================================
 
 |preview| |pypi| |versions|
 
-`Distributed Cloud Edge Container API`_: Google Distributed Cloud Edge allows you to run Kubernetes clusters on dedicated hardware provided and maintained by Google that is separate from the Google Cloud data center.
+`Distributed Cloud Edge Container`_: Google Distributed Cloud Edge allows you to run Kubernetes clusters on dedicated hardware provided and maintained by Google that is separate from the Google Cloud data center.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-edgecontainer.svg
    :target: https://pypi.org/project/google-cloud-edgecontainer/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-edgecontainer.svg
    :target: https://pypi.org/project/google-cloud-edgecontainer/
-.. _Distributed Cloud Edge Container API: https://cloud.google.com/distributed-cloud/edge
+.. _Distributed Cloud Edge Container: https://cloud.google.com/distributed-cloud/edge
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/edgecontainer/latest
 .. _Product Documentation:  https://cloud.google.com/distributed-cloud/edge
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Distributed Cloud Edge Container API.`_
+3. `Enable the Distributed Cloud Edge Container.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Distributed Cloud Edge Container API.:  https://cloud.google.com/distributed-cloud/edge
+.. _Enable the Distributed Cloud Edge Container.:  https://cloud.google.com/distributed-cloud/edge
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-edgecontainer
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Distributed Cloud Edge Container API
+-  Read the `Client Library Documentation`_ for Distributed Cloud Edge Container
    to see other available methods on the client.
--  Read the `Distributed Cloud Edge Container API Product documentation`_ to learn
+-  Read the `Distributed Cloud Edge Container Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Distributed Cloud Edge Container API Product documentation:  https://cloud.google.com/distributed-cloud/edge
+.. _Distributed Cloud Edge Container Product documentation:  https://cloud.google.com/distributed-cloud/edge
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-edgecontainer-0.5.1/google_cloud_edgecontainer.egg-info/SOURCES.txt` & `google-cloud-edgecontainer-0.5.2/google_cloud_edgecontainer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-edgecontainer-0.5.1/setup.py` & `google-cloud-edgecontainer-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-edgecontainer"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-edgecontainer-0.5.1/tests/__init__.py` & `google-cloud-edgecontainer-0.5.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-edgecontainer-0.5.1/tests/unit/__init__.py` & `google-cloud-edgecontainer-0.5.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-edgecontainer-0.5.1/tests/unit/gapic/__init__.py` & `google-cloud-edgecontainer-0.5.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-edgecontainer-0.5.1/tests/unit/gapic/edgecontainer_v1/__init__.py` & `google-cloud-edgecontainer-0.5.2/tests/unit/gapic/edgecontainer_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-edgecontainer-0.5.1/tests/unit/gapic/edgecontainer_v1/test_edge_container.py` & `google-cloud-edgecontainer-0.5.2/tests/unit/gapic/edgecontainer_v1/test_edge_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -1130,17 +1130,19 @@
                     resources.Cluster(),
                     resources.Cluster(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_clusters(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2748,17 +2750,19 @@
                     resources.NodePool(),
                     resources.NodePool(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_node_pools(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4120,17 +4124,19 @@
                     resources.Machine(),
                     resources.Machine(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_machines(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4806,17 +4812,19 @@
                     resources.VpnConnection(),
                     resources.VpnConnection(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_vpn_connections(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

