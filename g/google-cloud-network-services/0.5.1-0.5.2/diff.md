# Comparing `tmp/google-cloud-network-services-0.5.1.tar.gz` & `tmp/google-cloud-network-services-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-network-services-0.5.1.tar", last modified: Mon Mar 27 14:53:43 2023, max compression
+gzip compressed data, was "google-cloud-network-services-0.5.2.tar", last modified: Wed Jul  5 15:20:30 2023, max compression
```

## Comparing `google-cloud-network-services-0.5.1.tar` & `google-cloud-network-services-0.5.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:53:42.994025 google-cloud-network-services-0.5.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4527 2023-03-27 14:53:42.994025 google-cloud-network-services-0.5.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3597 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:53:42.982024 google-cloud-network-services-0.5.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:53:42.982024 google-cloud-network-services-0.5.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:53:42.982024 google-cloud-network-services-0.5.1/google/cloud/network_services/
--rw-rw-r--   0 root         (0)     1003     4690 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:53:42.982024 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/
--rw-rw-r--   0 root         (0)     1003     4248 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    15326 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:53:42.982024 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:53:42.986024 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/network_services/
--rw-rw-r--   0 root         (0)     1003      773 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/network_services/__init__.py
--rw-rw-r--   0 root         (0)     1003   235603 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/network_services/async_client.py
--rw-rw-r--   0 root         (0)     1003   256276 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/network_services/client.py
--rw-rw-r--   0 root         (0)     1003    41523 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/network_services/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:53:42.986024 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/network_services/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/network_services/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    26595 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/network_services/transports/base.py
--rw-rw-r--   0 root         (0)     1003    65448 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/network_services/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    66851 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/network_services/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   247097 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/network_services/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:53:42.990024 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/
--rw-rw-r--   0 root         (0)     1003     3919 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     8227 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003    10783 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/endpoint_policy.py
--rw-rw-r--   0 root         (0)     1003     9330 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/gateway.py
--rw-rw-r--   0 root         (0)     1003    26034 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/grpc_route.py
--rw-rw-r--   0 root         (0)     1003    41493 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/http_route.py
--rw-rw-r--   0 root         (0)     1003     7522 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/mesh.py
--rw-rw-r--   0 root         (0)     1003      774 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/network_services.py
--rw-rw-r--   0 root         (0)     1003     6349 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/service_binding.py
--rw-rw-r--   0 root         (0)     1003    13242 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/tcp_route.py
--rw-rw-r--   0 root         (0)     1003    12022 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/tls_route.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:53:42.990024 google-cloud-network-services-0.5.1/google_cloud_network_services.egg-info/
--rw-r--r--   0 root         (0)     1003     4527 2023-03-27 14:53:42.000000 google-cloud-network-services-0.5.1/google_cloud_network_services.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2248 2023-03-27 14:53:42.000000 google-cloud-network-services-0.5.1/google_cloud_network_services.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:53:42.000000 google-cloud-network-services-0.5.1/google_cloud_network_services.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:53:42.000000 google-cloud-network-services-0.5.1/google_cloud_network_services.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:53:42.000000 google-cloud-network-services-0.5.1/google_cloud_network_services.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 14:53:42.000000 google-cloud-network-services-0.5.1/google_cloud_network_services.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:53:42.000000 google-cloud-network-services-0.5.1/google_cloud_network_services.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 14:53:42.994025 google-cloud-network-services-0.5.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3010 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:53:42.990024 google-cloud-network-services-0.5.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:53:42.994025 google-cloud-network-services-0.5.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:53:42.994025 google-cloud-network-services-0.5.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:53:42.994025 google-cloud-network-services-0.5.1/tests/unit/gapic/network_services_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/tests/unit/gapic/network_services_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   977345 2023-03-27 14:51:34.000000 google-cloud-network-services-0.5.1/tests/unit/gapic/network_services_v1/test_network_services.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:20:30.154844 google-cloud-network-services-0.5.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4527 2023-07-05 15:20:30.154844 google-cloud-network-services-0.5.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3597 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:20:30.142840 google-cloud-network-services-0.5.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:20:30.142840 google-cloud-network-services-0.5.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:20:30.146841 google-cloud-network-services-0.5.2/google/cloud/network_services/
+-rw-rw-r--   0 root         (0)     1003     4690 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:20:30.146841 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/
+-rw-rw-r--   0 root         (0)     1003     4248 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15326 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:20:30.146841 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:20:30.146841 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/network_services/
+-rw-rw-r--   0 root         (0)     1003      773 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/network_services/__init__.py
+-rw-rw-r--   0 root         (0)     1003   235635 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/network_services/async_client.py
+-rw-rw-r--   0 root         (0)     1003   256276 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/network_services/client.py
+-rw-rw-r--   0 root         (0)     1003    41523 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/network_services/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:20:30.146841 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/network_services/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/network_services/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26595 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/network_services/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    65448 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/network_services/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    66851 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/network_services/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   247061 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/network_services/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:20:30.150843 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3919 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8227 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003    10783 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/endpoint_policy.py
+-rw-rw-r--   0 root         (0)     1003     9330 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/gateway.py
+-rw-rw-r--   0 root         (0)     1003    26034 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/grpc_route.py
+-rw-rw-r--   0 root         (0)     1003    41493 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/http_route.py
+-rw-rw-r--   0 root         (0)     1003     7522 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/mesh.py
+-rw-rw-r--   0 root         (0)     1003      774 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/network_services.py
+-rw-rw-r--   0 root         (0)     1003     6349 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/service_binding.py
+-rw-rw-r--   0 root         (0)     1003    13242 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/tcp_route.py
+-rw-rw-r--   0 root         (0)     1003    12022 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/tls_route.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:20:30.150843 google-cloud-network-services-0.5.2/google_cloud_network_services.egg-info/
+-rw-r--r--   0 root         (0)     1003     4527 2023-07-05 15:20:30.000000 google-cloud-network-services-0.5.2/google_cloud_network_services.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2248 2023-07-05 15:20:30.000000 google-cloud-network-services-0.5.2/google_cloud_network_services.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:20:30.000000 google-cloud-network-services-0.5.2/google_cloud_network_services.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:20:30.000000 google-cloud-network-services-0.5.2/google_cloud_network_services.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:20:30.000000 google-cloud-network-services-0.5.2/google_cloud_network_services.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:20:30.000000 google-cloud-network-services-0.5.2/google_cloud_network_services.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:20:30.000000 google-cloud-network-services-0.5.2/google_cloud_network_services.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:20:30.154844 google-cloud-network-services-0.5.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3010 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:20:30.150843 google-cloud-network-services-0.5.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:20:30.150843 google-cloud-network-services-0.5.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:20:30.150843 google-cloud-network-services-0.5.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:20:30.154844 google-cloud-network-services-0.5.2/tests/unit/gapic/network_services_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/tests/unit/gapic/network_services_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   978937 2023-07-05 15:18:32.000000 google-cloud-network-services-0.5.2/tests/unit/gapic/network_services_v1/test_network_services.py
```

### Comparing `google-cloud-network-services-0.5.1/LICENSE` & `google-cloud-network-services-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/MANIFEST.in` & `google-cloud-network-services-0.5.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/PKG-INFO` & `google-cloud-network-services-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-network-services
-Version: 0.5.1
+Version: 0.5.2
 Summary: Google Cloud Network Services API client library
 Home-page: https://github.com/googleapis/python-network-services
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-network-services-0.5.1/README.rst` & `google-cloud-network-services-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services/__init__.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services/gapic_version.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services/gapic_version.py`

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
-__version__ = "0.5.1"  # {x-release-please-version}
+__version__ = "0.5.2"  # {x-release-please-version}
```

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/__init__.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/gapic_metadata.json` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/gapic_version.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/gapic_version.py`

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
-__version__ = "0.5.1"  # {x-release-please-version}
+__version__ = "0.5.2"  # {x-release-please-version}
```

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/__init__.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/network_services/__init__.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/network_services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/network_services/async_client.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/network_services/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -5774,15 +5774,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "NetworkServicesAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/network_services/client.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/network_services/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/network_services/pagers.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/network_services/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/network_services/transports/__init__.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/network_services/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/network_services/transports/base.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/network_services/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/network_services/transports/grpc.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/network_services/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/network_services/transports/grpc_asyncio.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/network_services/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/services/network_services/transports/rest.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/services/network_services/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -5919,15 +5919,15 @@
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
@@ -6021,15 +6021,15 @@
 
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
@@ -6090,15 +6090,15 @@
 
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

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/__init__.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/common.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/endpoint_policy.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/endpoint_policy.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/gateway.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/gateway.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/grpc_route.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/grpc_route.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/http_route.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/http_route.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/mesh.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/mesh.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/network_services.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/network_services.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/service_binding.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/service_binding.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/tcp_route.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/tcp_route.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google/cloud/network_services_v1/types/tls_route.py` & `google-cloud-network-services-0.5.2/google/cloud/network_services_v1/types/tls_route.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/google_cloud_network_services.egg-info/PKG-INFO` & `google-cloud-network-services-0.5.2/google_cloud_network_services.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-network-services
-Version: 0.5.1
+Version: 0.5.2
 Summary: Google Cloud Network Services API client library
 Home-page: https://github.com/googleapis/python-network-services
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-network-services-0.5.1/google_cloud_network_services.egg-info/SOURCES.txt` & `google-cloud-network-services-0.5.2/google_cloud_network_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/setup.py` & `google-cloud-network-services-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/tests/__init__.py` & `google-cloud-network-services-0.5.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/tests/unit/__init__.py` & `google-cloud-network-services-0.5.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/tests/unit/gapic/__init__.py` & `google-cloud-network-services-0.5.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/tests/unit/gapic/network_services_v1/__init__.py` & `google-cloud-network-services-0.5.2/tests/unit/gapic/network_services_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-services-0.5.1/tests/unit/gapic/network_services_v1/test_network_services.py` & `google-cloud-network-services-0.5.2/tests/unit/gapic/network_services_v1/test_network_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -1195,17 +1195,19 @@
                     endpoint_policy.EndpointPolicy(),
                     endpoint_policy.EndpointPolicy(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_endpoint_policies(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2641,17 +2643,19 @@
                     gateway.Gateway(),
                     gateway.Gateway(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_gateways(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4021,17 +4025,19 @@
                     grpc_route.GrpcRoute(),
                     grpc_route.GrpcRoute(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_grpc_routes(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5443,17 +5449,19 @@
                     http_route.HttpRoute(),
                     http_route.HttpRoute(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_http_routes(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -6865,17 +6873,19 @@
                     tcp_route.TcpRoute(),
                     tcp_route.TcpRoute(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_tcp_routes(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -8237,17 +8247,19 @@
                     tls_route.TlsRoute(),
                     tls_route.TlsRoute(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_tls_routes(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -9632,17 +9644,19 @@
                     service_binding.ServiceBinding(),
                     service_binding.ServiceBinding(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_service_bindings(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -10809,17 +10823,19 @@
                     mesh.Mesh(),
                     mesh.Mesh(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_meshes(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

