# Comparing `tmp/google-cloud-notebooks-1.7.0.tar.gz` & `tmp/google-cloud-notebooks-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-notebooks-1.7.0.tar", last modified: Mon Apr 17 10:44:39 2023, max compression
+gzip compressed data, was "google-cloud-notebooks-1.7.1.tar", last modified: Wed Jul  5 15:54:23 2023, max compression
```

## Comparing `google-cloud-notebooks-1.7.0.tar` & `google-cloud-notebooks-1.7.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.264064 google-cloud-notebooks-1.7.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4944 2023-04-17 10:44:39.264064 google-cloud-notebooks-1.7.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4022 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.244054 google-cloud-notebooks-1.7.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.244054 google-cloud-notebooks-1.7.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.248056 google-cloud-notebooks-1.7.0/google/cloud/notebooks/
--rw-rw-r--   0 root         (0)     1003     6284 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       83 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.248056 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/
--rw-rw-r--   0 root         (0)     1003     5773 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    12874 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       83 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.248056 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.252058 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/
--rw-rw-r--   0 root         (0)     1003      801 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    98226 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   108678 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/client.py
--rw-rw-r--   0 root         (0)     1003     5785 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.252058 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/transports/
--rw-rw-r--   0 root         (0)     1003     1273 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14018 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    35729 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    36386 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.252058 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   178928 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   194268 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/client.py
--rw-rw-r--   0 root         (0)     1003    20735 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.256060 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/transports/
--rw-rw-r--   0 root         (0)     1003     1202 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    23439 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    59398 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    60689 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.256060 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/
--rw-rw-r--   0 root         (0)     1003     5244 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2956 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/diagnostic_config.py
--rw-rw-r--   0 root         (0)     1003     5366 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/environment.py
--rw-rw-r--   0 root         (0)     1003     2808 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/event.py
--rw-rw-r--   0 root         (0)     1003    18072 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/execution.py
--rw-rw-r--   0 root         (0)     1003    31242 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/instance.py
--rw-rw-r--   0 root         (0)     1003     1524 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/instance_config.py
--rw-rw-r--   0 root         (0)     1003    12525 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/managed_service.py
--rw-rw-r--   0 root         (0)     1003    35699 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/runtime.py
--rw-rw-r--   0 root         (0)     1003     5388 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/schedule.py
--rw-rw-r--   0 root         (0)     1003    33632 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.256060 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/
--rw-rw-r--   0 root         (0)     1003     2530 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8015 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       83 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.256060 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.260062 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   104669 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   116232 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/client.py
--rw-rw-r--   0 root         (0)     1003    10868 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.260062 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    16641 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    42380 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    43205 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   140287 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.260062 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     2239 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     5390 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/types/environment.py
--rw-rw-r--   0 root         (0)     1003    18137 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/types/instance.py
--rw-rw-r--   0 root         (0)     1003    17607 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.260062 google-cloud-notebooks-1.7.0/google_cloud_notebooks.egg-info/
--rw-r--r--   0 root         (0)     1003     4944 2023-04-17 10:44:39.000000 google-cloud-notebooks-1.7.0/google_cloud_notebooks.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3805 2023-04-17 10:44:39.000000 google-cloud-notebooks-1.7.0/google_cloud_notebooks.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-17 10:44:39.000000 google-cloud-notebooks-1.7.0/google_cloud_notebooks.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-04-17 10:44:39.000000 google-cloud-notebooks-1.7.0/google_cloud_notebooks.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-17 10:44:39.000000 google-cloud-notebooks-1.7.0/google_cloud_notebooks.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-04-17 10:44:39.000000 google-cloud-notebooks-1.7.0/google_cloud_notebooks.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-17 10:44:39.000000 google-cloud-notebooks-1.7.0/google_cloud_notebooks.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-04-17 10:44:39.264064 google-cloud-notebooks-1.7.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2976 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.260062 google-cloud-notebooks-1.7.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.264064 google-cloud-notebooks-1.7.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.264064 google-cloud-notebooks-1.7.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.264064 google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   222490 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1/test_managed_notebook_service.py
--rw-rw-r--   0 root         (0)     1003   380606 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1/test_notebook_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.264064 google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   406758 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1beta1/test_notebook_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.400201 google-cloud-notebooks-1.7.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4911 2023-07-05 15:54:23.400201 google-cloud-notebooks-1.7.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3986 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.380201 google-cloud-notebooks-1.7.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.384201 google-cloud-notebooks-1.7.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.384201 google-cloud-notebooks-1.7.1/google/cloud/notebooks/
+-rw-rw-r--   0 root         (0)     1003     6284 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       83 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.384201 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/
+-rw-rw-r--   0 root         (0)     1003     5773 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12874 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       83 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.384201 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.388201 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/managed_notebook_service/
+-rw-rw-r--   0 root         (0)     1003      801 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/managed_notebook_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    98265 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/managed_notebook_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   108678 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/managed_notebook_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5785 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/managed_notebook_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.388201 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/managed_notebook_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1273 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/managed_notebook_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14018 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/managed_notebook_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    35729 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/managed_notebook_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    36386 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/managed_notebook_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.388201 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/notebook_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/notebook_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   178960 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/notebook_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   194268 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/notebook_service/client.py
+-rw-rw-r--   0 root         (0)     1003    20735 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/notebook_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.388201 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/notebook_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1202 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/notebook_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    23439 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/notebook_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    59398 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/notebook_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    60689 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/notebook_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.392201 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/
+-rw-rw-r--   0 root         (0)     1003     5244 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2956 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/diagnostic_config.py
+-rw-rw-r--   0 root         (0)     1003     5366 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/environment.py
+-rw-rw-r--   0 root         (0)     1003     2808 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/event.py
+-rw-rw-r--   0 root         (0)     1003    18072 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/execution.py
+-rw-rw-r--   0 root         (0)     1003    31242 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/instance.py
+-rw-rw-r--   0 root         (0)     1003     1524 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/instance_config.py
+-rw-rw-r--   0 root         (0)     1003    12525 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/managed_service.py
+-rw-rw-r--   0 root         (0)     1003    35699 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/runtime.py
+-rw-rw-r--   0 root         (0)     1003     5388 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/schedule.py
+-rw-rw-r--   0 root         (0)     1003    33632 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.392201 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     2530 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8015 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       83 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.392201 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.392201 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/notebook_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/notebook_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   104701 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/notebook_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   116232 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/notebook_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10868 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/notebook_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.392201 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/notebook_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/notebook_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16641 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/notebook_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    42380 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/notebook_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    43205 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/notebook_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   140251 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/notebook_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.396201 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     2239 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5390 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/types/environment.py
+-rw-rw-r--   0 root         (0)     1003    18137 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/types/instance.py
+-rw-rw-r--   0 root         (0)     1003    17607 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.396201 google-cloud-notebooks-1.7.1/google_cloud_notebooks.egg-info/
+-rw-r--r--   0 root         (0)     1003     4911 2023-07-05 15:54:23.000000 google-cloud-notebooks-1.7.1/google_cloud_notebooks.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3805 2023-07-05 15:54:23.000000 google-cloud-notebooks-1.7.1/google_cloud_notebooks.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:23.000000 google-cloud-notebooks-1.7.1/google_cloud_notebooks.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:54:23.000000 google-cloud-notebooks-1.7.1/google_cloud_notebooks.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:23.000000 google-cloud-notebooks-1.7.1/google_cloud_notebooks.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:54:23.000000 google-cloud-notebooks-1.7.1/google_cloud_notebooks.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:54:23.000000 google-cloud-notebooks-1.7.1/google_cloud_notebooks.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:54:23.400201 google-cloud-notebooks-1.7.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2979 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.396201 google-cloud-notebooks-1.7.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.396201 google-cloud-notebooks-1.7.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.396201 google-cloud-notebooks-1.7.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.396201 google-cloud-notebooks-1.7.1/tests/unit/gapic/notebooks_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/tests/unit/gapic/notebooks_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   222600 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/tests/unit/gapic/notebooks_v1/test_managed_notebook_service.py
+-rw-rw-r--   0 root         (0)     1003   381268 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/tests/unit/gapic/notebooks_v1/test_notebook_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:23.396201 google-cloud-notebooks-1.7.1/tests/unit/gapic/notebooks_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/tests/unit/gapic/notebooks_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   406888 2023-07-05 15:46:59.000000 google-cloud-notebooks-1.7.1/tests/unit/gapic/notebooks_v1beta1/test_notebook_service.py
```

### Comparing `google-cloud-notebooks-1.7.0/LICENSE` & `google-cloud-notebooks-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/MANIFEST.in` & `google-cloud-notebooks-1.7.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/PKG-INFO` & `google-cloud-notebooks-1.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-notebooks
-Version: 1.7.0
+Version: 1.7.1
 Summary: Google Cloud Notebooks API client library
-Home-page: https://github.com/googleapis/python-notebooks
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
 
-Python Client for AI Platform Notebooks API
-===========================================
+Python Client for AI Platform Notebooks
+=======================================
 
 |stable| |pypi| |versions|
 
-`AI Platform Notebooks API`_: is a managed service that offers an integrated and secure JupyterLab environment for data scientists and machine learning developers to experiment, develop, and deploy models into production. Users can create instances running JupyterLab that come pre-installed with the latest data science and machine learning frameworks in a single click.
+`AI Platform Notebooks`_: is a managed service that offers an integrated and secure JupyterLab environment for data scientists and machine learning developers to experiment, develop, and deploy models into production. Users can create instances running JupyterLab that come pre-installed with the latest data science and machine learning frameworks in a single click.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-notebooks.svg
    :target: https://pypi.org/project/google-cloud-notebooks/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-notebooks.svg
    :target: https://pypi.org/project/google-cloud-notebooks/
-.. _AI Platform Notebooks API: https://cloud.google.com/ai-platform/notebooks/
+.. _AI Platform Notebooks: https://cloud.google.com/ai-platform/notebooks/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/notebooks/latest
 .. _Product Documentation:  https://cloud.google.com/ai-platform/notebooks/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the AI Platform Notebooks API.`_
+3. `Enable the AI Platform Notebooks.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the AI Platform Notebooks API.:  https://cloud.google.com/ai-platform/notebooks/
+.. _Enable the AI Platform Notebooks.:  https://cloud.google.com/ai-platform/notebooks/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-notebooks
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for AI Platform Notebooks API
+-  Read the `Client Library Documentation`_ for AI Platform Notebooks
    to see other available methods on the client.
--  Read the `AI Platform Notebooks API Product documentation`_ to learn
+-  Read the `AI Platform Notebooks Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _AI Platform Notebooks API Product documentation:  https://cloud.google.com/ai-platform/notebooks/
+.. _AI Platform Notebooks Product documentation:  https://cloud.google.com/ai-platform/notebooks/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-notebooks-1.7.0/README.rst` & `google-cloud-notebooks-1.7.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for AI Platform Notebooks API
-===========================================
+Python Client for AI Platform Notebooks
+=======================================
 
 |stable| |pypi| |versions|
 
-`AI Platform Notebooks API`_: is a managed service that offers an integrated and secure JupyterLab environment for data scientists and machine learning developers to experiment, develop, and deploy models into production. Users can create instances running JupyterLab that come pre-installed with the latest data science and machine learning frameworks in a single click.
+`AI Platform Notebooks`_: is a managed service that offers an integrated and secure JupyterLab environment for data scientists and machine learning developers to experiment, develop, and deploy models into production. Users can create instances running JupyterLab that come pre-installed with the latest data science and machine learning frameworks in a single click.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-notebooks.svg
    :target: https://pypi.org/project/google-cloud-notebooks/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-notebooks.svg
    :target: https://pypi.org/project/google-cloud-notebooks/
-.. _AI Platform Notebooks API: https://cloud.google.com/ai-platform/notebooks/
+.. _AI Platform Notebooks: https://cloud.google.com/ai-platform/notebooks/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/notebooks/latest
 .. _Product Documentation:  https://cloud.google.com/ai-platform/notebooks/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the AI Platform Notebooks API.`_
+3. `Enable the AI Platform Notebooks.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the AI Platform Notebooks API.:  https://cloud.google.com/ai-platform/notebooks/
+.. _Enable the AI Platform Notebooks.:  https://cloud.google.com/ai-platform/notebooks/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-notebooks
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for AI Platform Notebooks API
+-  Read the `Client Library Documentation`_ for AI Platform Notebooks
    to see other available methods on the client.
--  Read the `AI Platform Notebooks API Product documentation`_ to learn
+-  Read the `AI Platform Notebooks Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _AI Platform Notebooks API Product documentation:  https://cloud.google.com/ai-platform/notebooks/
+.. _AI Platform Notebooks Product documentation:  https://cloud.google.com/ai-platform/notebooks/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks/__init__.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks/gapic_version.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks/gapic_version.py`

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
+__version__ = "1.7.1"  # {x-release-please-version}
```

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/__init__.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/gapic_metadata.json` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/gapic_version.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/gapic_version.py`

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
+__version__ = "1.7.1"  # {x-release-please-version}
```

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/__init__.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/__init__.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/managed_notebook_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/async_client.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/managed_notebook_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2445,15 +2445,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ManagedNotebookServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/client.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/managed_notebook_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/pagers.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/managed_notebook_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/transports/__init__.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/managed_notebook_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/transports/base.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/managed_notebook_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/transports/grpc.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/managed_notebook_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/transports/grpc_asyncio.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/managed_notebook_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/__init__.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/notebook_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/async_client.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/notebook_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4535,15 +4535,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "NotebookServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/client.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/notebook_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/pagers.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/notebook_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/transports/__init__.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/notebook_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/transports/base.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/notebook_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/transports/grpc.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/notebook_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/transports/grpc_asyncio.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/services/notebook_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/__init__.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/diagnostic_config.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/diagnostic_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/environment.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/environment.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/event.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/event.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/execution.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/execution.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/instance.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/instance.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/instance_config.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/instance_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/managed_service.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/managed_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/runtime.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/runtime.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/schedule.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/schedule.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/service.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/__init__.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/gapic_metadata.json` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/gapic_version.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/gapic_version.py`

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
+__version__ = "1.7.1"  # {x-release-please-version}
```

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/__init__.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/__init__.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/notebook_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/async_client.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/notebook_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2665,15 +2665,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "NotebookServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/client.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/notebook_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/pagers.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/notebook_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/transports/__init__.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/notebook_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/transports/base.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/notebook_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/transports/grpc.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/notebook_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/transports/grpc_asyncio.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/notebook_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/transports/rest.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/services/notebook_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -3206,15 +3206,15 @@
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
@@ -3278,15 +3278,15 @@
 
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
@@ -3347,15 +3347,15 @@
 
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

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/types/__init__.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/types/environment.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/types/environment.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/types/instance.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/types/instance.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/types/service.py` & `google-cloud-notebooks-1.7.1/google/cloud/notebooks_v1beta1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/google_cloud_notebooks.egg-info/PKG-INFO` & `google-cloud-notebooks-1.7.1/google_cloud_notebooks.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-notebooks
-Version: 1.7.0
+Version: 1.7.1
 Summary: Google Cloud Notebooks API client library
-Home-page: https://github.com/googleapis/python-notebooks
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
 
-Python Client for AI Platform Notebooks API
-===========================================
+Python Client for AI Platform Notebooks
+=======================================
 
 |stable| |pypi| |versions|
 
-`AI Platform Notebooks API`_: is a managed service that offers an integrated and secure JupyterLab environment for data scientists and machine learning developers to experiment, develop, and deploy models into production. Users can create instances running JupyterLab that come pre-installed with the latest data science and machine learning frameworks in a single click.
+`AI Platform Notebooks`_: is a managed service that offers an integrated and secure JupyterLab environment for data scientists and machine learning developers to experiment, develop, and deploy models into production. Users can create instances running JupyterLab that come pre-installed with the latest data science and machine learning frameworks in a single click.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-notebooks.svg
    :target: https://pypi.org/project/google-cloud-notebooks/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-notebooks.svg
    :target: https://pypi.org/project/google-cloud-notebooks/
-.. _AI Platform Notebooks API: https://cloud.google.com/ai-platform/notebooks/
+.. _AI Platform Notebooks: https://cloud.google.com/ai-platform/notebooks/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/notebooks/latest
 .. _Product Documentation:  https://cloud.google.com/ai-platform/notebooks/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the AI Platform Notebooks API.`_
+3. `Enable the AI Platform Notebooks.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the AI Platform Notebooks API.:  https://cloud.google.com/ai-platform/notebooks/
+.. _Enable the AI Platform Notebooks.:  https://cloud.google.com/ai-platform/notebooks/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-notebooks
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for AI Platform Notebooks API
+-  Read the `Client Library Documentation`_ for AI Platform Notebooks
    to see other available methods on the client.
--  Read the `AI Platform Notebooks API Product documentation`_ to learn
+-  Read the `AI Platform Notebooks Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _AI Platform Notebooks API Product documentation:  https://cloud.google.com/ai-platform/notebooks/
+.. _AI Platform Notebooks Product documentation:  https://cloud.google.com/ai-platform/notebooks/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-notebooks-1.7.0/google_cloud_notebooks.egg-info/SOURCES.txt` & `google-cloud-notebooks-1.7.1/google_cloud_notebooks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/setup.py` & `google-cloud-notebooks-1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
-url = "https://github.com/googleapis/python-notebooks"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-notebooks-1.7.0/tests/__init__.py` & `google-cloud-notebooks-1.7.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/tests/unit/__init__.py` & `google-cloud-notebooks-1.7.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/tests/unit/gapic/__init__.py` & `google-cloud-notebooks-1.7.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1/__init__.py` & `google-cloud-notebooks-1.7.1/tests/unit/gapic/notebooks_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1/test_managed_notebook_service.py` & `google-cloud-notebooks-1.7.1/tests/unit/gapic/notebooks_v1/test_managed_notebook_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1138,17 +1138,19 @@
                     runtime.Runtime(),
                     runtime.Runtime(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_runtimes(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1170,15 +1172,14 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_runtime), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = runtime.Runtime(
             name="name_value",
             state=runtime.Runtime.State.STARTING,
             health_state=runtime.Runtime.HealthState.HEALTHY,
-            virtual_machine=runtime.VirtualMachine(instance_name="instance_name_value"),
         )
         response = client.get_runtime(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == managed_service.GetRuntimeRequest()
```

### Comparing `google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1/test_notebook_service.py` & `google-cloud-notebooks-1.7.1/tests/unit/gapic/notebooks_v1/test_notebook_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1132,17 +1132,19 @@
                     instance.Instance(),
                     instance.Instance(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_instances(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1186,15 +1188,14 @@
             no_proxy_access=True,
             network="network_value",
             subnet="subnet_value",
             tags=["tags_value"],
             nic_type=instance.Instance.NicType.VIRTIO_NET,
             creator="creator_value",
             can_ip_forward=True,
-            vm_image=environment.VmImage(project="project_value"),
         )
         response = client.get_instance(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.GetInstanceRequest()
@@ -5173,17 +5174,19 @@
                     environment.Environment(),
                     environment.Environment(),
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
@@ -5206,15 +5209,14 @@
     with mock.patch.object(type(client.transport.get_environment), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = environment.Environment(
             name="name_value",
             display_name="display_name_value",
             description="description_value",
             post_startup_script="post_startup_script_value",
-            vm_image=environment.VmImage(project="project_value"),
         )
         response = client.get_environment(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.GetEnvironmentRequest()
@@ -6342,17 +6344,19 @@
                     schedule.Schedule(),
                     schedule.Schedule(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_schedules(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -7630,17 +7634,19 @@
                     execution.Execution(),
                     execution.Execution(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_executions(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1beta1/__init__.py` & `google-cloud-notebooks-1.7.1/tests/unit/gapic/notebooks_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1beta1/test_notebook_service.py` & `google-cloud-notebooks-1.7.1/tests/unit/gapic/notebooks_v1beta1/test_notebook_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1072,17 +1072,19 @@
                     instance.Instance(),
                     instance.Instance(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_instances(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1123,15 +1125,14 @@
             kms_key="kms_key_value",
             no_public_ip=True,
             no_proxy_access=True,
             network="network_value",
             subnet="subnet_value",
             nic_type=instance.Instance.NicType.VIRTIO_NET,
             can_ip_forward=True,
-            vm_image=environment.VmImage(project="project_value"),
         )
         response = client.get_instance(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.GetInstanceRequest()
@@ -3625,17 +3626,19 @@
                     environment.Environment(),
                     environment.Environment(),
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
@@ -3658,15 +3661,14 @@
     with mock.patch.object(type(client.transport.get_environment), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = environment.Environment(
             name="name_value",
             display_name="display_name_value",
             description="description_value",
             post_startup_script="post_startup_script_value",
-            vm_image=environment.VmImage(project="project_value"),
         )
         response = client.get_environment(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.GetEnvironmentRequest()
@@ -4427,15 +4429,14 @@
             kms_key="kms_key_value",
             no_public_ip=True,
             no_proxy_access=True,
             network="network_value",
             subnet="subnet_value",
             nic_type=instance.Instance.NicType.VIRTIO_NET,
             can_ip_forward=True,
-            vm_image=environment.VmImage(project="project_value"),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = instance.Instance.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -7818,15 +7819,14 @@
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = environment.Environment(
             name="name_value",
             display_name="display_name_value",
             description="description_value",
             post_startup_script="post_startup_script_value",
-            vm_image=environment.VmImage(project="project_value"),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = environment.Environment.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

