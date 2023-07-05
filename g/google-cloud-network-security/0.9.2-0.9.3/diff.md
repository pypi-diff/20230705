# Comparing `tmp/google-cloud-network-security-0.9.2.tar.gz` & `tmp/google-cloud-network-security-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-network-security-0.9.2.tar", last modified: Mon Mar 27 16:17:04 2023, max compression
+gzip compressed data, was "google-cloud-network-security-0.9.3.tar", last modified: Wed Jul  5 15:54:18 2023, max compression
```

## Comparing `google-cloud-network-security-0.9.2.tar` & `google-cloud-network-security-0.9.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:17:04.195591 google-cloud-network-security-0.9.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4743 2023-03-27 16:17:04.195591 google-cloud-network-security-0.9.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3813 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:17:04.175597 google-cloud-network-security-0.9.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:17:04.175597 google-cloud-network-security-0.9.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:17:04.179596 google-cloud-network-security-0.9.2/google/cloud/network_security/
--rw-rw-r--   0 root         (0)     1003     3041 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:17:04.179596 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/
--rw-rw-r--   0 root         (0)     1003     2744 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     7028 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:17:04.179596 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:17:04.179596 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/network_security/
--rw-rw-r--   0 root         (0)     1003      773 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/network_security/__init__.py
--rw-rw-r--   0 root         (0)     1003   117195 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/network_security/async_client.py
--rw-rw-r--   0 root         (0)     1003   130023 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/network_security/client.py
--rw-rw-r--   0 root         (0)     1003    17268 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/network_security/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:17:04.183595 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/network_security/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/network_security/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    16237 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/network_security/transports/base.py
--rw-rw-r--   0 root         (0)     1003    39723 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/network_security/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    40354 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/network_security/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   125857 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/network_security/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:17:04.183595 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/types/
--rw-rw-r--   0 root         (0)     1003     2439 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    16261 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/types/authorization_policy.py
--rw-rw-r--   0 root         (0)     1003     8833 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/types/client_tls_policy.py
--rw-rw-r--   0 root         (0)     1003     2861 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003      774 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/types/network_security.py
--rw-rw-r--   0 root         (0)     1003    10017 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/types/server_tls_policy.py
--rw-rw-r--   0 root         (0)     1003     5132 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1/types/tls.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:17:04.183595 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/
--rw-rw-r--   0 root         (0)     1003     2749 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4809 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:17:04.183595 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:17:04.187594 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/network_security/
--rw-rw-r--   0 root         (0)     1003      773 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/network_security/__init__.py
--rw-rw-r--   0 root         (0)     1003   117665 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/network_security/async_client.py
--rw-rw-r--   0 root         (0)     1003   130372 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/network_security/client.py
--rw-rw-r--   0 root         (0)     1003    17393 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/network_security/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:17:04.187594 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/network_security/transports/
--rw-rw-r--   0 root         (0)     1003     1202 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/network_security/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    16272 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/network_security/transports/base.py
--rw-rw-r--   0 root         (0)     1003    39828 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/network_security/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    40459 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/network_security/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   125822 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/network_security/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:17:04.191592 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     2439 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    16306 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/types/authorization_policy.py
--rw-rw-r--   0 root         (0)     1003     8868 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/types/client_tls_policy.py
--rw-rw-r--   0 root         (0)     1003     2866 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/types/common.py
--rw-rw-r--   0 root         (0)     1003      779 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/types/network_security.py
--rw-rw-r--   0 root         (0)     1003    10057 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/types/server_tls_policy.py
--rw-rw-r--   0 root         (0)     1003     5157 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/types/tls.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:17:04.191592 google-cloud-network-security-0.9.2/google_cloud_network_security.egg-info/
--rw-r--r--   0 root         (0)     1003     4743 2023-03-27 16:17:04.000000 google-cloud-network-security-0.9.2/google_cloud_network_security.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3598 2023-03-27 16:17:04.000000 google-cloud-network-security-0.9.2/google_cloud_network_security.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:17:04.000000 google-cloud-network-security-0.9.2/google_cloud_network_security.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 16:17:04.000000 google-cloud-network-security-0.9.2/google_cloud_network_security.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:17:04.000000 google-cloud-network-security-0.9.2/google_cloud_network_security.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 16:17:04.000000 google-cloud-network-security-0.9.2/google_cloud_network_security.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 16:17:04.000000 google-cloud-network-security-0.9.2/google_cloud_network_security.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 16:17:04.195591 google-cloud-network-security-0.9.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3062 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:17:04.191592 google-cloud-network-security-0.9.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:17:04.191592 google-cloud-network-security-0.9.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:17:04.191592 google-cloud-network-security-0.9.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:17:04.191592 google-cloud-network-security-0.9.2/tests/unit/gapic/network_security_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/tests/unit/gapic/network_security_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   462713 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/tests/unit/gapic/network_security_v1/test_network_security.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:17:04.191592 google-cloud-network-security-0.9.2/tests/unit/gapic/network_security_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/tests/unit/gapic/network_security_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   266806 2023-03-27 16:14:43.000000 google-cloud-network-security-0.9.2/tests/unit/gapic/network_security_v1beta1/test_network_security.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:18.108316 google-cloud-network-security-0.9.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4703 2023-07-05 15:54:18.108316 google-cloud-network-security-0.9.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3777 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:18.092316 google-cloud-network-security-0.9.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:18.096316 google-cloud-network-security-0.9.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:18.096316 google-cloud-network-security-0.9.3/google/cloud/network_security/
+-rw-rw-r--   0 root         (0)     1003     3041 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:18.096316 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/
+-rw-rw-r--   0 root         (0)     1003     2744 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7028 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:18.096316 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:18.100316 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/network_security/
+-rw-rw-r--   0 root         (0)     1003      773 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/network_security/__init__.py
+-rw-rw-r--   0 root         (0)     1003   117227 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/network_security/async_client.py
+-rw-rw-r--   0 root         (0)     1003   130023 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/network_security/client.py
+-rw-rw-r--   0 root         (0)     1003    17268 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/network_security/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:18.100316 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/network_security/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/network_security/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16237 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/network_security/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    39723 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/network_security/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    40354 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/network_security/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   125821 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/network_security/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:18.100316 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2439 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16261 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/types/authorization_policy.py
+-rw-rw-r--   0 root         (0)     1003     8833 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/types/client_tls_policy.py
+-rw-rw-r--   0 root         (0)     1003     2861 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003      774 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/types/network_security.py
+-rw-rw-r--   0 root         (0)     1003    10017 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/types/server_tls_policy.py
+-rw-rw-r--   0 root         (0)     1003     5132 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1/types/tls.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:18.100316 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     2749 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4809 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:18.100316 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:18.104316 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/network_security/
+-rw-rw-r--   0 root         (0)     1003      773 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/network_security/__init__.py
+-rw-rw-r--   0 root         (0)     1003   117697 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/network_security/async_client.py
+-rw-rw-r--   0 root         (0)     1003   130372 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/network_security/client.py
+-rw-rw-r--   0 root         (0)     1003    17393 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/network_security/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:18.104316 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/network_security/transports/
+-rw-rw-r--   0 root         (0)     1003     1202 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/network_security/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16272 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/network_security/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    39828 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/network_security/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    40459 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/network_security/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   125822 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/network_security/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:18.104316 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     2439 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16306 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/types/authorization_policy.py
+-rw-rw-r--   0 root         (0)     1003     8868 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/types/client_tls_policy.py
+-rw-rw-r--   0 root         (0)     1003     2866 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/types/common.py
+-rw-rw-r--   0 root         (0)     1003      779 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/types/network_security.py
+-rw-rw-r--   0 root         (0)     1003    10057 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/types/server_tls_policy.py
+-rw-rw-r--   0 root         (0)     1003     5157 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/types/tls.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:18.104316 google-cloud-network-security-0.9.3/google_cloud_network_security.egg-info/
+-rw-r--r--   0 root         (0)     1003     4703 2023-07-05 15:54:18.000000 google-cloud-network-security-0.9.3/google_cloud_network_security.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3598 2023-07-05 15:54:18.000000 google-cloud-network-security-0.9.3/google_cloud_network_security.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:18.000000 google-cloud-network-security-0.9.3/google_cloud_network_security.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:54:18.000000 google-cloud-network-security-0.9.3/google_cloud_network_security.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:18.000000 google-cloud-network-security-0.9.3/google_cloud_network_security.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:54:18.000000 google-cloud-network-security-0.9.3/google_cloud_network_security.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:54:18.000000 google-cloud-network-security-0.9.3/google_cloud_network_security.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:54:18.108316 google-cloud-network-security-0.9.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3006 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:18.104316 google-cloud-network-security-0.9.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:18.104316 google-cloud-network-security-0.9.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:18.108316 google-cloud-network-security-0.9.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:18.108316 google-cloud-network-security-0.9.3/tests/unit/gapic/network_security_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/tests/unit/gapic/network_security_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   463310 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/tests/unit/gapic/network_security_v1/test_network_security.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:18.108316 google-cloud-network-security-0.9.3/tests/unit/gapic/network_security_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/tests/unit/gapic/network_security_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   267403 2023-07-05 15:46:59.000000 google-cloud-network-security-0.9.3/tests/unit/gapic/network_security_v1beta1/test_network_security.py
```

### Comparing `google-cloud-network-security-0.9.2/LICENSE` & `google-cloud-network-security-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/MANIFEST.in` & `google-cloud-network-security-0.9.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/PKG-INFO` & `google-cloud-network-security-0.9.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-network-security
-Version: 0.9.2
+Version: 0.9.3
 Summary: Google Cloud Network Security API client library
-Home-page: https://github.com/googleapis/python-network-security
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
 
-Python Client for Network Security API
-======================================
+Python Client for Network Security
+==================================
 
 |preview| |pypi| |versions|
 
-`Network Security API`_: 
+`Network Security`_: 
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-network-security.svg
    :target: https://pypi.org/project/google-cloud-network-security/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-network-security.svg
    :target: https://pypi.org/project/google-cloud-network-security/
-.. _Network Security API: https://cloud.google.com/traffic-director/docs/reference/network-security/rest
+.. _Network Security: https://cloud.google.com/traffic-director/docs/reference/network-security/rest
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/networksecurity/latest
 .. _Product Documentation:  https://cloud.google.com/traffic-director/docs/reference/network-security/rest
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Network Security API.`_
+3. `Enable the Network Security.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Network Security API.:  https://cloud.google.com/traffic-director/docs/reference/network-security/rest
+.. _Enable the Network Security.:  https://cloud.google.com/traffic-director/docs/reference/network-security/rest
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-network-security
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Network Security API
+-  Read the `Client Library Documentation`_ for Network Security
    to see other available methods on the client.
--  Read the `Network Security API Product documentation`_ to learn
+-  Read the `Network Security Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Network Security API Product documentation:  https://cloud.google.com/traffic-director/docs/reference/network-security/rest
+.. _Network Security Product documentation:  https://cloud.google.com/traffic-director/docs/reference/network-security/rest
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-network-security-0.9.2/README.rst` & `google-cloud-network-security-0.9.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Network Security API
-======================================
+Python Client for Network Security
+==================================
 
 |preview| |pypi| |versions|
 
-`Network Security API`_: 
+`Network Security`_: 
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-network-security.svg
    :target: https://pypi.org/project/google-cloud-network-security/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-network-security.svg
    :target: https://pypi.org/project/google-cloud-network-security/
-.. _Network Security API: https://cloud.google.com/traffic-director/docs/reference/network-security/rest
+.. _Network Security: https://cloud.google.com/traffic-director/docs/reference/network-security/rest
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/networksecurity/latest
 .. _Product Documentation:  https://cloud.google.com/traffic-director/docs/reference/network-security/rest
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Network Security API.`_
+3. `Enable the Network Security.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Network Security API.:  https://cloud.google.com/traffic-director/docs/reference/network-security/rest
+.. _Enable the Network Security.:  https://cloud.google.com/traffic-director/docs/reference/network-security/rest
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-network-security
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Network Security API
+-  Read the `Client Library Documentation`_ for Network Security
    to see other available methods on the client.
--  Read the `Network Security API Product documentation`_ to learn
+-  Read the `Network Security Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Network Security API Product documentation:  https://cloud.google.com/traffic-director/docs/reference/network-security/rest
+.. _Network Security Product documentation:  https://cloud.google.com/traffic-director/docs/reference/network-security/rest
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security/__init__.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security/gapic_version.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security/gapic_version.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.9.2"  # {x-release-please-version}
+__version__ = "0.9.3"  # {x-release-please-version}
```

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1/__init__.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1/gapic_metadata.json` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1/gapic_version.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1/gapic_version.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.9.2"  # {x-release-please-version}
+__version__ = "0.9.3"  # {x-release-please-version}
```

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/__init__.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/network_security/__init__.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/network_security/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/network_security/async_client.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/network_security/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2823,15 +2823,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "NetworkSecurityAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/network_security/client.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/network_security/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/network_security/pagers.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/network_security/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/network_security/transports/__init__.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/network_security/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/network_security/transports/base.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/network_security/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/network_security/transports/grpc.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/network_security/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/network_security/transports/grpc_asyncio.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/network_security/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1/services/network_security/transports/rest.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1/services/network_security/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -2792,15 +2792,15 @@
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
@@ -2874,15 +2874,15 @@
 
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
@@ -2943,15 +2943,15 @@
 
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

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1/types/__init__.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1/types/authorization_policy.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1/types/authorization_policy.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1/types/client_tls_policy.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1/types/client_tls_policy.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1/types/common.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1/types/network_security.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1/types/network_security.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1/types/server_tls_policy.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1/types/server_tls_policy.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1/types/tls.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1/types/tls.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/__init__.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/gapic_metadata.json` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/gapic_version.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/gapic_version.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.9.2"  # {x-release-please-version}
+__version__ = "0.9.3"  # {x-release-please-version}
```

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/__init__.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/network_security/__init__.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/network_security/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/network_security/async_client.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/network_security/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2823,15 +2823,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "NetworkSecurityAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/network_security/client.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/network_security/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/network_security/pagers.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/network_security/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/network_security/transports/__init__.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/network_security/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/network_security/transports/base.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/network_security/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/network_security/transports/grpc.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/network_security/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/network_security/transports/grpc_asyncio.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/network_security/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/services/network_security/transports/rest.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/services/network_security/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/types/__init__.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/types/authorization_policy.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/types/authorization_policy.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/types/client_tls_policy.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/types/client_tls_policy.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/types/common.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/types/network_security.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/types/network_security.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/types/server_tls_policy.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/types/server_tls_policy.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google/cloud/network_security_v1beta1/types/tls.py` & `google-cloud-network-security-0.9.3/google/cloud/network_security_v1beta1/types/tls.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/google_cloud_network_security.egg-info/PKG-INFO` & `google-cloud-network-security-0.9.3/google_cloud_network_security.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-network-security
-Version: 0.9.2
+Version: 0.9.3
 Summary: Google Cloud Network Security API client library
-Home-page: https://github.com/googleapis/python-network-security
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
 
-Python Client for Network Security API
-======================================
+Python Client for Network Security
+==================================
 
 |preview| |pypi| |versions|
 
-`Network Security API`_: 
+`Network Security`_: 
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-network-security.svg
    :target: https://pypi.org/project/google-cloud-network-security/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-network-security.svg
    :target: https://pypi.org/project/google-cloud-network-security/
-.. _Network Security API: https://cloud.google.com/traffic-director/docs/reference/network-security/rest
+.. _Network Security: https://cloud.google.com/traffic-director/docs/reference/network-security/rest
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/networksecurity/latest
 .. _Product Documentation:  https://cloud.google.com/traffic-director/docs/reference/network-security/rest
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Network Security API.`_
+3. `Enable the Network Security.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Network Security API.:  https://cloud.google.com/traffic-director/docs/reference/network-security/rest
+.. _Enable the Network Security.:  https://cloud.google.com/traffic-director/docs/reference/network-security/rest
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-network-security
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Network Security API
+-  Read the `Client Library Documentation`_ for Network Security
    to see other available methods on the client.
--  Read the `Network Security API Product documentation`_ to learn
+-  Read the `Network Security Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Network Security API Product documentation:  https://cloud.google.com/traffic-director/docs/reference/network-security/rest
+.. _Network Security Product documentation:  https://cloud.google.com/traffic-director/docs/reference/network-security/rest
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-network-security-0.9.2/google_cloud_network_security.egg-info/SOURCES.txt` & `google-cloud-network-security-0.9.3/google_cloud_network_security.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/setup.py` & `google-cloud-network-security-0.9.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,33 +38,31 @@
     release_status = "Development Status :: 5 - Production/Stable"
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
-    "grpc-google-iam-v1 >=0.12.4, <1.0.0dev",
+    "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
-url = "https://github.com/googleapis/python-network-security"
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

### Comparing `google-cloud-network-security-0.9.2/tests/__init__.py` & `google-cloud-network-security-0.9.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/tests/unit/__init__.py` & `google-cloud-network-security-0.9.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/tests/unit/gapic/__init__.py` & `google-cloud-network-security-0.9.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/tests/unit/gapic/network_security_v1/__init__.py` & `google-cloud-network-security-0.9.3/tests/unit/gapic/network_security_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/tests/unit/gapic/network_security_v1/test_network_security.py` & `google-cloud-network-security-0.9.3/tests/unit/gapic/network_security_v1/test_network_security.py`

 * *Files 0% similar despite different names*

```diff
@@ -1191,17 +1191,19 @@
                     authorization_policy.AuthorizationPolicy(),
                     authorization_policy.AuthorizationPolicy(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_authorization_policies(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2658,17 +2660,19 @@
                     server_tls_policy.ServerTlsPolicy(),
                     server_tls_policy.ServerTlsPolicy(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_server_tls_policies(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4109,17 +4113,19 @@
                     client_tls_policy.ClientTlsPolicy(),
                     client_tls_policy.ClientTlsPolicy(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_client_tls_policies(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-network-security-0.9.2/tests/unit/gapic/network_security_v1beta1/__init__.py` & `google-cloud-network-security-0.9.3/tests/unit/gapic/network_security_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-security-0.9.2/tests/unit/gapic/network_security_v1beta1/test_network_security.py` & `google-cloud-network-security-0.9.3/tests/unit/gapic/network_security_v1beta1/test_network_security.py`

 * *Files 0% similar despite different names*

```diff
@@ -1159,17 +1159,19 @@
                     authorization_policy.AuthorizationPolicy(),
                     authorization_policy.AuthorizationPolicy(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_authorization_policies(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2626,17 +2628,19 @@
                     server_tls_policy.ServerTlsPolicy(),
                     server_tls_policy.ServerTlsPolicy(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_server_tls_policies(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4077,17 +4081,19 @@
                     client_tls_policy.ClientTlsPolicy(),
                     client_tls_policy.ClientTlsPolicy(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_client_tls_policies(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

