# Comparing `tmp/google-cloud-bare-metal-solution-1.4.1.tar.gz` & `tmp/google-cloud-bare-metal-solution-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-bare-metal-solution-1.4.1.tar", last modified: Mon Mar 27 14:52:43 2023, max compression
+gzip compressed data, was "google-cloud-bare-metal-solution-1.4.2.tar", last modified: Wed Jul  5 15:50:27 2023, max compression
```

## Comparing `google-cloud-bare-metal-solution-1.4.1.tar` & `google-cloud-bare-metal-solution-1.4.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:43.199518 google-cloud-bare-metal-solution-1.4.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4775 2023-03-27 14:52:43.199518 google-cloud-bare-metal-solution-1.4.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3823 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:43.187518 google-cloud-bare-metal-solution-1.4.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:43.191518 google-cloud-bare-metal-solution-1.4.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:43.191518 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution/
--rw-rw-r--   0 root         (0)     1003     3376 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:43.191518 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/
--rw-rw-r--   0 root         (0)     1003     2999 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     7854 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:43.191518 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:43.195518 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/
--rw-rw-r--   0 root         (0)     1003      781 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/__init__.py
--rw-rw-r--   0 root         (0)     1003   106341 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/async_client.py
--rw-rw-r--   0 root         (0)     1003   120820 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/client.py
--rw-rw-r--   0 root         (0)     1003    25653 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:43.195518 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    15537 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/base.py
--rw-rw-r--   0 root         (0)     1003    36145 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    36987 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   116864 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:43.195518 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/types/
--rw-rw-r--   0 root         (0)     1003     2661 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2832 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/types/baremetalsolution.py
--rw-rw-r--   0 root         (0)     1003    13502 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/types/instance.py
--rw-rw-r--   0 root         (0)     1003     6204 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/types/lun.py
--rw-rw-r--   0 root         (0)     1003    14699 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/types/network.py
--rw-rw-r--   0 root         (0)     1003     7836 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/types/nfs_share.py
--rw-rw-r--   0 root         (0)     1003    11611 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/types/volume.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:43.199518 google-cloud-bare-metal-solution-1.4.1/google_cloud_bare_metal_solution.egg-info/
--rw-r--r--   0 root         (0)     1003     4775 2023-03-27 14:52:43.000000 google-cloud-bare-metal-solution-1.4.1/google_cloud_bare_metal_solution.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2154 2023-03-27 14:52:43.000000 google-cloud-bare-metal-solution-1.4.1/google_cloud_bare_metal_solution.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:52:43.000000 google-cloud-bare-metal-solution-1.4.1/google_cloud_bare_metal_solution.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:52:43.000000 google-cloud-bare-metal-solution-1.4.1/google_cloud_bare_metal_solution.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:52:43.000000 google-cloud-bare-metal-solution-1.4.1/google_cloud_bare_metal_solution.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 14:52:43.000000 google-cloud-bare-metal-solution-1.4.1/google_cloud_bare_metal_solution.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:52:43.000000 google-cloud-bare-metal-solution-1.4.1/google_cloud_bare_metal_solution.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 14:52:43.199518 google-cloud-bare-metal-solution-1.4.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3022 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:43.199518 google-cloud-bare-metal-solution-1.4.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:43.199518 google-cloud-bare-metal-solution-1.4.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:43.199518 google-cloud-bare-metal-solution-1.4.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:43.199518 google-cloud-bare-metal-solution-1.4.1/tests/unit/gapic/bare_metal_solution_v2/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/tests/unit/gapic/bare_metal_solution_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003   498825 2023-03-27 14:50:47.000000 google-cloud-bare-metal-solution-1.4.1/tests/unit/gapic/bare_metal_solution_v2/test_bare_metal_solution.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:27.480445 google-cloud-bare-metal-solution-1.4.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4732 2023-07-05 15:50:27.480445 google-cloud-bare-metal-solution-1.4.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3787 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:27.472445 google-cloud-bare-metal-solution-1.4.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:27.472445 google-cloud-bare-metal-solution-1.4.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:27.476445 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution/
+-rw-rw-r--   0 root         (0)     1003     3376 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:27.476445 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/
+-rw-rw-r--   0 root         (0)     1003     2999 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7854 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:27.476445 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:27.476445 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/
+-rw-rw-r--   0 root         (0)     1003      781 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/__init__.py
+-rw-rw-r--   0 root         (0)     1003   106375 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/async_client.py
+-rw-rw-r--   0 root         (0)     1003   120820 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/client.py
+-rw-rw-r--   0 root         (0)     1003    25653 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:27.476445 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15537 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    36145 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    36987 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   116864 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:27.480445 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/types/
+-rw-rw-r--   0 root         (0)     1003     2661 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2832 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/types/baremetalsolution.py
+-rw-rw-r--   0 root         (0)     1003    13502 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/types/instance.py
+-rw-rw-r--   0 root         (0)     1003     6204 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/types/lun.py
+-rw-rw-r--   0 root         (0)     1003    14699 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/types/network.py
+-rw-rw-r--   0 root         (0)     1003     7836 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/types/nfs_share.py
+-rw-rw-r--   0 root         (0)     1003    11611 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/types/volume.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:27.480445 google-cloud-bare-metal-solution-1.4.2/google_cloud_bare_metal_solution.egg-info/
+-rw-r--r--   0 root         (0)     1003     4732 2023-07-05 15:50:27.000000 google-cloud-bare-metal-solution-1.4.2/google_cloud_bare_metal_solution.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2154 2023-07-05 15:50:27.000000 google-cloud-bare-metal-solution-1.4.2/google_cloud_bare_metal_solution.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:27.000000 google-cloud-bare-metal-solution-1.4.2/google_cloud_bare_metal_solution.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:50:27.000000 google-cloud-bare-metal-solution-1.4.2/google_cloud_bare_metal_solution.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:27.000000 google-cloud-bare-metal-solution-1.4.2/google_cloud_bare_metal_solution.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:50:27.000000 google-cloud-bare-metal-solution-1.4.2/google_cloud_bare_metal_solution.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:50:27.000000 google-cloud-bare-metal-solution-1.4.2/google_cloud_bare_metal_solution.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:50:27.480445 google-cloud-bare-metal-solution-1.4.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3015 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:27.480445 google-cloud-bare-metal-solution-1.4.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:27.480445 google-cloud-bare-metal-solution-1.4.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:27.480445 google-cloud-bare-metal-solution-1.4.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:27.480445 google-cloud-bare-metal-solution-1.4.2/tests/unit/gapic/bare_metal_solution_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/tests/unit/gapic/bare_metal_solution_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   499820 2023-07-05 15:46:58.000000 google-cloud-bare-metal-solution-1.4.2/tests/unit/gapic/bare_metal_solution_v2/test_bare_metal_solution.py
```

### Comparing `google-cloud-bare-metal-solution-1.4.1/LICENSE` & `google-cloud-bare-metal-solution-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/MANIFEST.in` & `google-cloud-bare-metal-solution-1.4.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/PKG-INFO` & `google-cloud-bare-metal-solution-1.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-bare-metal-solution
-Version: 1.4.1
+Version: 1.4.2
 Summary: Google Cloud Bare Metal Solution API client library
-Home-page: https://github.com/googleapis/python-bare-metal-solution
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
 
-Python Client for Bare Metal Solution API
-=========================================
+Python Client for Bare Metal Solution
+=====================================
 
 |stable| |pypi| |versions|
 
-`Bare Metal Solution API`_: Bring your Oracle workloads to Google Cloud with Bare Metal Solution and jumpstart your cloud journey with minimal risk.
+`Bare Metal Solution`_: Bring your Oracle workloads to Google Cloud with Bare Metal Solution and jumpstart your cloud journey with minimal risk.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-bare-metal-solution.svg
    :target: https://pypi.org/project/google-cloud-bare-metal-solution/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-bare-metal-solution.svg
    :target: https://pypi.org/project/google-cloud-bare-metal-solution/
-.. _Bare Metal Solution API: https://cloud.google.com/bare-metal/docs
+.. _Bare Metal Solution: https://cloud.google.com/bare-metal/docs
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/baremetalsolution/latest
 .. _Product Documentation:  https://cloud.google.com/bare-metal/docs
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Bare Metal Solution API.`_
+3. `Enable the Bare Metal Solution.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Bare Metal Solution API.:  https://cloud.google.com/bare-metal/docs
+.. _Enable the Bare Metal Solution.:  https://cloud.google.com/bare-metal/docs
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-bare-metal-solution
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Bare Metal Solution API
+-  Read the `Client Library Documentation`_ for Bare Metal Solution
    to see other available methods on the client.
--  Read the `Bare Metal Solution API Product documentation`_ to learn
+-  Read the `Bare Metal Solution Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Bare Metal Solution API Product documentation:  https://cloud.google.com/bare-metal/docs
+.. _Bare Metal Solution Product documentation:  https://cloud.google.com/bare-metal/docs
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-bare-metal-solution-1.4.1/README.rst` & `google-cloud-bare-metal-solution-1.4.2/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Bare Metal Solution API
-=========================================
+Python Client for Bare Metal Solution
+=====================================
 
 |stable| |pypi| |versions|
 
-`Bare Metal Solution API`_: Bring your Oracle workloads to Google Cloud with Bare Metal Solution and jumpstart your cloud journey with minimal risk.
+`Bare Metal Solution`_: Bring your Oracle workloads to Google Cloud with Bare Metal Solution and jumpstart your cloud journey with minimal risk.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-bare-metal-solution.svg
    :target: https://pypi.org/project/google-cloud-bare-metal-solution/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-bare-metal-solution.svg
    :target: https://pypi.org/project/google-cloud-bare-metal-solution/
-.. _Bare Metal Solution API: https://cloud.google.com/bare-metal/docs
+.. _Bare Metal Solution: https://cloud.google.com/bare-metal/docs
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/baremetalsolution/latest
 .. _Product Documentation:  https://cloud.google.com/bare-metal/docs
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Bare Metal Solution API.`_
+3. `Enable the Bare Metal Solution.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Bare Metal Solution API.:  https://cloud.google.com/bare-metal/docs
+.. _Enable the Bare Metal Solution.:  https://cloud.google.com/bare-metal/docs
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-bare-metal-solution
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Bare Metal Solution API
+-  Read the `Client Library Documentation`_ for Bare Metal Solution
    to see other available methods on the client.
--  Read the `Bare Metal Solution API Product documentation`_ to learn
+-  Read the `Bare Metal Solution Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Bare Metal Solution API Product documentation:  https://cloud.google.com/bare-metal/docs
+.. _Bare Metal Solution Product documentation:  https://cloud.google.com/bare-metal/docs
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution/__init__.py` & `google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution/gapic_version.py` & `google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.4.1"  # {x-release-please-version}
```

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/__init__.py` & `google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/gapic_metadata.json` & `google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/gapic_version.py` & `google-cloud-bare-metal-solution-1.4.2/tests/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.4.1"  # {x-release-please-version}
```

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/__init__.py` & `google-cloud-bare-metal-solution-1.4.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/__init__.py` & `google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/async_client.py` & `google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2645,15 +2645,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "BareMetalSolutionAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/client.py` & `google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/pagers.py` & `google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/__init__.py` & `google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/base.py` & `google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/grpc.py` & `google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/grpc_asyncio.py` & `google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/rest.py` & `google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/services/bare_metal_solution/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/types/__init__.py` & `google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/types/baremetalsolution.py` & `google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/types/baremetalsolution.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/types/instance.py` & `google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/types/instance.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/types/lun.py` & `google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/types/lun.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/types/network.py` & `google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/types/network.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/types/nfs_share.py` & `google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/types/nfs_share.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/google/cloud/bare_metal_solution_v2/types/volume.py` & `google-cloud-bare-metal-solution-1.4.2/google/cloud/bare_metal_solution_v2/types/volume.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/google_cloud_bare_metal_solution.egg-info/PKG-INFO` & `google-cloud-bare-metal-solution-1.4.2/google_cloud_bare_metal_solution.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-bare-metal-solution
-Version: 1.4.1
+Version: 1.4.2
 Summary: Google Cloud Bare Metal Solution API client library
-Home-page: https://github.com/googleapis/python-bare-metal-solution
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
 
-Python Client for Bare Metal Solution API
-=========================================
+Python Client for Bare Metal Solution
+=====================================
 
 |stable| |pypi| |versions|
 
-`Bare Metal Solution API`_: Bring your Oracle workloads to Google Cloud with Bare Metal Solution and jumpstart your cloud journey with minimal risk.
+`Bare Metal Solution`_: Bring your Oracle workloads to Google Cloud with Bare Metal Solution and jumpstart your cloud journey with minimal risk.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-bare-metal-solution.svg
    :target: https://pypi.org/project/google-cloud-bare-metal-solution/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-bare-metal-solution.svg
    :target: https://pypi.org/project/google-cloud-bare-metal-solution/
-.. _Bare Metal Solution API: https://cloud.google.com/bare-metal/docs
+.. _Bare Metal Solution: https://cloud.google.com/bare-metal/docs
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/baremetalsolution/latest
 .. _Product Documentation:  https://cloud.google.com/bare-metal/docs
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Bare Metal Solution API.`_
+3. `Enable the Bare Metal Solution.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Bare Metal Solution API.:  https://cloud.google.com/bare-metal/docs
+.. _Enable the Bare Metal Solution.:  https://cloud.google.com/bare-metal/docs
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-bare-metal-solution
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Bare Metal Solution API
+-  Read the `Client Library Documentation`_ for Bare Metal Solution
    to see other available methods on the client.
--  Read the `Bare Metal Solution API Product documentation`_ to learn
+-  Read the `Bare Metal Solution Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Bare Metal Solution API Product documentation:  https://cloud.google.com/bare-metal/docs
+.. _Bare Metal Solution Product documentation:  https://cloud.google.com/bare-metal/docs
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-bare-metal-solution-1.4.1/google_cloud_bare_metal_solution.egg-info/SOURCES.txt` & `google-cloud-bare-metal-solution-1.4.2/google_cloud_bare_metal_solution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/setup.py` & `google-cloud-bare-metal-solution-1.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
-url = "https://github.com/googleapis/python-bare-metal-solution"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-bare-metal-solution-1.4.1/tests/__init__.py` & `google-cloud-bare-metal-solution-1.4.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/tests/unit/__init__.py` & `google-cloud-bare-metal-solution-1.4.2/tests/unit/gapic/bare_metal_solution_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bare-metal-solution-1.4.1/tests/unit/gapic/bare_metal_solution_v2/test_bare_metal_solution.py` & `google-cloud-bare-metal-solution-1.4.2/tests/unit/gapic/bare_metal_solution_v2/test_bare_metal_solution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1169,17 +1169,19 @@
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
@@ -3003,17 +3005,19 @@
                     volume.Volume(),
                     volume.Volume(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_volumes(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4177,17 +4181,19 @@
                     network.Network(),
                     network.Network(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_networks(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5601,17 +5607,19 @@
                     lun.Lun(),
                     lun.Lun(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_luns(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -6265,17 +6273,19 @@
                     nfs_share.NfsShare(),
                     nfs_share.NfsShare(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_nfs_shares(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

