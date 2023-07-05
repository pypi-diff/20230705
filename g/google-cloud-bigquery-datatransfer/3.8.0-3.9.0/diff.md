# Comparing `tmp/google-cloud-bigquery-datatransfer-3.8.0.tar.gz` & `tmp/google-cloud-bigquery-datatransfer-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-bigquery-datatransfer-3.8.0.tar", last modified: Thu Dec 15 22:35:06 2022, max compression
+gzip compressed data, was "google-cloud-bigquery-datatransfer-3.9.0.tar", last modified: Wed Jan  4 15:57:08 2023, max compression
```

## Comparing `google-cloud-bigquery-datatransfer-3.8.0.tar` & `google-cloud-bigquery-datatransfer-3.9.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:06.149106 google-cloud-bigquery-datatransfer-3.8.0/
--rw-rw-r--   0 root         (0)     1003    11358 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4774 2022-12-15 22:35:06.149106 google-cloud-bigquery-datatransfer-3.8.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3867 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:06.141102 google-cloud-bigquery-datatransfer-3.8.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:06.141102 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:06.141102 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer/
--rw-rw-r--   0 root         (0)     1003     3018 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:06.145104 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/
--rw-rw-r--   0 root         (0)     1003     2802 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4548 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:06.145104 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:06.145104 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/
--rw-rw-r--   0 root         (0)     1003      789 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    82901 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    91570 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/client.py
--rw-rw-r--   0 root         (0)     1003    21661 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:06.145104 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/transports/
--rw-rw-r--   0 root         (0)     1003     1246 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    16855 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    29934 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    30572 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:06.145104 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/types/
--rw-rw-r--   0 root         (0)     1003     2479 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    37993 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/types/datatransfer.py
--rw-rw-r--   0 root         (0)     1003    17041 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/types/transfer.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:06.145104 google-cloud-bigquery-datatransfer-3.8.0/google_cloud_bigquery_datatransfer.egg-info/
--rw-r--r--   0 root         (0)     1003     4774 2022-12-15 22:35:06.000000 google-cloud-bigquery-datatransfer-3.8.0/google_cloud_bigquery_datatransfer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1970 2022-12-15 22:35:06.000000 google-cloud-bigquery-datatransfer-3.8.0/google_cloud_bigquery_datatransfer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-12-15 22:35:06.000000 google-cloud-bigquery-datatransfer-3.8.0/google_cloud_bigquery_datatransfer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-12-15 22:35:06.000000 google-cloud-bigquery-datatransfer-3.8.0/google_cloud_bigquery_datatransfer.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-12-15 22:35:06.000000 google-cloud-bigquery-datatransfer-3.8.0/google_cloud_bigquery_datatransfer.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      257 2022-12-15 22:35:06.000000 google-cloud-bigquery-datatransfer-3.8.0/google_cloud_bigquery_datatransfer.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-12-15 22:35:06.000000 google-cloud-bigquery-datatransfer-3.8.0/google_cloud_bigquery_datatransfer.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2022-12-15 22:35:06.149106 google-cloud-bigquery-datatransfer-3.8.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2923 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:06.149106 google-cloud-bigquery-datatransfer-3.8.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/tests/__init__.py
--rw-rw-r--   0 root         (0)     1003     1022 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/tests/system.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:06.149106 google-cloud-bigquery-datatransfer-3.8.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:06.149106 google-cloud-bigquery-datatransfer-3.8.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:06.149106 google-cloud-bigquery-datatransfer-3.8.0/tests/unit/gapic/bigquery_datatransfer_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/tests/unit/gapic/bigquery_datatransfer_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   213699 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/tests/unit/gapic/bigquery_datatransfer_v1/test_data_transfer_service.py
--rw-rw-r--   0 root         (0)     1003     1040 2022-12-15 22:31:39.000000 google-cloud-bigquery-datatransfer-3.8.0/tests/unit/test_shim.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-04 15:57:08.103196 google-cloud-bigquery-datatransfer-3.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4774 2023-01-04 15:57:08.103196 google-cloud-bigquery-datatransfer-3.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3867 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-04 15:57:08.095195 google-cloud-bigquery-datatransfer-3.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-04 15:57:08.095195 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-04 15:57:08.095195 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer/
+-rw-rw-r--   0 root         (0)     1003     3018 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-04 15:57:08.099196 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/
+-rw-rw-r--   0 root         (0)     1003     2802 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4548 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-04 15:57:08.099196 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-04 15:57:08.099196 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    87044 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    95673 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/client.py
+-rw-rw-r--   0 root         (0)     1003    21661 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-04 15:57:08.099196 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1246 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17446 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    31690 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    32328 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-04 15:57:08.099196 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2479 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    37993 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/types/datatransfer.py
+-rw-rw-r--   0 root         (0)     1003    17041 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/types/transfer.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-04 15:57:08.099196 google-cloud-bigquery-datatransfer-3.9.0/google_cloud_bigquery_datatransfer.egg-info/
+-rw-r--r--   0 root         (0)     1003     4774 2023-01-04 15:57:08.000000 google-cloud-bigquery-datatransfer-3.9.0/google_cloud_bigquery_datatransfer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1970 2023-01-04 15:57:08.000000 google-cloud-bigquery-datatransfer-3.9.0/google_cloud_bigquery_datatransfer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-04 15:57:08.000000 google-cloud-bigquery-datatransfer-3.9.0/google_cloud_bigquery_datatransfer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-01-04 15:57:08.000000 google-cloud-bigquery-datatransfer-3.9.0/google_cloud_bigquery_datatransfer.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-04 15:57:08.000000 google-cloud-bigquery-datatransfer-3.9.0/google_cloud_bigquery_datatransfer.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      257 2023-01-04 15:57:08.000000 google-cloud-bigquery-datatransfer-3.9.0/google_cloud_bigquery_datatransfer.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-01-04 15:57:08.000000 google-cloud-bigquery-datatransfer-3.9.0/google_cloud_bigquery_datatransfer.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-01-04 15:57:08.103196 google-cloud-bigquery-datatransfer-3.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2923 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-04 15:57:08.103196 google-cloud-bigquery-datatransfer-3.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/tests/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1022 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/tests/system.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-04 15:57:08.103196 google-cloud-bigquery-datatransfer-3.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-04 15:57:08.103196 google-cloud-bigquery-datatransfer-3.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-04 15:57:08.103196 google-cloud-bigquery-datatransfer-3.9.0/tests/unit/gapic/bigquery_datatransfer_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/tests/unit/gapic/bigquery_datatransfer_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   224733 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/tests/unit/gapic/bigquery_datatransfer_v1/test_data_transfer_service.py
+-rw-rw-r--   0 root         (0)     1003     1040 2023-01-04 15:53:52.000000 google-cloud-bigquery-datatransfer-3.9.0/tests/unit/test_shim.py
```

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/LICENSE` & `google-cloud-bigquery-datatransfer-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/MANIFEST.in` & `google-cloud-bigquery-datatransfer-3.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/PKG-INFO` & `google-cloud-bigquery-datatransfer-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-datatransfer
-Version: 3.8.0
+Version: 3.9.0
 Summary: Google Cloud Bigquery Datatransfer API client library
 Home-page: https://github.com/googleapis/python-bigquery-datatransfer
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/README.rst` & `google-cloud-bigquery-datatransfer-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer/__init__.py` & `google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer/gapic_version.py` & `google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer/gapic_version.py`

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
-__version__ = "3.8.0"  # {x-release-please-version}
+__version__ = "3.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/__init__.py` & `google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/gapic_metadata.json` & `google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/gapic_version.py` & `google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/gapic_version.py`

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
-__version__ = "3.8.0"  # {x-release-please-version}
+__version__ = "3.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/services/__init__.py` & `google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/__init__.py` & `google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/async_client.py` & `google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from google.cloud.bigquery_datatransfer_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
+from google.cloud.location import locations_pb2  # type: ignore
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import struct_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 
 from google.cloud.bigquery_datatransfer_v1.services.data_transfer_service import pagers
@@ -1965,14 +1966,122 @@
         await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
+    async def get_location(
+        self,
+        request: Optional[locations_pb2.GetLocationRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.Location:
+        r"""Gets information about a location.
+
+        Args:
+            request (:class:`~.location_pb2.GetLocationRequest`):
+                The request object. Request message for
+                `GetLocation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.Location:
+                Location object.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.GetLocationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.get_location,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def list_locations(
+        self,
+        request: Optional[locations_pb2.ListLocationsRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.ListLocationsResponse:
+        r"""Lists information about the supported locations for this service.
+
+        Args:
+            request (:class:`~.location_pb2.ListLocationsRequest`):
+                The request object. Request message for
+                `ListLocations` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.ListLocationsResponse:
+                Response message for ``ListLocations`` method.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.ListLocationsRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.list_locations,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
```

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/client.py` & `google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 from google.cloud.bigquery_datatransfer_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
+from google.cloud.location import locations_pb2  # type: ignore
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import struct_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 
 from google.cloud.bigquery_datatransfer_v1.services.data_transfer_service import pagers
@@ -2139,14 +2140,122 @@
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
+    def get_location(
+        self,
+        request: Optional[locations_pb2.GetLocationRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.Location:
+        r"""Gets information about a location.
+
+        Args:
+            request (:class:`~.location_pb2.GetLocationRequest`):
+                The request object. Request message for
+                `GetLocation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.Location:
+                Location object.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.GetLocationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.get_location,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def list_locations(
+        self,
+        request: Optional[locations_pb2.ListLocationsRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.ListLocationsResponse:
+        r"""Lists information about the supported locations for this service.
+
+        Args:
+            request (:class:`~.location_pb2.ListLocationsRequest`):
+                The request object. Request message for
+                `ListLocations` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.ListLocationsResponse:
+                Response message for ``ListLocations`` method.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.ListLocationsRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.list_locations,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
 __all__ = ("DataTransferServiceClient",)
```

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/pagers.py` & `google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/transports/__init__.py` & `google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/transports/base.py` & `google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/transports/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 
 from google.cloud.bigquery_datatransfer_v1 import gapic_version as package_version
 from google.cloud.bigquery_datatransfer_v1.types import datatransfer, transfer
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
@@ -462,12 +463,33 @@
     ) -> Callable[
         [datatransfer.EnrollDataSourcesRequest],
         Union[empty_pb2.Empty, Awaitable[empty_pb2.Empty]],
     ]:
         raise NotImplementedError()
 
     @property
+    def get_location(
+        self,
+    ) -> Callable[
+        [locations_pb2.GetLocationRequest],
+        Union[locations_pb2.Location, Awaitable[locations_pb2.Location]],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def list_locations(
+        self,
+    ) -> Callable[
+        [locations_pb2.ListLocationsRequest],
+        Union[
+            locations_pb2.ListLocationsResponse,
+            Awaitable[locations_pb2.ListLocationsResponse],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
     def kind(self) -> str:
         raise NotImplementedError()
 
 
 __all__ = ("DataTransferServiceTransport",)
```

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/transports/grpc.py` & `google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/transports/grpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from typing import Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
 from google.api_core import gapic_v1, grpc_helpers
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
 
 from google.cloud.bigquery_datatransfer_v1.types import datatransfer, transfer
 
 from .base import DEFAULT_CLIENT_INFO, DataTransferServiceTransport
 
@@ -660,12 +661,48 @@
             )
         return self._stubs["enroll_data_sources"]
 
     def close(self):
         self.grpc_channel.close()
 
     @property
+    def list_locations(
+        self,
+    ) -> Callable[
+        [locations_pb2.ListLocationsRequest], locations_pb2.ListLocationsResponse
+    ]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_locations" not in self._stubs:
+            self._stubs["list_locations"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/ListLocations",
+                request_serializer=locations_pb2.ListLocationsRequest.SerializeToString,
+                response_deserializer=locations_pb2.ListLocationsResponse.FromString,
+            )
+        return self._stubs["list_locations"]
+
+    @property
+    def get_location(
+        self,
+    ) -> Callable[[locations_pb2.GetLocationRequest], locations_pb2.Location]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_location" not in self._stubs:
+            self._stubs["get_location"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/GetLocation",
+                request_serializer=locations_pb2.GetLocationRequest.SerializeToString,
+                response_deserializer=locations_pb2.Location.FromString,
+            )
+        return self._stubs["get_location"]
+
+    @property
     def kind(self) -> str:
         return "grpc"
 
 
 __all__ = ("DataTransferServiceGrpcTransport",)
```

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/transports/grpc_asyncio.py` & `google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/services/data_transfer_service/transports/grpc_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
 from google.api_core import gapic_v1, grpc_helpers_async
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.cloud.bigquery_datatransfer_v1.types import datatransfer, transfer
 
 from .base import DEFAULT_CLIENT_INFO, DataTransferServiceTransport
@@ -678,9 +679,45 @@
                 response_deserializer=empty_pb2.Empty.FromString,
             )
         return self._stubs["enroll_data_sources"]
 
     def close(self):
         return self.grpc_channel.close()
 
+    @property
+    def list_locations(
+        self,
+    ) -> Callable[
+        [locations_pb2.ListLocationsRequest], locations_pb2.ListLocationsResponse
+    ]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_locations" not in self._stubs:
+            self._stubs["list_locations"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/ListLocations",
+                request_serializer=locations_pb2.ListLocationsRequest.SerializeToString,
+                response_deserializer=locations_pb2.ListLocationsResponse.FromString,
+            )
+        return self._stubs["list_locations"]
+
+    @property
+    def get_location(
+        self,
+    ) -> Callable[[locations_pb2.GetLocationRequest], locations_pb2.Location]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_location" not in self._stubs:
+            self._stubs["get_location"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/GetLocation",
+                request_serializer=locations_pb2.GetLocationRequest.SerializeToString,
+                response_deserializer=locations_pb2.Location.FromString,
+            )
+        return self._stubs["get_location"]
+
 
 __all__ = ("DataTransferServiceGrpcAsyncIOTransport",)
```

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/types/__init__.py` & `google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/types/datatransfer.py` & `google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/types/datatransfer.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/google/cloud/bigquery_datatransfer_v1/types/transfer.py` & `google-cloud-bigquery-datatransfer-3.9.0/google/cloud/bigquery_datatransfer_v1/types/transfer.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/google_cloud_bigquery_datatransfer.egg-info/PKG-INFO` & `google-cloud-bigquery-datatransfer-3.9.0/google_cloud_bigquery_datatransfer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-datatransfer
-Version: 3.8.0
+Version: 3.9.0
 Summary: Google Cloud Bigquery Datatransfer API client library
 Home-page: https://github.com/googleapis/python-bigquery-datatransfer
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/google_cloud_bigquery_datatransfer.egg-info/SOURCES.txt` & `google-cloud-bigquery-datatransfer-3.9.0/google_cloud_bigquery_datatransfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/setup.py` & `google-cloud-bigquery-datatransfer-3.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/tests/__init__.py` & `google-cloud-bigquery-datatransfer-3.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/tests/system.py` & `google-cloud-bigquery-datatransfer-3.9.0/tests/system.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/tests/unit/__init__.py` & `google-cloud-bigquery-datatransfer-3.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/tests/unit/gapic/__init__.py` & `google-cloud-bigquery-datatransfer-3.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/tests/unit/gapic/bigquery_datatransfer_v1/__init__.py` & `google-cloud-bigquery-datatransfer-3.9.0/tests/unit/gapic/bigquery_datatransfer_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/tests/unit/gapic/bigquery_datatransfer_v1/test_data_transfer_service.py` & `google-cloud-bigquery-datatransfer-3.9.0/tests/unit/gapic/bigquery_datatransfer_v1/test_data_transfer_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 from google.api_core import gapic_v1, grpc_helpers, grpc_helpers_async, path_template
 from google.api_core import client_options
 from google.api_core import exceptions as core_exceptions
 import google.auth
 from google.auth import credentials as ga_credentials
 from google.auth.exceptions import MutualTLSChannelError
+from google.cloud.location import locations_pb2
 from google.oauth2 import service_account
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import struct_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 import grpc
@@ -5334,14 +5335,16 @@
         "start_manual_transfer_runs",
         "get_transfer_run",
         "delete_transfer_run",
         "list_transfer_runs",
         "list_transfer_logs",
         "check_valid_creds",
         "enroll_data_sources",
+        "get_location",
+        "list_locations",
     )
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
     with pytest.raises(NotImplementedError):
         transport.close()
@@ -5893,14 +5896,304 @@
         type(getattr(client.transport, "grpc_channel")), "close"
     ) as close:
         async with client:
             close.assert_not_called()
         close.assert_called_once()
 
 
+def test_list_locations(transport: str = "grpc"):
+    client = DataTransferServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.ListLocationsRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.ListLocationsResponse()
+        response = client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.ListLocationsResponse)
+
+
+@pytest.mark.asyncio
+async def test_list_locations_async(transport: str = "grpc"):
+    client = DataTransferServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.ListLocationsRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.ListLocationsResponse()
+        )
+        response = await client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.ListLocationsResponse)
+
+
+def test_list_locations_field_headers():
+    client = DataTransferServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.ListLocationsRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        call.return_value = locations_pb2.ListLocationsResponse()
+
+        client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_list_locations_field_headers_async():
+    client = DataTransferServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.ListLocationsRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.ListLocationsResponse()
+        )
+        await client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+def test_list_locations_from_dict():
+    client = DataTransferServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.ListLocationsResponse()
+
+        response = client.list_locations(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_list_locations_from_dict_async():
+    client = DataTransferServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.ListLocationsResponse()
+        )
+        response = await client.list_locations(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+def test_get_location(transport: str = "grpc"):
+    client = DataTransferServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.GetLocationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.Location()
+        response = client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.Location)
+
+
+@pytest.mark.asyncio
+async def test_get_location_async(transport: str = "grpc_asyncio"):
+    client = DataTransferServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.GetLocationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.Location()
+        )
+        response = await client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.Location)
+
+
+def test_get_location_field_headers():
+    client = DataTransferServiceClient(
+        credentials=ga_credentials.AnonymousCredentials()
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.GetLocationRequest()
+    request.name = "locations/abc"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        call.return_value = locations_pb2.Location()
+
+        client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations/abc",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_get_location_field_headers_async():
+    client = DataTransferServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials()
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.GetLocationRequest()
+    request.name = "locations/abc"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.Location()
+        )
+        await client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations/abc",
+    ) in kw["metadata"]
+
+
+def test_get_location_from_dict():
+    client = DataTransferServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.Location()
+
+        response = client.get_location(
+            request={
+                "name": "locations/abc",
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_get_location_from_dict_async():
+    client = DataTransferServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.Location()
+        )
+        response = await client.get_location(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
 def test_transport_close():
     transports = {
         "grpc": "_grpc_channel",
     }
 
     for transport, close_name in transports.items():
         client = DataTransferServiceClient(
```

### Comparing `google-cloud-bigquery-datatransfer-3.8.0/tests/unit/test_shim.py` & `google-cloud-bigquery-datatransfer-3.9.0/tests/unit/test_shim.py`

 * *Files identical despite different names*

