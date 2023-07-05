# Comparing `tmp/google-cloud-beyondcorp-clientgateways-0.4.1.tar.gz` & `tmp/google-cloud-beyondcorp-clientgateways-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-beyondcorp-clientgateways-0.4.1.tar", last modified: Mon Mar 27 16:03:39 2023, max compression
+gzip compressed data, was "google-cloud-beyondcorp-clientgateways-0.4.2.tar", last modified: Wed Jul  5 15:50:49 2023, max compression
```

## Comparing `google-cloud-beyondcorp-clientgateways-0.4.1.tar` & `google-cloud-beyondcorp-clientgateways-0.4.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:39.024628 google-cloud-beyondcorp-clientgateways-0.4.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5027 2023-03-27 16:03:39.024628 google-cloud-beyondcorp-clientgateways-0.4.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4070 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:39.016627 google-cloud-beyondcorp-clientgateways-0.4.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:39.016627 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:39.020628 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways/
--rw-rw-r--   0 root         (0)     1003     1616 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       99 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:39.020628 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/
--rw-rw-r--   0 root         (0)     1003     1426 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2316 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       99 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:39.020628 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:39.020628 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/
--rw-rw-r--   0 root         (0)     1003      797 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    54914 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    64341 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/client.py
--rw-rw-r--   0 root         (0)     1003     6277 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:39.024628 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/
--rw-rw-r--   0 root         (0)     1003     1519 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10218 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    25521 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    25862 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    65336 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:39.024628 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/types/
--rw-rw-r--   0 root         (0)     1003     1092 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    11775 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/types/client_gateways_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:39.024628 google-cloud-beyondcorp-clientgateways-0.4.1/google_cloud_beyondcorp_clientgateways.egg-info/
--rw-r--r--   0 root         (0)     1003     5027 2023-03-27 16:03:38.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google_cloud_beyondcorp_clientgateways.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2105 2023-03-27 16:03:38.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google_cloud_beyondcorp_clientgateways.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:03:38.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google_cloud_beyondcorp_clientgateways.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 16:03:38.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google_cloud_beyondcorp_clientgateways.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:03:38.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google_cloud_beyondcorp_clientgateways.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 16:03:38.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google_cloud_beyondcorp_clientgateways.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 16:03:38.000000 google-cloud-beyondcorp-clientgateways-0.4.1/google_cloud_beyondcorp_clientgateways.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 16:03:39.024628 google-cloud-beyondcorp-clientgateways-0.4.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3060 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:39.024628 google-cloud-beyondcorp-clientgateways-0.4.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:39.024628 google-cloud-beyondcorp-clientgateways-0.4.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:39.024628 google-cloud-beyondcorp-clientgateways-0.4.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:39.024628 google-cloud-beyondcorp-clientgateways-0.4.1/tests/unit/gapic/beyondcorp_clientgateways_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/tests/unit/gapic/beyondcorp_clientgateways_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   215698 2023-03-27 16:00:59.000000 google-cloud-beyondcorp-clientgateways-0.4.1/tests/unit/gapic/beyondcorp_clientgateways_v1/test_client_gateways_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:49.642108 google-cloud-beyondcorp-clientgateways-0.4.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4978 2023-07-05 15:50:49.642108 google-cloud-beyondcorp-clientgateways-0.4.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4034 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:49.634107 google-cloud-beyondcorp-clientgateways-0.4.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:49.634107 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:49.638108 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways/
+-rw-rw-r--   0 root         (0)     1003     1616 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       99 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:49.638108 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/
+-rw-rw-r--   0 root         (0)     1003     1426 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2316 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       99 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:49.638108 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:49.638108 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/
+-rw-rw-r--   0 root         (0)     1003      797 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    54952 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    64341 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6277 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:49.642108 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1519 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10218 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    25521 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    25862 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    65300 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:49.642108 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1092 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11775 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/types/client_gateways_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:49.642108 google-cloud-beyondcorp-clientgateways-0.4.2/google_cloud_beyondcorp_clientgateways.egg-info/
+-rw-r--r--   0 root         (0)     1003     4978 2023-07-05 15:50:49.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google_cloud_beyondcorp_clientgateways.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2105 2023-07-05 15:50:49.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google_cloud_beyondcorp_clientgateways.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:49.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google_cloud_beyondcorp_clientgateways.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:50:49.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google_cloud_beyondcorp_clientgateways.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:49.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google_cloud_beyondcorp_clientgateways.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:50:49.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google_cloud_beyondcorp_clientgateways.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:50:49.000000 google-cloud-beyondcorp-clientgateways-0.4.2/google_cloud_beyondcorp_clientgateways.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:50:49.646108 google-cloud-beyondcorp-clientgateways-0.4.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3047 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:49.642108 google-cloud-beyondcorp-clientgateways-0.4.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:49.642108 google-cloud-beyondcorp-clientgateways-0.4.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:49.642108 google-cloud-beyondcorp-clientgateways-0.4.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:49.642108 google-cloud-beyondcorp-clientgateways-0.4.2/tests/unit/gapic/beyondcorp_clientgateways_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/tests/unit/gapic/beyondcorp_clientgateways_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   215897 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientgateways-0.4.2/tests/unit/gapic/beyondcorp_clientgateways_v1/test_client_gateways_service.py
```

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/LICENSE` & `google-cloud-beyondcorp-clientgateways-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/MANIFEST.in` & `google-cloud-beyondcorp-clientgateways-0.4.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/PKG-INFO` & `google-cloud-beyondcorp-clientgateways-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-beyondcorp-clientgateways
-Version: 0.4.1
+Version: 0.4.2
 Summary: Google Cloud Beyondcorp Clientgateways API client library
-Home-page: https://github.com/googleapis/python-beyondcorp-clientgateways
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
 
-Python Client for BeyondCorp ClientGateways API
-===============================================
+Python Client for BeyondCorp ClientGateways
+===========================================
 
 |preview| |pypi| |versions|
 
-`BeyondCorp ClientGateways API`_: Beyondcorp Enterprise provides identity and context aware access controls for enterprise resources and enables zero-trust access. Using the Beyondcorp Enterprise APIs, enterprises can set up multi-cloud and on-prem connectivity using the App Connector hybrid connectivity solution.
+`BeyondCorp ClientGateways`_: Beyondcorp Enterprise provides identity and context aware access controls for enterprise resources and enables zero-trust access. Using the Beyondcorp Enterprise APIs, enterprises can set up multi-cloud and on-prem connectivity using the App Connector hybrid connectivity solution.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-beyondcorp-clientgateways.svg
    :target: https://pypi.org/project/google-cloud-beyondcorp-clientgateways/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-beyondcorp-clientgateways.svg
    :target: https://pypi.org/project/google-cloud-beyondcorp-clientgateways/
-.. _BeyondCorp ClientGateways API: https://cloud.google.com/beyondcorp/
+.. _BeyondCorp ClientGateways: https://cloud.google.com/beyondcorp/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/beyondcorpclientgateways/latest
 .. _Product Documentation:  https://cloud.google.com/beyondcorp/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the BeyondCorp ClientGateways API.`_
+3. `Enable the BeyondCorp ClientGateways.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the BeyondCorp ClientGateways API.:  https://cloud.google.com/beyondcorp/
+.. _Enable the BeyondCorp ClientGateways.:  https://cloud.google.com/beyondcorp/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-beyondcorp-clientgateways
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for BeyondCorp ClientGateways API
+-  Read the `Client Library Documentation`_ for BeyondCorp ClientGateways
    to see other available methods on the client.
--  Read the `BeyondCorp ClientGateways API Product documentation`_ to learn
+-  Read the `BeyondCorp ClientGateways Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _BeyondCorp ClientGateways API Product documentation:  https://cloud.google.com/beyondcorp/
+.. _BeyondCorp ClientGateways Product documentation:  https://cloud.google.com/beyondcorp/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/README.rst` & `google-cloud-beyondcorp-clientgateways-0.4.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for BeyondCorp ClientGateways API
-===============================================
+Python Client for BeyondCorp ClientGateways
+===========================================
 
 |preview| |pypi| |versions|
 
-`BeyondCorp ClientGateways API`_: Beyondcorp Enterprise provides identity and context aware access controls for enterprise resources and enables zero-trust access. Using the Beyondcorp Enterprise APIs, enterprises can set up multi-cloud and on-prem connectivity using the App Connector hybrid connectivity solution.
+`BeyondCorp ClientGateways`_: Beyondcorp Enterprise provides identity and context aware access controls for enterprise resources and enables zero-trust access. Using the Beyondcorp Enterprise APIs, enterprises can set up multi-cloud and on-prem connectivity using the App Connector hybrid connectivity solution.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-beyondcorp-clientgateways.svg
    :target: https://pypi.org/project/google-cloud-beyondcorp-clientgateways/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-beyondcorp-clientgateways.svg
    :target: https://pypi.org/project/google-cloud-beyondcorp-clientgateways/
-.. _BeyondCorp ClientGateways API: https://cloud.google.com/beyondcorp/
+.. _BeyondCorp ClientGateways: https://cloud.google.com/beyondcorp/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/beyondcorpclientgateways/latest
 .. _Product Documentation:  https://cloud.google.com/beyondcorp/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the BeyondCorp ClientGateways API.`_
+3. `Enable the BeyondCorp ClientGateways.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the BeyondCorp ClientGateways API.:  https://cloud.google.com/beyondcorp/
+.. _Enable the BeyondCorp ClientGateways.:  https://cloud.google.com/beyondcorp/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-beyondcorp-clientgateways
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for BeyondCorp ClientGateways API
+-  Read the `Client Library Documentation`_ for BeyondCorp ClientGateways
    to see other available methods on the client.
--  Read the `BeyondCorp ClientGateways API Product documentation`_ to learn
+-  Read the `BeyondCorp ClientGateways Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _BeyondCorp ClientGateways API Product documentation:  https://cloud.google.com/beyondcorp/
+.. _BeyondCorp ClientGateways Product documentation:  https://cloud.google.com/beyondcorp/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways/__init__.py` & `google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways/gapic_version.py` & `google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.4.1"  # {x-release-please-version}
```

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/__init__.py` & `google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/gapic_metadata.json` & `google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/gapic_version.py` & `google-cloud-beyondcorp-clientgateways-0.4.2/tests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.4.1"  # {x-release-please-version}
```

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/__init__.py` & `google-cloud-beyondcorp-clientgateways-0.4.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/__init__.py` & `google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/async_client.py` & `google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1346,15 +1346,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ClientGatewaysServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/client.py` & `google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/pagers.py` & `google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/__init__.py` & `google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/base.py` & `google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/grpc.py` & `google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/grpc_asyncio.py` & `google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/rest.py` & `google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/services/client_gateways_service/transports/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1257,15 +1257,15 @@
                 },
             ]
 
             request, metadata = self._interceptor.pre_set_iam_policy(request, metadata)
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
@@ -1349,15 +1349,15 @@
 
             request, metadata = self._interceptor.pre_test_iam_permissions(
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
@@ -1418,15 +1418,15 @@
 
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

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/types/__init__.py` & `google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/google/cloud/beyondcorp_clientgateways_v1/types/client_gateways_service.py` & `google-cloud-beyondcorp-clientgateways-0.4.2/google/cloud/beyondcorp_clientgateways_v1/types/client_gateways_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/google_cloud_beyondcorp_clientgateways.egg-info/PKG-INFO` & `google-cloud-beyondcorp-clientgateways-0.4.2/google_cloud_beyondcorp_clientgateways.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-beyondcorp-clientgateways
-Version: 0.4.1
+Version: 0.4.2
 Summary: Google Cloud Beyondcorp Clientgateways API client library
-Home-page: https://github.com/googleapis/python-beyondcorp-clientgateways
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
 
-Python Client for BeyondCorp ClientGateways API
-===============================================
+Python Client for BeyondCorp ClientGateways
+===========================================
 
 |preview| |pypi| |versions|
 
-`BeyondCorp ClientGateways API`_: Beyondcorp Enterprise provides identity and context aware access controls for enterprise resources and enables zero-trust access. Using the Beyondcorp Enterprise APIs, enterprises can set up multi-cloud and on-prem connectivity using the App Connector hybrid connectivity solution.
+`BeyondCorp ClientGateways`_: Beyondcorp Enterprise provides identity and context aware access controls for enterprise resources and enables zero-trust access. Using the Beyondcorp Enterprise APIs, enterprises can set up multi-cloud and on-prem connectivity using the App Connector hybrid connectivity solution.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-beyondcorp-clientgateways.svg
    :target: https://pypi.org/project/google-cloud-beyondcorp-clientgateways/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-beyondcorp-clientgateways.svg
    :target: https://pypi.org/project/google-cloud-beyondcorp-clientgateways/
-.. _BeyondCorp ClientGateways API: https://cloud.google.com/beyondcorp/
+.. _BeyondCorp ClientGateways: https://cloud.google.com/beyondcorp/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/beyondcorpclientgateways/latest
 .. _Product Documentation:  https://cloud.google.com/beyondcorp/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the BeyondCorp ClientGateways API.`_
+3. `Enable the BeyondCorp ClientGateways.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the BeyondCorp ClientGateways API.:  https://cloud.google.com/beyondcorp/
+.. _Enable the BeyondCorp ClientGateways.:  https://cloud.google.com/beyondcorp/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-beyondcorp-clientgateways
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for BeyondCorp ClientGateways API
+-  Read the `Client Library Documentation`_ for BeyondCorp ClientGateways
    to see other available methods on the client.
--  Read the `BeyondCorp ClientGateways API Product documentation`_ to learn
+-  Read the `BeyondCorp ClientGateways Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _BeyondCorp ClientGateways API Product documentation:  https://cloud.google.com/beyondcorp/
+.. _BeyondCorp ClientGateways Product documentation:  https://cloud.google.com/beyondcorp/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/google_cloud_beyondcorp_clientgateways.egg-info/SOURCES.txt` & `google-cloud-beyondcorp-clientgateways-0.4.2/google_cloud_beyondcorp_clientgateways.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/setup.py` & `google-cloud-beyondcorp-clientgateways-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
-url = "https://github.com/googleapis/python-beyondcorp-clientgateways"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/tests/__init__.py` & `google-cloud-beyondcorp-clientgateways-0.4.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/tests/unit/__init__.py` & `google-cloud-beyondcorp-clientgateways-0.4.2/tests/unit/gapic/beyondcorp_clientgateways_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientgateways-0.4.1/tests/unit/gapic/beyondcorp_clientgateways_v1/test_client_gateways_service.py` & `google-cloud-beyondcorp-clientgateways-0.4.2/tests/unit/gapic/beyondcorp_clientgateways_v1/test_client_gateways_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1203,17 +1203,19 @@
                     client_gateways_service.ClientGateway(),
                     client_gateways_service.ClientGateway(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_client_gateways(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

