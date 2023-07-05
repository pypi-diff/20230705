# Comparing `tmp/google-cloud-workstations-0.4.0.tar.gz` & `tmp/google-cloud-workstations-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-workstations-0.4.0.tar", last modified: Wed May 17 17:31:22 2023, max compression
+gzip compressed data, was "google-cloud-workstations-0.4.1.tar", last modified: Wed Jul  5 15:56:53 2023, max compression
```

## Comparing `google-cloud-workstations-0.4.0.tar` & `google-cloud-workstations-0.4.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.340876 google-cloud-workstations-0.4.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4600 2023-05-17 17:31:22.340876 google-cloud-workstations-0.4.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3682 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.328870 google-cloud-workstations-0.4.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.328870 google-cloud-workstations-0.4.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.328870 google-cloud-workstations-0.4.0/google/cloud/workstations/
--rw-rw-r--   0 root         (0)     1003     3048 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.332872 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/
--rw-rw-r--   0 root         (0)     1003     2904 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8908 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.332872 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.332872 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/
--rw-rw-r--   0 root         (0)     1003      761 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/__init__.py
--rw-rw-r--   0 root         (0)     1003   129566 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/async_client.py
--rw-rw-r--   0 root         (0)     1003   140785 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/client.py
--rw-rw-r--   0 root         (0)     1003    27340 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.332872 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    20457 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/base.py
--rw-rw-r--   0 root         (0)     1003    43040 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    43871 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   142624 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.332872 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/types/
--rw-rw-r--   0 root         (0)     1003     2643 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    55514 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1/types/workstations.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.332872 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/
--rw-rw-r--   0 root         (0)     1003     2908 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     8916 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.332872 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.336874 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/
--rw-rw-r--   0 root         (0)     1003      761 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/__init__.py
--rw-rw-r--   0 root         (0)     1003   130002 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/async_client.py
--rw-rw-r--   0 root         (0)     1003   141221 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/client.py
--rw-rw-r--   0 root         (0)     1003    27504 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.336874 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    20465 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/base.py
--rw-rw-r--   0 root         (0)     1003    43124 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    43955 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   142768 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.336874 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     2643 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    58373 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/types/workstations.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.336874 google-cloud-workstations-0.4.0/google_cloud_workstations.egg-info/
--rw-r--r--   0 root         (0)     1003     4600 2023-05-17 17:31:22.000000 google-cloud-workstations-0.4.0/google_cloud_workstations.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2717 2023-05-17 17:31:22.000000 google-cloud-workstations-0.4.0/google_cloud_workstations.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-17 17:31:22.000000 google-cloud-workstations-0.4.0/google_cloud_workstations.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-05-17 17:31:22.000000 google-cloud-workstations-0.4.0/google_cloud_workstations.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-17 17:31:22.000000 google-cloud-workstations-0.4.0/google_cloud_workstations.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-05-17 17:31:22.000000 google-cloud-workstations-0.4.0/google_cloud_workstations.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-05-17 17:31:22.000000 google-cloud-workstations-0.4.0/google_cloud_workstations.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-05-17 17:31:22.340876 google-cloud-workstations-0.4.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2994 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.336874 google-cloud-workstations-0.4.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.336874 google-cloud-workstations-0.4.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.336874 google-cloud-workstations-0.4.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.336874 google-cloud-workstations-0.4.0/tests/unit/gapic/workstations_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/tests/unit/gapic/workstations_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   568245 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/tests/unit/gapic/workstations_v1/test_workstations.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-17 17:31:22.340876 google-cloud-workstations-0.4.0/tests/unit/gapic/workstations_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/tests/unit/gapic/workstations_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003   569173 2023-05-17 17:28:51.000000 google-cloud-workstations-0.4.0/tests/unit/gapic/workstations_v1beta/test_workstations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:53.015643 google-cloud-workstations-0.4.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4600 2023-07-05 15:56:53.015643 google-cloud-workstations-0.4.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3682 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:53.003643 google-cloud-workstations-0.4.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:53.003643 google-cloud-workstations-0.4.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:53.003643 google-cloud-workstations-0.4.1/google/cloud/workstations/
+-rw-rw-r--   0 root         (0)     1003     3048 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:53.003643 google-cloud-workstations-0.4.1/google/cloud/workstations_v1/
+-rw-rw-r--   0 root         (0)     1003     2904 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8908 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:53.003643 google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:53.007643 google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/workstations/
+-rw-rw-r--   0 root         (0)     1003      761 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/workstations/__init__.py
+-rw-rw-r--   0 root         (0)     1003   129595 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/workstations/async_client.py
+-rw-rw-r--   0 root         (0)     1003   140785 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/workstations/client.py
+-rw-rw-r--   0 root         (0)     1003    27340 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/workstations/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:53.007643 google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/workstations/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/workstations/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20457 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/workstations/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    43040 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/workstations/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    43871 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/workstations/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   142588 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/workstations/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:53.007643 google-cloud-workstations-0.4.1/google/cloud/workstations_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2643 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    55514 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1/types/workstations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:53.007643 google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/
+-rw-rw-r--   0 root         (0)     1003     2908 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8916 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:53.007643 google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:53.007643 google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/workstations/
+-rw-rw-r--   0 root         (0)     1003      761 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/workstations/__init__.py
+-rw-rw-r--   0 root         (0)     1003   130031 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/workstations/async_client.py
+-rw-rw-r--   0 root         (0)     1003   141221 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/workstations/client.py
+-rw-rw-r--   0 root         (0)     1003    27504 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/workstations/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:53.011643 google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/workstations/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/workstations/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20465 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/workstations/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    43124 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/workstations/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    43955 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/workstations/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   142732 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/workstations/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:53.011643 google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     2643 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    58373 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/types/workstations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:53.011643 google-cloud-workstations-0.4.1/google_cloud_workstations.egg-info/
+-rw-r--r--   0 root         (0)     1003     4600 2023-07-05 15:56:52.000000 google-cloud-workstations-0.4.1/google_cloud_workstations.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2717 2023-07-05 15:56:52.000000 google-cloud-workstations-0.4.1/google_cloud_workstations.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:56:52.000000 google-cloud-workstations-0.4.1/google_cloud_workstations.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:56:52.000000 google-cloud-workstations-0.4.1/google_cloud_workstations.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:56:52.000000 google-cloud-workstations-0.4.1/google_cloud_workstations.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:56:52.000000 google-cloud-workstations-0.4.1/google_cloud_workstations.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:56:52.000000 google-cloud-workstations-0.4.1/google_cloud_workstations.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:56:53.015643 google-cloud-workstations-0.4.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2994 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:53.011643 google-cloud-workstations-0.4.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:53.011643 google-cloud-workstations-0.4.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:53.011643 google-cloud-workstations-0.4.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:53.011643 google-cloud-workstations-0.4.1/tests/unit/gapic/workstations_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/tests/unit/gapic/workstations_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   569240 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/tests/unit/gapic/workstations_v1/test_workstations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:53.015643 google-cloud-workstations-0.4.1/tests/unit/gapic/workstations_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/tests/unit/gapic/workstations_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003   570168 2023-07-05 15:46:59.000000 google-cloud-workstations-0.4.1/tests/unit/gapic/workstations_v1beta/test_workstations.py
```

### Comparing `google-cloud-workstations-0.4.0/LICENSE` & `google-cloud-workstations-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/MANIFEST.in` & `google-cloud-workstations-0.4.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/PKG-INFO` & `google-cloud-workstations-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-workstations
-Version: 0.4.0
+Version: 0.4.1
 Summary: Google Cloud Workstations API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-workstations-0.4.0/README.rst` & `google-cloud-workstations-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations/__init__.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations/gapic_version.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations/gapic_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.4.0"  # {x-release-please-version}
+__version__ = "0.4.1"  # {x-release-please-version}
```

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/__init__.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/gapic_metadata.json` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/gapic_version.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1/gapic_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.4.0"  # {x-release-please-version}
+__version__ = "0.4.1"  # {x-release-please-version}
```

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/__init__.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/__init__.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/workstations/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/async_client.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/workstations/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3208,15 +3208,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "WorkstationsAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/client.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/workstations/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/pagers.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/workstations/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/__init__.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/workstations/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/base.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/workstations/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/grpc.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/workstations/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/grpc_asyncio.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/workstations/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/services/workstations/transports/rest.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1/services/workstations/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -3218,15 +3218,15 @@
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
@@ -3295,15 +3295,15 @@
 
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
@@ -3364,15 +3364,15 @@
 
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

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/types/__init__.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1/types/workstations.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1/types/workstations.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/__init__.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/gapic_metadata.json` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/gapic_version.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/gapic_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.4.0"  # {x-release-please-version}
+__version__ = "0.4.1"  # {x-release-please-version}
```

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/__init__.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/__init__.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/workstations/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/async_client.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/workstations/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3208,15 +3208,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "WorkstationsAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/client.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/workstations/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/pagers.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/workstations/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/__init__.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/workstations/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/base.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/workstations/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/grpc.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/workstations/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/grpc_asyncio.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/workstations/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/services/workstations/transports/rest.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/services/workstations/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -3218,15 +3218,15 @@
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
@@ -3295,15 +3295,15 @@
 
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
@@ -3364,15 +3364,15 @@
 
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

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/types/__init__.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google/cloud/workstations_v1beta/types/workstations.py` & `google-cloud-workstations-0.4.1/google/cloud/workstations_v1beta/types/workstations.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/google_cloud_workstations.egg-info/PKG-INFO` & `google-cloud-workstations-0.4.1/google_cloud_workstations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-workstations
-Version: 0.4.0
+Version: 0.4.1
 Summary: Google Cloud Workstations API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-workstations-0.4.0/google_cloud_workstations.egg-info/SOURCES.txt` & `google-cloud-workstations-0.4.1/google_cloud_workstations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/setup.py` & `google-cloud-workstations-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/tests/__init__.py` & `google-cloud-workstations-0.4.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/tests/unit/__init__.py` & `google-cloud-workstations-0.4.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/tests/unit/gapic/__init__.py` & `google-cloud-workstations-0.4.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/tests/unit/gapic/workstations_v1/__init__.py` & `google-cloud-workstations-0.4.1/tests/unit/gapic/workstations_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/tests/unit/gapic/workstations_v1/test_workstations.py` & `google-cloud-workstations-0.4.1/tests/unit/gapic/workstations_v1/test_workstations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1422,17 +1422,19 @@
                     workstations.WorkstationCluster(),
                     workstations.WorkstationCluster(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_workstation_clusters(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2889,17 +2891,19 @@
                     workstations.WorkstationConfig(),
                     workstations.WorkstationConfig(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_workstation_configs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3336,17 +3340,19 @@
                     workstations.WorkstationConfig(),
                     workstations.WorkstationConfig(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_usable_workstation_configs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4791,17 +4797,19 @@
                     workstations.Workstation(),
                     workstations.Workstation(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_workstations(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5238,17 +5246,19 @@
                     workstations.Workstation(),
                     workstations.Workstation(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_usable_workstations(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-workstations-0.4.0/tests/unit/gapic/workstations_v1beta/__init__.py` & `google-cloud-workstations-0.4.1/tests/unit/gapic/workstations_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.4.0/tests/unit/gapic/workstations_v1beta/test_workstations.py` & `google-cloud-workstations-0.4.1/tests/unit/gapic/workstations_v1beta/test_workstations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1422,17 +1422,19 @@
                     workstations.WorkstationCluster(),
                     workstations.WorkstationCluster(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_workstation_clusters(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2893,17 +2895,19 @@
                     workstations.WorkstationConfig(),
                     workstations.WorkstationConfig(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_workstation_configs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3340,17 +3344,19 @@
                     workstations.WorkstationConfig(),
                     workstations.WorkstationConfig(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_usable_workstation_configs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4795,17 +4801,19 @@
                     workstations.Workstation(),
                     workstations.Workstation(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_workstations(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5242,17 +5250,19 @@
                     workstations.Workstation(),
                     workstations.Workstation(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_usable_workstations(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

