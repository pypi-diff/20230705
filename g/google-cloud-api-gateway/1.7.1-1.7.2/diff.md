# Comparing `tmp/google-cloud-api-gateway-1.7.1.tar.gz` & `tmp/google-cloud-api-gateway-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-api-gateway-1.7.1.tar", last modified: Mon Mar 27 14:52:50 2023, max compression
+gzip compressed data, was "google-cloud-api-gateway-1.7.2.tar", last modified: Wed Jul  5 15:50:02 2023, max compression
```

## Comparing `google-cloud-api-gateway-1.7.1.tar` & `google-cloud-api-gateway-1.7.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:50.988873 google-cloud-api-gateway-1.7.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4875 2023-03-27 14:52:50.988873 google-cloud-api-gateway-1.7.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3947 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:50.976874 google-cloud-api-gateway-1.7.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:50.976874 google-cloud-api-gateway-1.7.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:50.980874 google-cloud-api-gateway-1.7.1/google/cloud/apigateway/
--rw-rw-r--   0 root         (0)     1003     2135 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/google/cloud/apigateway/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/google/cloud/apigateway/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       85 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/google/cloud/apigateway/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:50.980874 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/
--rw-rw-r--   0 root         (0)     1003     1994 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     6047 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       85 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:50.980874 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:50.980874 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/api_gateway_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/api_gateway_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    87212 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/api_gateway_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    97169 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/api_gateway_service/client.py
--rw-rw-r--   0 root         (0)     1003    15572 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/api_gateway_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:50.984873 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/api_gateway_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/api_gateway_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    15736 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/api_gateway_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    27727 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/api_gateway_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    28401 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/api_gateway_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    85599 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/api_gateway_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:50.984873 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/types/
--rw-rw-r--   0 root         (0)     1003     1695 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    30282 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/types/apigateway.py
--rw-rw-r--   0 root         (0)     1003      769 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/types/apigateway_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:50.984873 google-cloud-api-gateway-1.7.1/google_cloud_api_gateway.egg-info/
--rw-r--r--   0 root         (0)     1003     4875 2023-03-27 14:52:50.000000 google-cloud-api-gateway-1.7.1/google_cloud_api_gateway.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1694 2023-03-27 14:52:50.000000 google-cloud-api-gateway-1.7.1/google_cloud_api_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:52:50.000000 google-cloud-api-gateway-1.7.1/google_cloud_api_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:52:50.000000 google-cloud-api-gateway-1.7.1/google_cloud_api_gateway.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:52:50.000000 google-cloud-api-gateway-1.7.1/google_cloud_api_gateway.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 14:52:50.000000 google-cloud-api-gateway-1.7.1/google_cloud_api_gateway.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:52:50.000000 google-cloud-api-gateway-1.7.1/google_cloud_api_gateway.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 14:52:50.988873 google-cloud-api-gateway-1.7.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2936 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:50.984873 google-cloud-api-gateway-1.7.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:50.984873 google-cloud-api-gateway-1.7.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:50.984873 google-cloud-api-gateway-1.7.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:50.984873 google-cloud-api-gateway-1.7.1/tests/unit/gapic/apigateway_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/tests/unit/gapic/apigateway_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   369298 2023-03-27 14:50:14.000000 google-cloud-api-gateway-1.7.1/tests/unit/gapic/apigateway_v1/test_api_gateway_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:02.093930 google-cloud-api-gateway-1.7.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4840 2023-07-05 15:50:02.093930 google-cloud-api-gateway-1.7.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3911 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:02.085929 google-cloud-api-gateway-1.7.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:02.085929 google-cloud-api-gateway-1.7.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:02.089929 google-cloud-api-gateway-1.7.2/google/cloud/apigateway/
+-rw-rw-r--   0 root         (0)     1003     2135 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/google/cloud/apigateway/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/google/cloud/apigateway/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       85 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/google/cloud/apigateway/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:02.089929 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/
+-rw-rw-r--   0 root         (0)     1003     1994 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6047 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       85 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:02.089929 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:02.089929 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/api_gateway_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/api_gateway_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    87246 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/api_gateway_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    97169 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/api_gateway_service/client.py
+-rw-rw-r--   0 root         (0)     1003    15572 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/api_gateway_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:02.089929 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/api_gateway_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/api_gateway_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15736 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/api_gateway_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    27727 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/api_gateway_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    28401 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/api_gateway_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    85599 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/api_gateway_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:02.093930 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1695 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    30282 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/types/apigateway.py
+-rw-rw-r--   0 root         (0)     1003      769 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/types/apigateway_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:02.093930 google-cloud-api-gateway-1.7.2/google_cloud_api_gateway.egg-info/
+-rw-r--r--   0 root         (0)     1003     4840 2023-07-05 15:50:02.000000 google-cloud-api-gateway-1.7.2/google_cloud_api_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1694 2023-07-05 15:50:02.000000 google-cloud-api-gateway-1.7.2/google_cloud_api_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:02.000000 google-cloud-api-gateway-1.7.2/google_cloud_api_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:50:02.000000 google-cloud-api-gateway-1.7.2/google_cloud_api_gateway.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:02.000000 google-cloud-api-gateway-1.7.2/google_cloud_api_gateway.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:50:02.000000 google-cloud-api-gateway-1.7.2/google_cloud_api_gateway.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:50:02.000000 google-cloud-api-gateway-1.7.2/google_cloud_api_gateway.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:50:02.093930 google-cloud-api-gateway-1.7.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2937 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:02.093930 google-cloud-api-gateway-1.7.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:02.093930 google-cloud-api-gateway-1.7.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:02.093930 google-cloud-api-gateway-1.7.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:02.093930 google-cloud-api-gateway-1.7.2/tests/unit/gapic/apigateway_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/tests/unit/gapic/apigateway_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   369895 2023-07-05 15:46:58.000000 google-cloud-api-gateway-1.7.2/tests/unit/gapic/apigateway_v1/test_api_gateway_service.py
```

### Comparing `google-cloud-api-gateway-1.7.1/LICENSE` & `google-cloud-api-gateway-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/MANIFEST.in` & `google-cloud-api-gateway-1.7.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/PKG-INFO` & `google-cloud-api-gateway-1.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-api-gateway
-Version: 1.7.1
+Version: 1.7.2
 Summary: Google Cloud Api Gateway API client library
-Home-page: https://github.com/googleapis/python-api-gateway
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
 
-Python Client for API Gateway API
-=================================
+Python Client for API Gateway
+=============================
 
 |stable| |pypi| |versions|
 
-`API Gateway API`_: enables you to provide secure access to your backend services through a well-defined REST API that is consistent across all of your services, regardless of the service implementation. Clients consume your REST APIS to implement standalone apps for a mobile device or tablet, through apps running in a browser, or through any other type of app that can make a request to an HTTP endpoint.
+`API Gateway`_: enables you to provide secure access to your backend services through a well-defined REST API that is consistent across all of your services, regardless of the service implementation. Clients consume your REST APIS to implement standalone apps for a mobile device or tablet, through apps running in a browser, or through any other type of app that can make a request to an HTTP endpoint.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-api-gateway.svg
    :target: https://pypi.org/project/google-cloud-api-gateway/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-api-gateway.svg
    :target: https://pypi.org/project/google-cloud-api-gateway/
-.. _API Gateway API: https://cloud.google.com/api-gateway
+.. _API Gateway: https://cloud.google.com/api-gateway
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/apigateway/latest
 .. _Product Documentation:  https://cloud.google.com/api-gateway
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the API Gateway API.`_
+3. `Enable the API Gateway.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the API Gateway API.:  https://cloud.google.com/api-gateway
+.. _Enable the API Gateway.:  https://cloud.google.com/api-gateway
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-api-gateway
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for API Gateway API
+-  Read the `Client Library Documentation`_ for API Gateway
    to see other available methods on the client.
--  Read the `API Gateway API Product documentation`_ to learn
+-  Read the `API Gateway Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _API Gateway API Product documentation:  https://cloud.google.com/api-gateway
+.. _API Gateway Product documentation:  https://cloud.google.com/api-gateway
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-api-gateway-1.7.1/README.rst` & `google-cloud-api-gateway-1.7.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for API Gateway API
-=================================
+Python Client for API Gateway
+=============================
 
 |stable| |pypi| |versions|
 
-`API Gateway API`_: enables you to provide secure access to your backend services through a well-defined REST API that is consistent across all of your services, regardless of the service implementation. Clients consume your REST APIS to implement standalone apps for a mobile device or tablet, through apps running in a browser, or through any other type of app that can make a request to an HTTP endpoint.
+`API Gateway`_: enables you to provide secure access to your backend services through a well-defined REST API that is consistent across all of your services, regardless of the service implementation. Clients consume your REST APIS to implement standalone apps for a mobile device or tablet, through apps running in a browser, or through any other type of app that can make a request to an HTTP endpoint.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-api-gateway.svg
    :target: https://pypi.org/project/google-cloud-api-gateway/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-api-gateway.svg
    :target: https://pypi.org/project/google-cloud-api-gateway/
-.. _API Gateway API: https://cloud.google.com/api-gateway
+.. _API Gateway: https://cloud.google.com/api-gateway
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/apigateway/latest
 .. _Product Documentation:  https://cloud.google.com/api-gateway
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the API Gateway API.`_
+3. `Enable the API Gateway.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the API Gateway API.:  https://cloud.google.com/api-gateway
+.. _Enable the API Gateway.:  https://cloud.google.com/api-gateway
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-api-gateway
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for API Gateway API
+-  Read the `Client Library Documentation`_ for API Gateway
    to see other available methods on the client.
--  Read the `API Gateway API Product documentation`_ to learn
+-  Read the `API Gateway Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _API Gateway API Product documentation:  https://cloud.google.com/api-gateway
+.. _API Gateway Product documentation:  https://cloud.google.com/api-gateway
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-api-gateway-1.7.1/google/cloud/apigateway/__init__.py` & `google-cloud-api-gateway-1.7.2/google/cloud/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/google/cloud/apigateway/gapic_version.py` & `google-cloud-api-gateway-1.7.2/google/cloud/apigateway/gapic_version.py`

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

### Comparing `google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/__init__.py` & `google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/gapic_metadata.json` & `google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/gapic_version.py` & `google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/gapic_version.py`

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

### Comparing `google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/__init__.py` & `google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/api_gateway_service/__init__.py` & `google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/api_gateway_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/api_gateway_service/async_client.py` & `google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/api_gateway_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2159,15 +2159,15 @@
             empty_pb2.Empty,
             metadata_type=apigateway.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ApiGatewayServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/api_gateway_service/client.py` & `google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/api_gateway_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/api_gateway_service/pagers.py` & `google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/api_gateway_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/api_gateway_service/transports/__init__.py` & `google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/api_gateway_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/api_gateway_service/transports/base.py` & `google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/api_gateway_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/api_gateway_service/transports/grpc.py` & `google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/api_gateway_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/api_gateway_service/transports/grpc_asyncio.py` & `google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/api_gateway_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/services/api_gateway_service/transports/rest.py` & `google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/services/api_gateway_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/types/__init__.py` & `google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/types/apigateway.py` & `google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/types/apigateway.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/google/cloud/apigateway_v1/types/apigateway_service.py` & `google-cloud-api-gateway-1.7.2/google/cloud/apigateway_v1/types/apigateway_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/google_cloud_api_gateway.egg-info/PKG-INFO` & `google-cloud-api-gateway-1.7.2/google_cloud_api_gateway.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-api-gateway
-Version: 1.7.1
+Version: 1.7.2
 Summary: Google Cloud Api Gateway API client library
-Home-page: https://github.com/googleapis/python-api-gateway
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
 
-Python Client for API Gateway API
-=================================
+Python Client for API Gateway
+=============================
 
 |stable| |pypi| |versions|
 
-`API Gateway API`_: enables you to provide secure access to your backend services through a well-defined REST API that is consistent across all of your services, regardless of the service implementation. Clients consume your REST APIS to implement standalone apps for a mobile device or tablet, through apps running in a browser, or through any other type of app that can make a request to an HTTP endpoint.
+`API Gateway`_: enables you to provide secure access to your backend services through a well-defined REST API that is consistent across all of your services, regardless of the service implementation. Clients consume your REST APIS to implement standalone apps for a mobile device or tablet, through apps running in a browser, or through any other type of app that can make a request to an HTTP endpoint.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-api-gateway.svg
    :target: https://pypi.org/project/google-cloud-api-gateway/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-api-gateway.svg
    :target: https://pypi.org/project/google-cloud-api-gateway/
-.. _API Gateway API: https://cloud.google.com/api-gateway
+.. _API Gateway: https://cloud.google.com/api-gateway
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/apigateway/latest
 .. _Product Documentation:  https://cloud.google.com/api-gateway
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the API Gateway API.`_
+3. `Enable the API Gateway.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the API Gateway API.:  https://cloud.google.com/api-gateway
+.. _Enable the API Gateway.:  https://cloud.google.com/api-gateway
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-api-gateway
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for API Gateway API
+-  Read the `Client Library Documentation`_ for API Gateway
    to see other available methods on the client.
--  Read the `API Gateway API Product documentation`_ to learn
+-  Read the `API Gateway Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _API Gateway API Product documentation:  https://cloud.google.com/api-gateway
+.. _API Gateway Product documentation:  https://cloud.google.com/api-gateway
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-api-gateway-1.7.1/google_cloud_api_gateway.egg-info/SOURCES.txt` & `google-cloud-api-gateway-1.7.2/google_cloud_api_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/setup.py` & `google-cloud-api-gateway-1.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-api-gateway"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-api-gateway-1.7.1/tests/__init__.py` & `google-cloud-api-gateway-1.7.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/tests/unit/__init__.py` & `google-cloud-api-gateway-1.7.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/tests/unit/gapic/__init__.py` & `google-cloud-api-gateway-1.7.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/tests/unit/gapic/apigateway_v1/__init__.py` & `google-cloud-api-gateway-1.7.2/tests/unit/gapic/apigateway_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-api-gateway-1.7.1/tests/unit/gapic/apigateway_v1/test_api_gateway_service.py` & `google-cloud-api-gateway-1.7.2/tests/unit/gapic/apigateway_v1/test_api_gateway_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1157,17 +1157,19 @@
                     apigateway.Gateway(),
                     apigateway.Gateway(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_gateways(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2533,17 +2535,19 @@
                     apigateway.Api(),
                     apigateway.Api(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_apis(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3905,17 +3909,19 @@
                     apigateway.ApiConfig(),
                     apigateway.ApiConfig(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_api_configs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

