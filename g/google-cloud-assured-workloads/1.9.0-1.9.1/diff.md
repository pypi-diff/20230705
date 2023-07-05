# Comparing `tmp/google-cloud-assured-workloads-1.9.0.tar.gz` & `tmp/google-cloud-assured-workloads-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-assured-workloads-1.9.0.tar", last modified: Wed Jan 11 15:22:31 2023, max compression
+gzip compressed data, was "google-cloud-assured-workloads-1.9.1.tar", last modified: Mon Jan 23 15:51:52 2023, max compression
```

## Comparing `google-cloud-assured-workloads-1.9.0.tar` & `google-cloud-assured-workloads-1.9.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:22:31.909024 google-cloud-assured-workloads-1.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4922 2023-01-11 15:22:31.909024 google-cloud-assured-workloads-1.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3976 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:22:31.897025 google-cloud-assured-workloads-1.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:22:31.897025 google-cloud-assured-workloads-1.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:22:31.901025 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads/
--rw-rw-r--   0 root         (0)     1003     2107 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:22:31.901025 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/
--rw-rw-r--   0 root         (0)     1003     1939 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2864 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:22:31.901025 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:22:31.901025 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/services/assured_workloads_service/
--rw-rw-r--   0 root         (0)     1003      805 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/services/assured_workloads_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    53151 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/services/assured_workloads_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    64031 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/services/assured_workloads_service/client.py
--rw-rw-r--   0 root         (0)     1003    11030 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/services/assured_workloads_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:22:31.905025 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/services/assured_workloads_service/transports/
--rw-rw-r--   0 root         (0)     1003     1282 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/services/assured_workloads_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10738 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/services/assured_workloads_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    25040 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/services/assured_workloads_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    25540 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/services/assured_workloads_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:22:31.905025 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/types/
--rw-rw-r--   0 root         (0)     1003     1607 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    35892 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/types/assuredworkloads.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:22:31.905025 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/
--rw-rw-r--   0 root         (0)     1003     1703 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2384 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:22:31.905025 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:22:31.905025 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/
--rw-rw-r--   0 root         (0)     1003      805 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    47326 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    55983 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/client.py
--rw-rw-r--   0 root         (0)     1003     5945 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:22:31.905025 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/transports/
--rw-rw-r--   0 root         (0)     1003     1282 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11174 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22393 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    22835 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:22:31.905025 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1371 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    28185 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/types/assuredworkloads.py
--rw-rw-r--   0 root         (0)     1003      752 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/types/assuredworkloads_service.py
--rw-rw-r--   0 root         (0)     1003    22051 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/types/assuredworkloads_v1beta1.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:22:31.909024 google-cloud-assured-workloads-1.9.0/google_cloud_assured_workloads.egg-info/
--rw-r--r--   0 root         (0)     1003     4922 2023-01-11 15:22:31.000000 google-cloud-assured-workloads-1.9.0/google_cloud_assured_workloads.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3169 2023-01-11 15:22:31.000000 google-cloud-assured-workloads-1.9.0/google_cloud_assured_workloads.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-11 15:22:31.000000 google-cloud-assured-workloads-1.9.0/google_cloud_assured_workloads.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-11 15:22:31.000000 google-cloud-assured-workloads-1.9.0/google_cloud_assured_workloads.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-11 15:22:31.000000 google-cloud-assured-workloads-1.9.0/google_cloud_assured_workloads.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-01-11 15:22:31.000000 google-cloud-assured-workloads-1.9.0/google_cloud_assured_workloads.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-11 15:22:31.000000 google-cloud-assured-workloads-1.9.0/google_cloud_assured_workloads.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-01-11 15:22:31.909024 google-cloud-assured-workloads-1.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3019 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:22:31.909024 google-cloud-assured-workloads-1.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:22:31.909024 google-cloud-assured-workloads-1.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:22:31.909024 google-cloud-assured-workloads-1.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:22:31.909024 google-cloud-assured-workloads-1.9.0/tests/unit/gapic/assuredworkloads_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/tests/unit/gapic/assuredworkloads_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   150934 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/tests/unit/gapic/assuredworkloads_v1/test_assured_workloads_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:22:31.909024 google-cloud-assured-workloads-1.9.0/tests/unit/gapic/assuredworkloads_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/tests/unit/gapic/assuredworkloads_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   125919 2023-01-11 15:19:41.000000 google-cloud-assured-workloads-1.9.0/tests/unit/gapic/assuredworkloads_v1beta1/test_assured_workloads_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:52.262300 google-cloud-assured-workloads-1.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4922 2023-01-23 15:51:52.262300 google-cloud-assured-workloads-1.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3976 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:52.250302 google-cloud-assured-workloads-1.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:52.250302 google-cloud-assured-workloads-1.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:52.254302 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads/
+-rw-rw-r--   0 root         (0)     1003     2107 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:52.254302 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/
+-rw-rw-r--   0 root         (0)     1003     1939 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2864 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:52.254302 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:52.254302 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/services/assured_workloads_service/
+-rw-rw-r--   0 root         (0)     1003      805 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/services/assured_workloads_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    53151 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/services/assured_workloads_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    64066 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/services/assured_workloads_service/client.py
+-rw-rw-r--   0 root         (0)     1003    11030 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/services/assured_workloads_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:52.254302 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/services/assured_workloads_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1282 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/services/assured_workloads_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10738 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/services/assured_workloads_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    25040 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/services/assured_workloads_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    25540 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/services/assured_workloads_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:52.254302 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1607 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    41538 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/types/assuredworkloads.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:52.254302 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     1703 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2384 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:52.254302 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:52.258301 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/
+-rw-rw-r--   0 root         (0)     1003      805 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    47326 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    56018 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5945 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:52.258301 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1282 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11174 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22393 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    22835 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:52.258301 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1371 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    32215 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/types/assuredworkloads.py
+-rw-rw-r--   0 root         (0)     1003      752 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/types/assuredworkloads_service.py
+-rw-rw-r--   0 root         (0)     1003    22051 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/types/assuredworkloads_v1beta1.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:52.258301 google-cloud-assured-workloads-1.9.1/google_cloud_assured_workloads.egg-info/
+-rw-r--r--   0 root         (0)     1003     4922 2023-01-23 15:51:52.000000 google-cloud-assured-workloads-1.9.1/google_cloud_assured_workloads.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3169 2023-01-23 15:51:52.000000 google-cloud-assured-workloads-1.9.1/google_cloud_assured_workloads.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 15:51:52.000000 google-cloud-assured-workloads-1.9.1/google_cloud_assured_workloads.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-01-23 15:51:52.000000 google-cloud-assured-workloads-1.9.1/google_cloud_assured_workloads.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 15:51:52.000000 google-cloud-assured-workloads-1.9.1/google_cloud_assured_workloads.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-01-23 15:51:52.000000 google-cloud-assured-workloads-1.9.1/google_cloud_assured_workloads.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-01-23 15:51:52.000000 google-cloud-assured-workloads-1.9.1/google_cloud_assured_workloads.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-01-23 15:51:52.262300 google-cloud-assured-workloads-1.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3019 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:52.258301 google-cloud-assured-workloads-1.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:52.258301 google-cloud-assured-workloads-1.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:52.258301 google-cloud-assured-workloads-1.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:52.258301 google-cloud-assured-workloads-1.9.1/tests/unit/gapic/assuredworkloads_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/tests/unit/gapic/assuredworkloads_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   150934 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/tests/unit/gapic/assuredworkloads_v1/test_assured_workloads_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:52.262300 google-cloud-assured-workloads-1.9.1/tests/unit/gapic/assuredworkloads_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/tests/unit/gapic/assuredworkloads_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   125919 2023-01-23 15:49:03.000000 google-cloud-assured-workloads-1.9.1/tests/unit/gapic/assuredworkloads_v1beta1/test_assured_workloads_service.py
```

### Comparing `google-cloud-assured-workloads-1.9.0/LICENSE` & `google-cloud-assured-workloads-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/MANIFEST.in` & `google-cloud-assured-workloads-1.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/PKG-INFO` & `google-cloud-assured-workloads-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-assured-workloads
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Assured Workloads API client library
 Home-page: https://github.com/googleapis/python-assured-workloads
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-assured-workloads-1.9.0/README.rst` & `google-cloud-assured-workloads-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads/__init__.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads/gapic_version.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads/gapic_version.py`

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
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/__init__.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/gapic_metadata.json` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/gapic_version.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/gapic_version.py`

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
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/services/__init__.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/services/assured_workloads_service/__init__.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/services/assured_workloads_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/services/assured_workloads_service/async_client.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/services/assured_workloads_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/services/assured_workloads_service/client.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/services/assured_workloads_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1415,15 +1415,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "AssuredWorkloadsServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/services/assured_workloads_service/pagers.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/services/assured_workloads_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/services/assured_workloads_service/transports/__init__.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/services/assured_workloads_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/services/assured_workloads_service/transports/base.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/services/assured_workloads_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/services/assured_workloads_service/transports/grpc.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/services/assured_workloads_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/services/assured_workloads_service/transports/grpc_asyncio.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/services/assured_workloads_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/types/__init__.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1/types/assuredworkloads.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1/types/assuredworkloads.py`

 * *Files 22% similar despite different names*

```diff
@@ -296,15 +296,52 @@
             their environment.".
         partner (google.cloud.assuredworkloads_v1.types.Workload.Partner):
             Optional. Compliance Regime associated with
             this workload.
     """
 
     class ComplianceRegime(proto.Enum):
-        r"""Supported Compliance Regimes."""
+        r"""Supported Compliance Regimes.
+
+        Values:
+            COMPLIANCE_REGIME_UNSPECIFIED (0):
+                Unknown compliance regime.
+            IL4 (1):
+                Information protection as per DoD IL4
+                requirements.
+            CJIS (2):
+                Criminal Justice Information Services (CJIS)
+                Security policies.
+            FEDRAMP_HIGH (3):
+                FedRAMP High data protection controls
+            FEDRAMP_MODERATE (4):
+                FedRAMP Moderate data protection controls
+            US_REGIONAL_ACCESS (5):
+                Assured Workloads For US Regions data
+                protection controls
+            HIPAA (6):
+                Health Insurance Portability and
+                Accountability Act controls
+            HITRUST (7):
+                Health Information Trust Alliance controls
+            EU_REGIONS_AND_SUPPORT (8):
+                Assured Workloads For EU Regions and Support
+                controls
+            CA_REGIONS_AND_SUPPORT (9):
+                Assured Workloads For Canada Regions and
+                Support controls
+            ITAR (10):
+                International Traffic in Arms Regulations
+            AU_REGIONS_AND_US_SUPPORT (11):
+                Assured Workloads for Australia Regions and
+                Support controls Available for public preview
+                consumption. Don't create production workloads.
+            ASSURED_WORKLOADS_FOR_PARTNERS (12):
+                Assured Workloads for Partners
+        """
         COMPLIANCE_REGIME_UNSPECIFIED = 0
         IL4 = 1
         CJIS = 2
         FEDRAMP_HIGH = 3
         FEDRAMP_MODERATE = 4
         US_REGIONAL_ACCESS = 5
         HIPAA = 6
@@ -312,21 +349,37 @@
         EU_REGIONS_AND_SUPPORT = 8
         CA_REGIONS_AND_SUPPORT = 9
         ITAR = 10
         AU_REGIONS_AND_US_SUPPORT = 11
         ASSURED_WORKLOADS_FOR_PARTNERS = 12
 
     class KajEnrollmentState(proto.Enum):
-        r"""Key Access Justifications(KAJ) Enrollment State."""
+        r"""Key Access Justifications(KAJ) Enrollment State.
+
+        Values:
+            KAJ_ENROLLMENT_STATE_UNSPECIFIED (0):
+                Default State for KAJ Enrollment.
+            KAJ_ENROLLMENT_STATE_PENDING (1):
+                Pending State for KAJ Enrollment.
+            KAJ_ENROLLMENT_STATE_COMPLETE (2):
+                Complete State for KAJ Enrollment.
+        """
         KAJ_ENROLLMENT_STATE_UNSPECIFIED = 0
         KAJ_ENROLLMENT_STATE_PENDING = 1
         KAJ_ENROLLMENT_STATE_COMPLETE = 2
 
     class Partner(proto.Enum):
-        r"""Supported Assured Workloads Partners."""
+        r"""Supported Assured Workloads Partners.
+
+        Values:
+            PARTNER_UNSPECIFIED (0):
+                Unknown partner regime/controls.
+            LOCAL_CONTROLS_BY_S3NS (1):
+                S3NS regime/controls.
+        """
         PARTNER_UNSPECIFIED = 0
         LOCAL_CONTROLS_BY_S3NS = 1
 
     class ResourceInfo(proto.Message):
         r"""Represent the resources that are children of this Workload.
 
         Attributes:
@@ -334,15 +387,31 @@
                 Resource identifier. For a project this represents
                 project_number.
             resource_type (google.cloud.assuredworkloads_v1.types.Workload.ResourceInfo.ResourceType):
                 Indicates the type of resource.
         """
 
         class ResourceType(proto.Enum):
-            r"""The type of resource."""
+            r"""The type of resource.
+
+            Values:
+                RESOURCE_TYPE_UNSPECIFIED (0):
+                    Unknown resource type.
+                CONSUMER_PROJECT (1):
+                    Consumer project. AssuredWorkloads Projects are no longer
+                    supported. This field will be ignored only in CreateWorkload
+                    requests. ListWorkloads and GetWorkload will continue to
+                    provide projects information. Use CONSUMER_FOLDER instead.
+                CONSUMER_FOLDER (4):
+                    Consumer Folder.
+                ENCRYPTION_KEYS_PROJECT (2):
+                    Consumer project containing encryption keys.
+                KEYRING (3):
+                    Keyring resource that hosts encryption keys.
+            """
             RESOURCE_TYPE_UNSPECIFIED = 0
             CONSUMER_PROJECT = 1
             CONSUMER_FOLDER = 4
             ENCRYPTION_KEYS_PROJECT = 2
             KEYRING = 3
 
         resource_id: int = proto.Field(
@@ -432,21 +501,48 @@
 
                 This field is a member of `oneof`_ ``_setup_status``.
             setup_errors (MutableSequence[google.cloud.assuredworkloads_v1.types.Workload.SaaEnrollmentResponse.SetupError]):
                 Indicates SAA enrollment setup error if any.
         """
 
         class SetupState(proto.Enum):
-            r"""Setup state of SAA enrollment."""
+            r"""Setup state of SAA enrollment.
+
+            Values:
+                SETUP_STATE_UNSPECIFIED (0):
+                    Unspecified.
+                STATUS_PENDING (1):
+                    SAA enrollment pending.
+                STATUS_COMPLETE (2):
+                    SAA enrollment comopleted.
+            """
             SETUP_STATE_UNSPECIFIED = 0
             STATUS_PENDING = 1
             STATUS_COMPLETE = 2
 
         class SetupError(proto.Enum):
-            r"""Setup error of SAA enrollment."""
+            r"""Setup error of SAA enrollment.
+
+            Values:
+                SETUP_ERROR_UNSPECIFIED (0):
+                    Unspecified.
+                ERROR_INVALID_BASE_SETUP (1):
+                    Invalid states for all customers, to be
+                    redirected to AA UI for additional details.
+                ERROR_MISSING_EXTERNAL_SIGNING_KEY (2):
+                    Returned when there is not an EKM key
+                    configured.
+                ERROR_NOT_ALL_SERVICES_ENROLLED (3):
+                    Returned when there are no enrolled services
+                    or the customer is enrolled in CAA only for a
+                    subset of services.
+                ERROR_SETUP_CHECK_FAILED (4):
+                    Returned when exception was encountered
+                    during evaluation of other criteria.
+            """
             SETUP_ERROR_UNSPECIFIED = 0
             ERROR_INVALID_BASE_SETUP = 1
             ERROR_MISSING_EXTERNAL_SIGNING_KEY = 2
             ERROR_NOT_ALL_SERVICES_ENROLLED = 3
             ERROR_SETUP_CHECK_FAILED = 4
 
         setup_status: "Workload.SaaEnrollmentResponse.SetupState" = proto.Field(
@@ -588,15 +684,30 @@
             "organizations/123/locations/us-east1/workloads/assured-workload-1".
         restriction_type (google.cloud.assuredworkloads_v1.types.RestrictAllowedResourcesRequest.RestrictionType):
             Required. The type of restriction for using
             gcp products in the Workload environment.
     """
 
     class RestrictionType(proto.Enum):
-        r"""The type of restriction."""
+        r"""The type of restriction.
+
+        Values:
+            RESTRICTION_TYPE_UNSPECIFIED (0):
+                Unknown restriction type.
+            ALLOW_ALL_GCP_RESOURCES (1):
+                Allow the use all of all gcp products,
+                irrespective of the compliance posture. This
+                effectively removes gcp.restrictServiceUsage
+                OrgPolicy on the AssuredWorkloads Folder.
+            ALLOW_COMPLIANT_RESOURCES (2):
+                Based on Workload's compliance regime,
+                allowed list changes. See -
+                https://cloud.google.com/assured-workloads/docs/supported-products
+                for the list of supported resources.
+        """
         RESTRICTION_TYPE_UNSPECIFIED = 0
         ALLOW_ALL_GCP_RESOURCES = 1
         ALLOW_COMPLIANT_RESOURCES = 2
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
@@ -819,15 +930,26 @@
             Output only. Immutable. Audit Log link to
             find business justification provided for
             violation exception. Format:
             https://console.cloud.google.com/logs/query;query={logName}{protoPayload.resourceName}{protoPayload.methodName}{timeRange}{organization}
     """
 
     class State(proto.Enum):
-        r"""Violation State Values"""
+        r"""Violation State Values
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                Unspecified state.
+            RESOLVED (2):
+                Violation is resolved.
+            UNRESOLVED (3):
+                Violation is Unresolved
+            EXCEPTION (4):
+                Violation is Exception
+        """
         STATE_UNSPECIFIED = 0
         RESOLVED = 2
         UNRESOLVED = 3
         EXCEPTION = 4
 
     class Remediation(proto.Message):
         r"""Represents remediation guidance to resolve compliance
@@ -849,14 +971,29 @@
 
         class RemediationType(proto.Enum):
             r"""Classifying remediation into various types based on the kind
             of violation. For example, violations caused due to changes in
             boolean org policy requires different remediation instructions
             compared to violation caused due to changes in allowed values of
             list org policy.
+
+            Values:
+                REMEDIATION_TYPE_UNSPECIFIED (0):
+                    Unspecified remediation type
+                REMEDIATION_BOOLEAN_ORG_POLICY_VIOLATION (1):
+                    Remediation type for boolean org policy
+                REMEDIATION_LIST_ALLOWED_VALUES_ORG_POLICY_VIOLATION (2):
+                    Remediation type for list org policy which
+                    have allowed values in the monitoring rule
+                REMEDIATION_LIST_DENIED_VALUES_ORG_POLICY_VIOLATION (3):
+                    Remediation type for list org policy which
+                    have denied values in the monitoring rule
+                REMEDIATION_RESTRICT_CMEK_CRYPTO_KEY_PROJECTS_ORG_POLICY_VIOLATION (4):
+                    Remediation type for
+                    gcp.restrictCmekCryptoKeyProjects
             """
             REMEDIATION_TYPE_UNSPECIFIED = 0
             REMEDIATION_BOOLEAN_ORG_POLICY_VIOLATION = 1
             REMEDIATION_LIST_ALLOWED_VALUES_ORG_POLICY_VIOLATION = 2
             REMEDIATION_LIST_DENIED_VALUES_ORG_POLICY_VIOLATION = 3
             REMEDIATION_RESTRICT_CMEK_CRYPTO_KEY_PROJECTS_ORG_POLICY_VIOLATION = 4
```

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/__init__.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/gapic_metadata.json` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/gapic_version.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/gapic_version.py`

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
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/services/__init__.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/__init__.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/async_client.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/client.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1207,15 +1207,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "AssuredWorkloadsServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/pagers.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/transports/__init__.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/transports/base.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/transports/grpc.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/transports/grpc_asyncio.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/services/assured_workloads_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/types/__init__.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/types/assuredworkloads.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/types/assuredworkloads_v1beta1.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,32 +9,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from typing import MutableMapping, MutableSequence
-
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.assuredworkloads.v1beta1",
     manifest={
         "CreateWorkloadRequest",
         "UpdateWorkloadRequest",
-        "RestrictAllowedResourcesRequest",
-        "RestrictAllowedResourcesResponse",
         "DeleteWorkloadRequest",
         "GetWorkloadRequest",
-        "AnalyzeWorkloadMoveRequest",
-        "AnalyzeWorkloadMoveResponse",
         "ListWorkloadsRequest",
         "ListWorkloadsResponse",
         "Workload",
         "CreateWorkloadOperationMetadata",
     },
 )
 
@@ -54,110 +48,73 @@
             workload and underlying projects which allows
             for the break down of billing costs for a
             workload. The value provided for the identifier
             will add a label to the workload and contained
             projects with the identifier as the value.
     """
 
-    parent: str = proto.Field(
+    parent = proto.Field(
         proto.STRING,
         number=1,
     )
-    workload: "Workload" = proto.Field(
+    workload = proto.Field(
         proto.MESSAGE,
         number=2,
         message="Workload",
     )
-    external_id: str = proto.Field(
+    external_id = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class UpdateWorkloadRequest(proto.Message):
     r"""Request for Updating a workload.
 
     Attributes:
         workload (google.cloud.assuredworkloads_v1beta1.types.Workload):
-            Required. The workload to update. The workload's ``name``
+            Required. The workload to update. The workload’s ``name``
             field is used to identify the workload to be updated.
             Format:
             organizations/{org_id}/locations/{location_id}/workloads/{workload_id}
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. The list of fields to be updated.
     """
 
-    workload: "Workload" = proto.Field(
+    workload = proto.Field(
         proto.MESSAGE,
         number=1,
         message="Workload",
     )
-    update_mask: field_mask_pb2.FieldMask = proto.Field(
+    update_mask = proto.Field(
         proto.MESSAGE,
         number=2,
         message=field_mask_pb2.FieldMask,
     )
 
 
-class RestrictAllowedResourcesRequest(proto.Message):
-    r"""Request for restricting list of available resources in
-    Workload environment.
-
-    Attributes:
-        name (str):
-            Required. The resource name of the Workload. This is the
-            workloads's relative path in the API, formatted as
-            "organizations/{organization_id}/locations/{location_id}/workloads/{workload_id}".
-            For example,
-            "organizations/123/locations/us-east1/workloads/assured-workload-1".
-        restriction_type (google.cloud.assuredworkloads_v1beta1.types.RestrictAllowedResourcesRequest.RestrictionType):
-            Required. The type of restriction for using
-            gcp products in the Workload environment.
-    """
-
-    class RestrictionType(proto.Enum):
-        r"""The type of restriction."""
-        RESTRICTION_TYPE_UNSPECIFIED = 0
-        ALLOW_ALL_GCP_RESOURCES = 1
-        ALLOW_COMPLIANT_RESOURCES = 2
-
-    name: str = proto.Field(
-        proto.STRING,
-        number=1,
-    )
-    restriction_type: RestrictionType = proto.Field(
-        proto.ENUM,
-        number=2,
-        enum=RestrictionType,
-    )
-
-
-class RestrictAllowedResourcesResponse(proto.Message):
-    r"""Response for restricting the list of allowed resources."""
-
-
 class DeleteWorkloadRequest(proto.Message):
     r"""Request for deleting a Workload.
 
     Attributes:
         name (str):
             Required. The ``name`` field is used to identify the
             workload. Format:
             organizations/{org_id}/locations/{location_id}/workloads/{workload_id}
         etag (str):
             Optional. The etag of the workload.
             If this is provided, it must match the server's
             etag.
     """
 
-    name: str = proto.Field(
+    name = proto.Field(
         proto.STRING,
         number=1,
     )
-    etag: str = proto.Field(
+    etag = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class GetWorkloadRequest(proto.Message):
     r"""Request for fetching a workload.
@@ -167,89 +124,15 @@
             Required. The resource name of the Workload to fetch. This
             is the workloads's relative path in the API, formatted as
             "organizations/{organization_id}/locations/{location_id}/workloads/{workload_id}".
             For example,
             "organizations/123/locations/us-east1/workloads/assured-workload-1".
     """
 
-    name: str = proto.Field(
-        proto.STRING,
-        number=1,
-    )
-
-
-class AnalyzeWorkloadMoveRequest(proto.Message):
-    r"""A request to analyze a hypothetical move of a source project
-    or project-based workload to a target (destination) folder-based
-    workload.
-
-    This message has `oneof`_ fields (mutually exclusive fields).
-    For each oneof, at most one member field can be set at the same time.
-    Setting any member of the oneof automatically clears all other
-    members.
-
-    .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
-
-    Attributes:
-        source (str):
-            The source type is a project-based workload. Specify the
-            workloads's relative resource name, formatted as:
-            "organizations/{ORGANIZATION_ID}/locations/{LOCATION_ID}/workloads/{WORKLOAD_ID}"
-            For example:
-            "organizations/123/locations/us-east1/workloads/assured-workload-1".
-
-            This field is a member of `oneof`_ ``projectOrWorkloadResource``.
-        project (str):
-            The source type is a project. Specify the project's relative
-            resource name, formatted as either a project number or a
-            project ID: "projects/{PROJECT_NUMBER}" or
-            "projects/{PROJECT_ID}" For example: "projects/951040570662"
-            when specifying a project number, or
-            "projects/my-project-123" when specifying a project ID.
-
-            This field is a member of `oneof`_ ``projectOrWorkloadResource``.
-        target (str):
-            Required. The resource ID of the folder-based destination
-            workload. This workload is where the source project will
-            hypothetically be moved to. Specify the workload's relative
-            resource name, formatted as:
-            "organizations/{ORGANIZATION_ID}/locations/{LOCATION_ID}/workloads/{WORKLOAD_ID}"
-            For example:
-            "organizations/123/locations/us-east1/workloads/assured-workload-2".
-    """
-
-    source: str = proto.Field(
-        proto.STRING,
-        number=1,
-        oneof="projectOrWorkloadResource",
-    )
-    project: str = proto.Field(
-        proto.STRING,
-        number=3,
-        oneof="projectOrWorkloadResource",
-    )
-    target: str = proto.Field(
-        proto.STRING,
-        number=2,
-    )
-
-
-class AnalyzeWorkloadMoveResponse(proto.Message):
-    r"""A response that includes the analysis of the hypothetical
-    resource move.
-
-    Attributes:
-        blockers (MutableSequence[str]):
-            A list of blockers that should be addressed
-            before moving the source project or
-            project-based workload to the destination
-            folder-based workload.
-    """
-
-    blockers: MutableSequence[str] = proto.RepeatedField(
+    name = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ListWorkloadsRequest(proto.Message):
     r"""Request for fetching workloads in an organization.
@@ -267,53 +150,53 @@
             second and following requests.
         filter (str):
             A custom filter for filtering by properties
             of a workload. At this time, only filtering by
             labels is supported.
     """
 
-    parent: str = proto.Field(
+    parent = proto.Field(
         proto.STRING,
         number=1,
     )
-    page_size: int = proto.Field(
+    page_size = proto.Field(
         proto.INT32,
         number=2,
     )
-    page_token: str = proto.Field(
+    page_token = proto.Field(
         proto.STRING,
         number=3,
     )
-    filter: str = proto.Field(
+    filter = proto.Field(
         proto.STRING,
         number=4,
     )
 
 
 class ListWorkloadsResponse(proto.Message):
     r"""Response of ListWorkloads endpoint.
 
     Attributes:
-        workloads (MutableSequence[google.cloud.assuredworkloads_v1beta1.types.Workload]):
+        workloads (Sequence[google.cloud.assuredworkloads_v1beta1.types.Workload]):
             List of Workloads under a given parent.
         next_page_token (str):
             The next page token. Return empty if reached
             the last page.
     """
 
     @property
     def raw_page(self):
         return self
 
-    workloads: MutableSequence["Workload"] = proto.RepeatedField(
+    workloads = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="Workload",
     )
-    next_page_token: str = proto.Field(
+    next_page_token = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class Workload(proto.Message):
     r"""An Workload object for managing highly regulated workloads of
@@ -336,75 +219,75 @@
             Required. The user-assigned display name of
             the Workload. When present it must be between 4
             to 30 characters. Allowed characters are:
             lowercase and uppercase letters, numbers,
             hyphen, and spaces.
 
             Example: My Workload
-        resources (MutableSequence[google.cloud.assuredworkloads_v1beta1.types.Workload.ResourceInfo]):
+        resources (Sequence[google.cloud.assuredworkloads_v1beta1.types.Workload.ResourceInfo]):
             Output only. The resources associated with
             this workload. These resources will be created
             when creating the workload. If any of the
             projects already exist, the workload creation
             will fail. Always read only.
         compliance_regime (google.cloud.assuredworkloads_v1beta1.types.Workload.ComplianceRegime):
             Required. Immutable. Compliance Regime
             associated with this workload.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Immutable. The Workload creation
             timestamp.
         billing_account (str):
-            Output only. The billing account used for the resources
-            which are direct children of workload. This billing account
-            is initially associated with the resources created as part
-            of Workload creation. After the initial creation of these
+            Input only. The billing account used for the resources which
+            are direct children of workload. This billing account is
+            initially associated with the resources created as part of
+            Workload creation. After the initial creation of these
             resources, the customer can change the assigned billing
             account. The resource name has the form
             ``billingAccounts/{billing_account_id}``. For example,
             ``billingAccounts/012345-567890-ABCDEF``.
         il4_settings (google.cloud.assuredworkloads_v1beta1.types.Workload.IL4Settings):
-            Input only. Immutable. Settings specific to
-            resources needed for IL4.
+            Required. Input only. Immutable. Settings
+            specific to resources needed for IL4.
 
             This field is a member of `oneof`_ ``compliance_regime_settings``.
         cjis_settings (google.cloud.assuredworkloads_v1beta1.types.Workload.CJISSettings):
-            Input only. Immutable. Settings specific to
-            resources needed for CJIS.
+            Required. Input only. Immutable. Settings
+            specific to resources needed for CJIS.
 
             This field is a member of `oneof`_ ``compliance_regime_settings``.
         fedramp_high_settings (google.cloud.assuredworkloads_v1beta1.types.Workload.FedrampHighSettings):
-            Input only. Immutable. Settings specific to
-            resources needed for FedRAMP High.
+            Required. Input only. Immutable. Settings
+            specific to resources needed for FedRAMP High.
 
             This field is a member of `oneof`_ ``compliance_regime_settings``.
         fedramp_moderate_settings (google.cloud.assuredworkloads_v1beta1.types.Workload.FedrampModerateSettings):
-            Input only. Immutable. Settings specific to
-            resources needed for FedRAMP Moderate.
+            Required. Input only. Immutable. Settings
+            specific to resources needed for FedRAMP
+            Moderate.
 
             This field is a member of `oneof`_ ``compliance_regime_settings``.
         etag (str):
             Optional. ETag of the workload, it is
             calculated on the basis of the Workload
             contents. It will be used in Update & Delete
             operations.
-        labels (MutableMapping[str, str]):
+        labels (Mapping[str, str]):
             Optional. Labels applied to the workload.
         provisioned_resources_parent (str):
             Input only. The parent resource for the resources managed by
             this Assured Workload. May be either empty or a folder
             resource which is a child of the Workload parent. If not
             specified all resources are created under the parent
             organization. Format: folders/{folder_id}
         kms_settings (google.cloud.assuredworkloads_v1beta1.types.Workload.KMSSettings):
-            Input only. Settings used to create a CMEK crypto key. When
-            set, a project with a KMS CMEK key is provisioned. This
-            field is deprecated as of Feb 28, 2022. In order to create a
-            Keyring, callers should specify, ENCRYPTION_KEYS_PROJECT or
-            KEYRING in ResourceSettings.resource_type field.
-        resource_settings (MutableSequence[google.cloud.assuredworkloads_v1beta1.types.Workload.ResourceSettings]):
+            Input only. Settings used to create a CMEK
+            crypto key. When set a project with a KMS CMEK
+            key is provisioned. This field is mandatory for
+            a subset of Compliance Regimes.
+        resource_settings (Sequence[google.cloud.assuredworkloads_v1beta1.types.Workload.ResourceSettings]):
             Input only. Resource properties that are used
             to customize workload resources. These
             properties (such as custom project id) will be
             used to create workload resources if possible.
             This field is optional.
         kaj_enrollment_state (google.cloud.assuredworkloads_v1beta1.types.Workload.KajEnrollmentState):
             Output only. Represents the KAJ enrollment
@@ -415,38 +298,28 @@
             by Europe/Canada customers.
         saa_enrollment_response (google.cloud.assuredworkloads_v1beta1.types.Workload.SaaEnrollmentResponse):
             Output only. Represents the SAA enrollment
             response of the given workload. SAA enrollment
             response is queried during GetWorkload call. In
             failure cases, user friendly error message is
             shown in SAA details page.
-        compliant_but_disallowed_services (MutableSequence[str]):
-            Output only. Urls for services which are
-            compliant for this Assured Workload, but which
-            are currently disallowed by the
-            ResourceUsageRestriction org policy. Invoke
-            RestrictAllowedResources endpoint to allow your
-            project developers to use these services in
-            their environment.".
     """
 
     class ComplianceRegime(proto.Enum):
         r"""Supported Compliance Regimes."""
         COMPLIANCE_REGIME_UNSPECIFIED = 0
         IL4 = 1
         CJIS = 2
         FEDRAMP_HIGH = 3
         FEDRAMP_MODERATE = 4
         US_REGIONAL_ACCESS = 5
         HIPAA = 6
         HITRUST = 7
         EU_REGIONS_AND_SUPPORT = 8
         CA_REGIONS_AND_SUPPORT = 9
-        ITAR = 10
-        AU_REGIONS_AND_US_SUPPORT = 11
 
     class KajEnrollmentState(proto.Enum):
         r"""Key Access Justifications(KAJ) Enrollment State."""
         KAJ_ENROLLMENT_STATE_UNSPECIFIED = 0
         KAJ_ENROLLMENT_STATE_PENDING = 1
         KAJ_ENROLLMENT_STATE_COMPLETE = 2
 
@@ -465,19 +338,19 @@
             r"""The type of resource."""
             RESOURCE_TYPE_UNSPECIFIED = 0
             CONSUMER_PROJECT = 1
             CONSUMER_FOLDER = 4
             ENCRYPTION_KEYS_PROJECT = 2
             KEYRING = 3
 
-        resource_id: int = proto.Field(
+        resource_id = proto.Field(
             proto.INT64,
             number=1,
         )
-        resource_type: "Workload.ResourceInfo.ResourceType" = proto.Field(
+        resource_type = proto.Field(
             proto.ENUM,
             number=2,
             enum="Workload.ResourceInfo.ResourceType",
         )
 
     class KMSSettings(proto.Message):
         r"""Settings specific to the Key Management Service.
@@ -491,132 +364,128 @@
             rotation_period (google.protobuf.duration_pb2.Duration):
                 Required. Input only. Immutable. [next_rotation_time] will
                 be advanced by this period when the Key Management Service
                 automatically rotates a key. Must be at least 24 hours and
                 at most 876,000 hours.
         """
 
-        next_rotation_time: timestamp_pb2.Timestamp = proto.Field(
+        next_rotation_time = proto.Field(
             proto.MESSAGE,
             number=1,
             message=timestamp_pb2.Timestamp,
         )
-        rotation_period: duration_pb2.Duration = proto.Field(
+        rotation_period = proto.Field(
             proto.MESSAGE,
             number=2,
             message=duration_pb2.Duration,
         )
 
     class IL4Settings(proto.Message):
         r"""Settings specific to resources needed for IL4.
 
         Attributes:
             kms_settings (google.cloud.assuredworkloads_v1beta1.types.Workload.KMSSettings):
-                Input only. Immutable. Settings used to
-                create a CMEK crypto key.
+                Required. Input only. Immutable. Settings
+                used to create a CMEK crypto key.
         """
 
-        kms_settings: "Workload.KMSSettings" = proto.Field(
+        kms_settings = proto.Field(
             proto.MESSAGE,
             number=1,
             message="Workload.KMSSettings",
         )
 
     class CJISSettings(proto.Message):
         r"""Settings specific to resources needed for CJIS.
 
         Attributes:
             kms_settings (google.cloud.assuredworkloads_v1beta1.types.Workload.KMSSettings):
-                Input only. Immutable. Settings used to
-                create a CMEK crypto key.
+                Required. Input only. Immutable. Settings
+                used to create a CMEK crypto key.
         """
 
-        kms_settings: "Workload.KMSSettings" = proto.Field(
+        kms_settings = proto.Field(
             proto.MESSAGE,
             number=1,
             message="Workload.KMSSettings",
         )
 
     class FedrampHighSettings(proto.Message):
         r"""Settings specific to resources needed for FedRAMP High.
 
         Attributes:
             kms_settings (google.cloud.assuredworkloads_v1beta1.types.Workload.KMSSettings):
-                Input only. Immutable. Settings used to
-                create a CMEK crypto key.
+                Required. Input only. Immutable. Settings
+                used to create a CMEK crypto key.
         """
 
-        kms_settings: "Workload.KMSSettings" = proto.Field(
+        kms_settings = proto.Field(
             proto.MESSAGE,
             number=1,
             message="Workload.KMSSettings",
         )
 
     class FedrampModerateSettings(proto.Message):
         r"""Settings specific to resources needed for FedRAMP Moderate.
 
         Attributes:
             kms_settings (google.cloud.assuredworkloads_v1beta1.types.Workload.KMSSettings):
-                Input only. Immutable. Settings used to
-                create a CMEK crypto key.
+                Required. Input only. Immutable. Settings
+                used to create a CMEK crypto key.
         """
 
-        kms_settings: "Workload.KMSSettings" = proto.Field(
+        kms_settings = proto.Field(
             proto.MESSAGE,
             number=1,
             message="Workload.KMSSettings",
         )
 
     class ResourceSettings(proto.Message):
         r"""Represent the custom settings for the resources to be
         created.
 
         Attributes:
             resource_id (str):
                 Resource identifier. For a project this represents
                 project_id. If the project is already taken, the workload
-                creation will fail. For KeyRing, this represents the
-                keyring_id. For a folder, don't set this value as folder_id
-                is assigned by Google.
+                creation will fail.
             resource_type (google.cloud.assuredworkloads_v1beta1.types.Workload.ResourceInfo.ResourceType):
                 Indicates the type of resource. This field should be
                 specified to correspond the id to the right project type
                 (CONSUMER_PROJECT or ENCRYPTION_KEYS_PROJECT)
             display_name (str):
                 User-assigned resource display name.
                 If not empty it will be used to create a
                 resource with the specified name.
         """
 
-        resource_id: str = proto.Field(
+        resource_id = proto.Field(
             proto.STRING,
             number=1,
         )
-        resource_type: "Workload.ResourceInfo.ResourceType" = proto.Field(
+        resource_type = proto.Field(
             proto.ENUM,
             number=2,
             enum="Workload.ResourceInfo.ResourceType",
         )
-        display_name: str = proto.Field(
+        display_name = proto.Field(
             proto.STRING,
             number=3,
         )
 
     class SaaEnrollmentResponse(proto.Message):
         r"""Signed Access Approvals (SAA) enrollment response.
 
-        .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
-
         Attributes:
             setup_status (google.cloud.assuredworkloads_v1beta1.types.Workload.SaaEnrollmentResponse.SetupState):
                 Indicates SAA enrollment status of a given
                 workload.
 
                 This field is a member of `oneof`_ ``_setup_status``.
-            setup_errors (MutableSequence[google.cloud.assuredworkloads_v1beta1.types.Workload.SaaEnrollmentResponse.SetupError]):
+            setup_errors (Sequence[google.cloud.assuredworkloads_v1beta1.types.Workload.SaaEnrollmentResponse.SetupError]):
                 Indicates SAA enrollment setup error if any.
         """
 
         class SetupState(proto.Enum):
             r"""Setup state of SAA enrollment."""
             SETUP_STATE_UNSPECIFIED = 0
             STATUS_PENDING = 1
@@ -626,120 +495,114 @@
             r"""Setup error of SAA enrollment."""
             SETUP_ERROR_UNSPECIFIED = 0
             ERROR_INVALID_BASE_SETUP = 1
             ERROR_MISSING_EXTERNAL_SIGNING_KEY = 2
             ERROR_NOT_ALL_SERVICES_ENROLLED = 3
             ERROR_SETUP_CHECK_FAILED = 4
 
-        setup_status: "Workload.SaaEnrollmentResponse.SetupState" = proto.Field(
+        setup_status = proto.Field(
             proto.ENUM,
             number=1,
             optional=True,
             enum="Workload.SaaEnrollmentResponse.SetupState",
         )
-        setup_errors: MutableSequence[
-            "Workload.SaaEnrollmentResponse.SetupError"
-        ] = proto.RepeatedField(
+        setup_errors = proto.RepeatedField(
             proto.ENUM,
             number=2,
             enum="Workload.SaaEnrollmentResponse.SetupError",
         )
 
-    name: str = proto.Field(
+    name = proto.Field(
         proto.STRING,
         number=1,
     )
-    display_name: str = proto.Field(
+    display_name = proto.Field(
         proto.STRING,
         number=2,
     )
-    resources: MutableSequence[ResourceInfo] = proto.RepeatedField(
+    resources = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message=ResourceInfo,
     )
-    compliance_regime: ComplianceRegime = proto.Field(
+    compliance_regime = proto.Field(
         proto.ENUM,
         number=4,
         enum=ComplianceRegime,
     )
-    create_time: timestamp_pb2.Timestamp = proto.Field(
+    create_time = proto.Field(
         proto.MESSAGE,
         number=5,
         message=timestamp_pb2.Timestamp,
     )
-    billing_account: str = proto.Field(
+    billing_account = proto.Field(
         proto.STRING,
         number=6,
     )
-    il4_settings: IL4Settings = proto.Field(
+    il4_settings = proto.Field(
         proto.MESSAGE,
         number=7,
         oneof="compliance_regime_settings",
         message=IL4Settings,
     )
-    cjis_settings: CJISSettings = proto.Field(
+    cjis_settings = proto.Field(
         proto.MESSAGE,
         number=8,
         oneof="compliance_regime_settings",
         message=CJISSettings,
     )
-    fedramp_high_settings: FedrampHighSettings = proto.Field(
+    fedramp_high_settings = proto.Field(
         proto.MESSAGE,
         number=11,
         oneof="compliance_regime_settings",
         message=FedrampHighSettings,
     )
-    fedramp_moderate_settings: FedrampModerateSettings = proto.Field(
+    fedramp_moderate_settings = proto.Field(
         proto.MESSAGE,
         number=12,
         oneof="compliance_regime_settings",
         message=FedrampModerateSettings,
     )
-    etag: str = proto.Field(
+    etag = proto.Field(
         proto.STRING,
         number=9,
     )
-    labels: MutableMapping[str, str] = proto.MapField(
+    labels = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=10,
     )
-    provisioned_resources_parent: str = proto.Field(
+    provisioned_resources_parent = proto.Field(
         proto.STRING,
         number=13,
     )
-    kms_settings: KMSSettings = proto.Field(
+    kms_settings = proto.Field(
         proto.MESSAGE,
         number=14,
         message=KMSSettings,
     )
-    resource_settings: MutableSequence[ResourceSettings] = proto.RepeatedField(
+    resource_settings = proto.RepeatedField(
         proto.MESSAGE,
         number=15,
         message=ResourceSettings,
     )
-    kaj_enrollment_state: KajEnrollmentState = proto.Field(
+    kaj_enrollment_state = proto.Field(
         proto.ENUM,
         number=17,
         enum=KajEnrollmentState,
     )
-    enable_sovereign_controls: bool = proto.Field(
+    enable_sovereign_controls = proto.Field(
         proto.BOOL,
         number=18,
     )
-    saa_enrollment_response: SaaEnrollmentResponse = proto.Field(
+    saa_enrollment_response = proto.Field(
         proto.MESSAGE,
         number=20,
         message=SaaEnrollmentResponse,
     )
-    compliant_but_disallowed_services: MutableSequence[str] = proto.RepeatedField(
-        proto.STRING,
-        number=24,
-    )
 
 
 class CreateWorkloadOperationMetadata(proto.Message):
     r"""Operation metadata to give request details of CreateWorkload.
 
     Attributes:
         create_time (google.protobuf.timestamp_pb2.Timestamp):
@@ -749,41 +612,39 @@
             Optional. The display name of the workload.
         parent (str):
             Optional. The parent of the workload.
         compliance_regime (google.cloud.assuredworkloads_v1beta1.types.Workload.ComplianceRegime):
             Optional. Compliance controls that should be
             applied to the resources managed by the
             workload.
-        resource_settings (MutableSequence[google.cloud.assuredworkloads_v1beta1.types.Workload.ResourceSettings]):
+        resource_settings (Sequence[google.cloud.assuredworkloads_v1beta1.types.Workload.ResourceSettings]):
             Optional. Resource properties in the input
             that are used for creating/customizing workload
             resources.
     """
 
-    create_time: timestamp_pb2.Timestamp = proto.Field(
+    create_time = proto.Field(
         proto.MESSAGE,
         number=1,
         message=timestamp_pb2.Timestamp,
     )
-    display_name: str = proto.Field(
+    display_name = proto.Field(
         proto.STRING,
         number=2,
     )
-    parent: str = proto.Field(
+    parent = proto.Field(
         proto.STRING,
         number=3,
     )
-    compliance_regime: "Workload.ComplianceRegime" = proto.Field(
+    compliance_regime = proto.Field(
         proto.ENUM,
         number=4,
         enum="Workload.ComplianceRegime",
     )
-    resource_settings: MutableSequence[
-        "Workload.ResourceSettings"
-    ] = proto.RepeatedField(
+    resource_settings = proto.RepeatedField(
         proto.MESSAGE,
         number=5,
         message="Workload.ResourceSettings",
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/types/assuredworkloads_service.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/types/assuredworkloads_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/google/cloud/assuredworkloads_v1beta1/types/assuredworkloads_v1beta1.py` & `google-cloud-assured-workloads-1.9.1/google/cloud/assuredworkloads_v1beta1/types/assuredworkloads.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,26 +9,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.assuredworkloads.v1beta1",
     manifest={
         "CreateWorkloadRequest",
         "UpdateWorkloadRequest",
+        "RestrictAllowedResourcesRequest",
+        "RestrictAllowedResourcesResponse",
         "DeleteWorkloadRequest",
         "GetWorkloadRequest",
+        "AnalyzeWorkloadMoveRequest",
+        "AnalyzeWorkloadMoveResponse",
         "ListWorkloadsRequest",
         "ListWorkloadsResponse",
         "Workload",
         "CreateWorkloadOperationMetadata",
     },
 )
 
@@ -48,73 +54,125 @@
             workload and underlying projects which allows
             for the break down of billing costs for a
             workload. The value provided for the identifier
             will add a label to the workload and contained
             projects with the identifier as the value.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    workload = proto.Field(
+    workload: "Workload" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="Workload",
     )
-    external_id = proto.Field(
+    external_id: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class UpdateWorkloadRequest(proto.Message):
     r"""Request for Updating a workload.
 
     Attributes:
         workload (google.cloud.assuredworkloads_v1beta1.types.Workload):
-            Required. The workload to update. The workload’s ``name``
+            Required. The workload to update. The workload's ``name``
             field is used to identify the workload to be updated.
             Format:
             organizations/{org_id}/locations/{location_id}/workloads/{workload_id}
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. The list of fields to be updated.
     """
 
-    workload = proto.Field(
+    workload: "Workload" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="Workload",
     )
-    update_mask = proto.Field(
+    update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=2,
         message=field_mask_pb2.FieldMask,
     )
 
 
+class RestrictAllowedResourcesRequest(proto.Message):
+    r"""Request for restricting list of available resources in
+    Workload environment.
+
+    Attributes:
+        name (str):
+            Required. The resource name of the Workload. This is the
+            workloads's relative path in the API, formatted as
+            "organizations/{organization_id}/locations/{location_id}/workloads/{workload_id}".
+            For example,
+            "organizations/123/locations/us-east1/workloads/assured-workload-1".
+        restriction_type (google.cloud.assuredworkloads_v1beta1.types.RestrictAllowedResourcesRequest.RestrictionType):
+            Required. The type of restriction for using
+            gcp products in the Workload environment.
+    """
+
+    class RestrictionType(proto.Enum):
+        r"""The type of restriction.
+
+        Values:
+            RESTRICTION_TYPE_UNSPECIFIED (0):
+                Unknown restriction type.
+            ALLOW_ALL_GCP_RESOURCES (1):
+                Allow the use all of all gcp products,
+                irrespective of the compliance posture. This
+                effectively removes gcp.restrictServiceUsage
+                OrgPolicy on the AssuredWorkloads Folder.
+            ALLOW_COMPLIANT_RESOURCES (2):
+                Based on Workload's compliance regime,
+                allowed list changes. See -
+                https://cloud.google.com/assured-workloads/docs/supported-products
+                for the list of supported resources.
+        """
+        RESTRICTION_TYPE_UNSPECIFIED = 0
+        ALLOW_ALL_GCP_RESOURCES = 1
+        ALLOW_COMPLIANT_RESOURCES = 2
+
+    name: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    restriction_type: RestrictionType = proto.Field(
+        proto.ENUM,
+        number=2,
+        enum=RestrictionType,
+    )
+
+
+class RestrictAllowedResourcesResponse(proto.Message):
+    r"""Response for restricting the list of allowed resources."""
+
+
 class DeleteWorkloadRequest(proto.Message):
     r"""Request for deleting a Workload.
 
     Attributes:
         name (str):
             Required. The ``name`` field is used to identify the
             workload. Format:
             organizations/{org_id}/locations/{location_id}/workloads/{workload_id}
         etag (str):
             Optional. The etag of the workload.
             If this is provided, it must match the server's
             etag.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class GetWorkloadRequest(proto.Message):
     r"""Request for fetching a workload.
@@ -124,15 +182,89 @@
             Required. The resource name of the Workload to fetch. This
             is the workloads's relative path in the API, formatted as
             "organizations/{organization_id}/locations/{location_id}/workloads/{workload_id}".
             For example,
             "organizations/123/locations/us-east1/workloads/assured-workload-1".
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+
+
+class AnalyzeWorkloadMoveRequest(proto.Message):
+    r"""A request to analyze a hypothetical move of a source project
+    or project-based workload to a target (destination) folder-based
+    workload.
+
+    This message has `oneof`_ fields (mutually exclusive fields).
+    For each oneof, at most one member field can be set at the same time.
+    Setting any member of the oneof automatically clears all other
+    members.
+
+    .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
+
+    Attributes:
+        source (str):
+            The source type is a project-based workload. Specify the
+            workloads's relative resource name, formatted as:
+            "organizations/{ORGANIZATION_ID}/locations/{LOCATION_ID}/workloads/{WORKLOAD_ID}"
+            For example:
+            "organizations/123/locations/us-east1/workloads/assured-workload-1".
+
+            This field is a member of `oneof`_ ``projectOrWorkloadResource``.
+        project (str):
+            The source type is a project. Specify the project's relative
+            resource name, formatted as either a project number or a
+            project ID: "projects/{PROJECT_NUMBER}" or
+            "projects/{PROJECT_ID}" For example: "projects/951040570662"
+            when specifying a project number, or
+            "projects/my-project-123" when specifying a project ID.
+
+            This field is a member of `oneof`_ ``projectOrWorkloadResource``.
+        target (str):
+            Required. The resource ID of the folder-based destination
+            workload. This workload is where the source project will
+            hypothetically be moved to. Specify the workload's relative
+            resource name, formatted as:
+            "organizations/{ORGANIZATION_ID}/locations/{LOCATION_ID}/workloads/{WORKLOAD_ID}"
+            For example:
+            "organizations/123/locations/us-east1/workloads/assured-workload-2".
+    """
+
+    source: str = proto.Field(
+        proto.STRING,
+        number=1,
+        oneof="projectOrWorkloadResource",
+    )
+    project: str = proto.Field(
+        proto.STRING,
+        number=3,
+        oneof="projectOrWorkloadResource",
+    )
+    target: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+
+
+class AnalyzeWorkloadMoveResponse(proto.Message):
+    r"""A response that includes the analysis of the hypothetical
+    resource move.
+
+    Attributes:
+        blockers (MutableSequence[str]):
+            A list of blockers that should be addressed
+            before moving the source project or
+            project-based workload to the destination
+            folder-based workload.
+    """
+
+    blockers: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=1,
     )
 
 
 class ListWorkloadsRequest(proto.Message):
     r"""Request for fetching workloads in an organization.
@@ -150,53 +282,53 @@
             second and following requests.
         filter (str):
             A custom filter for filtering by properties
             of a workload. At this time, only filtering by
             labels is supported.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    page_size = proto.Field(
+    page_size: int = proto.Field(
         proto.INT32,
         number=2,
     )
-    page_token = proto.Field(
+    page_token: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    filter = proto.Field(
+    filter: str = proto.Field(
         proto.STRING,
         number=4,
     )
 
 
 class ListWorkloadsResponse(proto.Message):
     r"""Response of ListWorkloads endpoint.
 
     Attributes:
-        workloads (Sequence[google.cloud.assuredworkloads_v1beta1.types.Workload]):
+        workloads (MutableSequence[google.cloud.assuredworkloads_v1beta1.types.Workload]):
             List of Workloads under a given parent.
         next_page_token (str):
             The next page token. Return empty if reached
             the last page.
     """
 
     @property
     def raw_page(self):
         return self
 
-    workloads = proto.RepeatedField(
+    workloads: MutableSequence["Workload"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="Workload",
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class Workload(proto.Message):
     r"""An Workload object for managing highly regulated workloads of
@@ -219,75 +351,75 @@
             Required. The user-assigned display name of
             the Workload. When present it must be between 4
             to 30 characters. Allowed characters are:
             lowercase and uppercase letters, numbers,
             hyphen, and spaces.
 
             Example: My Workload
-        resources (Sequence[google.cloud.assuredworkloads_v1beta1.types.Workload.ResourceInfo]):
+        resources (MutableSequence[google.cloud.assuredworkloads_v1beta1.types.Workload.ResourceInfo]):
             Output only. The resources associated with
             this workload. These resources will be created
             when creating the workload. If any of the
             projects already exist, the workload creation
             will fail. Always read only.
         compliance_regime (google.cloud.assuredworkloads_v1beta1.types.Workload.ComplianceRegime):
             Required. Immutable. Compliance Regime
             associated with this workload.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Immutable. The Workload creation
             timestamp.
         billing_account (str):
-            Input only. The billing account used for the resources which
-            are direct children of workload. This billing account is
-            initially associated with the resources created as part of
-            Workload creation. After the initial creation of these
+            Output only. The billing account used for the resources
+            which are direct children of workload. This billing account
+            is initially associated with the resources created as part
+            of Workload creation. After the initial creation of these
             resources, the customer can change the assigned billing
             account. The resource name has the form
             ``billingAccounts/{billing_account_id}``. For example,
             ``billingAccounts/012345-567890-ABCDEF``.
         il4_settings (google.cloud.assuredworkloads_v1beta1.types.Workload.IL4Settings):
-            Required. Input only. Immutable. Settings
-            specific to resources needed for IL4.
+            Input only. Immutable. Settings specific to
+            resources needed for IL4.
 
             This field is a member of `oneof`_ ``compliance_regime_settings``.
         cjis_settings (google.cloud.assuredworkloads_v1beta1.types.Workload.CJISSettings):
-            Required. Input only. Immutable. Settings
-            specific to resources needed for CJIS.
+            Input only. Immutable. Settings specific to
+            resources needed for CJIS.
 
             This field is a member of `oneof`_ ``compliance_regime_settings``.
         fedramp_high_settings (google.cloud.assuredworkloads_v1beta1.types.Workload.FedrampHighSettings):
-            Required. Input only. Immutable. Settings
-            specific to resources needed for FedRAMP High.
+            Input only. Immutable. Settings specific to
+            resources needed for FedRAMP High.
 
             This field is a member of `oneof`_ ``compliance_regime_settings``.
         fedramp_moderate_settings (google.cloud.assuredworkloads_v1beta1.types.Workload.FedrampModerateSettings):
-            Required. Input only. Immutable. Settings
-            specific to resources needed for FedRAMP
-            Moderate.
+            Input only. Immutable. Settings specific to
+            resources needed for FedRAMP Moderate.
 
             This field is a member of `oneof`_ ``compliance_regime_settings``.
         etag (str):
             Optional. ETag of the workload, it is
             calculated on the basis of the Workload
             contents. It will be used in Update & Delete
             operations.
-        labels (Mapping[str, str]):
+        labels (MutableMapping[str, str]):
             Optional. Labels applied to the workload.
         provisioned_resources_parent (str):
             Input only. The parent resource for the resources managed by
             this Assured Workload. May be either empty or a folder
             resource which is a child of the Workload parent. If not
             specified all resources are created under the parent
             organization. Format: folders/{folder_id}
         kms_settings (google.cloud.assuredworkloads_v1beta1.types.Workload.KMSSettings):
-            Input only. Settings used to create a CMEK
-            crypto key. When set a project with a KMS CMEK
-            key is provisioned. This field is mandatory for
-            a subset of Compliance Regimes.
-        resource_settings (Sequence[google.cloud.assuredworkloads_v1beta1.types.Workload.ResourceSettings]):
+            Input only. Settings used to create a CMEK crypto key. When
+            set, a project with a KMS CMEK key is provisioned. This
+            field is deprecated as of Feb 28, 2022. In order to create a
+            Keyring, callers should specify, ENCRYPTION_KEYS_PROJECT or
+            KEYRING in ResourceSettings.resource_type field.
+        resource_settings (MutableSequence[google.cloud.assuredworkloads_v1beta1.types.Workload.ResourceSettings]):
             Input only. Resource properties that are used
             to customize workload resources. These
             properties (such as custom project id) will be
             used to create workload resources if possible.
             This field is optional.
         kaj_enrollment_state (google.cloud.assuredworkloads_v1beta1.types.Workload.KajEnrollmentState):
             Output only. Represents the KAJ enrollment
@@ -298,31 +430,84 @@
             by Europe/Canada customers.
         saa_enrollment_response (google.cloud.assuredworkloads_v1beta1.types.Workload.SaaEnrollmentResponse):
             Output only. Represents the SAA enrollment
             response of the given workload. SAA enrollment
             response is queried during GetWorkload call. In
             failure cases, user friendly error message is
             shown in SAA details page.
+        compliant_but_disallowed_services (MutableSequence[str]):
+            Output only. Urls for services which are
+            compliant for this Assured Workload, but which
+            are currently disallowed by the
+            ResourceUsageRestriction org policy. Invoke
+            RestrictAllowedResources endpoint to allow your
+            project developers to use these services in
+            their environment.".
     """
 
     class ComplianceRegime(proto.Enum):
-        r"""Supported Compliance Regimes."""
+        r"""Supported Compliance Regimes.
+
+        Values:
+            COMPLIANCE_REGIME_UNSPECIFIED (0):
+                Unknown compliance regime.
+            IL4 (1):
+                Information protection as per DoD IL4
+                requirements.
+            CJIS (2):
+                Criminal Justice Information Services (CJIS)
+                Security policies.
+            FEDRAMP_HIGH (3):
+                FedRAMP High data protection controls
+            FEDRAMP_MODERATE (4):
+                FedRAMP Moderate data protection controls
+            US_REGIONAL_ACCESS (5):
+                Assured Workloads For US Regions data
+                protection controls
+            HIPAA (6):
+                Health Insurance Portability and
+                Accountability Act controls
+            HITRUST (7):
+                Health Information Trust Alliance controls
+            EU_REGIONS_AND_SUPPORT (8):
+                Assured Workloads For EU Regions and Support
+                controls
+            CA_REGIONS_AND_SUPPORT (9):
+                Assured Workloads For Canada Regions and
+                Support controls
+            ITAR (10):
+                International Traffic in Arms Regulations
+            AU_REGIONS_AND_US_SUPPORT (11):
+                Assured Workloads for Australia Regions and
+                Support controls
+        """
         COMPLIANCE_REGIME_UNSPECIFIED = 0
         IL4 = 1
         CJIS = 2
         FEDRAMP_HIGH = 3
         FEDRAMP_MODERATE = 4
         US_REGIONAL_ACCESS = 5
         HIPAA = 6
         HITRUST = 7
         EU_REGIONS_AND_SUPPORT = 8
         CA_REGIONS_AND_SUPPORT = 9
+        ITAR = 10
+        AU_REGIONS_AND_US_SUPPORT = 11
 
     class KajEnrollmentState(proto.Enum):
-        r"""Key Access Justifications(KAJ) Enrollment State."""
+        r"""Key Access Justifications(KAJ) Enrollment State.
+
+        Values:
+            KAJ_ENROLLMENT_STATE_UNSPECIFIED (0):
+                Default State for KAJ Enrollment.
+            KAJ_ENROLLMENT_STATE_PENDING (1):
+                Pending State for KAJ Enrollment.
+            KAJ_ENROLLMENT_STATE_COMPLETE (2):
+                Complete State for KAJ Enrollment.
+        """
         KAJ_ENROLLMENT_STATE_UNSPECIFIED = 0
         KAJ_ENROLLMENT_STATE_PENDING = 1
         KAJ_ENROLLMENT_STATE_COMPLETE = 2
 
     class ResourceInfo(proto.Message):
         r"""Represent the resources that are children of this Workload.
 
@@ -331,26 +516,41 @@
                 Resource identifier. For a project this represents
                 project_number.
             resource_type (google.cloud.assuredworkloads_v1beta1.types.Workload.ResourceInfo.ResourceType):
                 Indicates the type of resource.
         """
 
         class ResourceType(proto.Enum):
-            r"""The type of resource."""
+            r"""The type of resource.
+
+            Values:
+                RESOURCE_TYPE_UNSPECIFIED (0):
+                    Unknown resource type.
+                CONSUMER_PROJECT (1):
+                    Deprecated. Existing workloads will continue
+                    to support this, but new CreateWorkloadRequests
+                    should not specify this as an input value.
+                CONSUMER_FOLDER (4):
+                    Consumer Folder.
+                ENCRYPTION_KEYS_PROJECT (2):
+                    Consumer project containing encryption keys.
+                KEYRING (3):
+                    Keyring resource that hosts encryption keys.
+            """
             RESOURCE_TYPE_UNSPECIFIED = 0
             CONSUMER_PROJECT = 1
             CONSUMER_FOLDER = 4
             ENCRYPTION_KEYS_PROJECT = 2
             KEYRING = 3
 
-        resource_id = proto.Field(
+        resource_id: int = proto.Field(
             proto.INT64,
             number=1,
         )
-        resource_type = proto.Field(
+        resource_type: "Workload.ResourceInfo.ResourceType" = proto.Field(
             proto.ENUM,
             number=2,
             enum="Workload.ResourceInfo.ResourceType",
         )
 
     class KMSSettings(proto.Message):
         r"""Settings specific to the Key Management Service.
@@ -364,245 +564,282 @@
             rotation_period (google.protobuf.duration_pb2.Duration):
                 Required. Input only. Immutable. [next_rotation_time] will
                 be advanced by this period when the Key Management Service
                 automatically rotates a key. Must be at least 24 hours and
                 at most 876,000 hours.
         """
 
-        next_rotation_time = proto.Field(
+        next_rotation_time: timestamp_pb2.Timestamp = proto.Field(
             proto.MESSAGE,
             number=1,
             message=timestamp_pb2.Timestamp,
         )
-        rotation_period = proto.Field(
+        rotation_period: duration_pb2.Duration = proto.Field(
             proto.MESSAGE,
             number=2,
             message=duration_pb2.Duration,
         )
 
     class IL4Settings(proto.Message):
         r"""Settings specific to resources needed for IL4.
 
         Attributes:
             kms_settings (google.cloud.assuredworkloads_v1beta1.types.Workload.KMSSettings):
-                Required. Input only. Immutable. Settings
-                used to create a CMEK crypto key.
+                Input only. Immutable. Settings used to
+                create a CMEK crypto key.
         """
 
-        kms_settings = proto.Field(
+        kms_settings: "Workload.KMSSettings" = proto.Field(
             proto.MESSAGE,
             number=1,
             message="Workload.KMSSettings",
         )
 
     class CJISSettings(proto.Message):
         r"""Settings specific to resources needed for CJIS.
 
         Attributes:
             kms_settings (google.cloud.assuredworkloads_v1beta1.types.Workload.KMSSettings):
-                Required. Input only. Immutable. Settings
-                used to create a CMEK crypto key.
+                Input only. Immutable. Settings used to
+                create a CMEK crypto key.
         """
 
-        kms_settings = proto.Field(
+        kms_settings: "Workload.KMSSettings" = proto.Field(
             proto.MESSAGE,
             number=1,
             message="Workload.KMSSettings",
         )
 
     class FedrampHighSettings(proto.Message):
         r"""Settings specific to resources needed for FedRAMP High.
 
         Attributes:
             kms_settings (google.cloud.assuredworkloads_v1beta1.types.Workload.KMSSettings):
-                Required. Input only. Immutable. Settings
-                used to create a CMEK crypto key.
+                Input only. Immutable. Settings used to
+                create a CMEK crypto key.
         """
 
-        kms_settings = proto.Field(
+        kms_settings: "Workload.KMSSettings" = proto.Field(
             proto.MESSAGE,
             number=1,
             message="Workload.KMSSettings",
         )
 
     class FedrampModerateSettings(proto.Message):
         r"""Settings specific to resources needed for FedRAMP Moderate.
 
         Attributes:
             kms_settings (google.cloud.assuredworkloads_v1beta1.types.Workload.KMSSettings):
-                Required. Input only. Immutable. Settings
-                used to create a CMEK crypto key.
+                Input only. Immutable. Settings used to
+                create a CMEK crypto key.
         """
 
-        kms_settings = proto.Field(
+        kms_settings: "Workload.KMSSettings" = proto.Field(
             proto.MESSAGE,
             number=1,
             message="Workload.KMSSettings",
         )
 
     class ResourceSettings(proto.Message):
         r"""Represent the custom settings for the resources to be
         created.
 
         Attributes:
             resource_id (str):
                 Resource identifier. For a project this represents
                 project_id. If the project is already taken, the workload
-                creation will fail.
+                creation will fail. For KeyRing, this represents the
+                keyring_id. For a folder, don't set this value as folder_id
+                is assigned by Google.
             resource_type (google.cloud.assuredworkloads_v1beta1.types.Workload.ResourceInfo.ResourceType):
                 Indicates the type of resource. This field should be
                 specified to correspond the id to the right project type
                 (CONSUMER_PROJECT or ENCRYPTION_KEYS_PROJECT)
             display_name (str):
                 User-assigned resource display name.
                 If not empty it will be used to create a
                 resource with the specified name.
         """
 
-        resource_id = proto.Field(
+        resource_id: str = proto.Field(
             proto.STRING,
             number=1,
         )
-        resource_type = proto.Field(
+        resource_type: "Workload.ResourceInfo.ResourceType" = proto.Field(
             proto.ENUM,
             number=2,
             enum="Workload.ResourceInfo.ResourceType",
         )
-        display_name = proto.Field(
+        display_name: str = proto.Field(
             proto.STRING,
             number=3,
         )
 
     class SaaEnrollmentResponse(proto.Message):
         r"""Signed Access Approvals (SAA) enrollment response.
 
+        .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
+
         Attributes:
             setup_status (google.cloud.assuredworkloads_v1beta1.types.Workload.SaaEnrollmentResponse.SetupState):
                 Indicates SAA enrollment status of a given
                 workload.
 
                 This field is a member of `oneof`_ ``_setup_status``.
-            setup_errors (Sequence[google.cloud.assuredworkloads_v1beta1.types.Workload.SaaEnrollmentResponse.SetupError]):
+            setup_errors (MutableSequence[google.cloud.assuredworkloads_v1beta1.types.Workload.SaaEnrollmentResponse.SetupError]):
                 Indicates SAA enrollment setup error if any.
         """
 
         class SetupState(proto.Enum):
-            r"""Setup state of SAA enrollment."""
+            r"""Setup state of SAA enrollment.
+
+            Values:
+                SETUP_STATE_UNSPECIFIED (0):
+                    Unspecified.
+                STATUS_PENDING (1):
+                    SAA enrollment pending.
+                STATUS_COMPLETE (2):
+                    SAA enrollment comopleted.
+            """
             SETUP_STATE_UNSPECIFIED = 0
             STATUS_PENDING = 1
             STATUS_COMPLETE = 2
 
         class SetupError(proto.Enum):
-            r"""Setup error of SAA enrollment."""
+            r"""Setup error of SAA enrollment.
+
+            Values:
+                SETUP_ERROR_UNSPECIFIED (0):
+                    Unspecified.
+                ERROR_INVALID_BASE_SETUP (1):
+                    Invalid states for all customers, to be
+                    redirected to AA UI for additional details.
+                ERROR_MISSING_EXTERNAL_SIGNING_KEY (2):
+                    Returned when there is not an EKM key
+                    configured.
+                ERROR_NOT_ALL_SERVICES_ENROLLED (3):
+                    Returned when there are no enrolled services
+                    or the customer is enrolled in CAA only for a
+                    subset of services.
+                ERROR_SETUP_CHECK_FAILED (4):
+                    Returned when exception was encountered
+                    during evaluation of other criteria.
+            """
             SETUP_ERROR_UNSPECIFIED = 0
             ERROR_INVALID_BASE_SETUP = 1
             ERROR_MISSING_EXTERNAL_SIGNING_KEY = 2
             ERROR_NOT_ALL_SERVICES_ENROLLED = 3
             ERROR_SETUP_CHECK_FAILED = 4
 
-        setup_status = proto.Field(
+        setup_status: "Workload.SaaEnrollmentResponse.SetupState" = proto.Field(
             proto.ENUM,
             number=1,
             optional=True,
             enum="Workload.SaaEnrollmentResponse.SetupState",
         )
-        setup_errors = proto.RepeatedField(
+        setup_errors: MutableSequence[
+            "Workload.SaaEnrollmentResponse.SetupError"
+        ] = proto.RepeatedField(
             proto.ENUM,
             number=2,
             enum="Workload.SaaEnrollmentResponse.SetupError",
         )
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    display_name = proto.Field(
+    display_name: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    resources = proto.RepeatedField(
+    resources: MutableSequence[ResourceInfo] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message=ResourceInfo,
     )
-    compliance_regime = proto.Field(
+    compliance_regime: ComplianceRegime = proto.Field(
         proto.ENUM,
         number=4,
         enum=ComplianceRegime,
     )
-    create_time = proto.Field(
+    create_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=5,
         message=timestamp_pb2.Timestamp,
     )
-    billing_account = proto.Field(
+    billing_account: str = proto.Field(
         proto.STRING,
         number=6,
     )
-    il4_settings = proto.Field(
+    il4_settings: IL4Settings = proto.Field(
         proto.MESSAGE,
         number=7,
         oneof="compliance_regime_settings",
         message=IL4Settings,
     )
-    cjis_settings = proto.Field(
+    cjis_settings: CJISSettings = proto.Field(
         proto.MESSAGE,
         number=8,
         oneof="compliance_regime_settings",
         message=CJISSettings,
     )
-    fedramp_high_settings = proto.Field(
+    fedramp_high_settings: FedrampHighSettings = proto.Field(
         proto.MESSAGE,
         number=11,
         oneof="compliance_regime_settings",
         message=FedrampHighSettings,
     )
-    fedramp_moderate_settings = proto.Field(
+    fedramp_moderate_settings: FedrampModerateSettings = proto.Field(
         proto.MESSAGE,
         number=12,
         oneof="compliance_regime_settings",
         message=FedrampModerateSettings,
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=9,
     )
-    labels = proto.MapField(
+    labels: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=10,
     )
-    provisioned_resources_parent = proto.Field(
+    provisioned_resources_parent: str = proto.Field(
         proto.STRING,
         number=13,
     )
-    kms_settings = proto.Field(
+    kms_settings: KMSSettings = proto.Field(
         proto.MESSAGE,
         number=14,
         message=KMSSettings,
     )
-    resource_settings = proto.RepeatedField(
+    resource_settings: MutableSequence[ResourceSettings] = proto.RepeatedField(
         proto.MESSAGE,
         number=15,
         message=ResourceSettings,
     )
-    kaj_enrollment_state = proto.Field(
+    kaj_enrollment_state: KajEnrollmentState = proto.Field(
         proto.ENUM,
         number=17,
         enum=KajEnrollmentState,
     )
-    enable_sovereign_controls = proto.Field(
+    enable_sovereign_controls: bool = proto.Field(
         proto.BOOL,
         number=18,
     )
-    saa_enrollment_response = proto.Field(
+    saa_enrollment_response: SaaEnrollmentResponse = proto.Field(
         proto.MESSAGE,
         number=20,
         message=SaaEnrollmentResponse,
     )
+    compliant_but_disallowed_services: MutableSequence[str] = proto.RepeatedField(
+        proto.STRING,
+        number=24,
+    )
 
 
 class CreateWorkloadOperationMetadata(proto.Message):
     r"""Operation metadata to give request details of CreateWorkload.
 
     Attributes:
         create_time (google.protobuf.timestamp_pb2.Timestamp):
@@ -612,39 +849,41 @@
             Optional. The display name of the workload.
         parent (str):
             Optional. The parent of the workload.
         compliance_regime (google.cloud.assuredworkloads_v1beta1.types.Workload.ComplianceRegime):
             Optional. Compliance controls that should be
             applied to the resources managed by the
             workload.
-        resource_settings (Sequence[google.cloud.assuredworkloads_v1beta1.types.Workload.ResourceSettings]):
+        resource_settings (MutableSequence[google.cloud.assuredworkloads_v1beta1.types.Workload.ResourceSettings]):
             Optional. Resource properties in the input
             that are used for creating/customizing workload
             resources.
     """
 
-    create_time = proto.Field(
+    create_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=1,
         message=timestamp_pb2.Timestamp,
     )
-    display_name = proto.Field(
+    display_name: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    compliance_regime = proto.Field(
+    compliance_regime: "Workload.ComplianceRegime" = proto.Field(
         proto.ENUM,
         number=4,
         enum="Workload.ComplianceRegime",
     )
-    resource_settings = proto.RepeatedField(
+    resource_settings: MutableSequence[
+        "Workload.ResourceSettings"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=5,
         message="Workload.ResourceSettings",
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `google-cloud-assured-workloads-1.9.0/google_cloud_assured_workloads.egg-info/PKG-INFO` & `google-cloud-assured-workloads-1.9.1/google_cloud_assured_workloads.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-assured-workloads
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Assured Workloads API client library
 Home-page: https://github.com/googleapis/python-assured-workloads
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-assured-workloads-1.9.0/google_cloud_assured_workloads.egg-info/SOURCES.txt` & `google-cloud-assured-workloads-1.9.1/google_cloud_assured_workloads.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/setup.py` & `google-cloud-assured-workloads-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/tests/__init__.py` & `google-cloud-assured-workloads-1.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/tests/unit/__init__.py` & `google-cloud-assured-workloads-1.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/tests/unit/gapic/__init__.py` & `google-cloud-assured-workloads-1.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/tests/unit/gapic/assuredworkloads_v1/__init__.py` & `google-cloud-assured-workloads-1.9.1/tests/unit/gapic/assuredworkloads_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/tests/unit/gapic/assuredworkloads_v1/test_assured_workloads_service.py` & `google-cloud-assured-workloads-1.9.1/tests/unit/gapic/assuredworkloads_v1/test_assured_workloads_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/tests/unit/gapic/assuredworkloads_v1beta1/__init__.py` & `google-cloud-assured-workloads-1.9.1/tests/unit/gapic/assuredworkloads_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-assured-workloads-1.9.0/tests/unit/gapic/assuredworkloads_v1beta1/test_assured_workloads_service.py` & `google-cloud-assured-workloads-1.9.1/tests/unit/gapic/assuredworkloads_v1beta1/test_assured_workloads_service.py`

 * *Files identical despite different names*

