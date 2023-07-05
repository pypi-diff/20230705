# Comparing `tmp/google-cloud-trace-1.9.0.tar.gz` & `tmp/google-cloud-trace-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-trace-1.9.0.tar", last modified: Tue Jan 10 17:28:11 2023, max compression
+gzip compressed data, was "google-cloud-trace-1.9.1.tar", last modified: Mon Jan 23 15:42:16 2023, max compression
```

## Comparing `google-cloud-trace-1.9.0.tar` & `google-cloud-trace-1.9.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:28:11.400496 google-cloud-trace-1.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4685 2023-01-10 17:28:11.400496 google-cloud-trace-1.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3775 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:28:11.388496 google-cloud-trace-1.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:28:11.388496 google-cloud-trace-1.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:28:11.392496 google-cloud-trace-1.9.0/google/cloud/trace/
--rw-rw-r--   0 root         (0)     1003     1290 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       79 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:28:11.392496 google-cloud-trace-1.9.0/google/cloud/trace_v1/
--rw-rw-r--   0 root         (0)     1003     1164 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1235 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       79 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:28:11.392496 google-cloud-trace-1.9.0/google/cloud/trace_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:28:11.392496 google-cloud-trace-1.9.0/google/cloud/trace_v1/services/trace_service/
--rw-rw-r--   0 root         (0)     1003      761 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v1/services/trace_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    24134 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v1/services/trace_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    31794 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v1/services/trace_service/client.py
--rw-rw-r--   0 root         (0)     1003     5562 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v1/services/trace_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:28:11.392496 google-cloud-trace-1.9.0/google/cloud/trace_v1/services/trace_service/transports/
--rw-rw-r--   0 root         (0)     1003     1175 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v1/services/trace_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8094 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v1/services/trace_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14424 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v1/services/trace_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14686 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v1/services/trace_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:28:11.392496 google-cloud-trace-1.9.0/google/cloud/trace_v1/types/
--rw-rw-r--   0 root         (0)     1003      912 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    13258 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v1/types/trace.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:28:11.396496 google-cloud-trace-1.9.0/google/cloud/trace_v2/
--rw-rw-r--   0 root         (0)     1003     1117 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     1029 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       79 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:28:11.396496 google-cloud-trace-1.9.0/google/cloud/trace_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:28:11.396496 google-cloud-trace-1.9.0/google/cloud/trace_v2/services/trace_service/
--rw-rw-r--   0 root         (0)     1003      761 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v2/services/trace_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    18246 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v2/services/trace_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    26988 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v2/services/trace_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:28:11.396496 google-cloud-trace-1.9.0/google/cloud/trace_v2/services/trace_service/transports/
--rw-rw-r--   0 root         (0)     1003     1175 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v2/services/trace_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6861 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v2/services/trace_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13049 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v2/services/trace_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13274 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v2/services/trace_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:28:11.396496 google-cloud-trace-1.9.0/google/cloud/trace_v2/types/
--rw-rw-r--   0 root         (0)     1003      859 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    23916 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v2/types/trace.py
--rw-rw-r--   0 root         (0)     1003     1612 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/google/cloud/trace_v2/types/tracing.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:28:11.400496 google-cloud-trace-1.9.0/google_cloud_trace.egg-info/
--rw-r--r--   0 root         (0)     1003     4685 2023-01-10 17:28:11.000000 google-cloud-trace-1.9.0/google_cloud_trace.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2195 2023-01-10 17:28:11.000000 google-cloud-trace-1.9.0/google_cloud_trace.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-10 17:28:11.000000 google-cloud-trace-1.9.0/google_cloud_trace.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-10 17:28:11.000000 google-cloud-trace-1.9.0/google_cloud_trace.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-10 17:28:11.000000 google-cloud-trace-1.9.0/google_cloud_trace.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-01-10 17:28:11.000000 google-cloud-trace-1.9.0/google_cloud_trace.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-10 17:28:11.000000 google-cloud-trace-1.9.0/google_cloud_trace.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-01-10 17:28:11.400496 google-cloud-trace-1.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2966 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:28:11.400496 google-cloud-trace-1.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:28:11.400496 google-cloud-trace-1.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:28:11.400496 google-cloud-trace-1.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:28:11.400496 google-cloud-trace-1.9.0/tests/unit/gapic/trace_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/tests/unit/gapic/trace_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    80999 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/tests/unit/gapic/trace_v1/test_trace_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:28:11.400496 google-cloud-trace-1.9.0/tests/unit/gapic/trace_v2/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/tests/unit/gapic/trace_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003    64526 2023-01-10 17:24:24.000000 google-cloud-trace-1.9.0/tests/unit/gapic/trace_v2/test_trace_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:16.951496 google-cloud-trace-1.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4685 2023-01-23 15:42:16.951496 google-cloud-trace-1.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3775 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:16.915500 google-cloud-trace-1.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:16.915500 google-cloud-trace-1.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:16.923499 google-cloud-trace-1.9.1/google/cloud/trace/
+-rw-rw-r--   0 root         (0)     1003     1290 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       79 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:16.923499 google-cloud-trace-1.9.1/google/cloud/trace_v1/
+-rw-rw-r--   0 root         (0)     1003     1164 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1235 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       79 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:16.923499 google-cloud-trace-1.9.1/google/cloud/trace_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:16.927498 google-cloud-trace-1.9.1/google/cloud/trace_v1/services/trace_service/
+-rw-rw-r--   0 root         (0)     1003      761 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v1/services/trace_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24134 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v1/services/trace_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    31818 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v1/services/trace_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5562 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v1/services/trace_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:16.931498 google-cloud-trace-1.9.1/google/cloud/trace_v1/services/trace_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1175 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v1/services/trace_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8094 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v1/services/trace_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14424 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v1/services/trace_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14686 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v1/services/trace_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:16.931498 google-cloud-trace-1.9.1/google/cloud/trace_v1/types/
+-rw-rw-r--   0 root         (0)     1003      912 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14382 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v1/types/trace.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:16.935498 google-cloud-trace-1.9.1/google/cloud/trace_v2/
+-rw-rw-r--   0 root         (0)     1003     1117 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1029 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       79 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:16.935498 google-cloud-trace-1.9.1/google/cloud/trace_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:16.939497 google-cloud-trace-1.9.1/google/cloud/trace_v2/services/trace_service/
+-rw-rw-r--   0 root         (0)     1003      761 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v2/services/trace_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18246 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v2/services/trace_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27012 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v2/services/trace_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:16.943497 google-cloud-trace-1.9.1/google/cloud/trace_v2/services/trace_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1175 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v2/services/trace_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6861 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v2/services/trace_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13049 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v2/services/trace_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13274 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v2/services/trace_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:16.947497 google-cloud-trace-1.9.1/google/cloud/trace_v2/types/
+-rw-rw-r--   0 root         (0)     1003      859 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25968 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v2/types/trace.py
+-rw-rw-r--   0 root         (0)     1003     1612 2023-01-23 15:38:48.000000 google-cloud-trace-1.9.1/google/cloud/trace_v2/types/tracing.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:16.947497 google-cloud-trace-1.9.1/google_cloud_trace.egg-info/
+-rw-r--r--   0 root         (0)     1003     4685 2023-01-23 15:42:16.000000 google-cloud-trace-1.9.1/google_cloud_trace.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2195 2023-01-23 15:42:16.000000 google-cloud-trace-1.9.1/google_cloud_trace.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 15:42:16.000000 google-cloud-trace-1.9.1/google_cloud_trace.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-01-23 15:42:16.000000 google-cloud-trace-1.9.1/google_cloud_trace.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 15:42:16.000000 google-cloud-trace-1.9.1/google_cloud_trace.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-01-23 15:42:16.000000 google-cloud-trace-1.9.1/google_cloud_trace.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-01-23 15:42:16.000000 google-cloud-trace-1.9.1/google_cloud_trace.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-01-23 15:42:16.951496 google-cloud-trace-1.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2966 2023-01-23 15:38:49.000000 google-cloud-trace-1.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:16.947497 google-cloud-trace-1.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:38:49.000000 google-cloud-trace-1.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:16.947497 google-cloud-trace-1.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:38:49.000000 google-cloud-trace-1.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:16.947497 google-cloud-trace-1.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:38:49.000000 google-cloud-trace-1.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:16.947497 google-cloud-trace-1.9.1/tests/unit/gapic/trace_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:38:49.000000 google-cloud-trace-1.9.1/tests/unit/gapic/trace_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    80999 2023-01-23 15:38:49.000000 google-cloud-trace-1.9.1/tests/unit/gapic/trace_v1/test_trace_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:16.951496 google-cloud-trace-1.9.1/tests/unit/gapic/trace_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:38:49.000000 google-cloud-trace-1.9.1/tests/unit/gapic/trace_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    64526 2023-01-23 15:38:49.000000 google-cloud-trace-1.9.1/tests/unit/gapic/trace_v2/test_trace_service.py
```

### Comparing `google-cloud-trace-1.9.0/LICENSE` & `google-cloud-trace-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/MANIFEST.in` & `google-cloud-trace-1.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/PKG-INFO` & `google-cloud-trace-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-trace
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Trace API client library
 Home-page: https://github.com/googleapis/python-trace
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-trace-1.9.0/README.rst` & `google-cloud-trace-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace/__init__.py` & `google-cloud-trace-1.9.1/google/cloud/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace/gapic_version.py` & `google-cloud-trace-1.9.1/google/cloud/trace/gapic_version.py`

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

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v1/__init__.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v1/gapic_metadata.json` & `google-cloud-trace-1.9.1/google/cloud/trace_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v1/gapic_version.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v1/gapic_version.py`

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

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v1/services/__init__.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v1/services/trace_service/__init__.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v1/services/trace_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v1/services/trace_service/async_client.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v1/services/trace_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v1/services/trace_service/client.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v1/services/trace_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -762,15 +762,15 @@
         rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
-    def __enter__(self):
+    def __enter__(self) -> "TraceServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v1/services/trace_service/pagers.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v1/services/trace_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v1/services/trace_service/transports/__init__.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v1/services/trace_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v1/services/trace_service/transports/base.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v1/services/trace_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v1/services/trace_service/transports/grpc.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v1/services/trace_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v1/services/trace_service/transports/grpc_asyncio.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v1/services/trace_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v1/types/__init__.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v1/types/trace.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v1/types/trace.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,14 +153,26 @@
             -  ``/stacktrace``
             -  ``/tid``
     """
 
     class SpanKind(proto.Enum):
         r"""Type of span. Can be used to specify additional relationships
         between spans in addition to a parent/child relationship.
+
+        Values:
+            SPAN_KIND_UNSPECIFIED (0):
+                Unspecified.
+            RPC_SERVER (1):
+                Indicates that the span covers server-side
+                handling of an RPC or other remote network
+                request.
+            RPC_CLIENT (2):
+                Indicates that the span covers the
+                client-side wrapper around an RPC or other
+                remote request.
         """
         SPAN_KIND_UNSPECIFIED = 0
         RPC_SERVER = 1
         RPC_CLIENT = 2
 
     span_id: int = proto.Field(
         proto.FIXED64,
@@ -272,15 +284,32 @@
             Descending order can be specified by appending ``desc`` to
             the sort field (for example, ``name desc``).
 
             Only one sort field is permitted.
     """
 
     class ViewType(proto.Enum):
-        r"""Type of data returned for traces in the list."""
+        r"""Type of data returned for traces in the list.
+
+        Values:
+            VIEW_TYPE_UNSPECIFIED (0):
+                Default is ``MINIMAL`` if unspecified.
+            MINIMAL (1):
+                Minimal view of the trace record that
+                contains only the project and trace IDs.
+            ROOTSPAN (2):
+                Root span view of the trace record that
+                returns the root spans along with the minimal
+                trace data.
+            COMPLETE (3):
+                Complete view of the trace record that contains the actual
+                trace data. This is equivalent to calling the REST ``get``
+                or RPC ``GetTrace`` method using the ID of each listed
+                trace.
+        """
         VIEW_TYPE_UNSPECIFIED = 0
         MINIMAL = 1
         ROOTSPAN = 2
         COMPLETE = 3
 
     project_id: str = proto.Field(
         proto.STRING,
```

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v2/__init__.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v2/gapic_metadata.json` & `google-cloud-trace-1.9.1/google/cloud/trace_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v2/gapic_version.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v2/gapic_version.py`

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

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v2/services/__init__.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v2/services/trace_service/__init__.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v2/services/trace_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v2/services/trace_service/async_client.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v2/services/trace_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v2/services/trace_service/client.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v2/services/trace_service/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -647,15 +647,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "TraceServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v2/services/trace_service/transports/__init__.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v2/services/trace_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v2/services/trace_service/transports/base.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v2/services/trace_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v2/services/trace_service/transports/grpc.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v2/services/trace_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v2/services/trace_service/transports/grpc_asyncio.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v2/services/trace_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v2/types/__init__.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v2/types/trace.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v2/types/trace.py`

 * *Files 8% similar despite different names*

```diff
@@ -117,14 +117,44 @@
             name may be distinguished using ``CLIENT`` (caller) and
             ``SERVER`` (callee) to identify an RPC call.
     """
 
     class SpanKind(proto.Enum):
         r"""Type of span. Can be used to specify additional relationships
         between spans in addition to a parent/child relationship.
+
+        Values:
+            SPAN_KIND_UNSPECIFIED (0):
+                Unspecified. Do NOT use as default.
+                Implementations MAY assume SpanKind.INTERNAL to
+                be default.
+            INTERNAL (1):
+                Indicates that the span is used internally.
+                Default value.
+            SERVER (2):
+                Indicates that the span covers server-side
+                handling of an RPC or other remote network
+                request.
+            CLIENT (3):
+                Indicates that the span covers the
+                client-side wrapper around an RPC or other
+                remote request.
+            PRODUCER (4):
+                Indicates that the span describes producer
+                sending a message to a broker. Unlike client and
+                server, there is no direct critical path latency
+                relationship between producer and consumer spans
+                (e.g. publishing a message to a pubsub service).
+            CONSUMER (5):
+                Indicates that the span describes consumer
+                receiving a message from a broker. Unlike client
+                and  server, there is no direct critical path
+                latency relationship between producer and
+                consumer spans (e.g. receiving a message from a
+                pubsub service subscription).
         """
         SPAN_KIND_UNSPECIFIED = 0
         INTERNAL = 1
         SERVER = 2
         CLIENT = 3
         PRODUCER = 4
         CONSUMER = 5
@@ -230,15 +260,24 @@
                 compressed_size_bytes (int):
                     The number of compressed bytes sent or
                     received. If missing assumed to be the same size
                     as uncompressed.
             """
 
             class Type(proto.Enum):
-                r"""Indicates whether the message was sent or received."""
+                r"""Indicates whether the message was sent or received.
+
+                Values:
+                    TYPE_UNSPECIFIED (0):
+                        Unknown event type.
+                    SENT (1):
+                        Indicates a sent message.
+                    RECEIVED (2):
+                        Indicates a received message.
+                """
                 TYPE_UNSPECIFIED = 0
                 SENT = 1
                 RECEIVED = 2
 
             type: "Span.TimeEvent.MessageEvent.Type" = proto.Field(
                 proto.ENUM,
                 number=1,
@@ -326,14 +365,24 @@
                 A set of attributes on the link. You have
                 have up to  32 attributes per link.
         """
 
         class Type(proto.Enum):
             r"""The relationship of the current span relative to the linked
             span: child, parent, or unspecified.
+
+            Values:
+                TYPE_UNSPECIFIED (0):
+                    The relationship of the two spans is unknown.
+                CHILD_LINKED_SPAN (1):
+                    The linked span is a child of the current
+                    span.
+                PARENT_LINKED_SPAN (2):
+                    The linked span is a parent of the current
+                    span.
             """
             TYPE_UNSPECIFIED = 0
             CHILD_LINKED_SPAN = 1
             PARENT_LINKED_SPAN = 2
 
         trace_id: str = proto.Field(
             proto.STRING,
```

### Comparing `google-cloud-trace-1.9.0/google/cloud/trace_v2/types/tracing.py` & `google-cloud-trace-1.9.1/google/cloud/trace_v2/types/tracing.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/google_cloud_trace.egg-info/PKG-INFO` & `google-cloud-trace-1.9.1/google_cloud_trace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-trace
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Trace API client library
 Home-page: https://github.com/googleapis/python-trace
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-trace-1.9.0/google_cloud_trace.egg-info/SOURCES.txt` & `google-cloud-trace-1.9.1/google_cloud_trace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/setup.py` & `google-cloud-trace-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/tests/__init__.py` & `google-cloud-trace-1.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/tests/unit/__init__.py` & `google-cloud-trace-1.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/tests/unit/gapic/__init__.py` & `google-cloud-trace-1.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/tests/unit/gapic/trace_v1/__init__.py` & `google-cloud-trace-1.9.1/tests/unit/gapic/trace_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/tests/unit/gapic/trace_v1/test_trace_service.py` & `google-cloud-trace-1.9.1/tests/unit/gapic/trace_v1/test_trace_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/tests/unit/gapic/trace_v2/__init__.py` & `google-cloud-trace-1.9.1/tests/unit/gapic/trace_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-trace-1.9.0/tests/unit/gapic/trace_v2/test_trace_service.py` & `google-cloud-trace-1.9.1/tests/unit/gapic/trace_v2/test_trace_service.py`

 * *Files identical despite different names*

