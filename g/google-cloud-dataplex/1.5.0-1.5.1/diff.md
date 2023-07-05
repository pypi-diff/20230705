# Comparing `tmp/google-cloud-dataplex-1.5.0.tar.gz` & `tmp/google-cloud-dataplex-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-dataplex-1.5.0.tar", last modified: Wed May 31 20:48:21 2023, max compression
+gzip compressed data, was "google-cloud-dataplex-1.5.1.tar", last modified: Wed Jul  5 15:52:12 2023, max compression
```

## Comparing `google-cloud-dataplex-1.5.0.tar` & `google-cloud-dataplex-1.5.1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.081312 google-cloud-dataplex-1.5.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4728 2023-05-31 20:48:21.081312 google-cloud-dataplex-1.5.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3809 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.065312 google-cloud-dataplex-1.5.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.065312 google-cloud-dataplex-1.5.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.065312 google-cloud-dataplex-1.5.0/google/cloud/dataplex/
--rw-rw-r--   0 root         (0)     1003     7243 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.069312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/
--rw-rw-r--   0 root         (0)     1003     6436 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    15314 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.069312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.069312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/
--rw-rw-r--   0 root         (0)     1003      769 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    62823 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    71605 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/client.py
--rw-rw-r--   0 root         (0)     1003     5658 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.069312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/transports/
--rw-rw-r--   0 root         (0)     1003     1193 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12118 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    25618 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    25992 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.069312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    62227 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    73395 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/client.py
--rw-rw-r--   0 root         (0)     1003    10807 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.069312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/transports/
--rw-rw-r--   0 root         (0)     1003     1202 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10921 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    25499 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    25983 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.073312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   186240 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   199302 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/client.py
--rw-rw-r--   0 root         (0)     1003    49482 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.073312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/transports/
--rw-rw-r--   0 root         (0)     1003     1202 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    26223 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    52208 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    53320 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.073312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    61597 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    72083 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/client.py
--rw-rw-r--   0 root         (0)     1003    10685 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.073312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/transports/
--rw-rw-r--   0 root         (0)     1003     1202 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12419 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    25614 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    26039 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.077312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/
--rw-rw-r--   0 root         (0)     1003     5638 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    16335 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/analyze.py
--rw-rw-r--   0 root         (0)     1003     6555 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/content.py
--rw-rw-r--   0 root         (0)     1003    15619 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/data_profile.py
--rw-rw-r--   0 root         (0)     1003    16628 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/data_quality.py
--rw-rw-r--   0 root         (0)     1003    24703 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/datascans.py
--rw-rw-r--   0 root         (0)     1003    22735 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/logs.py
--rw-rw-r--   0 root         (0)     1003    38144 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/metadata_.py
--rw-rw-r--   0 root         (0)     1003     5857 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/processing.py
--rw-rw-r--   0 root         (0)     1003    50791 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/resources.py
--rw-rw-r--   0 root         (0)     1003    39146 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/service.py
--rw-rw-r--   0 root         (0)     1003    26001 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/tasks.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.077312 google-cloud-dataplex-1.5.0/google_cloud_dataplex.egg-info/
--rw-r--r--   0 root         (0)     1003     4728 2023-05-31 20:48:21.000000 google-cloud-dataplex-1.5.0/google_cloud_dataplex.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3701 2023-05-31 20:48:21.000000 google-cloud-dataplex-1.5.0/google_cloud_dataplex.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-31 20:48:21.000000 google-cloud-dataplex-1.5.0/google_cloud_dataplex.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-05-31 20:48:21.000000 google-cloud-dataplex-1.5.0/google_cloud_dataplex.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-31 20:48:21.000000 google-cloud-dataplex-1.5.0/google_cloud_dataplex.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-05-31 20:48:21.000000 google-cloud-dataplex-1.5.0/google_cloud_dataplex.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-05-31 20:48:21.000000 google-cloud-dataplex-1.5.0/google_cloud_dataplex.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-05-31 20:48:21.081312 google-cloud-dataplex-1.5.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2972 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.077312 google-cloud-dataplex-1.5.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.077312 google-cloud-dataplex-1.5.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.077312 google-cloud-dataplex-1.5.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.081312 google-cloud-dataplex-1.5.0/tests/unit/gapic/dataplex_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/tests/unit/gapic/dataplex_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   154569 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/tests/unit/gapic/dataplex_v1/test_content_service.py
--rw-rw-r--   0 root         (0)     1003   169734 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/tests/unit/gapic/dataplex_v1/test_data_scan_service.py
--rw-rw-r--   0 root         (0)     1003   429857 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/tests/unit/gapic/dataplex_v1/test_dataplex_service.py
--rw-rw-r--   0 root         (0)     1003   175411 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/tests/unit/gapic/dataplex_v1/test_metadata_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.681151 google-cloud-dataplex-1.5.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4696 2023-07-05 15:52:12.681151 google-cloud-dataplex-1.5.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3773 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.665150 google-cloud-dataplex-1.5.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.665150 google-cloud-dataplex-1.5.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.665150 google-cloud-dataplex-1.5.1/google/cloud/dataplex/
+-rw-rw-r--   0 root         (0)     1003     7243 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.669150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/
+-rw-rw-r--   0 root         (0)     1003     6436 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15314 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.669150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.669150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/
+-rw-rw-r--   0 root         (0)     1003      769 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    62854 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    71605 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5658 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.669150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1193 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12118 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    25618 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    25992 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.669150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    62259 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    73395 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10807 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.673150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1202 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10921 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    25499 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    25983 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.673150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   186272 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   199302 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/client.py
+-rw-rw-r--   0 root         (0)     1003    49482 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.673150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1202 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26223 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    52208 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    53320 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.677150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    61629 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    72083 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10685 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.677150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1202 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12419 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    25614 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    26039 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.677150 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/
+-rw-rw-r--   0 root         (0)     1003     5638 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16335 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/analyze.py
+-rw-rw-r--   0 root         (0)     1003     6555 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/content.py
+-rw-rw-r--   0 root         (0)     1003    15619 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/data_profile.py
+-rw-rw-r--   0 root         (0)     1003    16628 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/data_quality.py
+-rw-rw-r--   0 root         (0)     1003    24703 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/datascans.py
+-rw-rw-r--   0 root         (0)     1003    22735 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/logs.py
+-rw-rw-r--   0 root         (0)     1003    38144 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/metadata_.py
+-rw-rw-r--   0 root         (0)     1003     5857 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/processing.py
+-rw-rw-r--   0 root         (0)     1003    50791 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/resources.py
+-rw-rw-r--   0 root         (0)     1003    39146 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/service.py
+-rw-rw-r--   0 root         (0)     1003    26001 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/tasks.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.681151 google-cloud-dataplex-1.5.1/google_cloud_dataplex.egg-info/
+-rw-r--r--   0 root         (0)     1003     4696 2023-07-05 15:52:12.000000 google-cloud-dataplex-1.5.1/google_cloud_dataplex.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3701 2023-07-05 15:52:12.000000 google-cloud-dataplex-1.5.1/google_cloud_dataplex.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:12.000000 google-cloud-dataplex-1.5.1/google_cloud_dataplex.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:52:12.000000 google-cloud-dataplex-1.5.1/google_cloud_dataplex.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:12.000000 google-cloud-dataplex-1.5.1/google_cloud_dataplex.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:52:12.000000 google-cloud-dataplex-1.5.1/google_cloud_dataplex.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:52:12.000000 google-cloud-dataplex-1.5.1/google_cloud_dataplex.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:52:12.681151 google-cloud-dataplex-1.5.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2976 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.681151 google-cloud-dataplex-1.5.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.681151 google-cloud-dataplex-1.5.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.681151 google-cloud-dataplex-1.5.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:12.681151 google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   154372 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/test_content_service.py
+-rw-rw-r--   0 root         (0)     1003   169258 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/test_data_scan_service.py
+-rw-rw-r--   0 root         (0)     1003   431726 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/test_dataplex_service.py
+-rw-rw-r--   0 root         (0)     1003   175809 2023-07-05 15:46:58.000000 google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/test_metadata_service.py
```

### Comparing `google-cloud-dataplex-1.5.0/LICENSE` & `google-cloud-dataplex-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/MANIFEST.in` & `google-cloud-dataplex-1.5.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/PKG-INFO` & `google-cloud-dataplex-1.5.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-dataplex
-Version: 1.5.0
+Version: 1.5.1
 Summary: Google Cloud Dataplex API client library
-Home-page: https://github.com/googleapis/python-dataplex
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
 
-Python Client for Cloud Dataplex API
-====================================
+Python Client for Cloud Dataplex
+================================
 
 |stable| |pypi| |versions|
 
-`Cloud Dataplex API`_: provides intelligent data fabric that enables organizations to centrally manage, monitor, and govern their data across data lakes, data warehouses, and data marts with consistent controls, providing access to trusted data and powering analytics at scale.
+`Cloud Dataplex`_: provides intelligent data fabric that enables organizations to centrally manage, monitor, and govern their data across data lakes, data warehouses, and data marts with consistent controls, providing access to trusted data and powering analytics at scale.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-dataplex.svg
    :target: https://pypi.org/project/google-cloud-dataplex/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-dataplex.svg
    :target: https://pypi.org/project/google-cloud-dataplex/
-.. _Cloud Dataplex API: https://cloud.google.com/dataplex
+.. _Cloud Dataplex: https://cloud.google.com/dataplex
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/dataplex/latest
 .. _Product Documentation:  https://cloud.google.com/dataplex
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Dataplex API.`_
+3. `Enable the Cloud Dataplex.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Dataplex API.:  https://cloud.google.com/dataplex
+.. _Enable the Cloud Dataplex.:  https://cloud.google.com/dataplex
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-dataplex
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Dataplex API
+-  Read the `Client Library Documentation`_ for Cloud Dataplex
    to see other available methods on the client.
--  Read the `Cloud Dataplex API Product documentation`_ to learn
+-  Read the `Cloud Dataplex Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Dataplex API Product documentation:  https://cloud.google.com/dataplex
+.. _Cloud Dataplex Product documentation:  https://cloud.google.com/dataplex
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-dataplex-1.5.0/README.rst` & `google-cloud-dataplex-1.5.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Cloud Dataplex API
-====================================
+Python Client for Cloud Dataplex
+================================
 
 |stable| |pypi| |versions|
 
-`Cloud Dataplex API`_: provides intelligent data fabric that enables organizations to centrally manage, monitor, and govern their data across data lakes, data warehouses, and data marts with consistent controls, providing access to trusted data and powering analytics at scale.
+`Cloud Dataplex`_: provides intelligent data fabric that enables organizations to centrally manage, monitor, and govern their data across data lakes, data warehouses, and data marts with consistent controls, providing access to trusted data and powering analytics at scale.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-dataplex.svg
    :target: https://pypi.org/project/google-cloud-dataplex/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-dataplex.svg
    :target: https://pypi.org/project/google-cloud-dataplex/
-.. _Cloud Dataplex API: https://cloud.google.com/dataplex
+.. _Cloud Dataplex: https://cloud.google.com/dataplex
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/dataplex/latest
 .. _Product Documentation:  https://cloud.google.com/dataplex
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Dataplex API.`_
+3. `Enable the Cloud Dataplex.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Dataplex API.:  https://cloud.google.com/dataplex
+.. _Enable the Cloud Dataplex.:  https://cloud.google.com/dataplex
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-dataplex
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Dataplex API
+-  Read the `Client Library Documentation`_ for Cloud Dataplex
    to see other available methods on the client.
--  Read the `Cloud Dataplex API Product documentation`_ to learn
+-  Read the `Cloud Dataplex Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Dataplex API Product documentation:  https://cloud.google.com/dataplex
+.. _Cloud Dataplex Product documentation:  https://cloud.google.com/dataplex
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex/__init__.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex/gapic_version.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.5.0"  # {x-release-please-version}
```

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/__init__.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/gapic_metadata.json` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/gapic_version.py` & `google-cloud-dataplex-1.5.1/tests/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.5.0"  # {x-release-please-version}
```

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/__init__.py` & `google-cloud-dataplex-1.5.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/__init__.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/async_client.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1526,15 +1526,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ContentServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/client.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/pagers.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/transports/__init__.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/transports/base.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/transports/grpc.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/transports/grpc_asyncio.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/content_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/__init__.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/async_client.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1537,15 +1537,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "DataScanServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/client.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/pagers.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/transports/__init__.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/transports/base.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc_asyncio.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/__init__.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/async_client.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4658,15 +4658,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "DataplexServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/client.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/pagers.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/transports/__init__.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/transports/base.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc_asyncio.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/__init__.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/async_client.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1527,15 +1527,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "MetadataServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/client.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/pagers.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/transports/__init__.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/transports/base.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/transports/grpc.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/transports/grpc_asyncio.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/services/metadata_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/__init__.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/analyze.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/analyze.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/content.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/content.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/data_profile.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/data_profile.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/data_quality.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/data_quality.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/datascans.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/datascans.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/logs.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/logs.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/metadata_.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/metadata_.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/processing.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/processing.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/resources.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/service.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/tasks.py` & `google-cloud-dataplex-1.5.1/google/cloud/dataplex_v1/types/tasks.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/google_cloud_dataplex.egg-info/PKG-INFO` & `google-cloud-dataplex-1.5.1/google_cloud_dataplex.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-dataplex
-Version: 1.5.0
+Version: 1.5.1
 Summary: Google Cloud Dataplex API client library
-Home-page: https://github.com/googleapis/python-dataplex
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
 
-Python Client for Cloud Dataplex API
-====================================
+Python Client for Cloud Dataplex
+================================
 
 |stable| |pypi| |versions|
 
-`Cloud Dataplex API`_: provides intelligent data fabric that enables organizations to centrally manage, monitor, and govern their data across data lakes, data warehouses, and data marts with consistent controls, providing access to trusted data and powering analytics at scale.
+`Cloud Dataplex`_: provides intelligent data fabric that enables organizations to centrally manage, monitor, and govern their data across data lakes, data warehouses, and data marts with consistent controls, providing access to trusted data and powering analytics at scale.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-dataplex.svg
    :target: https://pypi.org/project/google-cloud-dataplex/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-dataplex.svg
    :target: https://pypi.org/project/google-cloud-dataplex/
-.. _Cloud Dataplex API: https://cloud.google.com/dataplex
+.. _Cloud Dataplex: https://cloud.google.com/dataplex
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/dataplex/latest
 .. _Product Documentation:  https://cloud.google.com/dataplex
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Dataplex API.`_
+3. `Enable the Cloud Dataplex.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Dataplex API.:  https://cloud.google.com/dataplex
+.. _Enable the Cloud Dataplex.:  https://cloud.google.com/dataplex
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-dataplex
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Dataplex API
+-  Read the `Client Library Documentation`_ for Cloud Dataplex
    to see other available methods on the client.
--  Read the `Cloud Dataplex API Product documentation`_ to learn
+-  Read the `Cloud Dataplex Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Dataplex API Product documentation:  https://cloud.google.com/dataplex
+.. _Cloud Dataplex Product documentation:  https://cloud.google.com/dataplex
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-dataplex-1.5.0/google_cloud_dataplex.egg-info/SOURCES.txt` & `google-cloud-dataplex-1.5.1/google_cloud_dataplex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/setup.py` & `google-cloud-dataplex-1.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
-url = "https://github.com/googleapis/python-dataplex"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-dataplex-1.5.0/tests/__init__.py` & `google-cloud-dataplex-1.5.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/tests/unit/__init__.py` & `google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.5.0/tests/unit/gapic/dataplex_v1/test_content_service.py` & `google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/test_content_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -712,17 +712,14 @@
         # Designate an appropriate return value for the call.
         call.return_value = analyze.Content(
             name="name_value",
             uid="uid_value",
             path="path_value",
             description="description_value",
             data_text="data_text_value",
-            sql_script=analyze.Content.SqlScript(
-                engine=analyze.Content.SqlScript.QueryEngine.SPARK
-            ),
         )
         response = client.create_content(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == gcd_content.CreateContentRequest()
@@ -966,17 +963,14 @@
         # Designate an appropriate return value for the call.
         call.return_value = analyze.Content(
             name="name_value",
             uid="uid_value",
             path="path_value",
             description="description_value",
             data_text="data_text_value",
-            sql_script=analyze.Content.SqlScript(
-                engine=analyze.Content.SqlScript.QueryEngine.SPARK
-            ),
         )
         response = client.update_content(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == gcd_content.UpdateContentRequest()
@@ -1440,17 +1434,14 @@
         # Designate an appropriate return value for the call.
         call.return_value = analyze.Content(
             name="name_value",
             uid="uid_value",
             path="path_value",
             description="description_value",
             data_text="data_text_value",
-            sql_script=analyze.Content.SqlScript(
-                engine=analyze.Content.SqlScript.QueryEngine.SPARK
-            ),
         )
         response = client.get_content(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == content.GetContentRequest()
@@ -2669,17 +2660,19 @@
                     analyze.Content(),
                     analyze.Content(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_content(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
```

### Comparing `google-cloud-dataplex-1.5.0/tests/unit/gapic/dataplex_v1/test_data_scan_service.py` & `google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/test_data_scan_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1449,24 +1449,14 @@
         call.return_value = datascans.DataScan(
             name="name_value",
             uid="uid_value",
             description="description_value",
             display_name="display_name_value",
             state=resources.State.ACTIVE,
             type_=datascans.DataScanType.DATA_QUALITY,
-            data_quality_spec=data_quality.DataQualitySpec(
-                rules=[
-                    data_quality.DataQualityRule(
-                        range_expectation=data_quality.DataQualityRule.RangeExpectation(
-                            min_value="min_value_value"
-                        )
-                    )
-                ]
-            ),
-            data_quality_result=data_quality.DataQualityResult(passed=True),
         )
         response = client.get_data_scan(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == datascans.GetDataScanRequest()
@@ -2096,17 +2086,19 @@
                     datascans.DataScan(),
                     datascans.DataScan(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_data_scans(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2358,24 +2350,14 @@
         # Designate an appropriate return value for the call.
         call.return_value = datascans.DataScanJob(
             name="name_value",
             uid="uid_value",
             state=datascans.DataScanJob.State.RUNNING,
             message="message_value",
             type_=datascans.DataScanType.DATA_QUALITY,
-            data_quality_spec=data_quality.DataQualitySpec(
-                rules=[
-                    data_quality.DataQualityRule(
-                        range_expectation=data_quality.DataQualityRule.RangeExpectation(
-                            min_value="min_value_value"
-                        )
-                    )
-                ]
-            ),
-            data_quality_result=data_quality.DataQualityResult(passed=True),
         )
         response = client.get_data_scan_job(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == datascans.GetDataScanJobRequest()
@@ -3036,17 +3018,19 @@
                     datascans.DataScanJob(),
                     datascans.DataScanJob(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_data_scan_jobs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
```

### Comparing `google-cloud-dataplex-1.5.0/tests/unit/gapic/dataplex_v1/test_dataplex_service.py` & `google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/test_dataplex_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1832,17 +1832,19 @@
                     resources.Lake(),
                     resources.Lake(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_lakes(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2522,17 +2524,19 @@
                     resources.Action(),
                     resources.Action(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_lake_actions(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3650,17 +3654,19 @@
                     resources.Zone(),
                     resources.Zone(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_zones(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4340,17 +4346,19 @@
                     resources.Action(),
                     resources.Action(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_zone_actions(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5468,17 +5476,19 @@
                     resources.Asset(),
                     resources.Asset(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_assets(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -6154,17 +6164,19 @@
                     resources.Action(),
                     resources.Action(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_asset_actions(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -7286,17 +7298,19 @@
                     tasks.Task(),
                     tasks.Task(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_tasks(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -7320,17 +7334,14 @@
         # Designate an appropriate return value for the call.
         call.return_value = tasks.Task(
             name="name_value",
             uid="uid_value",
             description="description_value",
             display_name="display_name_value",
             state=resources.State.ACTIVE,
-            spark=tasks.Task.SparkTaskConfig(
-                main_jar_file_uri="main_jar_file_uri_value"
-            ),
         )
         response = client.get_task(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.GetTaskRequest()
@@ -7953,17 +7964,19 @@
                     tasks.Job(),
                     tasks.Job(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_jobs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -9843,17 +9856,19 @@
                     analyze.Environment(),
                     analyze.Environment(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_environments(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -10507,17 +10522,19 @@
                     analyze.Session(),
                     analyze.Session(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_sessions(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
```

### Comparing `google-cloud-dataplex-1.5.0/tests/unit/gapic/dataplex_v1/test_metadata_service.py` & `google-cloud-dataplex-1.5.1/tests/unit/gapic/dataplex_v1/test_metadata_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -2074,17 +2074,19 @@
                     metadata_.Entity(),
                     metadata_.Entity(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_entities(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3204,17 +3206,19 @@
                     metadata_.Partition(),
                     metadata_.Partition(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_partitions(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
```

