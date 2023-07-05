# Comparing `tmp/google-cloud-private-ca-1.8.0.tar.gz` & `tmp/google-cloud-private-ca-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-private-ca-1.8.0.tar", last modified: Wed Apr  5 20:25:10 2023, max compression
+gzip compressed data, was "google-cloud-private-ca-1.8.1.tar", last modified: Wed Jul  5 15:54:40 2023, max compression
```

## Comparing `google-cloud-private-ca-1.8.0.tar` & `google-cloud-private-ca-1.8.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:25:10.604873 google-cloud-private-ca-1.8.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4809 2023-04-05 20:25:10.604873 google-cloud-private-ca-1.8.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3875 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:25:10.584874 google-cloud-private-ca-1.8.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:25:10.584874 google-cloud-private-ca-1.8.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:25:10.588874 google-cloud-private-ca-1.8.0/google/cloud/security/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:25:10.588874 google-cloud-private-ca-1.8.0/google/cloud/security/privateca/
--rw-rw-r--   0 root         (0)     1003     4727 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:25:10.588874 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/
--rw-rw-r--   0 root         (0)     1003     4518 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    12904 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:25:10.588874 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:25:10.592874 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/certificate_authority_service/
--rw-rw-r--   0 root         (0)     1003      821 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/certificate_authority_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   192772 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/certificate_authority_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   209001 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/certificate_authority_service/client.py
--rw-rw-r--   0 root         (0)     1003    27275 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/certificate_authority_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:25:10.592874 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/
--rw-rw-r--   0 root         (0)     1003     1603 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    22039 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    59192 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    60216 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   206208 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:25:10.596874 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/types/
--rw-rw-r--   0 root         (0)     1003     4155 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    95027 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/types/resources.py
--rw-rw-r--   0 root         (0)     1003    65412 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:25:10.596874 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/
--rw-rw-r--   0 root         (0)     1003     3695 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     9422 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:25:10.596874 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:25:10.596874 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/
--rw-rw-r--   0 root         (0)     1003      821 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   119803 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   134267 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/client.py
--rw-rw-r--   0 root         (0)     1003    22326 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:25:10.596874 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/
--rw-rw-r--   0 root         (0)     1003     1603 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    15738 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    39612 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    40390 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   124692 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:25:10.600873 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     3327 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    74757 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/types/resources.py
--rw-rw-r--   0 root         (0)     1003    43189 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:25:10.600873 google-cloud-private-ca-1.8.0/google_cloud_private_ca.egg-info/
--rw-r--r--   0 root         (0)     1003     4809 2023-04-05 20:25:10.000000 google-cloud-private-ca-1.8.0/google_cloud_private_ca.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3372 2023-04-05 20:25:10.000000 google-cloud-private-ca-1.8.0/google_cloud_private_ca.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-05 20:25:10.000000 google-cloud-private-ca-1.8.0/google_cloud_private_ca.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       42 2023-04-05 20:25:10.000000 google-cloud-private-ca-1.8.0/google_cloud_private_ca.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-05 20:25:10.000000 google-cloud-private-ca-1.8.0/google_cloud_private_ca.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-04-05 20:25:10.000000 google-cloud-private-ca-1.8.0/google_cloud_private_ca.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-05 20:25:10.000000 google-cloud-private-ca-1.8.0/google_cloud_private_ca.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-04-05 20:25:10.604873 google-cloud-private-ca-1.8.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3028 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:25:10.600873 google-cloud-private-ca-1.8.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:25:10.600873 google-cloud-private-ca-1.8.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:25:10.600873 google-cloud-private-ca-1.8.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:25:10.600873 google-cloud-private-ca-1.8.0/tests/unit/gapic/privateca_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/tests/unit/gapic/privateca_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   837318 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/tests/unit/gapic/privateca_v1/test_certificate_authority_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:25:10.604873 google-cloud-private-ca-1.8.0/tests/unit/gapic/privateca_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/tests/unit/gapic/privateca_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   545460 2023-04-05 20:23:00.000000 google-cloud-private-ca-1.8.0/tests/unit/gapic/privateca_v1beta1/test_certificate_authority_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:40.019811 google-cloud-private-ca-1.8.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4766 2023-07-05 15:54:40.019811 google-cloud-private-ca-1.8.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3839 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:40.003811 google-cloud-private-ca-1.8.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:40.003811 google-cloud-private-ca-1.8.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:40.003811 google-cloud-private-ca-1.8.1/google/cloud/security/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:40.003811 google-cloud-private-ca-1.8.1/google/cloud/security/privateca/
+-rw-rw-r--   0 root         (0)     1003     4727 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:40.007811 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/
+-rw-rw-r--   0 root         (0)     1003     4518 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12904 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:40.007811 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:40.007811 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/certificate_authority_service/
+-rw-rw-r--   0 root         (0)     1003      821 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/certificate_authority_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   192816 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/certificate_authority_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   209001 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/certificate_authority_service/client.py
+-rw-rw-r--   0 root         (0)     1003    27275 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/certificate_authority_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:40.007811 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1603 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22039 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    59192 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    60216 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   206172 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:40.011811 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/types/
+-rw-rw-r--   0 root         (0)     1003     4155 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    95027 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/types/resources.py
+-rw-rw-r--   0 root         (0)     1003    65412 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:40.011811 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     3695 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9422 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:40.011811 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:40.011811 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/
+-rw-rw-r--   0 root         (0)     1003      821 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   119847 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   134267 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/client.py
+-rw-rw-r--   0 root         (0)     1003    22326 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:40.011811 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1603 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15738 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    39612 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    40390 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   124692 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:40.015811 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     3327 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    74757 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/types/resources.py
+-rw-rw-r--   0 root         (0)     1003    43189 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:40.015811 google-cloud-private-ca-1.8.1/google_cloud_private_ca.egg-info/
+-rw-r--r--   0 root         (0)     1003     4766 2023-07-05 15:54:39.000000 google-cloud-private-ca-1.8.1/google_cloud_private_ca.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3372 2023-07-05 15:54:39.000000 google-cloud-private-ca-1.8.1/google_cloud_private_ca.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:39.000000 google-cloud-private-ca-1.8.1/google_cloud_private_ca.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       42 2023-07-05 15:54:39.000000 google-cloud-private-ca-1.8.1/google_cloud_private_ca.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:39.000000 google-cloud-private-ca-1.8.1/google_cloud_private_ca.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:54:39.000000 google-cloud-private-ca-1.8.1/google_cloud_private_ca.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:54:39.000000 google-cloud-private-ca-1.8.1/google_cloud_private_ca.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:54:40.019811 google-cloud-private-ca-1.8.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3021 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:40.015811 google-cloud-private-ca-1.8.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:40.015811 google-cloud-private-ca-1.8.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:40.015811 google-cloud-private-ca-1.8.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:40.015811 google-cloud-private-ca-1.8.1/tests/unit/gapic/privateca_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/tests/unit/gapic/privateca_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   838313 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/tests/unit/gapic/privateca_v1/test_certificate_authority_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:40.019811 google-cloud-private-ca-1.8.1/tests/unit/gapic/privateca_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/tests/unit/gapic/privateca_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   546256 2023-07-05 15:46:59.000000 google-cloud-private-ca-1.8.1/tests/unit/gapic/privateca_v1beta1/test_certificate_authority_service.py
```

### Comparing `google-cloud-private-ca-1.8.0/LICENSE` & `google-cloud-private-ca-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/MANIFEST.in` & `google-cloud-private-ca-1.8.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/PKG-INFO` & `google-cloud-private-ca-1.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-private-ca
-Version: 1.8.0
+Version: 1.8.1
 Summary: Google Cloud Private Ca API client library
-Home-page: https://github.com/googleapis/python-security-private-ca
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
 
-Python Client for Private Certificate Authority API
-===================================================
+Python Client for Private Certificate Authority
+===============================================
 
 |stable| |pypi| |versions|
 
-`Private Certificate Authority API`_: simplifies the deployment and management of private CAs without managing infrastructure.
+`Private Certificate Authority`_: simplifies the deployment and management of private CAs without managing infrastructure.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-private-ca.svg
    :target: https://pypi.org/project/google-cloud-private-ca/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-private-ca.svg
    :target: https://pypi.org/project/google-cloud-private-ca/
-.. _Private Certificate Authority API: https://cloud.google.com/certificate-authority-service
+.. _Private Certificate Authority: https://cloud.google.com/certificate-authority-service
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/privateca/latest
 .. _Product Documentation:  https://cloud.google.com/certificate-authority-service
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Private Certificate Authority API.`_
+3. `Enable the Private Certificate Authority.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Private Certificate Authority API.:  https://cloud.google.com/certificate-authority-service
+.. _Enable the Private Certificate Authority.:  https://cloud.google.com/certificate-authority-service
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-private-ca
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Private Certificate Authority API
+-  Read the `Client Library Documentation`_ for Private Certificate Authority
    to see other available methods on the client.
--  Read the `Private Certificate Authority API Product documentation`_ to learn
+-  Read the `Private Certificate Authority Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Private Certificate Authority API Product documentation:  https://cloud.google.com/certificate-authority-service
+.. _Private Certificate Authority Product documentation:  https://cloud.google.com/certificate-authority-service
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-private-ca-1.8.0/README.rst` & `google-cloud-private-ca-1.8.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Private Certificate Authority API
-===================================================
+Python Client for Private Certificate Authority
+===============================================
 
 |stable| |pypi| |versions|
 
-`Private Certificate Authority API`_: simplifies the deployment and management of private CAs without managing infrastructure.
+`Private Certificate Authority`_: simplifies the deployment and management of private CAs without managing infrastructure.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-private-ca.svg
    :target: https://pypi.org/project/google-cloud-private-ca/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-private-ca.svg
    :target: https://pypi.org/project/google-cloud-private-ca/
-.. _Private Certificate Authority API: https://cloud.google.com/certificate-authority-service
+.. _Private Certificate Authority: https://cloud.google.com/certificate-authority-service
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/privateca/latest
 .. _Product Documentation:  https://cloud.google.com/certificate-authority-service
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Private Certificate Authority API.`_
+3. `Enable the Private Certificate Authority.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Private Certificate Authority API.:  https://cloud.google.com/certificate-authority-service
+.. _Enable the Private Certificate Authority.:  https://cloud.google.com/certificate-authority-service
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-private-ca
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Private Certificate Authority API
+-  Read the `Client Library Documentation`_ for Private Certificate Authority
    to see other available methods on the client.
--  Read the `Private Certificate Authority API Product documentation`_ to learn
+-  Read the `Private Certificate Authority Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Private Certificate Authority API Product documentation:  https://cloud.google.com/certificate-authority-service
+.. _Private Certificate Authority Product documentation:  https://cloud.google.com/certificate-authority-service
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca/__init__.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca/gapic_version.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca/gapic_version.py`

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
-__version__ = "1.8.0"  # {x-release-please-version}
+__version__ = "1.8.1"  # {x-release-please-version}
```

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/__init__.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/gapic_metadata.json` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/gapic_version.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/gapic_version.py`

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
-__version__ = "1.8.0"  # {x-release-please-version}
+__version__ = "1.8.1"  # {x-release-please-version}
```

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/__init__.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/certificate_authority_service/__init__.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/certificate_authority_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/certificate_authority_service/async_client.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/certificate_authority_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4512,15 +4512,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "CertificateAuthorityServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/certificate_authority_service/client.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/certificate_authority_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/certificate_authority_service/pagers.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/certificate_authority_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/__init__.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/base.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/grpc.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/grpc_asyncio.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/rest.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/services/certificate_authority_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -4647,15 +4647,15 @@
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
@@ -4729,15 +4729,15 @@
 
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
@@ -4798,15 +4798,15 @@
 
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

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/types/__init__.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/types/resources.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/types/resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1/types/service.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/__init__.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/gapic_metadata.json` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/gapic_version.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/gapic_version.py`

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
-__version__ = "1.8.0"  # {x-release-please-version}
+__version__ = "1.8.1"  # {x-release-please-version}
```

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/__init__.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/__init__.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/async_client.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2712,15 +2712,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "CertificateAuthorityServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/client.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/pagers.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/__init__.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/base.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/grpc.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/grpc_asyncio.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/rest.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/services/certificate_authority_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/types/__init__.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/types/resources.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/types/resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google/cloud/security/privateca_v1beta1/types/service.py` & `google-cloud-private-ca-1.8.1/google/cloud/security/privateca_v1beta1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/google_cloud_private_ca.egg-info/PKG-INFO` & `google-cloud-private-ca-1.8.1/google_cloud_private_ca.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-private-ca
-Version: 1.8.0
+Version: 1.8.1
 Summary: Google Cloud Private Ca API client library
-Home-page: https://github.com/googleapis/python-security-private-ca
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
 
-Python Client for Private Certificate Authority API
-===================================================
+Python Client for Private Certificate Authority
+===============================================
 
 |stable| |pypi| |versions|
 
-`Private Certificate Authority API`_: simplifies the deployment and management of private CAs without managing infrastructure.
+`Private Certificate Authority`_: simplifies the deployment and management of private CAs without managing infrastructure.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-private-ca.svg
    :target: https://pypi.org/project/google-cloud-private-ca/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-private-ca.svg
    :target: https://pypi.org/project/google-cloud-private-ca/
-.. _Private Certificate Authority API: https://cloud.google.com/certificate-authority-service
+.. _Private Certificate Authority: https://cloud.google.com/certificate-authority-service
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/privateca/latest
 .. _Product Documentation:  https://cloud.google.com/certificate-authority-service
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Private Certificate Authority API.`_
+3. `Enable the Private Certificate Authority.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Private Certificate Authority API.:  https://cloud.google.com/certificate-authority-service
+.. _Enable the Private Certificate Authority.:  https://cloud.google.com/certificate-authority-service
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-private-ca
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Private Certificate Authority API
+-  Read the `Client Library Documentation`_ for Private Certificate Authority
    to see other available methods on the client.
--  Read the `Private Certificate Authority API Product documentation`_ to learn
+-  Read the `Private Certificate Authority Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Private Certificate Authority API Product documentation:  https://cloud.google.com/certificate-authority-service
+.. _Private Certificate Authority Product documentation:  https://cloud.google.com/certificate-authority-service
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-private-ca-1.8.0/google_cloud_private_ca.egg-info/SOURCES.txt` & `google-cloud-private-ca-1.8.1/google_cloud_private_ca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/setup.py` & `google-cloud-private-ca-1.8.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
-url = "https://github.com/googleapis/python-security-private-ca"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-private-ca-1.8.0/tests/__init__.py` & `google-cloud-private-ca-1.8.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/tests/unit/__init__.py` & `google-cloud-private-ca-1.8.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/tests/unit/gapic/__init__.py` & `google-cloud-private-ca-1.8.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/tests/unit/gapic/privateca_v1/__init__.py` & `google-cloud-private-ca-1.8.1/tests/unit/gapic/privateca_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/tests/unit/gapic/privateca_v1/test_certificate_authority_service.py` & `google-cloud-private-ca-1.8.1/tests/unit/gapic/privateca_v1/test_certificate_authority_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1750,17 +1750,19 @@
                     resources.Certificate(),
                     resources.Certificate(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_certificates(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4238,17 +4240,19 @@
                     resources.CertificateAuthority(),
                     resources.CertificateAuthority(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_certificate_authorities(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -6109,17 +6113,19 @@
                     resources.CaPool(),
                     resources.CaPool(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_ca_pools(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -7277,17 +7283,19 @@
                     resources.CertificateRevocationList(),
                     resources.CertificateRevocationList(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_certificate_revocation_lists(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -8735,17 +8743,19 @@
                     resources.CertificateTemplate(),
                     resources.CertificateTemplate(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_certificate_templates(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-private-ca-1.8.0/tests/unit/gapic/privateca_v1beta1/__init__.py` & `google-cloud-private-ca-1.8.1/tests/unit/gapic/privateca_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-private-ca-1.8.0/tests/unit/gapic/privateca_v1beta1/test_certificate_authority_service.py` & `google-cloud-private-ca-1.8.1/tests/unit/gapic/privateca_v1beta1/test_certificate_authority_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1721,17 +1721,19 @@
                     resources.Certificate(),
                     resources.Certificate(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_certificates(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4185,17 +4187,19 @@
                     resources.CertificateAuthority(),
                     resources.CertificateAuthority(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_certificate_authorities(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5630,17 +5634,19 @@
                     resources.CertificateRevocationList(),
                     resources.CertificateRevocationList(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_certificate_revocation_lists(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -6585,17 +6591,19 @@
                     resources.ReusableConfig(),
                     resources.ReusableConfig(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_reusable_configs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

