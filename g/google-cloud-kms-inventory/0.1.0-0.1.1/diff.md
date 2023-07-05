# Comparing `tmp/google-cloud-kms-inventory-0.1.0.tar.gz` & `tmp/google-cloud-kms-inventory-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-kms-inventory-0.1.0.tar", last modified: Thu Jun 22 19:38:59 2023, max compression
+gzip compressed data, was "google-cloud-kms-inventory-0.1.1.tar", last modified: Wed Jul  5 15:53:38 2023, max compression
```

## Comparing `google-cloud-kms-inventory-0.1.0.tar` & `google-cloud-kms-inventory-0.1.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 19:38:59.501442 google-cloud-kms-inventory-0.1.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4523 2023-06-22 19:38:59.501442 google-cloud-kms-inventory-0.1.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3603 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 19:38:59.489441 google-cloud-kms-inventory-0.1.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 19:38:59.489441 google-cloud-kms-inventory-0.1.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 19:38:59.493441 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory/
--rw-rw-r--   0 root         (0)     1003     1961 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       87 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 19:38:59.493441 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/
--rw-rw-r--   0 root         (0)     1003     1642 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2377 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       87 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 19:38:59.493441 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 19:38:59.493441 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    14920 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    24901 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/client.py
--rw-rw-r--   0 root         (0)     1003     6018 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 19:38:59.493441 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/
--rw-rw-r--   0 root         (0)     1003     1478 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6136 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12095 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12305 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12523 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 19:38:59.497442 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_tracking_service/
--rw-rw-r--   0 root         (0)     1003      785 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_tracking_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    20296 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_tracking_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    30846 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_tracking_service/client.py
--rw-rw-r--   0 root         (0)     1003     6306 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_tracking_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 19:38:59.497442 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/
--rw-rw-r--   0 root         (0)     1003     1464 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6773 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13849 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14080 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    18871 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 19:38:59.497442 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/types/
--rw-rw-r--   0 root         (0)     1003     1143 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2810 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/types/key_dashboard_service.py
--rw-rw-r--   0 root         (0)     1003     9093 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/types/key_tracking_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 19:38:59.497442 google-cloud-kms-inventory-0.1.0/google_cloud_kms_inventory.egg-info/
--rw-r--r--   0 root         (0)     1003     4523 2023-06-22 19:38:59.000000 google-cloud-kms-inventory-0.1.0/google_cloud_kms_inventory.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2555 2023-06-22 19:38:59.000000 google-cloud-kms-inventory-0.1.0/google_cloud_kms_inventory.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-22 19:38:59.000000 google-cloud-kms-inventory-0.1.0/google_cloud_kms_inventory.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-06-22 19:38:59.000000 google-cloud-kms-inventory-0.1.0/google_cloud_kms_inventory.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-22 19:38:59.000000 google-cloud-kms-inventory-0.1.0/google_cloud_kms_inventory.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      291 2023-06-22 19:38:59.000000 google-cloud-kms-inventory-0.1.0/google_cloud_kms_inventory.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-22 19:38:59.000000 google-cloud-kms-inventory-0.1.0/google_cloud_kms_inventory.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-06-22 19:38:59.501442 google-cloud-kms-inventory-0.1.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2931 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 19:38:59.497442 google-cloud-kms-inventory-0.1.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 19:38:59.497442 google-cloud-kms-inventory-0.1.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 19:38:59.497442 google-cloud-kms-inventory-0.1.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 19:38:59.501442 google-cloud-kms-inventory-0.1.0/tests/unit/gapic/kms_inventory_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/tests/unit/gapic/kms_inventory_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    83570 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/tests/unit/gapic/kms_inventory_v1/test_key_dashboard_service.py
--rw-rw-r--   0 root         (0)     1003   107293 2023-06-22 19:35:49.000000 google-cloud-kms-inventory-0.1.0/tests/unit/gapic/kms_inventory_v1/test_key_tracking_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.065025 google-cloud-kms-inventory-0.1.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4523 2023-07-05 15:53:38.065025 google-cloud-kms-inventory-0.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3603 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.053025 google-cloud-kms-inventory-0.1.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.053025 google-cloud-kms-inventory-0.1.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.057025 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory/
+-rw-rw-r--   0 root         (0)     1003     1961 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       87 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.057025 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/
+-rw-rw-r--   0 root         (0)     1003     1642 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2377 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       87 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.057025 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.057025 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14956 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    24901 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6018 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.057025 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1478 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6136 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12095 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12305 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12523 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.057025 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/
+-rw-rw-r--   0 root         (0)     1003      785 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20331 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    30846 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6306 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.061025 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1464 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6773 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13849 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14080 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    18871 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.061025 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1143 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2810 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/types/key_dashboard_service.py
+-rw-rw-r--   0 root         (0)     1003     9093 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/types/key_tracking_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.061025 google-cloud-kms-inventory-0.1.1/google_cloud_kms_inventory.egg-info/
+-rw-r--r--   0 root         (0)     1003     4523 2023-07-05 15:53:38.000000 google-cloud-kms-inventory-0.1.1/google_cloud_kms_inventory.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2555 2023-07-05 15:53:38.000000 google-cloud-kms-inventory-0.1.1/google_cloud_kms_inventory.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:38.000000 google-cloud-kms-inventory-0.1.1/google_cloud_kms_inventory.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:53:38.000000 google-cloud-kms-inventory-0.1.1/google_cloud_kms_inventory.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:38.000000 google-cloud-kms-inventory-0.1.1/google_cloud_kms_inventory.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      291 2023-07-05 15:53:38.000000 google-cloud-kms-inventory-0.1.1/google_cloud_kms_inventory.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:53:38.000000 google-cloud-kms-inventory-0.1.1/google_cloud_kms_inventory.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:53:38.065025 google-cloud-kms-inventory-0.1.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2931 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.061025 google-cloud-kms-inventory-0.1.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.061025 google-cloud-kms-inventory-0.1.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.061025 google-cloud-kms-inventory-0.1.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.061025 google-cloud-kms-inventory-0.1.1/tests/unit/gapic/kms_inventory_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/tests/unit/gapic/kms_inventory_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    83570 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/tests/unit/gapic/kms_inventory_v1/test_key_dashboard_service.py
+-rw-rw-r--   0 root         (0)     1003   107492 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/tests/unit/gapic/kms_inventory_v1/test_key_tracking_service.py
```

### Comparing `google-cloud-kms-inventory-0.1.0/LICENSE` & `google-cloud-kms-inventory-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/MANIFEST.in` & `google-cloud-kms-inventory-0.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/PKG-INFO` & `google-cloud-kms-inventory-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-kms-inventory
-Version: 0.1.0
+Version: 0.1.1
 Summary: Google Cloud Kms Inventory API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-kms-inventory-0.1.0/README.rst` & `google-cloud-kms-inventory-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory/__init__.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory/gapic_version.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory/gapic_version.py`

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
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.1.1"  # {x-release-please-version}
```

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/__init__.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/gapic_metadata.json` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/gapic_version.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/gapic_version.py`

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
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.1.1"  # {x-release-please-version}
```

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/__init__.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/__init__.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/async_client.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,15 +343,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "KeyDashboardServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/client.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/pagers.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/__init__.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/base.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/grpc.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/grpc_asyncio.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/rest.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_tracking_service/__init__.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_tracking_service/async_client.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,15 +465,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "KeyTrackingServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_tracking_service/client.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_tracking_service/pagers.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/__init__.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/base.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/grpc.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/grpc_asyncio.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/rest.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/types/__init__.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/types/key_dashboard_service.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/types/key_dashboard_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google/cloud/kms_inventory_v1/types/key_tracking_service.py` & `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/types/key_tracking_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/google_cloud_kms_inventory.egg-info/PKG-INFO` & `google-cloud-kms-inventory-0.1.1/google_cloud_kms_inventory.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-kms-inventory
-Version: 0.1.0
+Version: 0.1.1
 Summary: Google Cloud Kms Inventory API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-kms-inventory-0.1.0/google_cloud_kms_inventory.egg-info/SOURCES.txt` & `google-cloud-kms-inventory-0.1.1/google_cloud_kms_inventory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/setup.py` & `google-cloud-kms-inventory-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/tests/__init__.py` & `google-cloud-kms-inventory-0.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/tests/unit/__init__.py` & `google-cloud-kms-inventory-0.1.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/tests/unit/gapic/__init__.py` & `google-cloud-kms-inventory-0.1.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/tests/unit/gapic/kms_inventory_v1/__init__.py` & `google-cloud-kms-inventory-0.1.1/tests/unit/gapic/kms_inventory_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/tests/unit/gapic/kms_inventory_v1/test_key_dashboard_service.py` & `google-cloud-kms-inventory-0.1.1/tests/unit/gapic/kms_inventory_v1/test_key_dashboard_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.0/tests/unit/gapic/kms_inventory_v1/test_key_tracking_service.py` & `google-cloud-kms-inventory-0.1.1/tests/unit/gapic/kms_inventory_v1/test_key_tracking_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1432,17 +1432,19 @@
                     key_tracking_service.ProtectedResource(),
                     key_tracking_service.ProtectedResource(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.search_protected_resources(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

