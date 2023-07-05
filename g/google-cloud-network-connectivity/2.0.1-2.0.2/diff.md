# Comparing `tmp/google-cloud-network-connectivity-2.0.1.tar.gz` & `tmp/google-cloud-network-connectivity-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-network-connectivity-2.0.1.tar", last modified: Mon Mar 27 16:14:07 2023, max compression
+gzip compressed data, was "google-cloud-network-connectivity-2.0.2.tar", last modified: Wed Jul  5 15:54:09 2023, max compression
```

## Comparing `google-cloud-network-connectivity-2.0.1.tar` & `google-cloud-network-connectivity-2.0.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:14:07.272462 google-cloud-network-connectivity-2.0.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5131 2023-03-27 16:14:07.272462 google-cloud-network-connectivity-2.0.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4176 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:14:07.260461 google-cloud-network-connectivity-2.0.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:14:07.260461 google-cloud-network-connectivity-2.0.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:14:07.264461 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity/
--rw-rw-r--   0 root         (0)     1003     2176 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       94 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:14:07.264461 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/
--rw-rw-r--   0 root         (0)     1003     1968 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2845 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       94 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:14:07.264461 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:14:07.264461 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/services/hub_service/
--rw-rw-r--   0 root         (0)     1003      753 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/services/hub_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    86576 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/services/hub_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    99067 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/services/hub_service/client.py
--rw-rw-r--   0 root         (0)     1003    10468 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/services/hub_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:14:07.264461 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/services/hub_service/transports/
--rw-rw-r--   0 root         (0)     1003     1157 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/services/hub_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12177 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/services/hub_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    31097 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/services/hub_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    31586 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/services/hub_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:14:07.268462 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/types/
--rw-rw-r--   0 root         (0)     1003     1703 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2865 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003    30582 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/types/hub.py
--rw-rw-r--   0 root         (0)     1003    17025 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/types/policy_based_routing.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:14:07.268462 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/
--rw-rw-r--   0 root         (0)     1003     1658 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2857 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       94 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:14:07.268462 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:14:07.268462 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/services/hub_service/
--rw-rw-r--   0 root         (0)     1003      753 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/services/hub_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    60368 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/services/hub_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    72567 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/services/hub_service/client.py
--rw-rw-r--   0 root         (0)     1003    10570 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/services/hub_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:14:07.268462 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/services/hub_service/transports/
--rw-rw-r--   0 root         (0)     1003     1157 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/services/hub_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9867 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/services/hub_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22022 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/services/hub_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    22511 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/services/hub_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:14:07.268462 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/types/
--rw-rw-r--   0 root         (0)     1003     1387 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2871 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/types/common.py
--rw-rw-r--   0 root         (0)     1003    23044 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/types/hub.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:14:07.272462 google-cloud-network-connectivity-2.0.1/google_cloud_network_connectivity.egg-info/
--rw-r--r--   0 root         (0)     1003     5131 2023-03-27 16:14:07.000000 google-cloud-network-connectivity-2.0.1/google_cloud_network_connectivity.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3072 2023-03-27 16:14:07.000000 google-cloud-network-connectivity-2.0.1/google_cloud_network_connectivity.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:14:07.000000 google-cloud-network-connectivity-2.0.1/google_cloud_network_connectivity.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 16:14:07.000000 google-cloud-network-connectivity-2.0.1/google_cloud_network_connectivity.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:14:07.000000 google-cloud-network-connectivity-2.0.1/google_cloud_network_connectivity.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 16:14:07.000000 google-cloud-network-connectivity-2.0.1/google_cloud_network_connectivity.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 16:14:07.000000 google-cloud-network-connectivity-2.0.1/google_cloud_network_connectivity.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 16:14:07.272462 google-cloud-network-connectivity-2.0.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3025 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:14:07.272462 google-cloud-network-connectivity-2.0.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:14:07.272462 google-cloud-network-connectivity-2.0.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:14:07.272462 google-cloud-network-connectivity-2.0.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:14:07.272462 google-cloud-network-connectivity-2.0.1/tests/unit/gapic/networkconnectivity_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/tests/unit/gapic/networkconnectivity_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   199461 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/tests/unit/gapic/networkconnectivity_v1/test_hub_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:14:07.272462 google-cloud-network-connectivity-2.0.1/tests/unit/gapic/networkconnectivity_v1alpha1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/tests/unit/gapic/networkconnectivity_v1alpha1/__init__.py
--rw-rw-r--   0 root         (0)     1003   149479 2023-03-27 16:11:34.000000 google-cloud-network-connectivity-2.0.1/tests/unit/gapic/networkconnectivity_v1alpha1/test_hub_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:09.196500 google-cloud-network-connectivity-2.0.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5087 2023-07-05 15:54:09.196500 google-cloud-network-connectivity-2.0.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4140 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:09.184500 google-cloud-network-connectivity-2.0.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:09.184500 google-cloud-network-connectivity-2.0.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:09.188500 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity/
+-rw-rw-r--   0 root         (0)     1003     2176 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       94 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:09.188500 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/
+-rw-rw-r--   0 root         (0)     1003     1968 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2845 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       94 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:09.188500 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:09.188500 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/services/hub_service/
+-rw-rw-r--   0 root         (0)     1003      753 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/services/hub_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    86603 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/services/hub_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    99067 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/services/hub_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10468 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/services/hub_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:09.188500 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/services/hub_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1157 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/services/hub_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12177 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/services/hub_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    31097 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/services/hub_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    31586 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/services/hub_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:09.192500 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1703 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2865 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003    30582 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/types/hub.py
+-rw-rw-r--   0 root         (0)     1003    17025 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/types/policy_based_routing.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:09.192500 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/
+-rw-rw-r--   0 root         (0)     1003     1658 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2857 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       94 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:09.192500 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:09.192500 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/services/hub_service/
+-rw-rw-r--   0 root         (0)     1003      753 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/services/hub_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    60395 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/services/hub_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    72567 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/services/hub_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10570 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/services/hub_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:09.192500 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/services/hub_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1157 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/services/hub_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9867 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/services/hub_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22022 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/services/hub_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    22511 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/services/hub_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:09.192500 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/types/
+-rw-rw-r--   0 root         (0)     1003     1387 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2871 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/types/common.py
+-rw-rw-r--   0 root         (0)     1003    23044 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/types/hub.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:09.192500 google-cloud-network-connectivity-2.0.2/google_cloud_network_connectivity.egg-info/
+-rw-r--r--   0 root         (0)     1003     5087 2023-07-05 15:54:09.000000 google-cloud-network-connectivity-2.0.2/google_cloud_network_connectivity.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3072 2023-07-05 15:54:09.000000 google-cloud-network-connectivity-2.0.2/google_cloud_network_connectivity.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:09.000000 google-cloud-network-connectivity-2.0.2/google_cloud_network_connectivity.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:54:09.000000 google-cloud-network-connectivity-2.0.2/google_cloud_network_connectivity.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:09.000000 google-cloud-network-connectivity-2.0.2/google_cloud_network_connectivity.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:54:09.000000 google-cloud-network-connectivity-2.0.2/google_cloud_network_connectivity.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:54:09.000000 google-cloud-network-connectivity-2.0.2/google_cloud_network_connectivity.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:54:09.196500 google-cloud-network-connectivity-2.0.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3017 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:09.192500 google-cloud-network-connectivity-2.0.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:09.196500 google-cloud-network-connectivity-2.0.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:09.196500 google-cloud-network-connectivity-2.0.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:09.196500 google-cloud-network-connectivity-2.0.2/tests/unit/gapic/networkconnectivity_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/tests/unit/gapic/networkconnectivity_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   199859 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/tests/unit/gapic/networkconnectivity_v1/test_hub_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:09.196500 google-cloud-network-connectivity-2.0.2/tests/unit/gapic/networkconnectivity_v1alpha1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/tests/unit/gapic/networkconnectivity_v1alpha1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   149877 2023-07-05 15:46:59.000000 google-cloud-network-connectivity-2.0.2/tests/unit/gapic/networkconnectivity_v1alpha1/test_hub_service.py
```

### Comparing `google-cloud-network-connectivity-2.0.1/LICENSE` & `google-cloud-network-connectivity-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/MANIFEST.in` & `google-cloud-network-connectivity-2.0.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/PKG-INFO` & `google-cloud-network-connectivity-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-network-connectivity
-Version: 2.0.1
+Version: 2.0.2
 Summary: Google Cloud Network Connectivity API client library
-Home-page: https://github.com/googleapis/python-network-connectivity
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
 
-Python Client for Network Connectivity Center API
-=================================================
+Python Client for Network Connectivity Center
+=============================================
 
 |stable| |pypi| |versions|
 
-`Network Connectivity Center API`_: The Network Connectivity API will be home to various services which provide information pertaining to network connectivity.  This includes information like interconnects, VPNs, VPCs, routing information, ip address details, etc. This information will help customers verify their network configurations and helps them to discover misconfigurations, inconsistencies, etc.
+`Network Connectivity Center`_: The Network Connectivity API will be home to various services which provide information pertaining to network connectivity.  This includes information like interconnects, VPNs, VPCs, routing information, ip address details, etc. This information will help customers verify their network configurations and helps them to discover misconfigurations, inconsistencies, etc.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-network-connectivity.svg
    :target: https://pypi.org/project/google-cloud-network-connectivity/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-network-connectivity.svg
    :target: https://pypi.org/project/google-cloud-network-connectivity/
-.. _Network Connectivity Center API: https://cloud.google.com/network-connectivity/
+.. _Network Connectivity Center: https://cloud.google.com/network-connectivity/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/networkconnectivity/latest
 .. _Product Documentation:  https://cloud.google.com/network-connectivity/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Network Connectivity Center API.`_
+3. `Enable the Network Connectivity Center.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Network Connectivity Center API.:  https://cloud.google.com/network-connectivity/
+.. _Enable the Network Connectivity Center.:  https://cloud.google.com/network-connectivity/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-network-connectivity
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Network Connectivity Center API
+-  Read the `Client Library Documentation`_ for Network Connectivity Center
    to see other available methods on the client.
--  Read the `Network Connectivity Center API Product documentation`_ to learn
+-  Read the `Network Connectivity Center Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Network Connectivity Center API Product documentation:  https://cloud.google.com/network-connectivity/
+.. _Network Connectivity Center Product documentation:  https://cloud.google.com/network-connectivity/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-network-connectivity-2.0.1/README.rst` & `google-cloud-network-connectivity-2.0.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Network Connectivity Center API
-=================================================
+Python Client for Network Connectivity Center
+=============================================
 
 |stable| |pypi| |versions|
 
-`Network Connectivity Center API`_: The Network Connectivity API will be home to various services which provide information pertaining to network connectivity.  This includes information like interconnects, VPNs, VPCs, routing information, ip address details, etc. This information will help customers verify their network configurations and helps them to discover misconfigurations, inconsistencies, etc.
+`Network Connectivity Center`_: The Network Connectivity API will be home to various services which provide information pertaining to network connectivity.  This includes information like interconnects, VPNs, VPCs, routing information, ip address details, etc. This information will help customers verify their network configurations and helps them to discover misconfigurations, inconsistencies, etc.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-network-connectivity.svg
    :target: https://pypi.org/project/google-cloud-network-connectivity/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-network-connectivity.svg
    :target: https://pypi.org/project/google-cloud-network-connectivity/
-.. _Network Connectivity Center API: https://cloud.google.com/network-connectivity/
+.. _Network Connectivity Center: https://cloud.google.com/network-connectivity/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/networkconnectivity/latest
 .. _Product Documentation:  https://cloud.google.com/network-connectivity/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Network Connectivity Center API.`_
+3. `Enable the Network Connectivity Center.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Network Connectivity Center API.:  https://cloud.google.com/network-connectivity/
+.. _Enable the Network Connectivity Center.:  https://cloud.google.com/network-connectivity/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-network-connectivity
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Network Connectivity Center API
+-  Read the `Client Library Documentation`_ for Network Connectivity Center
    to see other available methods on the client.
--  Read the `Network Connectivity Center API Product documentation`_ to learn
+-  Read the `Network Connectivity Center Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Network Connectivity Center API Product documentation:  https://cloud.google.com/network-connectivity/
+.. _Network Connectivity Center Product documentation:  https://cloud.google.com/network-connectivity/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity/__init__.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity/gapic_version.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.0.1"  # {x-release-please-version}
+__version__ = "2.0.2"  # {x-release-please-version}
```

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/__init__.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/gapic_metadata.json` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/gapic_version.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.0.1"  # {x-release-please-version}
+__version__ = "2.0.2"  # {x-release-please-version}
```

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/services/__init__.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/services/hub_service/__init__.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/services/hub_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/services/hub_service/async_client.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/services/hub_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2124,15 +2124,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "HubServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/services/hub_service/client.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/services/hub_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/services/hub_service/pagers.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/services/hub_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/services/hub_service/transports/__init__.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/services/hub_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/services/hub_service/transports/base.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/services/hub_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/services/hub_service/transports/grpc.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/services/hub_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/services/hub_service/transports/grpc_asyncio.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/services/hub_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/types/__init__.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/types/common.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/types/hub.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/types/hub.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1/types/policy_based_routing.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1/types/policy_based_routing.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/__init__.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/gapic_metadata.json` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/gapic_version.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.0.1"  # {x-release-please-version}
+__version__ = "2.0.2"  # {x-release-please-version}
```

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/services/__init__.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/services/hub_service/__init__.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/services/hub_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/services/hub_service/async_client.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/services/hub_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1460,15 +1460,15 @@
             empty_pb2.Empty,
             metadata_type=common.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "HubServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/services/hub_service/client.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/services/hub_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/services/hub_service/pagers.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/services/hub_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/services/hub_service/transports/__init__.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/services/hub_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/services/hub_service/transports/base.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/services/hub_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/services/hub_service/transports/grpc.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/services/hub_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/services/hub_service/transports/grpc_asyncio.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/services/hub_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/types/__init__.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/types/common.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google/cloud/networkconnectivity_v1alpha1/types/hub.py` & `google-cloud-network-connectivity-2.0.2/google/cloud/networkconnectivity_v1alpha1/types/hub.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/google_cloud_network_connectivity.egg-info/PKG-INFO` & `google-cloud-network-connectivity-2.0.2/google_cloud_network_connectivity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-network-connectivity
-Version: 2.0.1
+Version: 2.0.2
 Summary: Google Cloud Network Connectivity API client library
-Home-page: https://github.com/googleapis/python-network-connectivity
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
 
-Python Client for Network Connectivity Center API
-=================================================
+Python Client for Network Connectivity Center
+=============================================
 
 |stable| |pypi| |versions|
 
-`Network Connectivity Center API`_: The Network Connectivity API will be home to various services which provide information pertaining to network connectivity.  This includes information like interconnects, VPNs, VPCs, routing information, ip address details, etc. This information will help customers verify their network configurations and helps them to discover misconfigurations, inconsistencies, etc.
+`Network Connectivity Center`_: The Network Connectivity API will be home to various services which provide information pertaining to network connectivity.  This includes information like interconnects, VPNs, VPCs, routing information, ip address details, etc. This information will help customers verify their network configurations and helps them to discover misconfigurations, inconsistencies, etc.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-network-connectivity.svg
    :target: https://pypi.org/project/google-cloud-network-connectivity/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-network-connectivity.svg
    :target: https://pypi.org/project/google-cloud-network-connectivity/
-.. _Network Connectivity Center API: https://cloud.google.com/network-connectivity/
+.. _Network Connectivity Center: https://cloud.google.com/network-connectivity/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/networkconnectivity/latest
 .. _Product Documentation:  https://cloud.google.com/network-connectivity/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Network Connectivity Center API.`_
+3. `Enable the Network Connectivity Center.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Network Connectivity Center API.:  https://cloud.google.com/network-connectivity/
+.. _Enable the Network Connectivity Center.:  https://cloud.google.com/network-connectivity/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-network-connectivity
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Network Connectivity Center API
+-  Read the `Client Library Documentation`_ for Network Connectivity Center
    to see other available methods on the client.
--  Read the `Network Connectivity Center API Product documentation`_ to learn
+-  Read the `Network Connectivity Center Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Network Connectivity Center API Product documentation:  https://cloud.google.com/network-connectivity/
+.. _Network Connectivity Center Product documentation:  https://cloud.google.com/network-connectivity/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-network-connectivity-2.0.1/google_cloud_network_connectivity.egg-info/SOURCES.txt` & `google-cloud-network-connectivity-2.0.2/google_cloud_network_connectivity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/setup.py` & `google-cloud-network-connectivity-2.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
-url = "https://github.com/googleapis/python-network-connectivity"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-network-connectivity-2.0.1/tests/__init__.py` & `google-cloud-network-connectivity-2.0.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/tests/unit/__init__.py` & `google-cloud-network-connectivity-2.0.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/tests/unit/gapic/__init__.py` & `google-cloud-network-connectivity-2.0.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/tests/unit/gapic/networkconnectivity_v1/__init__.py` & `google-cloud-network-connectivity-2.0.2/tests/unit/gapic/networkconnectivity_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/tests/unit/gapic/networkconnectivity_v1/test_hub_service.py` & `google-cloud-network-connectivity-2.0.2/tests/unit/gapic/networkconnectivity_v1/test_hub_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1088,17 +1088,19 @@
                     hub.Hub(),
                     hub.Hub(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_hubs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2460,17 +2462,19 @@
                     hub.Spoke(),
                     hub.Spoke(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_spokes(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-network-connectivity-2.0.1/tests/unit/gapic/networkconnectivity_v1alpha1/__init__.py` & `google-cloud-network-connectivity-2.0.2/tests/unit/gapic/networkconnectivity_v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-connectivity-2.0.1/tests/unit/gapic/networkconnectivity_v1alpha1/test_hub_service.py` & `google-cloud-network-connectivity-2.0.2/tests/unit/gapic/networkconnectivity_v1alpha1/test_hub_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1084,17 +1084,19 @@
                     hub.Hub(),
                     hub.Hub(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_hubs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2460,17 +2462,19 @@
                     hub.Spoke(),
                     hub.Spoke(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_spokes(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

