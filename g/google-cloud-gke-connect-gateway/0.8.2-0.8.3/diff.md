# Comparing `tmp/google-cloud-gke-connect-gateway-0.8.2.tar.gz` & `tmp/google-cloud-gke-connect-gateway-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-gke-connect-gateway-0.8.2.tar", last modified: Mon Mar 27 15:00:15 2023, max compression
+gzip compressed data, was "google-cloud-gke-connect-gateway-0.8.3.tar", last modified: Wed Jul  5 15:53:18 2023, max compression
```

## Comparing `google-cloud-gke-connect-gateway-0.8.2.tar` & `google-cloud-gke-connect-gateway-0.8.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:15.493787 google-cloud-gke-connect-gateway-0.8.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5044 2023-03-27 15:00:15.493787 google-cloud-gke-connect-gateway-0.8.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4105 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:15.489785 google-cloud-gke-connect-gateway-0.8.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:15.489785 google-cloud-gke-connect-gateway-0.8.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:15.489785 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:15.489785 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway/
--rw-rw-r--   0 root         (0)     1003     1037 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:15.489785 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/
--rw-rw-r--   0 root         (0)     1003      892 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1781 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:15.489785 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:15.489785 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/
--rw-rw-r--   0 root         (0)     1003      769 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    42223 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    50395 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:15.493787 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/transports/
--rw-rw-r--   0 root         (0)     1003     1193 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7646 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    16399 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16737 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:15.493787 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003      614 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003      782 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/types/gateway.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:15.493787 google-cloud-gke-connect-gateway-0.8.2/google_cloud_gke_connect_gateway.egg-info/
--rw-r--r--   0 root         (0)     1003     5044 2023-03-27 15:00:15.000000 google-cloud-gke-connect-gateway-0.8.2/google_cloud_gke_connect_gateway.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1729 2023-03-27 15:00:15.000000 google-cloud-gke-connect-gateway-0.8.2/google_cloud_gke_connect_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:00:15.000000 google-cloud-gke-connect-gateway-0.8.2/google_cloud_gke_connect_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       44 2023-03-27 15:00:15.000000 google-cloud-gke-connect-gateway-0.8.2/google_cloud_gke_connect_gateway.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:00:15.000000 google-cloud-gke-connect-gateway-0.8.2/google_cloud_gke_connect_gateway.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 15:00:15.000000 google-cloud-gke-connect-gateway-0.8.2/google_cloud_gke_connect_gateway.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:00:15.000000 google-cloud-gke-connect-gateway-0.8.2/google_cloud_gke_connect_gateway.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:00:15.493787 google-cloud-gke-connect-gateway-0.8.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3001 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:15.493787 google-cloud-gke-connect-gateway-0.8.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:15.493787 google-cloud-gke-connect-gateway-0.8.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:15.493787 google-cloud-gke-connect-gateway-0.8.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:15.493787 google-cloud-gke-connect-gateway-0.8.2/tests/unit/gapic/gateway_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/tests/unit/gapic/gateway_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    70907 2023-03-27 14:57:40.000000 google-cloud-gke-connect-gateway-0.8.2/tests/unit/gapic/gateway_v1beta1/test_gateway_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:18.033250 google-cloud-gke-connect-gateway-0.8.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5001 2023-07-05 15:53:18.033250 google-cloud-gke-connect-gateway-0.8.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4069 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:18.025250 google-cloud-gke-connect-gateway-0.8.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:18.025250 google-cloud-gke-connect-gateway-0.8.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:18.025250 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:18.025250 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway/
+-rw-rw-r--   0 root         (0)     1003     1037 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:18.029250 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      892 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1781 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:18.029250 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:18.029250 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/
+-rw-rw-r--   0 root         (0)     1003      769 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    42254 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    50395 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:18.029250 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1193 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7646 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    16399 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16737 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:18.029250 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003      614 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003      782 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/types/gateway.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:18.029250 google-cloud-gke-connect-gateway-0.8.3/google_cloud_gke_connect_gateway.egg-info/
+-rw-r--r--   0 root         (0)     1003     5001 2023-07-05 15:53:17.000000 google-cloud-gke-connect-gateway-0.8.3/google_cloud_gke_connect_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1729 2023-07-05 15:53:17.000000 google-cloud-gke-connect-gateway-0.8.3/google_cloud_gke_connect_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:17.000000 google-cloud-gke-connect-gateway-0.8.3/google_cloud_gke_connect_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       44 2023-07-05 15:53:17.000000 google-cloud-gke-connect-gateway-0.8.3/google_cloud_gke_connect_gateway.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:17.000000 google-cloud-gke-connect-gateway-0.8.3/google_cloud_gke_connect_gateway.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:53:17.000000 google-cloud-gke-connect-gateway-0.8.3/google_cloud_gke_connect_gateway.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:53:17.000000 google-cloud-gke-connect-gateway-0.8.3/google_cloud_gke_connect_gateway.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:53:18.033250 google-cloud-gke-connect-gateway-0.8.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2994 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:18.029250 google-cloud-gke-connect-gateway-0.8.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:18.033250 google-cloud-gke-connect-gateway-0.8.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:18.033250 google-cloud-gke-connect-gateway-0.8.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:18.033250 google-cloud-gke-connect-gateway-0.8.3/tests/unit/gapic/gateway_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/tests/unit/gapic/gateway_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    70907 2023-07-05 15:46:59.000000 google-cloud-gke-connect-gateway-0.8.3/tests/unit/gapic/gateway_v1beta1/test_gateway_service.py
```

### Comparing `google-cloud-gke-connect-gateway-0.8.2/LICENSE` & `google-cloud-gke-connect-gateway-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-connect-gateway-0.8.2/MANIFEST.in` & `google-cloud-gke-connect-gateway-0.8.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-connect-gateway-0.8.2/PKG-INFO` & `google-cloud-gke-connect-gateway-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-gke-connect-gateway
-Version: 0.8.2
+Version: 0.8.3
 Summary: Google Cloud Gke Connect Gateway API client library
-Home-page: https://github.com/googleapis/python-gke-connect-gateway
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
 
-Python Client for GKE Connect Gateway API
-=========================================
+Python Client for GKE Connect Gateway
+=====================================
 
 |preview| |pypi| |versions|
 
-`GKE Connect Gateway API`_: builds on the power of fleets to let Anthos users connect to and run commands against registered Anthos clusters in a simple, consistent, and secured way, whether the clusters are on Google Cloud, other public clouds, or on premises, and makes it easier to automate DevOps processes across all your clusters.
+`GKE Connect Gateway`_: builds on the power of fleets to let Anthos users connect to and run commands against registered Anthos clusters in a simple, consistent, and secured way, whether the clusters are on Google Cloud, other public clouds, or on premises, and makes it easier to automate DevOps processes across all your clusters.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-gke-connect-gateway.svg
    :target: https://pypi.org/project/google-cloud-gke-connect-gateway/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-gke-connect-gateway.svg
    :target: https://pypi.org/project/google-cloud-gke-connect-gateway/
-.. _GKE Connect Gateway API: https://cloud.google.com/anthos/multicluster-management/gateway
+.. _GKE Connect Gateway: https://cloud.google.com/anthos/multicluster-management/gateway
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/connectgateway/latest
 .. _Product Documentation:  https://cloud.google.com/anthos/multicluster-management/gateway
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the GKE Connect Gateway API.`_
+3. `Enable the GKE Connect Gateway.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the GKE Connect Gateway API.:  https://cloud.google.com/anthos/multicluster-management/gateway
+.. _Enable the GKE Connect Gateway.:  https://cloud.google.com/anthos/multicluster-management/gateway
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-gke-connect-gateway
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for GKE Connect Gateway API
+-  Read the `Client Library Documentation`_ for GKE Connect Gateway
    to see other available methods on the client.
--  Read the `GKE Connect Gateway API Product documentation`_ to learn
+-  Read the `GKE Connect Gateway Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _GKE Connect Gateway API Product documentation:  https://cloud.google.com/anthos/multicluster-management/gateway
+.. _GKE Connect Gateway Product documentation:  https://cloud.google.com/anthos/multicluster-management/gateway
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-gke-connect-gateway-0.8.2/README.rst` & `google-cloud-gke-connect-gateway-0.8.3/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for GKE Connect Gateway API
-=========================================
+Python Client for GKE Connect Gateway
+=====================================
 
 |preview| |pypi| |versions|
 
-`GKE Connect Gateway API`_: builds on the power of fleets to let Anthos users connect to and run commands against registered Anthos clusters in a simple, consistent, and secured way, whether the clusters are on Google Cloud, other public clouds, or on premises, and makes it easier to automate DevOps processes across all your clusters.
+`GKE Connect Gateway`_: builds on the power of fleets to let Anthos users connect to and run commands against registered Anthos clusters in a simple, consistent, and secured way, whether the clusters are on Google Cloud, other public clouds, or on premises, and makes it easier to automate DevOps processes across all your clusters.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-gke-connect-gateway.svg
    :target: https://pypi.org/project/google-cloud-gke-connect-gateway/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-gke-connect-gateway.svg
    :target: https://pypi.org/project/google-cloud-gke-connect-gateway/
-.. _GKE Connect Gateway API: https://cloud.google.com/anthos/multicluster-management/gateway
+.. _GKE Connect Gateway: https://cloud.google.com/anthos/multicluster-management/gateway
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/connectgateway/latest
 .. _Product Documentation:  https://cloud.google.com/anthos/multicluster-management/gateway
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the GKE Connect Gateway API.`_
+3. `Enable the GKE Connect Gateway.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the GKE Connect Gateway API.:  https://cloud.google.com/anthos/multicluster-management/gateway
+.. _Enable the GKE Connect Gateway.:  https://cloud.google.com/anthos/multicluster-management/gateway
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-gke-connect-gateway
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for GKE Connect Gateway API
+-  Read the `Client Library Documentation`_ for GKE Connect Gateway
    to see other available methods on the client.
--  Read the `GKE Connect Gateway API Product documentation`_ to learn
+-  Read the `GKE Connect Gateway Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _GKE Connect Gateway API Product documentation:  https://cloud.google.com/anthos/multicluster-management/gateway
+.. _GKE Connect Gateway Product documentation:  https://cloud.google.com/anthos/multicluster-management/gateway
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway/__init__.py` & `google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway/gapic_version.py` & `google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway/gapic_version.py`

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
-__version__ = "0.8.2"  # {x-release-please-version}
+__version__ = "0.8.3"  # {x-release-please-version}
```

### Comparing `google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/__init__.py` & `google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/gapic_metadata.json` & `google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/gapic_version.py` & `google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/gapic_version.py`

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
-__version__ = "0.8.2"  # {x-release-please-version}
+__version__ = "0.8.3"  # {x-release-please-version}
```

### Comparing `google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/services/__init__.py` & `google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/__init__.py` & `google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/async_client.py` & `google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1059,15 +1059,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "GatewayServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/client.py` & `google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/transports/__init__.py` & `google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/transports/base.py` & `google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/transports/grpc.py` & `google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/transports/grpc_asyncio.py` & `google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/services/gateway_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/types/__init__.py` & `google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-connect-gateway-0.8.2/google/cloud/gkeconnect/gateway_v1beta1/types/gateway.py` & `google-cloud-gke-connect-gateway-0.8.3/google/cloud/gkeconnect/gateway_v1beta1/types/gateway.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-connect-gateway-0.8.2/google_cloud_gke_connect_gateway.egg-info/PKG-INFO` & `google-cloud-gke-connect-gateway-0.8.3/google_cloud_gke_connect_gateway.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-gke-connect-gateway
-Version: 0.8.2
+Version: 0.8.3
 Summary: Google Cloud Gke Connect Gateway API client library
-Home-page: https://github.com/googleapis/python-gke-connect-gateway
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
 
-Python Client for GKE Connect Gateway API
-=========================================
+Python Client for GKE Connect Gateway
+=====================================
 
 |preview| |pypi| |versions|
 
-`GKE Connect Gateway API`_: builds on the power of fleets to let Anthos users connect to and run commands against registered Anthos clusters in a simple, consistent, and secured way, whether the clusters are on Google Cloud, other public clouds, or on premises, and makes it easier to automate DevOps processes across all your clusters.
+`GKE Connect Gateway`_: builds on the power of fleets to let Anthos users connect to and run commands against registered Anthos clusters in a simple, consistent, and secured way, whether the clusters are on Google Cloud, other public clouds, or on premises, and makes it easier to automate DevOps processes across all your clusters.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-gke-connect-gateway.svg
    :target: https://pypi.org/project/google-cloud-gke-connect-gateway/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-gke-connect-gateway.svg
    :target: https://pypi.org/project/google-cloud-gke-connect-gateway/
-.. _GKE Connect Gateway API: https://cloud.google.com/anthos/multicluster-management/gateway
+.. _GKE Connect Gateway: https://cloud.google.com/anthos/multicluster-management/gateway
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/connectgateway/latest
 .. _Product Documentation:  https://cloud.google.com/anthos/multicluster-management/gateway
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the GKE Connect Gateway API.`_
+3. `Enable the GKE Connect Gateway.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the GKE Connect Gateway API.:  https://cloud.google.com/anthos/multicluster-management/gateway
+.. _Enable the GKE Connect Gateway.:  https://cloud.google.com/anthos/multicluster-management/gateway
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-gke-connect-gateway
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for GKE Connect Gateway API
+-  Read the `Client Library Documentation`_ for GKE Connect Gateway
    to see other available methods on the client.
--  Read the `GKE Connect Gateway API Product documentation`_ to learn
+-  Read the `GKE Connect Gateway Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _GKE Connect Gateway API Product documentation:  https://cloud.google.com/anthos/multicluster-management/gateway
+.. _GKE Connect Gateway Product documentation:  https://cloud.google.com/anthos/multicluster-management/gateway
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-gke-connect-gateway-0.8.2/google_cloud_gke_connect_gateway.egg-info/SOURCES.txt` & `google-cloud-gke-connect-gateway-0.8.3/google_cloud_gke_connect_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-connect-gateway-0.8.2/setup.py` & `google-cloud-gke-connect-gateway-0.8.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-gke-connect-gateway"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-gke-connect-gateway-0.8.2/tests/__init__.py` & `google-cloud-gke-connect-gateway-0.8.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-connect-gateway-0.8.2/tests/unit/__init__.py` & `google-cloud-gke-connect-gateway-0.8.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-connect-gateway-0.8.2/tests/unit/gapic/__init__.py` & `google-cloud-gke-connect-gateway-0.8.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-connect-gateway-0.8.2/tests/unit/gapic/gateway_v1beta1/__init__.py` & `google-cloud-gke-connect-gateway-0.8.3/tests/unit/gapic/gateway_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-connect-gateway-0.8.2/tests/unit/gapic/gateway_v1beta1/test_gateway_service.py` & `google-cloud-gke-connect-gateway-0.8.3/tests/unit/gapic/gateway_v1beta1/test_gateway_service.py`

 * *Files identical despite different names*

