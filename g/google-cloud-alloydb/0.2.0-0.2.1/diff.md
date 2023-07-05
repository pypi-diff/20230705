# Comparing `tmp/google-cloud-alloydb-0.2.0.tar.gz` & `tmp/google-cloud-alloydb-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-alloydb-0.2.0.tar", last modified: Tue Jun 13 15:01:16 2023, max compression
+gzip compressed data, was "google-cloud-alloydb-0.2.1.tar", last modified: Wed Jul  5 15:49:56 2023, max compression
```

## Comparing `google-cloud-alloydb-0.2.0.tar` & `google-cloud-alloydb-0.2.1.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.429958 google-cloud-alloydb-0.2.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4362 2023-06-13 15:01:16.429958 google-cloud-alloydb-0.2.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3454 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.409957 google-cloud-alloydb-0.2.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.409957 google-cloud-alloydb-0.2.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.413957 google-cloud-alloydb-0.2.0/google/cloud/alloydb/
--rw-rw-r--   0 root         (0)     1003     4025 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       81 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.413957 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/
--rw-rw-r--   0 root         (0)     1003     3871 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    11355 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       81 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.413957 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.413957 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/alloy_db_admin/
--rw-rw-r--   0 root         (0)     1003      761 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/alloy_db_admin/__init__.py
--rw-rw-r--   0 root         (0)     1003   165381 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/alloy_db_admin/async_client.py
--rw-rw-r--   0 root         (0)     1003   179610 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/alloy_db_admin/client.py
--rw-rw-r--   0 root         (0)     1003    25613 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/alloy_db_admin/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.413957 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    22170 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/base.py
--rw-rw-r--   0 root         (0)     1003    49405 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    50442 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   176665 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.417957 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/types/
--rw-rw-r--   0 root         (0)     1003     3607 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    62689 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/types/resources.py
--rw-rw-r--   0 root         (0)     1003    65977 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.417957 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/
--rw-rw-r--   0 root         (0)     1003     4138 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003    12199 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       81 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.417957 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.417957 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/
--rw-rw-r--   0 root         (0)     1003      761 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/__init__.py
--rw-rw-r--   0 root         (0)     1003   176250 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/async_client.py
--rw-rw-r--   0 root         (0)     1003   190294 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/client.py
--rw-rw-r--   0 root         (0)     1003    25818 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.421958 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    24539 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/base.py
--rw-rw-r--   0 root         (0)     1003    52275 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    53370 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   187741 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.421958 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/types/
--rw-rw-r--   0 root         (0)     1003     3869 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    67262 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/types/resources.py
--rw-rw-r--   0 root         (0)     1003    71128 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.421958 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/
--rw-rw-r--   0 root         (0)     1003     4137 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003    12197 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       81 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.421958 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.421958 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/
--rw-rw-r--   0 root         (0)     1003      761 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/__init__.py
--rw-rw-r--   0 root         (0)     1003   176074 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/async_client.py
--rw-rw-r--   0 root         (0)     1003   190118 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/client.py
--rw-rw-r--   0 root         (0)     1003    25777 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.425958 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    24537 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/base.py
--rw-rw-r--   0 root         (0)     1003    52243 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    53338 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   187531 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.425958 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     3869 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    67217 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/types/resources.py
--rw-rw-r--   0 root         (0)     1003    71098 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.425958 google-cloud-alloydb-0.2.0/google_cloud_alloydb.egg-info/
--rw-r--r--   0 root         (0)     1003     4362 2023-06-13 15:01:16.000000 google-cloud-alloydb-0.2.0/google_cloud_alloydb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3705 2023-06-13 15:01:16.000000 google-cloud-alloydb-0.2.0/google_cloud_alloydb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-13 15:01:16.000000 google-cloud-alloydb-0.2.0/google_cloud_alloydb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-06-13 15:01:16.000000 google-cloud-alloydb-0.2.0/google_cloud_alloydb.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-13 15:01:16.000000 google-cloud-alloydb-0.2.0/google_cloud_alloydb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-06-13 15:01:16.000000 google-cloud-alloydb-0.2.0/google_cloud_alloydb.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-13 15:01:16.000000 google-cloud-alloydb-0.2.0/google_cloud_alloydb.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-06-13 15:01:16.429958 google-cloud-alloydb-0.2.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2973 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.425958 google-cloud-alloydb-0.2.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.425958 google-cloud-alloydb-0.2.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.425958 google-cloud-alloydb-0.2.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.425958 google-cloud-alloydb-0.2.0/tests/unit/gapic/alloydb_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/tests/unit/gapic/alloydb_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   711930 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/tests/unit/gapic/alloydb_v1/test_alloy_db_admin.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.429958 google-cloud-alloydb-0.2.0/tests/unit/gapic/alloydb_v1alpha/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/tests/unit/gapic/alloydb_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003   753611 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/tests/unit/gapic/alloydb_v1alpha/test_alloy_db_admin.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:01:16.429958 google-cloud-alloydb-0.2.0/tests/unit/gapic/alloydb_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/tests/unit/gapic/alloydb_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003   753576 2023-06-13 14:58:22.000000 google-cloud-alloydb-0.2.0/tests/unit/gapic/alloydb_v1beta/test_alloy_db_admin.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.877320 google-cloud-alloydb-0.2.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4362 2023-07-05 15:49:56.877320 google-cloud-alloydb-0.2.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3454 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.857317 google-cloud-alloydb-0.2.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.861318 google-cloud-alloydb-0.2.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.861318 google-cloud-alloydb-0.2.1/google/cloud/alloydb/
+-rw-rw-r--   0 root         (0)     1003     4025 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       81 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.865318 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/
+-rw-rw-r--   0 root         (0)     1003     3871 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11355 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       81 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.865318 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.865318 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/
+-rw-rw-r--   0 root         (0)     1003      761 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/__init__.py
+-rw-rw-r--   0 root         (0)     1003   165410 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/async_client.py
+-rw-rw-r--   0 root         (0)     1003   179610 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/client.py
+-rw-rw-r--   0 root         (0)     1003    25613 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.865318 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22170 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    49405 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    50442 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   176653 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.865318 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3607 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    62689 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/types/resources.py
+-rw-rw-r--   0 root         (0)     1003    65977 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.865318 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/
+-rw-rw-r--   0 root         (0)     1003     4138 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12199 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       81 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.865318 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.869319 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/
+-rw-rw-r--   0 root         (0)     1003      761 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/__init__.py
+-rw-rw-r--   0 root         (0)     1003   176279 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/async_client.py
+-rw-rw-r--   0 root         (0)     1003   190294 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/client.py
+-rw-rw-r--   0 root         (0)     1003    25818 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.869319 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24539 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    52275 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    53370 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   187729 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.869319 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/types/
+-rw-rw-r--   0 root         (0)     1003     3869 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    67262 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/types/resources.py
+-rw-rw-r--   0 root         (0)     1003    71128 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.869319 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/
+-rw-rw-r--   0 root         (0)     1003     4137 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12197 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       81 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.869319 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.873319 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/
+-rw-rw-r--   0 root         (0)     1003      761 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/__init__.py
+-rw-rw-r--   0 root         (0)     1003   176103 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/async_client.py
+-rw-rw-r--   0 root         (0)     1003   190118 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/client.py
+-rw-rw-r--   0 root         (0)     1003    25777 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.873319 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24537 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    52243 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    53338 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   187531 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.873319 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     3869 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    67217 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/types/resources.py
+-rw-rw-r--   0 root         (0)     1003    71098 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.873319 google-cloud-alloydb-0.2.1/google_cloud_alloydb.egg-info/
+-rw-r--r--   0 root         (0)     1003     4362 2023-07-05 15:49:56.000000 google-cloud-alloydb-0.2.1/google_cloud_alloydb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3705 2023-07-05 15:49:56.000000 google-cloud-alloydb-0.2.1/google_cloud_alloydb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:49:56.000000 google-cloud-alloydb-0.2.1/google_cloud_alloydb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:49:56.000000 google-cloud-alloydb-0.2.1/google_cloud_alloydb.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:49:56.000000 google-cloud-alloydb-0.2.1/google_cloud_alloydb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:49:56.000000 google-cloud-alloydb-0.2.1/google_cloud_alloydb.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:49:56.000000 google-cloud-alloydb-0.2.1/google_cloud_alloydb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:49:56.877320 google-cloud-alloydb-0.2.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2973 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.873319 google-cloud-alloydb-0.2.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.877320 google-cloud-alloydb-0.2.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.877320 google-cloud-alloydb-0.2.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.877320 google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   712763 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1/test_alloy_db_admin.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.877320 google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1alpha/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003   754444 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1alpha/test_alloy_db_admin.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.877320 google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003   754409 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1beta/test_alloy_db_admin.py
```

### Comparing `google-cloud-alloydb-0.2.0/LICENSE` & `google-cloud-alloydb-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/MANIFEST.in` & `google-cloud-alloydb-0.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/PKG-INFO` & `google-cloud-alloydb-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-alloydb
-Version: 0.2.0
+Version: 0.2.1
 Summary: Google Cloud Alloydb API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-alloydb-0.2.0/README.rst` & `google-cloud-alloydb-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb/__init__.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb/gapic_version.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb/gapic_version.py`

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
-__version__ = "0.2.0"  # {x-release-please-version}
+__version__ = "0.2.1"  # {x-release-please-version}
```

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/__init__.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/gapic_metadata.json` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/gapic_version.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/gapic_version.py`

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
-__version__ = "0.2.0"  # {x-release-please-version}
+__version__ = "0.2.1"  # {x-release-please-version}
```

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/__init__.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/alloy_db_admin/__init__.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/alloy_db_admin/async_client.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4130,15 +4130,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "AlloyDBAdminAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/alloy_db_admin/client.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/alloy_db_admin/pagers.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/__init__.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/base.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/grpc.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/grpc_asyncio.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/rest.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -4292,15 +4292,15 @@
 
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

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/types/__init__.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/types/resources.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/types/resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1/types/service.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/__init__.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/gapic_metadata.json` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/gapic_version.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/gapic_version.py`

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
-__version__ = "0.2.0"  # {x-release-please-version}
+__version__ = "0.2.1"  # {x-release-please-version}
```

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/__init__.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/__init__.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/async_client.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4383,15 +4383,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "AlloyDBAdminAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/client.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/pagers.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/__init__.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/base.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/grpc.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/grpc_asyncio.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/rest.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -4566,15 +4566,15 @@
 
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

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/types/__init__.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/types/resources.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/types/resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1alpha/types/service.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/__init__.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/gapic_metadata.json` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/gapic_version.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/gapic_version.py`

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
-__version__ = "0.2.0"  # {x-release-please-version}
+__version__ = "0.2.1"  # {x-release-please-version}
```

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/__init__.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/__init__.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/async_client.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4383,15 +4383,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "AlloyDBAdminAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/client.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/pagers.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/__init__.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/base.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/grpc.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/grpc_asyncio.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/rest.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/types/__init__.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/types/resources.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/types/resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google/cloud/alloydb_v1beta/types/service.py` & `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/google_cloud_alloydb.egg-info/PKG-INFO` & `google-cloud-alloydb-0.2.1/google_cloud_alloydb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-alloydb
-Version: 0.2.0
+Version: 0.2.1
 Summary: Google Cloud Alloydb API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-alloydb-0.2.0/google_cloud_alloydb.egg-info/SOURCES.txt` & `google-cloud-alloydb-0.2.1/google_cloud_alloydb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/setup.py` & `google-cloud-alloydb-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/tests/__init__.py` & `google-cloud-alloydb-0.2.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/tests/unit/__init__.py` & `google-cloud-alloydb-0.2.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/tests/unit/gapic/__init__.py` & `google-cloud-alloydb-0.2.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/tests/unit/gapic/alloydb_v1/__init__.py` & `google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/tests/unit/gapic/alloydb_v1/test_alloy_db_admin.py` & `google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1/test_alloy_db_admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1121,17 +1121,19 @@
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
@@ -1159,15 +1161,14 @@
             uid="uid_value",
             state=resources.Cluster.State.READY,
             cluster_type=resources.Cluster.ClusterType.PRIMARY,
             database_version=resources.DatabaseVersion.POSTGRES_13,
             network="network_value",
             etag="etag_value",
             reconciling=True,
-            backup_source=resources.BackupSource(backup_uid="backup_uid_value"),
         )
         response = client.get_cluster(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.GetClusterRequest()
@@ -3180,17 +3181,19 @@
                     resources.Instance(),
                     resources.Instance(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_instances(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5692,17 +5695,19 @@
                     resources.Backup(),
                     resources.Backup(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_backups(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -7111,17 +7116,19 @@
                     resources.SupportedDatabaseFlag(),
                     resources.SupportedDatabaseFlag(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_supported_database_flags(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -7535,17 +7542,19 @@
                     resources.User(),
                     resources.User(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_users(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -8882,15 +8891,14 @@
             uid="uid_value",
             state=resources.Cluster.State.READY,
             cluster_type=resources.Cluster.ClusterType.PRIMARY,
             database_version=resources.DatabaseVersion.POSTGRES_13,
             network="network_value",
             etag="etag_value",
             reconciling=True,
-            backup_source=resources.BackupSource(backup_uid="backup_uid_value"),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = resources.Cluster.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

### Comparing `google-cloud-alloydb-0.2.0/tests/unit/gapic/alloydb_v1alpha/__init__.py` & `google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/tests/unit/gapic/alloydb_v1alpha/test_alloy_db_admin.py` & `google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1alpha/test_alloy_db_admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1121,17 +1121,19 @@
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
@@ -1159,15 +1161,14 @@
             uid="uid_value",
             state=resources.Cluster.State.READY,
             cluster_type=resources.Cluster.ClusterType.PRIMARY,
             database_version=resources.DatabaseVersion.POSTGRES_13,
             network="network_value",
             etag="etag_value",
             reconciling=True,
-            backup_source=resources.BackupSource(backup_uid="backup_uid_value"),
         )
         response = client.get_cluster(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.GetClusterRequest()
@@ -3180,17 +3181,19 @@
                     resources.Instance(),
                     resources.Instance(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_instances(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5692,17 +5695,19 @@
                     resources.Backup(),
                     resources.Backup(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_backups(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -7111,17 +7116,19 @@
                     resources.SupportedDatabaseFlag(),
                     resources.SupportedDatabaseFlag(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_supported_database_flags(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -8048,17 +8055,19 @@
                     resources.User(),
                     resources.User(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_users(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -9396,15 +9405,14 @@
             uid="uid_value",
             state=resources.Cluster.State.READY,
             cluster_type=resources.Cluster.ClusterType.PRIMARY,
             database_version=resources.DatabaseVersion.POSTGRES_13,
             network="network_value",
             etag="etag_value",
             reconciling=True,
-            backup_source=resources.BackupSource(backup_uid="backup_uid_value"),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = resources.Cluster.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

### Comparing `google-cloud-alloydb-0.2.0/tests/unit/gapic/alloydb_v1beta/__init__.py` & `google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.0/tests/unit/gapic/alloydb_v1beta/test_alloy_db_admin.py` & `google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1beta/test_alloy_db_admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1121,17 +1121,19 @@
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
@@ -1159,15 +1161,14 @@
             uid="uid_value",
             state=resources.Cluster.State.READY,
             cluster_type=resources.Cluster.ClusterType.PRIMARY,
             database_version=resources.DatabaseVersion.POSTGRES_13,
             network="network_value",
             etag="etag_value",
             reconciling=True,
-            backup_source=resources.BackupSource(backup_uid="backup_uid_value"),
         )
         response = client.get_cluster(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.GetClusterRequest()
@@ -3180,17 +3181,19 @@
                     resources.Instance(),
                     resources.Instance(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_instances(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5692,17 +5695,19 @@
                     resources.Backup(),
                     resources.Backup(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_backups(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -7111,17 +7116,19 @@
                     resources.SupportedDatabaseFlag(),
                     resources.SupportedDatabaseFlag(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_supported_database_flags(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -8048,17 +8055,19 @@
                     resources.User(),
                     resources.User(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_users(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -9396,15 +9405,14 @@
             uid="uid_value",
             state=resources.Cluster.State.READY,
             cluster_type=resources.Cluster.ClusterType.PRIMARY,
             database_version=resources.DatabaseVersion.POSTGRES_13,
             network="network_value",
             etag="etag_value",
             reconciling=True,
-            backup_source=resources.BackupSource(backup_uid="backup_uid_value"),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = resources.Cluster.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

