# Comparing `tmp/google-cloud-bigquery-analyticshub-0.4.0.tar.gz` & `tmp/google-cloud-bigquery-analyticshub-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-bigquery-analyticshub-0.4.0.tar", last modified: Tue Jun 20 13:26:56 2023, max compression
+gzip compressed data, was "google-cloud-bigquery-analyticshub-0.4.1.tar", last modified: Wed Jul  5 15:50:53 2023, max compression
```

## Comparing `google-cloud-bigquery-analyticshub-0.4.0.tar` & `google-cloud-bigquery-analyticshub-0.4.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.120734 google-cloud-bigquery-analyticshub-0.4.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4933 2023-06-20 13:26:56.120734 google-cloud-bigquery-analyticshub-0.4.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3997 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.108733 google-cloud-bigquery-analyticshub-0.4.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.112733 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.112733 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub/
--rw-rw-r--   0 root         (0)     1003     2347 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.112733 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/
--rw-rw-r--   0 root         (0)     1003     2171 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4388 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.112733 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.116734 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    81556 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    93411 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/client.py
--rw-rw-r--   0 root         (0)     1003    16387 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.116734 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/
--rw-rw-r--   0 root         (0)     1003     1246 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12705 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    28714 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    29292 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.116734 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/types/
--rw-rw-r--   0 root         (0)     1003     1851 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    26368 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/types/analyticshub.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.116734 google-cloud-bigquery-analyticshub-0.4.0/google_cloud_bigquery_analyticshub.egg-info/
--rw-r--r--   0 root         (0)     1003     4933 2023-06-20 13:26:56.000000 google-cloud-bigquery-analyticshub-0.4.0/google_cloud_bigquery_analyticshub.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1874 2023-06-20 13:26:56.000000 google-cloud-bigquery-analyticshub-0.4.0/google_cloud_bigquery_analyticshub.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-20 13:26:56.000000 google-cloud-bigquery-analyticshub-0.4.0/google_cloud_bigquery_analyticshub.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-06-20 13:26:56.000000 google-cloud-bigquery-analyticshub-0.4.0/google_cloud_bigquery_analyticshub.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-20 13:26:56.000000 google-cloud-bigquery-analyticshub-0.4.0/google_cloud_bigquery_analyticshub.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-06-20 13:26:56.000000 google-cloud-bigquery-analyticshub-0.4.0/google_cloud_bigquery_analyticshub.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-20 13:26:56.000000 google-cloud-bigquery-analyticshub-0.4.0/google_cloud_bigquery_analyticshub.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-06-20 13:26:56.120734 google-cloud-bigquery-analyticshub-0.4.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3021 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.116734 google-cloud-bigquery-analyticshub-0.4.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.116734 google-cloud-bigquery-analyticshub-0.4.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.116734 google-cloud-bigquery-analyticshub-0.4.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.120734 google-cloud-bigquery-analyticshub-0.4.0/tests/unit/gapic/bigquery_analyticshub_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/tests/unit/gapic/bigquery_analyticshub_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   206173 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/tests/unit/gapic/bigquery_analyticshub_v1/test_analytics_hub_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:53.726367 google-cloud-bigquery-analyticshub-0.4.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4933 2023-07-05 15:50:53.726367 google-cloud-bigquery-analyticshub-0.4.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3997 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:53.714366 google-cloud-bigquery-analyticshub-0.4.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:53.714366 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:53.718366 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub/
+-rw-rw-r--   0 root         (0)     1003     2347 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:53.718366 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/
+-rw-rw-r--   0 root         (0)     1003     2171 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4388 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:53.718366 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:53.718366 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    81592 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    93411 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16387 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:53.722367 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1246 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12705 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    28714 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    29292 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:53.722367 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1851 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26368 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/types/analyticshub.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:53.722367 google-cloud-bigquery-analyticshub-0.4.1/google_cloud_bigquery_analyticshub.egg-info/
+-rw-r--r--   0 root         (0)     1003     4933 2023-07-05 15:50:53.000000 google-cloud-bigquery-analyticshub-0.4.1/google_cloud_bigquery_analyticshub.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1874 2023-07-05 15:50:53.000000 google-cloud-bigquery-analyticshub-0.4.1/google_cloud_bigquery_analyticshub.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:53.000000 google-cloud-bigquery-analyticshub-0.4.1/google_cloud_bigquery_analyticshub.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:50:53.000000 google-cloud-bigquery-analyticshub-0.4.1/google_cloud_bigquery_analyticshub.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:53.000000 google-cloud-bigquery-analyticshub-0.4.1/google_cloud_bigquery_analyticshub.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:50:53.000000 google-cloud-bigquery-analyticshub-0.4.1/google_cloud_bigquery_analyticshub.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:50:53.000000 google-cloud-bigquery-analyticshub-0.4.1/google_cloud_bigquery_analyticshub.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:50:53.726367 google-cloud-bigquery-analyticshub-0.4.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3021 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:53.722367 google-cloud-bigquery-analyticshub-0.4.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:53.722367 google-cloud-bigquery-analyticshub-0.4.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:53.722367 google-cloud-bigquery-analyticshub-0.4.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:53.726367 google-cloud-bigquery-analyticshub-0.4.1/tests/unit/gapic/bigquery_analyticshub_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/tests/unit/gapic/bigquery_analyticshub_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   206386 2023-07-05 15:46:58.000000 google-cloud-bigquery-analyticshub-0.4.1/tests/unit/gapic/bigquery_analyticshub_v1/test_analytics_hub_service.py
```

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/LICENSE` & `google-cloud-bigquery-analyticshub-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/MANIFEST.in` & `google-cloud-bigquery-analyticshub-0.4.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/PKG-INFO` & `google-cloud-bigquery-analyticshub-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-analyticshub
-Version: 0.4.0
+Version: 0.4.1
 Summary: Google Cloud Bigquery Analyticshub API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/README.rst` & `google-cloud-bigquery-analyticshub-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub/__init__.py` & `google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub/gapic_version.py` & `google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub/gapic_version.py`

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
-__version__ = "0.4.0"  # {x-release-please-version}
+__version__ = "0.4.1"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/__init__.py` & `google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/gapic_metadata.json` & `google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/gapic_version.py` & `google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/gapic_version.py`

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
-__version__ = "0.4.0"  # {x-release-please-version}
+__version__ = "0.4.1"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/__init__.py` & `google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/__init__.py` & `google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/async_client.py` & `google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1925,15 +1925,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "AnalyticsHubServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/client.py` & `google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/pagers.py` & `google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/__init__.py` & `google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/base.py` & `google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/grpc.py` & `google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/grpc_asyncio.py` & `google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/types/__init__.py` & `google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/types/analyticshub.py` & `google-cloud-bigquery-analyticshub-0.4.1/google/cloud/bigquery_analyticshub_v1/types/analyticshub.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/google_cloud_bigquery_analyticshub.egg-info/PKG-INFO` & `google-cloud-bigquery-analyticshub-0.4.1/google_cloud_bigquery_analyticshub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-analyticshub
-Version: 0.4.0
+Version: 0.4.1
 Summary: Google Cloud Bigquery Analyticshub API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/google_cloud_bigquery_analyticshub.egg-info/SOURCES.txt` & `google-cloud-bigquery-analyticshub-0.4.1/google_cloud_bigquery_analyticshub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/setup.py` & `google-cloud-bigquery-analyticshub-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/tests/__init__.py` & `google-cloud-bigquery-analyticshub-0.4.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/tests/unit/__init__.py` & `google-cloud-bigquery-analyticshub-0.4.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/tests/unit/gapic/__init__.py` & `google-cloud-bigquery-analyticshub-0.4.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/tests/unit/gapic/bigquery_analyticshub_v1/__init__.py` & `google-cloud-bigquery-analyticshub-0.4.1/tests/unit/gapic/bigquery_analyticshub_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.4.0/tests/unit/gapic/bigquery_analyticshub_v1/test_analytics_hub_service.py` & `google-cloud-bigquery-analyticshub-0.4.1/tests/unit/gapic/bigquery_analyticshub_v1/test_analytics_hub_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1142,17 +1142,19 @@
                     analyticshub.DataExchange(),
                     analyticshub.DataExchange(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_data_exchanges(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1585,17 +1587,19 @@
                     analyticshub.DataExchange(),
                     analyticshub.DataExchange(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_org_data_exchanges(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3069,17 +3073,19 @@
                     analyticshub.Listing(),
                     analyticshub.Listing(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_listings(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3107,17 +3113,14 @@
             description="description_value",
             primary_contact="primary_contact_value",
             documentation="documentation_value",
             state=analyticshub.Listing.State.ACTIVE,
             icon=b"icon_blob",
             categories=[analyticshub.Listing.Category.CATEGORY_OTHERS],
             request_access="request_access_value",
-            bigquery_dataset=analyticshub.Listing.BigQueryDatasetSource(
-                dataset="dataset_value"
-            ),
         )
         response = client.get_listing(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == analyticshub.GetListingRequest()
@@ -3374,17 +3377,14 @@
             description="description_value",
             primary_contact="primary_contact_value",
             documentation="documentation_value",
             state=analyticshub.Listing.State.ACTIVE,
             icon=b"icon_blob",
             categories=[analyticshub.Listing.Category.CATEGORY_OTHERS],
             request_access="request_access_value",
-            bigquery_dataset=analyticshub.Listing.BigQueryDatasetSource(
-                dataset="dataset_value"
-            ),
         )
         response = client.create_listing(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == analyticshub.CreateListingRequest()
@@ -3675,17 +3675,14 @@
             description="description_value",
             primary_contact="primary_contact_value",
             documentation="documentation_value",
             state=analyticshub.Listing.State.ACTIVE,
             icon=b"icon_blob",
             categories=[analyticshub.Listing.Category.CATEGORY_OTHERS],
             request_access="request_access_value",
-            bigquery_dataset=analyticshub.Listing.BigQueryDatasetSource(
-                dataset="dataset_value"
-            ),
         )
         response = client.update_listing(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == analyticshub.UpdateListingRequest()
```

