# Comparing `tmp/google-cloud-apigee-connect-1.7.0.tar.gz` & `tmp/google-cloud-apigee-connect-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-apigee-connect-1.7.0.tar", last modified: Wed Jan 11 19:57:47 2023, max compression
+gzip compressed data, was "google-cloud-apigee-connect-1.7.2.tar", last modified: Wed Jul  5 15:50:11 2023, max compression
```

## Comparing `google-cloud-apigee-connect-1.7.0.tar` & `google-cloud-apigee-connect-1.7.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 19:57:47.345542 google-cloud-apigee-connect-1.7.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4822 2023-01-11 19:57:47.345542 google-cloud-apigee-connect-1.7.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3885 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 19:57:47.333542 google-cloud-apigee-connect-1.7.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 19:57:47.337542 google-cloud-apigee-connect-1.7.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 19:57:47.337542 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect/
--rw-rw-r--   0 root         (0)     1003     1902 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       88 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 19:57:47.337542 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/
--rw-rw-r--   0 root         (0)     1003     1615 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1298 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       88 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 19:57:47.337542 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 19:57:47.341542 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/connection_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/connection_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    14568 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/connection_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    23022 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/connection_service/client.py
--rw-rw-r--   0 root         (0)     1003     5859 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/connection_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 19:57:47.341542 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/connection_service/transports/
--rw-rw-r--   0 root         (0)     1003     1220 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/connection_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6481 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/connection_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    11881 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/connection_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12098 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/connection_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 19:57:47.341542 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/tether/
--rw-rw-r--   0 root         (0)     1003      737 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/tether/__init__.py
--rw-rw-r--   0 root         (0)     1003    12604 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/tether/async_client.py
--rw-rw-r--   0 root         (0)     1003    20837 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/tether/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 19:57:47.341542 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/tether/transports/
--rw-rw-r--   0 root         (0)     1003     1121 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/tether/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     5948 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/tether/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12144 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/tether/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12356 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/tether/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 19:57:47.341542 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/types/
--rw-rw-r--   0 root         (0)     1003     1205 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3834 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/types/connection.py
--rw-rw-r--   0 root         (0)     1003     9467 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/types/tether.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 19:57:47.345542 google-cloud-apigee-connect-1.7.0/google_cloud_apigee_connect.egg-info/
--rw-r--r--   0 root         (0)     1003     4822 2023-01-11 19:57:47.000000 google-cloud-apigee-connect-1.7.0/google_cloud_apigee_connect.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2179 2023-01-11 19:57:47.000000 google-cloud-apigee-connect-1.7.0/google_cloud_apigee_connect.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-11 19:57:47.000000 google-cloud-apigee-connect-1.7.0/google_cloud_apigee_connect.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-11 19:57:47.000000 google-cloud-apigee-connect-1.7.0/google_cloud_apigee_connect.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-11 19:57:47.000000 google-cloud-apigee-connect-1.7.0/google_cloud_apigee_connect.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-01-11 19:57:47.000000 google-cloud-apigee-connect-1.7.0/google_cloud_apigee_connect.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-11 19:57:47.000000 google-cloud-apigee-connect-1.7.0/google_cloud_apigee_connect.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-01-11 19:57:47.345542 google-cloud-apigee-connect-1.7.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3007 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 19:57:47.345542 google-cloud-apigee-connect-1.7.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 19:57:47.345542 google-cloud-apigee-connect-1.7.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 19:57:47.345542 google-cloud-apigee-connect-1.7.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 19:57:47.345542 google-cloud-apigee-connect-1.7.0/tests/unit/gapic/apigeeconnect_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/tests/unit/gapic/apigeeconnect_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    66012 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/tests/unit/gapic/apigeeconnect_v1/test_connection_service.py
--rw-rw-r--   0 root         (0)     1003    50792 2023-01-11 19:54:24.000000 google-cloud-apigee-connect-1.7.0/tests/unit/gapic/apigeeconnect_v1/test_tether.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:11.162911 google-cloud-apigee-connect-1.7.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4784 2023-07-05 15:50:11.162911 google-cloud-apigee-connect-1.7.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3849 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:11.154910 google-cloud-apigee-connect-1.7.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:11.154910 google-cloud-apigee-connect-1.7.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:11.158911 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect/
+-rw-rw-r--   0 root         (0)     1003     1902 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       88 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:11.158911 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/
+-rw-rw-r--   0 root         (0)     1003     1618 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1298 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       88 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:11.158911 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:11.158911 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/connection_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/connection_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14602 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/connection_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    23051 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/connection_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5859 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/connection_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:11.158911 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/connection_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1220 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/connection_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6481 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/connection_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    11881 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/connection_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12098 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/connection_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:11.158911 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/tether/
+-rw-rw-r--   0 root         (0)     1003      737 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/tether/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12627 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/tether/async_client.py
+-rw-rw-r--   0 root         (0)     1003    20855 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/tether/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:11.162911 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/tether/transports/
+-rw-rw-r--   0 root         (0)     1003     1121 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/tether/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5948 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/tether/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12144 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/tether/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12356 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/tether/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:11.162911 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1205 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3870 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/types/connection.py
+-rw-rw-r--   0 root         (0)     1003    10111 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/types/tether.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:11.162911 google-cloud-apigee-connect-1.7.2/google_cloud_apigee_connect.egg-info/
+-rw-r--r--   0 root         (0)     1003     4784 2023-07-05 15:50:11.000000 google-cloud-apigee-connect-1.7.2/google_cloud_apigee_connect.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2179 2023-07-05 15:50:11.000000 google-cloud-apigee-connect-1.7.2/google_cloud_apigee_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:11.000000 google-cloud-apigee-connect-1.7.2/google_cloud_apigee_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:50:11.000000 google-cloud-apigee-connect-1.7.2/google_cloud_apigee_connect.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:11.000000 google-cloud-apigee-connect-1.7.2/google_cloud_apigee_connect.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:50:11.000000 google-cloud-apigee-connect-1.7.2/google_cloud_apigee_connect.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:50:11.000000 google-cloud-apigee-connect-1.7.2/google_cloud_apigee_connect.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:50:11.162911 google-cloud-apigee-connect-1.7.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2952 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:11.162911 google-cloud-apigee-connect-1.7.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:11.162911 google-cloud-apigee-connect-1.7.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:11.162911 google-cloud-apigee-connect-1.7.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:11.162911 google-cloud-apigee-connect-1.7.2/tests/unit/gapic/apigeeconnect_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/tests/unit/gapic/apigeeconnect_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    66211 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/tests/unit/gapic/apigeeconnect_v1/test_connection_service.py
+-rw-rw-r--   0 root         (0)     1003    50792 2023-07-05 15:46:58.000000 google-cloud-apigee-connect-1.7.2/tests/unit/gapic/apigeeconnect_v1/test_tether.py
```

### Comparing `google-cloud-apigee-connect-1.7.0/LICENSE` & `google-cloud-apigee-connect-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/MANIFEST.in` & `google-cloud-apigee-connect-1.7.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/PKG-INFO` & `google-cloud-apigee-connect-1.7.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-apigee-connect
-Version: 1.7.0
+Version: 1.7.2
 Summary: Google Cloud Apigee Connect API client library
-Home-page: https://github.com/googleapis/python-apigee-connect
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
 
-Python Client for Apigee Connect API
-====================================
+Python Client for Apigee Connect
+================================
 
 |stable| |pypi| |versions|
 
-`Apigee Connect API`_: allows the Apigee hybrid management plane to connect securely to the MART service in the runtime plane without requiring you to expose the MART endpoint on the internet.
+`Apigee Connect`_: allows the Apigee hybrid management plane to connect securely to the MART service in the runtime plane without requiring you to expose the MART endpoint on the internet.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-apigee-connect.svg
    :target: https://pypi.org/project/google-cloud-apigee-connect/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-apigee-connect.svg
    :target: https://pypi.org/project/google-cloud-apigee-connect/
-.. _Apigee Connect API: https://cloud.google.com/apigee/docs/hybrid/v1.4/apigee-connect
+.. _Apigee Connect: https://cloud.google.com/apigee/docs/hybrid/v1.4/apigee-connect
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/apigeeconnect/latest
 .. _Product Documentation:  https://cloud.google.com/apigee/docs/hybrid/v1.4/apigee-connect
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Apigee Connect API.`_
+3. `Enable the Apigee Connect.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Apigee Connect API.:  https://cloud.google.com/apigee/docs/hybrid/v1.4/apigee-connect
+.. _Enable the Apigee Connect.:  https://cloud.google.com/apigee/docs/hybrid/v1.4/apigee-connect
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-apigee-connect
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Apigee Connect API
+-  Read the `Client Library Documentation`_ for Apigee Connect
    to see other available methods on the client.
--  Read the `Apigee Connect API Product documentation`_ to learn
+-  Read the `Apigee Connect Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Apigee Connect API Product documentation:  https://cloud.google.com/apigee/docs/hybrid/v1.4/apigee-connect
+.. _Apigee Connect Product documentation:  https://cloud.google.com/apigee/docs/hybrid/v1.4/apigee-connect
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-apigee-connect-1.7.0/README.rst` & `google-cloud-apigee-connect-1.7.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Apigee Connect API
-====================================
+Python Client for Apigee Connect
+================================
 
 |stable| |pypi| |versions|
 
-`Apigee Connect API`_: allows the Apigee hybrid management plane to connect securely to the MART service in the runtime plane without requiring you to expose the MART endpoint on the internet.
+`Apigee Connect`_: allows the Apigee hybrid management plane to connect securely to the MART service in the runtime plane without requiring you to expose the MART endpoint on the internet.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-apigee-connect.svg
    :target: https://pypi.org/project/google-cloud-apigee-connect/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-apigee-connect.svg
    :target: https://pypi.org/project/google-cloud-apigee-connect/
-.. _Apigee Connect API: https://cloud.google.com/apigee/docs/hybrid/v1.4/apigee-connect
+.. _Apigee Connect: https://cloud.google.com/apigee/docs/hybrid/v1.4/apigee-connect
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/apigeeconnect/latest
 .. _Product Documentation:  https://cloud.google.com/apigee/docs/hybrid/v1.4/apigee-connect
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Apigee Connect API.`_
+3. `Enable the Apigee Connect.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Apigee Connect API.:  https://cloud.google.com/apigee/docs/hybrid/v1.4/apigee-connect
+.. _Enable the Apigee Connect.:  https://cloud.google.com/apigee/docs/hybrid/v1.4/apigee-connect
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-apigee-connect
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Apigee Connect API
+-  Read the `Client Library Documentation`_ for Apigee Connect
    to see other available methods on the client.
--  Read the `Apigee Connect API Product documentation`_ to learn
+-  Read the `Apigee Connect Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Apigee Connect API Product documentation:  https://cloud.google.com/apigee/docs/hybrid/v1.4/apigee-connect
+.. _Apigee Connect Product documentation:  https://cloud.google.com/apigee/docs/hybrid/v1.4/apigee-connect
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect/__init__.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect/gapic_version.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect/gapic_version.py`

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
-__version__ = "1.7.0"  # {x-release-please-version}
+__version__ = "1.7.2"  # {x-release-please-version}
```

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/__init__.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.apigeeconnect import gapic_version as package_version
+from google.cloud.apigeeconnect_v1 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
 from .services.connection_service import (
     ConnectionServiceAsyncClient,
     ConnectionServiceClient,
```

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/gapic_metadata.json` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/gapic_version.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/gapic_version.py`

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
-__version__ = "1.7.0"  # {x-release-please-version}
+__version__ = "1.7.2"  # {x-release-please-version}
```

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/__init__.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/connection_service/__init__.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/connection_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/connection_service/async_client.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/connection_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,15 +338,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ConnectionServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/connection_service/client.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/connection_service/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -550,15 +550,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "ConnectionServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/connection_service/pagers.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/connection_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/connection_service/transports/__init__.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/connection_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/connection_service/transports/base.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/connection_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/connection_service/transports/grpc.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/connection_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/connection_service/transports/grpc_asyncio.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/connection_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/tether/__init__.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/tether/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/tether/async_client.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/tether/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,15 +293,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "TetherAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/tether/client.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/tether/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -503,15 +503,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "TetherClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/tether/transports/__init__.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/tether/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/tether/transports/base.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/tether/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/tether/transports/grpc.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/tether/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/services/tether/transports/grpc_asyncio.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/services/tether/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/types/__init__.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/types/connection.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/types/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.apigeeconnect.v1",
     manifest={
```

### Comparing `google-cloud-apigee-connect-1.7.0/google/cloud/apigeeconnect_v1/types/tether.py` & `google-cloud-apigee-connect-1.7.2/google/cloud/apigeeconnect_v1/types/tether.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import duration_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
@@ -34,29 +36,55 @@
         "Header",
         "HttpResponse",
     },
 )
 
 
 class Action(proto.Enum):
-    r"""The action taken by agent."""
+    r"""The action taken by agent.
+
+    Values:
+        ACTION_UNSPECIFIED (0):
+            Unspecified Action.
+        OPEN_NEW_STREAM (1):
+            Indicates that agent should open a new
+            stream.
+    """
     ACTION_UNSPECIFIED = 0
     OPEN_NEW_STREAM = 1
 
 
 class TetherEndpoint(proto.Enum):
-    r"""Endpoint indicates where the messages will be delivered."""
+    r"""Endpoint indicates where the messages will be delivered.
+
+    Values:
+        TETHER_ENDPOINT_UNSPECIFIED (0):
+            Unspecified tether endpoint.
+        APIGEE_MART (1):
+            Apigee MART endpoint.
+        APIGEE_RUNTIME (2):
+            Apigee Runtime endpoint.
+        APIGEE_MINT_RATING (3):
+            Apigee Mint Rating endpoint.
+    """
     TETHER_ENDPOINT_UNSPECIFIED = 0
     APIGEE_MART = 1
     APIGEE_RUNTIME = 2
     APIGEE_MINT_RATING = 3
 
 
 class Scheme(proto.Enum):
-    r"""HTTP Scheme."""
+    r"""HTTP Scheme.
+
+    Values:
+        SCHEME_UNSPECIFIED (0):
+            Unspecified scheme.
+        HTTPS (1):
+            HTTPS protocol.
+    """
     SCHEME_UNSPECIFIED = 0
     HTTPS = 1
 
 
 class EgressRequest(proto.Message):
     r"""gRPC request payload for tether.
```

### Comparing `google-cloud-apigee-connect-1.7.0/google_cloud_apigee_connect.egg-info/PKG-INFO` & `google-cloud-apigee-connect-1.7.2/google_cloud_apigee_connect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-apigee-connect
-Version: 1.7.0
+Version: 1.7.2
 Summary: Google Cloud Apigee Connect API client library
-Home-page: https://github.com/googleapis/python-apigee-connect
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
 
-Python Client for Apigee Connect API
-====================================
+Python Client for Apigee Connect
+================================
 
 |stable| |pypi| |versions|
 
-`Apigee Connect API`_: allows the Apigee hybrid management plane to connect securely to the MART service in the runtime plane without requiring you to expose the MART endpoint on the internet.
+`Apigee Connect`_: allows the Apigee hybrid management plane to connect securely to the MART service in the runtime plane without requiring you to expose the MART endpoint on the internet.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-apigee-connect.svg
    :target: https://pypi.org/project/google-cloud-apigee-connect/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-apigee-connect.svg
    :target: https://pypi.org/project/google-cloud-apigee-connect/
-.. _Apigee Connect API: https://cloud.google.com/apigee/docs/hybrid/v1.4/apigee-connect
+.. _Apigee Connect: https://cloud.google.com/apigee/docs/hybrid/v1.4/apigee-connect
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/apigeeconnect/latest
 .. _Product Documentation:  https://cloud.google.com/apigee/docs/hybrid/v1.4/apigee-connect
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Apigee Connect API.`_
+3. `Enable the Apigee Connect.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Apigee Connect API.:  https://cloud.google.com/apigee/docs/hybrid/v1.4/apigee-connect
+.. _Enable the Apigee Connect.:  https://cloud.google.com/apigee/docs/hybrid/v1.4/apigee-connect
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-apigee-connect
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Apigee Connect API
+-  Read the `Client Library Documentation`_ for Apigee Connect
    to see other available methods on the client.
--  Read the `Apigee Connect API Product documentation`_ to learn
+-  Read the `Apigee Connect Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Apigee Connect API Product documentation:  https://cloud.google.com/apigee/docs/hybrid/v1.4/apigee-connect
+.. _Apigee Connect Product documentation:  https://cloud.google.com/apigee/docs/hybrid/v1.4/apigee-connect
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-apigee-connect-1.7.0/google_cloud_apigee_connect.egg-info/SOURCES.txt` & `google-cloud-apigee-connect-1.7.2/google_cloud_apigee_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/setup.py` & `google-cloud-apigee-connect-1.7.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,31 +39,29 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-apigee-connect"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 packages = [
     package
     for package in setuptools.PEP420PackageFinder.find()
     if package.startswith("google")
 ]
 
-namespaces = ["google"]
-if "google.cloud" in packages:
-    namespaces.append("google.cloud")
+namespaces = ["google", "google.cloud"]
 
 setuptools.setup(
     name=name,
     version=version,
     description=description,
     long_description=readme,
     author="Google LLC",
```

### Comparing `google-cloud-apigee-connect-1.7.0/tests/__init__.py` & `google-cloud-apigee-connect-1.7.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/tests/unit/__init__.py` & `google-cloud-apigee-connect-1.7.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/tests/unit/gapic/__init__.py` & `google-cloud-apigee-connect-1.7.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/tests/unit/gapic/apigeeconnect_v1/__init__.py` & `google-cloud-apigee-connect-1.7.2/tests/unit/gapic/apigeeconnect_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-connect-1.7.0/tests/unit/gapic/apigeeconnect_v1/test_connection_service.py` & `google-cloud-apigee-connect-1.7.2/tests/unit/gapic/apigeeconnect_v1/test_connection_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1103,17 +1103,19 @@
                     connection.Connection(),
                     connection.Connection(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_connections(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
```

### Comparing `google-cloud-apigee-connect-1.7.0/tests/unit/gapic/apigeeconnect_v1/test_tether.py` & `google-cloud-apigee-connect-1.7.2/tests/unit/gapic/apigeeconnect_v1/test_tether.py`

 * *Files identical despite different names*

