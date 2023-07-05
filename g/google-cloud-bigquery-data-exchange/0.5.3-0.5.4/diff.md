# Comparing `tmp/google-cloud-bigquery-data-exchange-0.5.3.tar.gz` & `tmp/google-cloud-bigquery-data-exchange-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-bigquery-data-exchange-0.5.3.tar", last modified: Thu Apr 13 13:55:30 2023, max compression
+gzip compressed data, was "google-cloud-bigquery-data-exchange-0.5.4.tar", last modified: Wed Jul  5 15:51:01 2023, max compression
```

## Comparing `google-cloud-bigquery-data-exchange-0.5.3.tar` & `google-cloud-bigquery-data-exchange-0.5.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.909110 google-cloud-bigquery-data-exchange-0.5.3/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4952 2023-04-13 13:55:30.909110 google-cloud-bigquery-data-exchange-0.5.3/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4004 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.901104 google-cloud-bigquery-data-exchange-0.5.3/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.901104 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.905107 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange/
--rw-rw-r--   0 root         (0)     1003     2366 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       96 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.905107 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/
--rw-rw-r--   0 root         (0)     1003     2177 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4399 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       96 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.905107 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.905107 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    86164 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    97979 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/client.py
--rw-rw-r--   0 root         (0)     1003    16537 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.905107 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/
--rw-rw-r--   0 root         (0)     1003     1246 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    13308 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    30551 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    31129 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.905107 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1851 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    26457 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/types/dataexchange.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.909110 google-cloud-bigquery-data-exchange-0.5.3/google_cloud_bigquery_data_exchange.egg-info/
--rw-r--r--   0 root         (0)     1003     4952 2023-04-13 13:55:30.000000 google-cloud-bigquery-data-exchange-0.5.3/google_cloud_bigquery_data_exchange.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1986 2023-04-13 13:55:30.000000 google-cloud-bigquery-data-exchange-0.5.3/google_cloud_bigquery_data_exchange.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-13 13:55:30.000000 google-cloud-bigquery-data-exchange-0.5.3/google_cloud_bigquery_data_exchange.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-04-13 13:55:30.000000 google-cloud-bigquery-data-exchange-0.5.3/google_cloud_bigquery_data_exchange.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-13 13:55:30.000000 google-cloud-bigquery-data-exchange-0.5.3/google_cloud_bigquery_data_exchange.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-04-13 13:55:30.000000 google-cloud-bigquery-data-exchange-0.5.3/google_cloud_bigquery_data_exchange.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-13 13:55:30.000000 google-cloud-bigquery-data-exchange-0.5.3/google_cloud_bigquery_data_exchange.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-04-13 13:55:30.909110 google-cloud-bigquery-data-exchange-0.5.3/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3034 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.909110 google-cloud-bigquery-data-exchange-0.5.3/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.909110 google-cloud-bigquery-data-exchange-0.5.3/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.909110 google-cloud-bigquery-data-exchange-0.5.3/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.909110 google-cloud-bigquery-data-exchange-0.5.3/tests/unit/gapic/bigquery_data_exchange_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/tests/unit/gapic/bigquery_data_exchange_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   217243 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/tests/unit/gapic/bigquery_data_exchange_v1beta1/test_analytics_hub_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.902845 google-cloud-bigquery-data-exchange-0.5.4/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4906 2023-07-05 15:51:01.902845 google-cloud-bigquery-data-exchange-0.5.4/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3968 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.890844 google-cloud-bigquery-data-exchange-0.5.4/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.890844 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.894844 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange/
+-rw-rw-r--   0 root         (0)     1003     2366 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       96 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.894844 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     2177 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4399 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       96 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.894844 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.894844 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    86200 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    97979 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16537 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.898845 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1246 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13308 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    30551 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    31129 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.898845 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1851 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26457 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/types/dataexchange.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.898845 google-cloud-bigquery-data-exchange-0.5.4/google_cloud_bigquery_data_exchange.egg-info/
+-rw-r--r--   0 root         (0)     1003     4906 2023-07-05 15:51:01.000000 google-cloud-bigquery-data-exchange-0.5.4/google_cloud_bigquery_data_exchange.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1986 2023-07-05 15:51:01.000000 google-cloud-bigquery-data-exchange-0.5.4/google_cloud_bigquery_data_exchange.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:51:01.000000 google-cloud-bigquery-data-exchange-0.5.4/google_cloud_bigquery_data_exchange.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:51:01.000000 google-cloud-bigquery-data-exchange-0.5.4/google_cloud_bigquery_data_exchange.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:51:01.000000 google-cloud-bigquery-data-exchange-0.5.4/google_cloud_bigquery_data_exchange.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:51:01.000000 google-cloud-bigquery-data-exchange-0.5.4/google_cloud_bigquery_data_exchange.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:51:01.000000 google-cloud-bigquery-data-exchange-0.5.4/google_cloud_bigquery_data_exchange.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:51:01.902845 google-cloud-bigquery-data-exchange-0.5.4/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3024 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.898845 google-cloud-bigquery-data-exchange-0.5.4/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.898845 google-cloud-bigquery-data-exchange-0.5.4/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.898845 google-cloud-bigquery-data-exchange-0.5.4/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.898845 google-cloud-bigquery-data-exchange-0.5.4/tests/unit/gapic/bigquery_data_exchange_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/tests/unit/gapic/bigquery_data_exchange_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   217456 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/tests/unit/gapic/bigquery_data_exchange_v1beta1/test_analytics_hub_service.py
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/LICENSE` & `google-cloud-bigquery-data-exchange-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/MANIFEST.in` & `google-cloud-bigquery-data-exchange-0.5.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/PKG-INFO` & `google-cloud-bigquery-data-exchange-0.5.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-data-exchange
-Version: 0.5.3
+Version: 0.5.4
 Summary: Google Cloud Bigquery Data Exchange API client library
-Home-page: https://github.com/googleapis/python-bigquery-data-exchange
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
 
-Python Client for BigQuery Analytics Hub API
-============================================
+Python Client for BigQuery Analytics Hub
+========================================
 
 |preview| |pypi| |versions|
 
-`BigQuery Analytics Hub API`_: is a data exchange that allows you to efficiently and securely exchange data assets across organizations to address challenges of data reliability and cost.
+`BigQuery Analytics Hub`_: is a data exchange that allows you to efficiently and securely exchange data assets across organizations to address challenges of data reliability and cost.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-data-exchange.svg
    :target: https://pypi.org/project/google-cloud-bigquery-data-exchange/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-bigquery-data-exchange.svg
    :target: https://pypi.org/project/google-cloud-bigquery-data-exchange/
-.. _BigQuery Analytics Hub API: https://cloud.google.com/bigquery/docs/analytics-hub-introduction
+.. _BigQuery Analytics Hub: https://cloud.google.com/bigquery/docs/analytics-hub-introduction
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/analyticshub/latest
 .. _Product Documentation:  https://cloud.google.com/bigquery/docs/analytics-hub-introduction
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the BigQuery Analytics Hub API.`_
+3. `Enable the BigQuery Analytics Hub.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the BigQuery Analytics Hub API.:  https://cloud.google.com/bigquery/docs/analytics-hub-introduction
+.. _Enable the BigQuery Analytics Hub.:  https://cloud.google.com/bigquery/docs/analytics-hub-introduction
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-bigquery-data-exchange
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for BigQuery Analytics Hub API
+-  Read the `Client Library Documentation`_ for BigQuery Analytics Hub
    to see other available methods on the client.
--  Read the `BigQuery Analytics Hub API Product documentation`_ to learn
+-  Read the `BigQuery Analytics Hub Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _BigQuery Analytics Hub API Product documentation:  https://cloud.google.com/bigquery/docs/analytics-hub-introduction
+.. _BigQuery Analytics Hub Product documentation:  https://cloud.google.com/bigquery/docs/analytics-hub-introduction
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/README.rst` & `google-cloud-bigquery-data-exchange-0.5.4/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for BigQuery Analytics Hub API
-============================================
+Python Client for BigQuery Analytics Hub
+========================================
 
 |preview| |pypi| |versions|
 
-`BigQuery Analytics Hub API`_: is a data exchange that allows you to efficiently and securely exchange data assets across organizations to address challenges of data reliability and cost.
+`BigQuery Analytics Hub`_: is a data exchange that allows you to efficiently and securely exchange data assets across organizations to address challenges of data reliability and cost.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-data-exchange.svg
    :target: https://pypi.org/project/google-cloud-bigquery-data-exchange/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-bigquery-data-exchange.svg
    :target: https://pypi.org/project/google-cloud-bigquery-data-exchange/
-.. _BigQuery Analytics Hub API: https://cloud.google.com/bigquery/docs/analytics-hub-introduction
+.. _BigQuery Analytics Hub: https://cloud.google.com/bigquery/docs/analytics-hub-introduction
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/analyticshub/latest
 .. _Product Documentation:  https://cloud.google.com/bigquery/docs/analytics-hub-introduction
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the BigQuery Analytics Hub API.`_
+3. `Enable the BigQuery Analytics Hub.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the BigQuery Analytics Hub API.:  https://cloud.google.com/bigquery/docs/analytics-hub-introduction
+.. _Enable the BigQuery Analytics Hub.:  https://cloud.google.com/bigquery/docs/analytics-hub-introduction
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-bigquery-data-exchange
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for BigQuery Analytics Hub API
+-  Read the `Client Library Documentation`_ for BigQuery Analytics Hub
    to see other available methods on the client.
--  Read the `BigQuery Analytics Hub API Product documentation`_ to learn
+-  Read the `BigQuery Analytics Hub Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _BigQuery Analytics Hub API Product documentation:  https://cloud.google.com/bigquery/docs/analytics-hub-introduction
+.. _BigQuery Analytics Hub Product documentation:  https://cloud.google.com/bigquery/docs/analytics-hub-introduction
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange/gapic_version.py` & `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange/gapic_version.py`

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
-__version__ = "0.5.3"  # {x-release-please-version}
+__version__ = "0.5.4"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/gapic_metadata.json` & `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/gapic_version.py` & `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/gapic_version.py`

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
-__version__ = "0.5.3"  # {x-release-please-version}
+__version__ = "0.5.4"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/async_client.py` & `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2036,15 +2036,15 @@
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

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/client.py` & `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/pagers.py` & `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/base.py` & `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc.py` & `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc_asyncio.py` & `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/types/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/types/dataexchange.py` & `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/types/dataexchange.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/google_cloud_bigquery_data_exchange.egg-info/PKG-INFO` & `google-cloud-bigquery-data-exchange-0.5.4/google_cloud_bigquery_data_exchange.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-data-exchange
-Version: 0.5.3
+Version: 0.5.4
 Summary: Google Cloud Bigquery Data Exchange API client library
-Home-page: https://github.com/googleapis/python-bigquery-data-exchange
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
 
-Python Client for BigQuery Analytics Hub API
-============================================
+Python Client for BigQuery Analytics Hub
+========================================
 
 |preview| |pypi| |versions|
 
-`BigQuery Analytics Hub API`_: is a data exchange that allows you to efficiently and securely exchange data assets across organizations to address challenges of data reliability and cost.
+`BigQuery Analytics Hub`_: is a data exchange that allows you to efficiently and securely exchange data assets across organizations to address challenges of data reliability and cost.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-data-exchange.svg
    :target: https://pypi.org/project/google-cloud-bigquery-data-exchange/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-bigquery-data-exchange.svg
    :target: https://pypi.org/project/google-cloud-bigquery-data-exchange/
-.. _BigQuery Analytics Hub API: https://cloud.google.com/bigquery/docs/analytics-hub-introduction
+.. _BigQuery Analytics Hub: https://cloud.google.com/bigquery/docs/analytics-hub-introduction
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/analyticshub/latest
 .. _Product Documentation:  https://cloud.google.com/bigquery/docs/analytics-hub-introduction
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the BigQuery Analytics Hub API.`_
+3. `Enable the BigQuery Analytics Hub.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the BigQuery Analytics Hub API.:  https://cloud.google.com/bigquery/docs/analytics-hub-introduction
+.. _Enable the BigQuery Analytics Hub.:  https://cloud.google.com/bigquery/docs/analytics-hub-introduction
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-bigquery-data-exchange
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for BigQuery Analytics Hub API
+-  Read the `Client Library Documentation`_ for BigQuery Analytics Hub
    to see other available methods on the client.
--  Read the `BigQuery Analytics Hub API Product documentation`_ to learn
+-  Read the `BigQuery Analytics Hub Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _BigQuery Analytics Hub API Product documentation:  https://cloud.google.com/bigquery/docs/analytics-hub-introduction
+.. _BigQuery Analytics Hub Product documentation:  https://cloud.google.com/bigquery/docs/analytics-hub-introduction
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/google_cloud_bigquery_data_exchange.egg-info/SOURCES.txt` & `google-cloud-bigquery-data-exchange-0.5.4/google_cloud_bigquery_data_exchange.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/setup.py` & `google-cloud-bigquery-data-exchange-0.5.4/setup.py`

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
-url = "https://github.com/googleapis/python-bigquery-data-exchange"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/tests/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/tests/unit/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.4/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/tests/unit/gapic/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.4/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/tests/unit/gapic/bigquery_data_exchange_v1beta1/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.4/tests/unit/gapic/bigquery_data_exchange_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.3/tests/unit/gapic/bigquery_data_exchange_v1beta1/test_analytics_hub_service.py` & `google-cloud-bigquery-data-exchange-0.5.4/tests/unit/gapic/bigquery_data_exchange_v1beta1/test_analytics_hub_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1143,17 +1143,19 @@
                     dataexchange.DataExchange(),
                     dataexchange.DataExchange(),
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
@@ -1586,17 +1588,19 @@
                     dataexchange.DataExchange(),
                     dataexchange.DataExchange(),
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
@@ -3070,17 +3074,19 @@
                     dataexchange.Listing(),
                     dataexchange.Listing(),
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
@@ -3108,17 +3114,14 @@
             description="description_value",
             primary_contact="primary_contact_value",
             documentation="documentation_value",
             state=dataexchange.Listing.State.ACTIVE,
             icon=b"icon_blob",
             categories=[dataexchange.Listing.Category.CATEGORY_OTHERS],
             request_access="request_access_value",
-            bigquery_dataset=dataexchange.Listing.BigQueryDatasetSource(
-                dataset="dataset_value"
-            ),
         )
         response = client.get_listing(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == dataexchange.GetListingRequest()
@@ -3375,17 +3378,14 @@
             description="description_value",
             primary_contact="primary_contact_value",
             documentation="documentation_value",
             state=dataexchange.Listing.State.ACTIVE,
             icon=b"icon_blob",
             categories=[dataexchange.Listing.Category.CATEGORY_OTHERS],
             request_access="request_access_value",
-            bigquery_dataset=dataexchange.Listing.BigQueryDatasetSource(
-                dataset="dataset_value"
-            ),
         )
         response = client.create_listing(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == dataexchange.CreateListingRequest()
@@ -3676,17 +3676,14 @@
             description="description_value",
             primary_contact="primary_contact_value",
             documentation="documentation_value",
             state=dataexchange.Listing.State.ACTIVE,
             icon=b"icon_blob",
             categories=[dataexchange.Listing.Category.CATEGORY_OTHERS],
             request_access="request_access_value",
-            bigquery_dataset=dataexchange.Listing.BigQueryDatasetSource(
-                dataset="dataset_value"
-            ),
         )
         response = client.update_listing(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == dataexchange.UpdateListingRequest()
```

