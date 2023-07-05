# Comparing `tmp/google-cloud-bigquery-biglake-0.4.0.tar.gz` & `tmp/google-cloud-bigquery-biglake-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-bigquery-biglake-0.4.0.tar", last modified: Tue Jun 20 13:27:00 2023, max compression
+gzip compressed data, was "google-cloud-bigquery-biglake-0.4.1.tar", last modified: Wed Jul  5 15:50:57 2023, max compression
```

## Comparing `google-cloud-bigquery-biglake-0.4.0.tar` & `google-cloud-bigquery-biglake-0.4.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.489223 google-cloud-bigquery-biglake-0.4.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4685 2023-06-20 13:27:00.485222 google-cloud-bigquery-biglake-0.4.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3759 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.473221 google-cloud-bigquery-biglake-0.4.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.473221 google-cloud-bigquery-biglake-0.4.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.477221 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake/
--rw-rw-r--   0 root         (0)     1003     2242 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.477221 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/
--rw-rw-r--   0 root         (0)     1003     2085 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     6058 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.477221 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.477221 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/
--rw-rw-r--   0 root         (0)     1003      777 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    78072 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    90722 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/client.py
--rw-rw-r--   0 root         (0)     1003    15709 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.477221 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11893 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    27356 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    28003 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    82223 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.481222 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/types/
--rw-rw-r--   0 root         (0)     1003     1786 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    26313 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/types/metastore.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.481222 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/
--rw-rw-r--   0 root         (0)     1003     2349 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/__init__.py
--rw-rw-r--   0 root         (0)     1003     7450 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.481222 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.481222 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/
--rw-rw-r--   0 root         (0)     1003      777 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    95711 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   109684 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/client.py
--rw-rw-r--   0 root         (0)     1003    20793 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.481222 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    13545 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    31716 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    32496 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   101231 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.481222 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/types/
--rw-rw-r--   0 root         (0)     1003     2044 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    32213 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/types/metastore.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.485222 google-cloud-bigquery-biglake-0.4.0/google_cloud_bigquery_biglake.egg-info/
--rw-r--r--   0 root         (0)     1003     4685 2023-06-20 13:27:00.000000 google-cloud-bigquery-biglake-0.4.0/google_cloud_bigquery_biglake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3031 2023-06-20 13:27:00.000000 google-cloud-bigquery-biglake-0.4.0/google_cloud_bigquery_biglake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-20 13:27:00.000000 google-cloud-bigquery-biglake-0.4.0/google_cloud_bigquery_biglake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-06-20 13:27:00.000000 google-cloud-bigquery-biglake-0.4.0/google_cloud_bigquery_biglake.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-20 13:27:00.000000 google-cloud-bigquery-biglake-0.4.0/google_cloud_bigquery_biglake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-06-20 13:27:00.000000 google-cloud-bigquery-biglake-0.4.0/google_cloud_bigquery_biglake.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-20 13:27:00.000000 google-cloud-bigquery-biglake-0.4.0/google_cloud_bigquery_biglake.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-06-20 13:27:00.489223 google-cloud-bigquery-biglake-0.4.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2959 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.485222 google-cloud-bigquery-biglake-0.4.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.485222 google-cloud-bigquery-biglake-0.4.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.485222 google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.485222 google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/bigquery_biglake_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/bigquery_biglake_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   369886 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/bigquery_biglake_v1/test_metastore_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.485222 google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/bigquery_biglake_v1alpha1/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/bigquery_biglake_v1alpha1/__init__.py
--rw-rw-r--   0 root         (0)     1003   451218 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/bigquery_biglake_v1alpha1/test_metastore_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:57.586599 google-cloud-bigquery-biglake-0.4.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4685 2023-07-05 15:50:57.586599 google-cloud-bigquery-biglake-0.4.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3759 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:57.574598 google-cloud-bigquery-biglake-0.4.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:57.574598 google-cloud-bigquery-biglake-0.4.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:57.574598 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake/
+-rw-rw-r--   0 root         (0)     1003     2242 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:57.574598 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/
+-rw-rw-r--   0 root         (0)     1003     2085 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6058 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:57.574598 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:57.578599 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/metastore_service/
+-rw-rw-r--   0 root         (0)     1003      777 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/metastore_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    78105 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/metastore_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    90722 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/metastore_service/client.py
+-rw-rw-r--   0 root         (0)     1003    15709 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/metastore_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:57.578599 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11893 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    27356 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    28003 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    82223 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:57.578599 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1786 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26313 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/types/metastore.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:57.578599 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/
+-rw-rw-r--   0 root         (0)     1003     2349 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7450 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:57.578599 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:57.582599 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/
+-rw-rw-r--   0 root         (0)     1003      777 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    95744 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   109684 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/client.py
+-rw-rw-r--   0 root         (0)     1003    20793 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:57.582599 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13545 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    31716 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    32496 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   101231 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:57.582599 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/types/
+-rw-rw-r--   0 root         (0)     1003     2044 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    32213 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/types/metastore.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:57.586599 google-cloud-bigquery-biglake-0.4.1/google_cloud_bigquery_biglake.egg-info/
+-rw-r--r--   0 root         (0)     1003     4685 2023-07-05 15:50:57.000000 google-cloud-bigquery-biglake-0.4.1/google_cloud_bigquery_biglake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3031 2023-07-05 15:50:57.000000 google-cloud-bigquery-biglake-0.4.1/google_cloud_bigquery_biglake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:57.000000 google-cloud-bigquery-biglake-0.4.1/google_cloud_bigquery_biglake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:50:57.000000 google-cloud-bigquery-biglake-0.4.1/google_cloud_bigquery_biglake.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:57.000000 google-cloud-bigquery-biglake-0.4.1/google_cloud_bigquery_biglake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:50:57.000000 google-cloud-bigquery-biglake-0.4.1/google_cloud_bigquery_biglake.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:50:57.000000 google-cloud-bigquery-biglake-0.4.1/google_cloud_bigquery_biglake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:50:57.586599 google-cloud-bigquery-biglake-0.4.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2959 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:57.586599 google-cloud-bigquery-biglake-0.4.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:57.586599 google-cloud-bigquery-biglake-0.4.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:57.586599 google-cloud-bigquery-biglake-0.4.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:57.586599 google-cloud-bigquery-biglake-0.4.1/tests/unit/gapic/bigquery_biglake_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/tests/unit/gapic/bigquery_biglake_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   368275 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/tests/unit/gapic/bigquery_biglake_v1/test_metastore_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:57.586599 google-cloud-bigquery-biglake-0.4.1/tests/unit/gapic/bigquery_biglake_v1alpha1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/tests/unit/gapic/bigquery_biglake_v1alpha1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   449806 2023-07-05 15:46:58.000000 google-cloud-bigquery-biglake-0.4.1/tests/unit/gapic/bigquery_biglake_v1alpha1/test_metastore_service.py
```

### Comparing `google-cloud-bigquery-biglake-0.4.0/LICENSE` & `google-cloud-bigquery-biglake-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/MANIFEST.in` & `google-cloud-bigquery-biglake-0.4.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/PKG-INFO` & `google-cloud-bigquery-biglake-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-biglake
-Version: 0.4.0
+Version: 0.4.1
 Summary: Google Cloud Bigquery Biglake API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-bigquery-biglake-0.4.0/README.rst` & `google-cloud-bigquery-biglake-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake/__init__.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake/gapic_version.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake/gapic_version.py`

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

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/__init__.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/gapic_metadata.json` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/gapic_version.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/gapic_version.py`

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

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/__init__.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/__init__.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/metastore_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/async_client.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/metastore_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1905,15 +1905,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "MetastoreServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/client.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/metastore_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/pagers.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/metastore_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/__init__.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/base.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/grpc.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/grpc_asyncio.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/rest.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/types/__init__.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/types/metastore.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1/types/metastore.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/__init__.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/gapic_metadata.json` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/gapic_version.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/gapic_version.py`

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

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/__init__.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/__init__.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/async_client.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2328,15 +2328,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "MetastoreServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/client.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/pagers.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/__init__.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/base.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/grpc.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/grpc_asyncio.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/rest.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/types/__init__.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/types/metastore.py` & `google-cloud-bigquery-biglake-0.4.1/google/cloud/bigquery_biglake_v1alpha1/types/metastore.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/google_cloud_bigquery_biglake.egg-info/PKG-INFO` & `google-cloud-bigquery-biglake-0.4.1/google_cloud_bigquery_biglake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-biglake
-Version: 0.4.0
+Version: 0.4.1
 Summary: Google Cloud Bigquery Biglake API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-bigquery-biglake-0.4.0/google_cloud_bigquery_biglake.egg-info/SOURCES.txt` & `google-cloud-bigquery-biglake-0.4.1/google_cloud_bigquery_biglake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/setup.py` & `google-cloud-bigquery-biglake-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/tests/__init__.py` & `google-cloud-bigquery-biglake-0.4.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/tests/unit/__init__.py` & `google-cloud-bigquery-biglake-0.4.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/__init__.py` & `google-cloud-bigquery-biglake-0.4.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/bigquery_biglake_v1/__init__.py` & `google-cloud-bigquery-biglake-0.4.1/tests/unit/gapic/bigquery_biglake_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/bigquery_biglake_v1/test_metastore_service.py` & `google-cloud-bigquery-biglake-0.4.1/tests/unit/gapic/bigquery_biglake_v1/test_metastore_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1849,17 +1849,19 @@
                     metastore.Catalog(),
                     metastore.Catalog(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_catalogs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1880,17 +1882,14 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_database), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = metastore.Database(
             name="name_value",
             type_=metastore.Database.Type.HIVE,
-            hive_options=metastore.HiveDatabaseOptions(
-                location_uri="location_uri_value"
-            ),
         )
         response = client.create_database(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metastore.CreateDatabaseRequest()
@@ -2159,17 +2158,14 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_database), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = metastore.Database(
             name="name_value",
             type_=metastore.Database.Type.HIVE,
-            hive_options=metastore.HiveDatabaseOptions(
-                location_uri="location_uri_value"
-            ),
         )
         response = client.delete_database(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metastore.DeleteDatabaseRequest()
@@ -2394,17 +2390,14 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_database), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = metastore.Database(
             name="name_value",
             type_=metastore.Database.Type.HIVE,
-            hive_options=metastore.HiveDatabaseOptions(
-                location_uri="location_uri_value"
-            ),
         )
         response = client.update_database(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metastore.UpdateDatabaseRequest()
@@ -2663,17 +2656,14 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_database), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = metastore.Database(
             name="name_value",
             type_=metastore.Database.Type.HIVE,
-            hive_options=metastore.HiveDatabaseOptions(
-                location_uri="location_uri_value"
-            ),
         )
         response = client.get_database(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metastore.GetDatabaseRequest()
@@ -3287,17 +3277,19 @@
                     metastore.Database(),
                     metastore.Database(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_databases(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3319,17 +3311,14 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_table), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = metastore.Table(
             name="name_value",
             type_=metastore.Table.Type.HIVE,
             etag="etag_value",
-            hive_options=metastore.HiveTableOptions(
-                parameters={"key_value": "value_value"}
-            ),
         )
         response = client.create_table(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metastore.CreateTableRequest()
@@ -3602,17 +3591,14 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_table), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = metastore.Table(
             name="name_value",
             type_=metastore.Table.Type.HIVE,
             etag="etag_value",
-            hive_options=metastore.HiveTableOptions(
-                parameters={"key_value": "value_value"}
-            ),
         )
         response = client.delete_table(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metastore.DeleteTableRequest()
@@ -3841,17 +3827,14 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_table), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = metastore.Table(
             name="name_value",
             type_=metastore.Table.Type.HIVE,
             etag="etag_value",
-            hive_options=metastore.HiveTableOptions(
-                parameters={"key_value": "value_value"}
-            ),
         )
         response = client.update_table(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metastore.UpdateTableRequest()
@@ -4114,17 +4097,14 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.rename_table), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = metastore.Table(
             name="name_value",
             type_=metastore.Table.Type.HIVE,
             etag="etag_value",
-            hive_options=metastore.HiveTableOptions(
-                parameters={"key_value": "value_value"}
-            ),
         )
         response = client.rename_table(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metastore.RenameTableRequest()
@@ -4363,17 +4343,14 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_table), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = metastore.Table(
             name="name_value",
             type_=metastore.Table.Type.HIVE,
             etag="etag_value",
-            hive_options=metastore.HiveTableOptions(
-                parameters={"key_value": "value_value"}
-            ),
         )
         response = client.get_table(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metastore.GetTableRequest()
@@ -4990,17 +4967,19 @@
                     metastore.Table(),
                     metastore.Table(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_tables(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -6193,17 +6172,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = metastore.Database(
             name="name_value",
             type_=metastore.Database.Type.HIVE,
-            hive_options=metastore.HiveDatabaseOptions(
-                location_uri="location_uri_value"
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = metastore.Database.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -6514,17 +6490,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = metastore.Database(
             name="name_value",
             type_=metastore.Database.Type.HIVE,
-            hive_options=metastore.HiveDatabaseOptions(
-                location_uri="location_uri_value"
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = metastore.Database.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -6802,17 +6775,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = metastore.Database(
             name="name_value",
             type_=metastore.Database.Type.HIVE,
-            hive_options=metastore.HiveDatabaseOptions(
-                location_uri="location_uri_value"
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = metastore.Database.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -7100,17 +7070,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = metastore.Database(
             name="name_value",
             type_=metastore.Database.Type.HIVE,
-            hive_options=metastore.HiveDatabaseOptions(
-                location_uri="location_uri_value"
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = metastore.Database.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -7733,17 +7700,14 @@
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = metastore.Table(
             name="name_value",
             type_=metastore.Table.Type.HIVE,
             etag="etag_value",
-            hive_options=metastore.HiveTableOptions(
-                parameters={"key_value": "value_value"}
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = metastore.Table.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -8064,17 +8028,14 @@
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = metastore.Table(
             name="name_value",
             type_=metastore.Table.Type.HIVE,
             etag="etag_value",
-            hive_options=metastore.HiveTableOptions(
-                parameters={"key_value": "value_value"}
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = metastore.Table.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -8360,17 +8321,14 @@
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = metastore.Table(
             name="name_value",
             type_=metastore.Table.Type.HIVE,
             etag="etag_value",
-            hive_options=metastore.HiveTableOptions(
-                parameters={"key_value": "value_value"}
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = metastore.Table.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -8666,17 +8624,14 @@
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = metastore.Table(
             name="name_value",
             type_=metastore.Table.Type.HIVE,
             etag="etag_value",
-            hive_options=metastore.HiveTableOptions(
-                parameters={"key_value": "value_value"}
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = metastore.Table.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -8956,17 +8911,14 @@
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = metastore.Table(
             name="name_value",
             type_=metastore.Table.Type.HIVE,
             etag="etag_value",
-            hive_options=metastore.HiveTableOptions(
-                parameters={"key_value": "value_value"}
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = metastore.Table.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

### Comparing `google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/bigquery_biglake_v1alpha1/__init__.py` & `google-cloud-bigquery-biglake-0.4.1/tests/unit/gapic/bigquery_biglake_v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/bigquery_biglake_v1alpha1/test_metastore_service.py` & `google-cloud-bigquery-biglake-0.4.1/tests/unit/gapic/bigquery_biglake_v1alpha1/test_metastore_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1849,17 +1849,19 @@
                     metastore.Catalog(),
                     metastore.Catalog(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_catalogs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1880,17 +1882,14 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_database), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = metastore.Database(
             name="name_value",
             type_=metastore.Database.Type.HIVE,
-            hive_options=metastore.HiveDatabaseOptions(
-                location_uri="location_uri_value"
-            ),
         )
         response = client.create_database(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metastore.CreateDatabaseRequest()
@@ -2159,17 +2158,14 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_database), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = metastore.Database(
             name="name_value",
             type_=metastore.Database.Type.HIVE,
-            hive_options=metastore.HiveDatabaseOptions(
-                location_uri="location_uri_value"
-            ),
         )
         response = client.delete_database(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metastore.DeleteDatabaseRequest()
@@ -2394,17 +2390,14 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_database), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = metastore.Database(
             name="name_value",
             type_=metastore.Database.Type.HIVE,
-            hive_options=metastore.HiveDatabaseOptions(
-                location_uri="location_uri_value"
-            ),
         )
         response = client.update_database(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metastore.UpdateDatabaseRequest()
@@ -2663,17 +2656,14 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_database), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = metastore.Database(
             name="name_value",
             type_=metastore.Database.Type.HIVE,
-            hive_options=metastore.HiveDatabaseOptions(
-                location_uri="location_uri_value"
-            ),
         )
         response = client.get_database(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metastore.GetDatabaseRequest()
@@ -3287,17 +3277,19 @@
                     metastore.Database(),
                     metastore.Database(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_databases(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3319,17 +3311,14 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_table), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = metastore.Table(
             name="name_value",
             type_=metastore.Table.Type.HIVE,
             etag="etag_value",
-            hive_options=metastore.HiveTableOptions(
-                parameters={"key_value": "value_value"}
-            ),
         )
         response = client.create_table(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metastore.CreateTableRequest()
@@ -3602,17 +3591,14 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_table), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = metastore.Table(
             name="name_value",
             type_=metastore.Table.Type.HIVE,
             etag="etag_value",
-            hive_options=metastore.HiveTableOptions(
-                parameters={"key_value": "value_value"}
-            ),
         )
         response = client.delete_table(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metastore.DeleteTableRequest()
@@ -3841,17 +3827,14 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_table), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = metastore.Table(
             name="name_value",
             type_=metastore.Table.Type.HIVE,
             etag="etag_value",
-            hive_options=metastore.HiveTableOptions(
-                parameters={"key_value": "value_value"}
-            ),
         )
         response = client.update_table(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metastore.UpdateTableRequest()
@@ -4114,17 +4097,14 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.rename_table), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = metastore.Table(
             name="name_value",
             type_=metastore.Table.Type.HIVE,
             etag="etag_value",
-            hive_options=metastore.HiveTableOptions(
-                parameters={"key_value": "value_value"}
-            ),
         )
         response = client.rename_table(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metastore.RenameTableRequest()
@@ -4363,17 +4343,14 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_table), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = metastore.Table(
             name="name_value",
             type_=metastore.Table.Type.HIVE,
             etag="etag_value",
-            hive_options=metastore.HiveTableOptions(
-                parameters={"key_value": "value_value"}
-            ),
         )
         response = client.get_table(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metastore.GetTableRequest()
@@ -4990,17 +4967,19 @@
                     metastore.Table(),
                     metastore.Table(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_tables(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -6114,17 +6093,19 @@
                     metastore.Lock(),
                     metastore.Lock(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_locks(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -7321,17 +7302,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = metastore.Database(
             name="name_value",
             type_=metastore.Database.Type.HIVE,
-            hive_options=metastore.HiveDatabaseOptions(
-                location_uri="location_uri_value"
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = metastore.Database.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -7642,17 +7620,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = metastore.Database(
             name="name_value",
             type_=metastore.Database.Type.HIVE,
-            hive_options=metastore.HiveDatabaseOptions(
-                location_uri="location_uri_value"
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = metastore.Database.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -7930,17 +7905,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = metastore.Database(
             name="name_value",
             type_=metastore.Database.Type.HIVE,
-            hive_options=metastore.HiveDatabaseOptions(
-                location_uri="location_uri_value"
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = metastore.Database.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -8228,17 +8200,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = metastore.Database(
             name="name_value",
             type_=metastore.Database.Type.HIVE,
-            hive_options=metastore.HiveDatabaseOptions(
-                location_uri="location_uri_value"
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = metastore.Database.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -8861,17 +8830,14 @@
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = metastore.Table(
             name="name_value",
             type_=metastore.Table.Type.HIVE,
             etag="etag_value",
-            hive_options=metastore.HiveTableOptions(
-                parameters={"key_value": "value_value"}
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = metastore.Table.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -9192,17 +9158,14 @@
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = metastore.Table(
             name="name_value",
             type_=metastore.Table.Type.HIVE,
             etag="etag_value",
-            hive_options=metastore.HiveTableOptions(
-                parameters={"key_value": "value_value"}
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = metastore.Table.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -9488,17 +9451,14 @@
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = metastore.Table(
             name="name_value",
             type_=metastore.Table.Type.HIVE,
             etag="etag_value",
-            hive_options=metastore.HiveTableOptions(
-                parameters={"key_value": "value_value"}
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = metastore.Table.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -9794,17 +9754,14 @@
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = metastore.Table(
             name="name_value",
             type_=metastore.Table.Type.HIVE,
             etag="etag_value",
-            hive_options=metastore.HiveTableOptions(
-                parameters={"key_value": "value_value"}
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = metastore.Table.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -10084,17 +10041,14 @@
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = metastore.Table(
             name="name_value",
             type_=metastore.Table.Type.HIVE,
             etag="etag_value",
-            hive_options=metastore.HiveTableOptions(
-                parameters={"key_value": "value_value"}
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = metastore.Table.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

