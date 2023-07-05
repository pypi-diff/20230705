# Comparing `tmp/google-cloud-apigee-registry-0.6.2.tar.gz` & `tmp/google-cloud-apigee-registry-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-apigee-registry-0.6.2.tar", last modified: Mon Mar 27 15:49:17 2023, max compression
+gzip compressed data, was "google-cloud-apigee-registry-0.6.3.tar", last modified: Wed Jul  5 15:50:15 2023, max compression
```

## Comparing `google-cloud-apigee-registry-0.6.2.tar` & `google-cloud-apigee-registry-0.6.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:17.382907 google-cloud-apigee-registry-0.6.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4830 2023-03-27 15:49:17.382907 google-cloud-apigee-registry-0.6.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3903 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:17.370907 google-cloud-apigee-registry-0.6.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:17.370907 google-cloud-apigee-registry-0.6.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:17.370907 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry/
--rw-rw-r--   0 root         (0)     1003     4353 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:17.374907 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/
--rw-rw-r--   0 root         (0)     1003     3983 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    15584 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:17.374907 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:17.374907 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/provisioning/
--rw-rw-r--   0 root         (0)     1003      761 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/provisioning/__init__.py
--rw-rw-r--   0 root         (0)     1003    49258 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/provisioning/async_client.py
--rw-rw-r--   0 root         (0)     1003    58565 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/provisioning/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:17.374907 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/provisioning/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/provisioning/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9491 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/provisioning/transports/base.py
--rw-rw-r--   0 root         (0)     1003    23646 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/provisioning/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    23965 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/provisioning/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    61763 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/provisioning/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:17.374907 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/registry/
--rw-rw-r--   0 root         (0)     1003      745 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/registry/__init__.py
--rw-rw-r--   0 root         (0)     1003   209757 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/registry/async_client.py
--rw-rw-r--   0 root         (0)     1003   212494 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/registry/client.py
--rw-rw-r--   0 root         (0)     1003    37074 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/registry/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:17.378907 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/registry/transports/
--rw-rw-r--   0 root         (0)     1003     1316 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/registry/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    40671 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/registry/transports/base.py
--rw-rw-r--   0 root         (0)     1003    60686 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/registry/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    61882 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/registry/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   237310 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/registry/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:17.378907 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/types/
--rw-rw-r--   0 root         (0)     1003     3591 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     7614 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/types/provisioning_service.py
--rw-rw-r--   0 root         (0)     1003    20527 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/types/registry_models.py
--rw-rw-r--   0 root         (0)     1003    35297 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/types/registry_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:17.378907 google-cloud-apigee-registry-0.6.2/google_cloud_apigee_registry.egg-info/
--rw-r--r--   0 root         (0)     1003     4830 2023-03-27 15:49:17.000000 google-cloud-apigee-registry-0.6.2/google_cloud_apigee_registry.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2421 2023-03-27 15:49:17.000000 google-cloud-apigee-registry-0.6.2/google_cloud_apigee_registry.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:49:17.000000 google-cloud-apigee-registry-0.6.2/google_cloud_apigee_registry.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:49:17.000000 google-cloud-apigee-registry-0.6.2/google_cloud_apigee_registry.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:49:17.000000 google-cloud-apigee-registry-0.6.2/google_cloud_apigee_registry.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 15:49:17.000000 google-cloud-apigee-registry-0.6.2/google_cloud_apigee_registry.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:49:17.000000 google-cloud-apigee-registry-0.6.2/google_cloud_apigee_registry.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:49:17.382907 google-cloud-apigee-registry-0.6.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3006 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:17.378907 google-cloud-apigee-registry-0.6.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:17.378907 google-cloud-apigee-registry-0.6.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:17.382907 google-cloud-apigee-registry-0.6.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:17.382907 google-cloud-apigee-registry-0.6.2/tests/unit/gapic/apigee_registry_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/tests/unit/gapic/apigee_registry_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   179639 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/tests/unit/gapic/apigee_registry_v1/test_provisioning.py
--rw-rw-r--   0 root         (0)     1003   853839 2023-03-27 15:46:27.000000 google-cloud-apigee-registry-0.6.2/tests/unit/gapic/apigee_registry_v1/test_registry.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:15.187316 google-cloud-apigee-registry-0.6.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4791 2023-07-05 15:50:15.187316 google-cloud-apigee-registry-0.6.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3867 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:15.175315 google-cloud-apigee-registry-0.6.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:15.175315 google-cloud-apigee-registry-0.6.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:15.179315 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry/
+-rw-rw-r--   0 root         (0)     1003     4353 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:15.179315 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/
+-rw-rw-r--   0 root         (0)     1003     3983 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15584 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:15.179315 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:15.179315 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/provisioning/
+-rw-rw-r--   0 root         (0)     1003      761 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/provisioning/__init__.py
+-rw-rw-r--   0 root         (0)     1003    49287 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/provisioning/async_client.py
+-rw-rw-r--   0 root         (0)     1003    58565 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/provisioning/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:15.179315 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/provisioning/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/provisioning/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9491 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/provisioning/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    23646 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/provisioning/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    23965 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/provisioning/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    61727 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/provisioning/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:15.183316 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/registry/
+-rw-rw-r--   0 root         (0)     1003      745 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/registry/__init__.py
+-rw-rw-r--   0 root         (0)     1003   209782 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/registry/async_client.py
+-rw-rw-r--   0 root         (0)     1003   212494 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/registry/client.py
+-rw-rw-r--   0 root         (0)     1003    37074 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/registry/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:15.183316 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/registry/transports/
+-rw-rw-r--   0 root         (0)     1003     1316 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/registry/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    40671 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/registry/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    60686 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/registry/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    61882 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/registry/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   237274 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/registry/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:15.183316 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3591 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7614 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/types/provisioning_service.py
+-rw-rw-r--   0 root         (0)     1003    20527 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/types/registry_models.py
+-rw-rw-r--   0 root         (0)     1003    35297 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/types/registry_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:15.183316 google-cloud-apigee-registry-0.6.3/google_cloud_apigee_registry.egg-info/
+-rw-r--r--   0 root         (0)     1003     4791 2023-07-05 15:50:15.000000 google-cloud-apigee-registry-0.6.3/google_cloud_apigee_registry.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2421 2023-07-05 15:50:15.000000 google-cloud-apigee-registry-0.6.3/google_cloud_apigee_registry.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:15.000000 google-cloud-apigee-registry-0.6.3/google_cloud_apigee_registry.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:50:15.000000 google-cloud-apigee-registry-0.6.3/google_cloud_apigee_registry.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:15.000000 google-cloud-apigee-registry-0.6.3/google_cloud_apigee_registry.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:50:15.000000 google-cloud-apigee-registry-0.6.3/google_cloud_apigee_registry.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:50:15.000000 google-cloud-apigee-registry-0.6.3/google_cloud_apigee_registry.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:50:15.187316 google-cloud-apigee-registry-0.6.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3003 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:15.183316 google-cloud-apigee-registry-0.6.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:15.183316 google-cloud-apigee-registry-0.6.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:15.183316 google-cloud-apigee-registry-0.6.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:15.187316 google-cloud-apigee-registry-0.6.3/tests/unit/gapic/apigee_registry_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/tests/unit/gapic/apigee_registry_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   179639 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/tests/unit/gapic/apigee_registry_v1/test_provisioning.py
+-rw-rw-r--   0 root         (0)     1003   855232 2023-07-05 15:46:58.000000 google-cloud-apigee-registry-0.6.3/tests/unit/gapic/apigee_registry_v1/test_registry.py
```

### Comparing `google-cloud-apigee-registry-0.6.2/LICENSE` & `google-cloud-apigee-registry-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/MANIFEST.in` & `google-cloud-apigee-registry-0.6.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/PKG-INFO` & `google-cloud-apigee-registry-0.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-apigee-registry
-Version: 0.6.2
+Version: 0.6.3
 Summary: Google Cloud Apigee Registry API client library
-Home-page: https://github.com/googleapis/python-apigee-registry
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
 
-Python Client for Apigee Registry API API
-=========================================
+Python Client for Apigee Registry API
+=====================================
 
 |preview| |pypi| |versions|
 
-`Apigee Registry API API`_: allows teams to upload and share machine-readable descriptions of APIs that are in use and in development.
+`Apigee Registry API`_: allows teams to upload and share machine-readable descriptions of APIs that are in use and in development.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-apigee-registry.svg
    :target: https://pypi.org/project/google-cloud-apigee-registry/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-apigee-registry.svg
    :target: https://pypi.org/project/google-cloud-apigee-registry/
-.. _Apigee Registry API API: https://cloud.google.com/apigee/docs/api-hub/get-started-registry-api
+.. _Apigee Registry API: https://cloud.google.com/apigee/docs/api-hub/get-started-registry-api
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/apigeeregistry/latest
 .. _Product Documentation:  https://cloud.google.com/apigee/docs/api-hub/get-started-registry-api
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Apigee Registry API API.`_
+3. `Enable the Apigee Registry API.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Apigee Registry API API.:  https://cloud.google.com/apigee/docs/api-hub/get-started-registry-api
+.. _Enable the Apigee Registry API.:  https://cloud.google.com/apigee/docs/api-hub/get-started-registry-api
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-apigee-registry
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Apigee Registry API API
+-  Read the `Client Library Documentation`_ for Apigee Registry API
    to see other available methods on the client.
--  Read the `Apigee Registry API API Product documentation`_ to learn
+-  Read the `Apigee Registry API Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Apigee Registry API API Product documentation:  https://cloud.google.com/apigee/docs/api-hub/get-started-registry-api
+.. _Apigee Registry API Product documentation:  https://cloud.google.com/apigee/docs/api-hub/get-started-registry-api
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-apigee-registry-0.6.2/README.rst` & `google-cloud-apigee-registry-0.6.3/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Apigee Registry API API
-=========================================
+Python Client for Apigee Registry API
+=====================================
 
 |preview| |pypi| |versions|
 
-`Apigee Registry API API`_: allows teams to upload and share machine-readable descriptions of APIs that are in use and in development.
+`Apigee Registry API`_: allows teams to upload and share machine-readable descriptions of APIs that are in use and in development.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-apigee-registry.svg
    :target: https://pypi.org/project/google-cloud-apigee-registry/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-apigee-registry.svg
    :target: https://pypi.org/project/google-cloud-apigee-registry/
-.. _Apigee Registry API API: https://cloud.google.com/apigee/docs/api-hub/get-started-registry-api
+.. _Apigee Registry API: https://cloud.google.com/apigee/docs/api-hub/get-started-registry-api
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/apigeeregistry/latest
 .. _Product Documentation:  https://cloud.google.com/apigee/docs/api-hub/get-started-registry-api
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Apigee Registry API API.`_
+3. `Enable the Apigee Registry API.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Apigee Registry API API.:  https://cloud.google.com/apigee/docs/api-hub/get-started-registry-api
+.. _Enable the Apigee Registry API.:  https://cloud.google.com/apigee/docs/api-hub/get-started-registry-api
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-apigee-registry
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Apigee Registry API API
+-  Read the `Client Library Documentation`_ for Apigee Registry API
    to see other available methods on the client.
--  Read the `Apigee Registry API API Product documentation`_ to learn
+-  Read the `Apigee Registry API Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Apigee Registry API API Product documentation:  https://cloud.google.com/apigee/docs/api-hub/get-started-registry-api
+.. _Apigee Registry API Product documentation:  https://cloud.google.com/apigee/docs/api-hub/get-started-registry-api
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry/__init__.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry/gapic_version.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry/gapic_version.py`

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
-__version__ = "0.6.2"  # {x-release-please-version}
+__version__ = "0.6.3"  # {x-release-please-version}
```

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/__init__.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/gapic_metadata.json` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/gapic_version.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/gapic_version.py`

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
-__version__ = "0.6.2"  # {x-release-please-version}
+__version__ = "0.6.3"  # {x-release-please-version}
```

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/__init__.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/provisioning/__init__.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/provisioning/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/provisioning/async_client.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/provisioning/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1211,15 +1211,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ProvisioningAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/provisioning/client.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/provisioning/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/provisioning/transports/__init__.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/provisioning/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/provisioning/transports/base.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/provisioning/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/provisioning/transports/grpc.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/provisioning/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/provisioning/transports/grpc_asyncio.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/provisioning/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/provisioning/transports/rest.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/provisioning/transports/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1149,15 +1149,15 @@
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
@@ -1266,15 +1266,15 @@
 
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
@@ -1335,15 +1335,15 @@
 
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

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/registry/__init__.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/registry/async_client.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/registry/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -5169,15 +5169,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "RegistryAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/registry/client.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/registry/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/registry/pagers.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/registry/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/registry/transports/__init__.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/registry/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/registry/transports/base.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/registry/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/registry/transports/grpc.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/registry/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/registry/transports/grpc_asyncio.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/registry/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/services/registry/transports/rest.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/services/registry/transports/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -5565,15 +5565,15 @@
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
@@ -5682,15 +5682,15 @@
 
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
@@ -5751,15 +5751,15 @@
 
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

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/types/__init__.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/types/provisioning_service.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/types/provisioning_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/types/registry_models.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/types/registry_models.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/google/cloud/apigee_registry_v1/types/registry_service.py` & `google-cloud-apigee-registry-0.6.3/google/cloud/apigee_registry_v1/types/registry_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/google_cloud_apigee_registry.egg-info/PKG-INFO` & `google-cloud-apigee-registry-0.6.3/google_cloud_apigee_registry.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-apigee-registry
-Version: 0.6.2
+Version: 0.6.3
 Summary: Google Cloud Apigee Registry API client library
-Home-page: https://github.com/googleapis/python-apigee-registry
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
 
-Python Client for Apigee Registry API API
-=========================================
+Python Client for Apigee Registry API
+=====================================
 
 |preview| |pypi| |versions|
 
-`Apigee Registry API API`_: allows teams to upload and share machine-readable descriptions of APIs that are in use and in development.
+`Apigee Registry API`_: allows teams to upload and share machine-readable descriptions of APIs that are in use and in development.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-apigee-registry.svg
    :target: https://pypi.org/project/google-cloud-apigee-registry/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-apigee-registry.svg
    :target: https://pypi.org/project/google-cloud-apigee-registry/
-.. _Apigee Registry API API: https://cloud.google.com/apigee/docs/api-hub/get-started-registry-api
+.. _Apigee Registry API: https://cloud.google.com/apigee/docs/api-hub/get-started-registry-api
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/apigeeregistry/latest
 .. _Product Documentation:  https://cloud.google.com/apigee/docs/api-hub/get-started-registry-api
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Apigee Registry API API.`_
+3. `Enable the Apigee Registry API.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Apigee Registry API API.:  https://cloud.google.com/apigee/docs/api-hub/get-started-registry-api
+.. _Enable the Apigee Registry API.:  https://cloud.google.com/apigee/docs/api-hub/get-started-registry-api
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-apigee-registry
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Apigee Registry API API
+-  Read the `Client Library Documentation`_ for Apigee Registry API
    to see other available methods on the client.
--  Read the `Apigee Registry API API Product documentation`_ to learn
+-  Read the `Apigee Registry API Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Apigee Registry API API Product documentation:  https://cloud.google.com/apigee/docs/api-hub/get-started-registry-api
+.. _Apigee Registry API Product documentation:  https://cloud.google.com/apigee/docs/api-hub/get-started-registry-api
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-apigee-registry-0.6.2/google_cloud_apigee_registry.egg-info/SOURCES.txt` & `google-cloud-apigee-registry-0.6.3/google_cloud_apigee_registry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/setup.py` & `google-cloud-apigee-registry-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
-url = "https://github.com/googleapis/python-apigee-registry"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-apigee-registry-0.6.2/tests/__init__.py` & `google-cloud-apigee-registry-0.6.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/tests/unit/__init__.py` & `google-cloud-apigee-registry-0.6.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/tests/unit/gapic/__init__.py` & `google-cloud-apigee-registry-0.6.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/tests/unit/gapic/apigee_registry_v1/__init__.py` & `google-cloud-apigee-registry-0.6.3/tests/unit/gapic/apigee_registry_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/tests/unit/gapic/apigee_registry_v1/test_provisioning.py` & `google-cloud-apigee-registry-0.6.3/tests/unit/gapic/apigee_registry_v1/test_provisioning.py`

 * *Files identical despite different names*

### Comparing `google-cloud-apigee-registry-0.6.2/tests/unit/gapic/apigee_registry_v1/test_registry.py` & `google-cloud-apigee-registry-0.6.3/tests/unit/gapic/apigee_registry_v1/test_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1084,17 +1084,19 @@
                     registry_models.Api(),
                     registry_models.Api(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_apis(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2521,17 +2523,19 @@
                     registry_models.ApiVersion(),
                     registry_models.ApiVersion(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_api_versions(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3968,17 +3972,19 @@
                     registry_models.ApiSpec(),
                     registry_models.ApiSpec(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_api_specs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5811,17 +5817,19 @@
                     registry_models.ApiSpec(),
                     registry_models.ApiSpec(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_api_spec_revisions(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -6726,17 +6734,19 @@
                     registry_models.ApiDeployment(),
                     registry_models.ApiDeployment(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_api_deployments(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -8378,17 +8388,19 @@
                     registry_models.ApiDeployment(),
                     registry_models.ApiDeployment(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_api_deployment_revisions(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -9270,17 +9282,19 @@
                     registry_models.Artifact(),
                     registry_models.Artifact(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_artifacts(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

