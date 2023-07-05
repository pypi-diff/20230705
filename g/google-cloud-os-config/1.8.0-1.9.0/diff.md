# Comparing `tmp/google-cloud-os-config-1.8.0.tar.gz` & `tmp/google-cloud-os-config-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-os-config-1.8.0.tar", last modified: Thu Nov  4 14:35:56 2021, max compression
+gzip compressed data, was "google-cloud-os-config-1.9.0.tar", last modified: Thu Nov 11 22:35:54 2021, max compression
```

## Comparing `google-cloud-os-config-1.8.0.tar` & `google-cloud-os-config-1.9.0.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.832577 google-cloud-os-config-1.8.0/
--rw-rw-r--   0 root         (0)     1003    11358 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     3936 2021-11-04 14:35:56.832577 google-cloud-os-config-1.8.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3013 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.812587 google-cloud-os-config-1.8.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.816585 google-cloud-os-config-1.8.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.816585 google-cloud-os-config-1.8.0/google/cloud/osconfig/
--rw-rw-r--   0 root         (0)     1003     7784 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig/__init__.py
--rw-rw-r--   0 root         (0)     1003       83 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.816585 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/
--rw-rw-r--   0 root         (0)     1003     6058 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     6698 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       83 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.816585 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.820583 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_service/
--rw-rw-r--   0 root         (0)     1003      773 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    36527 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    47056 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_service/client.py
--rw-rw-r--   0 root         (0)     1003    16607 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.820583 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_service/transports/
--rw-rw-r--   0 root         (0)     1003     1203 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9689 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    21304 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    21791 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.820583 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_zonal_service/
--rw-rw-r--   0 root         (0)     1003      793 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_zonal_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    59004 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_zonal_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    72584 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_zonal_service/client.py
--rw-rw-r--   0 root         (0)     1003    28529 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_zonal_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.820583 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_zonal_service/transports/
--rw-rw-r--   0 root         (0)     1003     1256 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_zonal_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12249 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_zonal_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    29098 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_zonal_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    29673 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_zonal_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.824581 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/
--rw-rw-r--   0 root         (0)     1003     4165 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    21752 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/inventory.py
--rw-rw-r--   0 root         (0)     1003    35341 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/os_policy.py
--rw-rw-r--   0 root         (0)     1003    14816 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/os_policy_assignment_reports.py
--rw-rw-r--   0 root         (0)     1003    17373 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/os_policy_assignments.py
--rw-rw-r--   0 root         (0)     1003     1753 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/osconfig_common.py
--rw-rw-r--   0 root         (0)     1003      729 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/osconfig_service.py
--rw-rw-r--   0 root         (0)     1003      729 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/osconfig_zonal_service.py
--rw-rw-r--   0 root         (0)     1003    14282 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/patch_deployments.py
--rw-rw-r--   0 root         (0)     1003    31988 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/patch_jobs.py
--rw-rw-r--   0 root         (0)     1003    14760 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/vulnerability.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.824581 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/
--rw-rw-r--   0 root         (0)     1003     3734 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003     4057 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       83 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.824581 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/services/
--rw-rw-r--   0 root         (0)     1003      600 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.824581 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/
--rw-rw-r--   0 root         (0)     1003      793 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    58790 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    71707 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/client.py
--rw-rw-r--   0 root         (0)     1003    28943 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.824581 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/transports/
--rw-rw-r--   0 root         (0)     1003     1256 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12338 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    29309 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    29906 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.828579 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/types/
--rw-rw-r--   0 root         (0)     1003     2758 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3934 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/types/config_common.py
--rw-rw-r--   0 root         (0)     1003     8534 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/types/instance_os_policies_compliance.py
--rw-rw-r--   0 root         (0)     1003    22005 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/types/inventory.py
--rw-rw-r--   0 root         (0)     1003    34950 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/types/os_policy.py
--rw-rw-r--   0 root         (0)     1003    16412 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/types/os_policy_assignments.py
--rw-rw-r--   0 root         (0)     1003     1758 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/types/osconfig_common.py
--rw-rw-r--   0 root         (0)     1003      734 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/types/osconfig_zonal_service.py
--rw-rw-r--   0 root         (0)     1003    14801 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/types/vulnerability.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.828579 google-cloud-os-config-1.8.0/google_cloud_os_config.egg-info/
--rw-r--r--   0 root         (0)     1003     3936 2021-11-04 14:35:56.000000 google-cloud-os-config-1.8.0/google_cloud_os_config.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     4040 2021-11-04 14:35:56.000000 google-cloud-os-config-1.8.0/google_cloud_os_config.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2021-11-04 14:35:56.000000 google-cloud-os-config-1.8.0/google_cloud_os_config.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2021-11-04 14:35:56.000000 google-cloud-os-config-1.8.0/google_cloud_os_config.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2021-11-04 14:35:56.000000 google-cloud-os-config-1.8.0/google_cloud_os_config.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003       59 2021-11-04 14:35:56.000000 google-cloud-os-config-1.8.0/google_cloud_os_config.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2021-11-04 14:35:56.000000 google-cloud-os-config-1.8.0/google_cloud_os_config.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.828579 google-cloud-os-config-1.8.0/scripts/
--rw-rw-r--   0 root         (0)     1003     6505 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/scripts/fixup_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2021-11-04 14:35:56.832577 google-cloud-os-config-1.8.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3003 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.828579 google-cloud-os-config-1.8.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.828579 google-cloud-os-config-1.8.0/tests/system/
--rw-rw-r--   0 root         (0)     1003     3992 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/tests/system/test_os_config_service_v1.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.828579 google-cloud-os-config-1.8.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.828579 google-cloud-os-config-1.8.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.832577 google-cloud-os-config-1.8.0/tests/unit/gapic/osconfig_v1/
--rw-rw-r--   0 root         (0)     1003      600 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/tests/unit/gapic/osconfig_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   134999 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/tests/unit/gapic/osconfig_v1/test_os_config_service.py
--rw-rw-r--   0 root         (0)     1003   191558 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/tests/unit/gapic/osconfig_v1/test_os_config_zonal_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-11-04 14:35:56.832577 google-cloud-os-config-1.8.0/tests/unit/gapic/osconfig_v1alpha/
--rw-rw-r--   0 root         (0)     1003      600 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/tests/unit/gapic/osconfig_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003   192146 2021-11-04 14:33:25.000000 google-cloud-os-config-1.8.0/tests/unit/gapic/osconfig_v1alpha/test_os_config_zonal_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.185057 google-cloud-os-config-1.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     3936 2021-11-11 22:35:54.185057 google-cloud-os-config-1.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3013 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.165057 google-cloud-os-config-1.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.169057 google-cloud-os-config-1.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.169057 google-cloud-os-config-1.9.0/google/cloud/osconfig/
+-rw-rw-r--   0 root         (0)     1003     7784 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig/__init__.py
+-rw-rw-r--   0 root         (0)     1003       83 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.169057 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/
+-rw-rw-r--   0 root         (0)     1003     6058 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6698 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       83 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.169057 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.173056 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_service/
+-rw-rw-r--   0 root         (0)     1003      773 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    36604 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    47376 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16607 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.173056 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1203 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9625 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    21272 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    21759 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.173056 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_zonal_service/
+-rw-rw-r--   0 root         (0)     1003      793 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_zonal_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    59081 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_zonal_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    72904 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_zonal_service/client.py
+-rw-rw-r--   0 root         (0)     1003    28529 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_zonal_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.173056 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_zonal_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1256 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_zonal_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12169 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_zonal_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    29050 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_zonal_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    29625 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_zonal_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.177056 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/
+-rw-rw-r--   0 root         (0)     1003     4165 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21763 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/inventory.py
+-rw-rw-r--   0 root         (0)     1003    35363 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/os_policy.py
+-rw-rw-r--   0 root         (0)     1003    14817 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/os_policy_assignment_reports.py
+-rw-rw-r--   0 root         (0)     1003    17373 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/os_policy_assignments.py
+-rw-rw-r--   0 root         (0)     1003     1755 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/osconfig_common.py
+-rw-rw-r--   0 root         (0)     1003      729 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/osconfig_service.py
+-rw-rw-r--   0 root         (0)     1003      729 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/osconfig_zonal_service.py
+-rw-rw-r--   0 root         (0)     1003    14288 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/patch_deployments.py
+-rw-rw-r--   0 root         (0)     1003    31990 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/patch_jobs.py
+-rw-rw-r--   0 root         (0)     1003    16942 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/vulnerability.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.177056 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/
+-rw-rw-r--   0 root         (0)     1003     3734 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4057 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       83 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.177056 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/services/
+-rw-rw-r--   0 root         (0)     1003      600 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.177056 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/
+-rw-rw-r--   0 root         (0)     1003      793 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    58867 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    72027 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/client.py
+-rw-rw-r--   0 root         (0)     1003    28943 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.177056 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1256 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12258 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    29261 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    29858 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.181057 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/types/
+-rw-rw-r--   0 root         (0)     1003     2758 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3935 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/types/config_common.py
+-rw-rw-r--   0 root         (0)     1003     8534 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/types/instance_os_policies_compliance.py
+-rw-rw-r--   0 root         (0)     1003    22016 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/types/inventory.py
+-rw-rw-r--   0 root         (0)     1003    34972 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/types/os_policy.py
+-rw-rw-r--   0 root         (0)     1003    16412 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/types/os_policy_assignments.py
+-rw-rw-r--   0 root         (0)     1003     1760 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/types/osconfig_common.py
+-rw-rw-r--   0 root         (0)     1003      734 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/types/osconfig_zonal_service.py
+-rw-rw-r--   0 root         (0)     1003    14801 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/types/vulnerability.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.181057 google-cloud-os-config-1.9.0/google_cloud_os_config.egg-info/
+-rw-r--r--   0 root         (0)     1003     3936 2021-11-11 22:35:54.000000 google-cloud-os-config-1.9.0/google_cloud_os_config.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     4040 2021-11-11 22:35:54.000000 google-cloud-os-config-1.9.0/google_cloud_os_config.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2021-11-11 22:35:54.000000 google-cloud-os-config-1.9.0/google_cloud_os_config.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2021-11-11 22:35:54.000000 google-cloud-os-config-1.9.0/google_cloud_os_config.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2021-11-11 22:35:54.000000 google-cloud-os-config-1.9.0/google_cloud_os_config.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003       59 2021-11-11 22:35:54.000000 google-cloud-os-config-1.9.0/google_cloud_os_config.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2021-11-11 22:35:54.000000 google-cloud-os-config-1.9.0/google_cloud_os_config.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.181057 google-cloud-os-config-1.9.0/scripts/
+-rw-rw-r--   0 root         (0)     1003     6505 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/scripts/fixup_keywords.py
+-rw-rw-r--   0 root         (0)     1003       67 2021-11-11 22:35:54.185057 google-cloud-os-config-1.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3003 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.181057 google-cloud-os-config-1.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.181057 google-cloud-os-config-1.9.0/tests/system/
+-rw-rw-r--   0 root         (0)     1003     3992 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/tests/system/test_os_config_service_v1.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.181057 google-cloud-os-config-1.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.181057 google-cloud-os-config-1.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.185057 google-cloud-os-config-1.9.0/tests/unit/gapic/osconfig_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/tests/unit/gapic/osconfig_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   135783 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/tests/unit/gapic/osconfig_v1/test_os_config_service.py
+-rw-rw-r--   0 root         (0)     1003   192850 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/tests/unit/gapic/osconfig_v1/test_os_config_zonal_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-11-11 22:35:54.185057 google-cloud-os-config-1.9.0/tests/unit/gapic/osconfig_v1alpha/
+-rw-rw-r--   0 root         (0)     1003      600 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/tests/unit/gapic/osconfig_v1alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003   193438 2021-11-11 22:33:20.000000 google-cloud-os-config-1.9.0/tests/unit/gapic/osconfig_v1alpha/test_os_config_zonal_service.py
```

### Comparing `google-cloud-os-config-1.8.0/LICENSE` & `google-cloud-os-config-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/MANIFEST.in` & `google-cloud-os-config-1.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/PKG-INFO` & `google-cloud-os-config-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-os-config
-Version: 1.8.0
+Version: 1.9.0
 Summary: Google Cloud OS Config API client library
 Home-page: https://github.com/googleapis/python-os-config
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-os-config-1.8.0/README.rst` & `google-cloud-os-config-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig/__init__.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/__init__.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/gapic_metadata.json` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/__init__.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_service/__init__.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_service/async_client.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,25 @@
 #
 from collections import OrderedDict
 import functools
 import re
 from typing import Dict, Sequence, Tuple, Type, Union
 import pkg_resources
 
-from google.api_core.client_options import ClientOptions  # type: ignore
-from google.api_core import exceptions as core_exceptions  # type: ignore
-from google.api_core import gapic_v1  # type: ignore
-from google.api_core import retry as retries  # type: ignore
+from google.api_core.client_options import ClientOptions
+from google.api_core import exceptions as core_exceptions
+from google.api_core import gapic_v1
+from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-OptionalRetry = Union[retries.Retry, object]
+try:
+    OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
+except AttributeError:  # pragma: NO COVER
+    OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.cloud.osconfig_v1.services.os_config_service import pagers
 from google.cloud.osconfig_v1.types import patch_deployments
 from google.cloud.osconfig_v1.types import patch_jobs
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from .transports.base import OsConfigServiceTransport, DEFAULT_CLIENT_INFO
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_service/client.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_service/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,31 +10,33 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
-from distutils import util
 import os
 import re
 from typing import Dict, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
-from google.api_core import client_options as client_options_lib  # type: ignore
-from google.api_core import exceptions as core_exceptions  # type: ignore
-from google.api_core import gapic_v1  # type: ignore
-from google.api_core import retry as retries  # type: ignore
+from google.api_core import client_options as client_options_lib
+from google.api_core import exceptions as core_exceptions
+from google.api_core import gapic_v1
+from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-OptionalRetry = Union[retries.Retry, object]
+try:
+    OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
+except AttributeError:  # pragma: NO COVER
+    OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.cloud.osconfig_v1.services.os_config_service import pagers
 from google.cloud.osconfig_v1.types import patch_deployments
 from google.cloud.osconfig_v1.types import patch_jobs
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from .transports.base import OsConfigServiceTransport, DEFAULT_CLIENT_INFO
@@ -315,16 +317,23 @@
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
 
         # Create SSL credentials for mutual TLS if needed.
-        use_client_cert = bool(
-            util.strtobool(os.getenv("GOOGLE_API_USE_CLIENT_CERTIFICATE", "false"))
+        if os.getenv("GOOGLE_API_USE_CLIENT_CERTIFICATE", "false") not in (
+            "true",
+            "false",
+        ):
+            raise ValueError(
+                "Environment variable `GOOGLE_API_USE_CLIENT_CERTIFICATE` must be either `true` or `false`"
+            )
+        use_client_cert = (
+            os.getenv("GOOGLE_API_USE_CLIENT_CERTIFICATE", "false") == "true"
         )
 
         client_cert_source_func = None
         is_mtls = False
         if use_client_cert:
             if client_options.client_cert_source:
                 is_mtls = True
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_service/pagers.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_service/transports/__init__.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_service/transports/base.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_service/transports/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 # limitations under the License.
 #
 import abc
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Union
 import pkg_resources
 
 import google.auth  # type: ignore
-import google.api_core  # type: ignore
-from google.api_core import exceptions as core_exceptions  # type: ignore
-from google.api_core import gapic_v1  # type: ignore
-from google.api_core import retry as retries  # type: ignore
+import google.api_core
+from google.api_core import exceptions as core_exceptions
+from google.api_core import gapic_v1
+from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 from google.cloud.osconfig_v1.types import patch_deployments
 from google.cloud.osconfig_v1.types import patch_jobs
 from google.protobuf import empty_pb2  # type: ignore
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_service/transports/grpc.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import warnings
 from typing import Callable, Dict, Optional, Sequence, Tuple, Union
 
-from google.api_core import grpc_helpers  # type: ignore
-from google.api_core import gapic_v1  # type: ignore
+from google.api_core import grpc_helpers
+from google.api_core import gapic_v1
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
 
 from google.cloud.osconfig_v1.types import patch_deployments
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_service/transports/grpc_asyncio.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_service/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import warnings
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
 
-from google.api_core import gapic_v1  # type: ignore
-from google.api_core import grpc_helpers_async  # type: ignore
+from google.api_core import gapic_v1
+from google.api_core import grpc_helpers_async
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.cloud.osconfig_v1.types import patch_deployments
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_zonal_service/__init__.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_zonal_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_zonal_service/async_client.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_zonal_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,25 @@
 #
 from collections import OrderedDict
 import functools
 import re
 from typing import Dict, Sequence, Tuple, Type, Union
 import pkg_resources
 
-from google.api_core.client_options import ClientOptions  # type: ignore
-from google.api_core import exceptions as core_exceptions  # type: ignore
-from google.api_core import gapic_v1  # type: ignore
-from google.api_core import retry as retries  # type: ignore
+from google.api_core.client_options import ClientOptions
+from google.api_core import exceptions as core_exceptions
+from google.api_core import gapic_v1
+from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-OptionalRetry = Union[retries.Retry, object]
+try:
+    OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
+except AttributeError:  # pragma: NO COVER
+    OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 from google.cloud.osconfig_v1.services.os_config_zonal_service import pagers
 from google.cloud.osconfig_v1.types import inventory
 from google.cloud.osconfig_v1.types import os_policy
 from google.cloud.osconfig_v1.types import os_policy_assignment_reports
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_zonal_service/client.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_zonal_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,31 +10,33 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
-from distutils import util
 import os
 import re
 from typing import Dict, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
-from google.api_core import client_options as client_options_lib  # type: ignore
-from google.api_core import exceptions as core_exceptions  # type: ignore
-from google.api_core import gapic_v1  # type: ignore
-from google.api_core import retry as retries  # type: ignore
+from google.api_core import client_options as client_options_lib
+from google.api_core import exceptions as core_exceptions
+from google.api_core import gapic_v1
+from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-OptionalRetry = Union[retries.Retry, object]
+try:
+    OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
+except AttributeError:  # pragma: NO COVER
+    OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 from google.cloud.osconfig_v1.services.os_config_zonal_service import pagers
 from google.cloud.osconfig_v1.types import inventory
 from google.cloud.osconfig_v1.types import os_policy
 from google.cloud.osconfig_v1.types import os_policy_assignment_reports
@@ -388,16 +390,23 @@
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
 
         # Create SSL credentials for mutual TLS if needed.
-        use_client_cert = bool(
-            util.strtobool(os.getenv("GOOGLE_API_USE_CLIENT_CERTIFICATE", "false"))
+        if os.getenv("GOOGLE_API_USE_CLIENT_CERTIFICATE", "false") not in (
+            "true",
+            "false",
+        ):
+            raise ValueError(
+                "Environment variable `GOOGLE_API_USE_CLIENT_CERTIFICATE` must be either `true` or `false`"
+            )
+        use_client_cert = (
+            os.getenv("GOOGLE_API_USE_CLIENT_CERTIFICATE", "false") == "true"
         )
 
         client_cert_source_func = None
         is_mtls = False
         if use_client_cert:
             if client_options.client_cert_source:
                 is_mtls = True
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_zonal_service/pagers.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_zonal_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_zonal_service/transports/__init__.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_zonal_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_zonal_service/transports/base.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_zonal_service/transports/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 # limitations under the License.
 #
 import abc
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Union
 import pkg_resources
 
 import google.auth  # type: ignore
-import google.api_core  # type: ignore
-from google.api_core import exceptions as core_exceptions  # type: ignore
-from google.api_core import gapic_v1  # type: ignore
-from google.api_core import retry as retries  # type: ignore
-from google.api_core import operations_v1  # type: ignore
+import google.api_core
+from google.api_core import exceptions as core_exceptions
+from google.api_core import gapic_v1
+from google.api_core import retry as retries
+from google.api_core import operations_v1
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 from google.cloud.osconfig_v1.types import inventory
 from google.cloud.osconfig_v1.types import os_policy_assignment_reports
 from google.cloud.osconfig_v1.types import os_policy_assignments
 from google.cloud.osconfig_v1.types import vulnerability
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_zonal_service/transports/grpc.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_zonal_service/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import warnings
 from typing import Callable, Dict, Optional, Sequence, Tuple, Union
 
-from google.api_core import grpc_helpers  # type: ignore
-from google.api_core import operations_v1  # type: ignore
-from google.api_core import gapic_v1  # type: ignore
+from google.api_core import grpc_helpers
+from google.api_core import operations_v1
+from google.api_core import gapic_v1
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
 
 from google.cloud.osconfig_v1.types import inventory
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/services/os_config_zonal_service/transports/grpc_asyncio.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/services/os_config_zonal_service/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import warnings
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
 
-from google.api_core import gapic_v1  # type: ignore
-from google.api_core import grpc_helpers_async  # type: ignore
-from google.api_core import operations_v1  # type: ignore
+from google.api_core import gapic_v1
+from google.api_core import grpc_helpers_async
+from google.api_core import operations_v1
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.cloud.osconfig_v1.types import inventory
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/__init__.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/inventory.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/inventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,18 +126,20 @@
             update_time (google.protobuf.timestamp_pb2.Timestamp):
                 When this inventory item was last modified.
             type_ (google.cloud.osconfig_v1.types.Inventory.Item.Type):
                 The specific type of inventory, correlating
                 to its specific details.
             installed_package (google.cloud.osconfig_v1.types.Inventory.SoftwarePackage):
                 Software package present on the VM instance.
+
                 This field is a member of `oneof`_ ``details``.
             available_package (google.cloud.osconfig_v1.types.Inventory.SoftwarePackage):
                 Software package available to be installed on
                 the VM instance.
+
                 This field is a member of `oneof`_ ``details``.
         """
 
         class OriginType(proto.Enum):
             r"""The origin of a specific inventory item."""
             ORIGIN_TYPE_UNSPECIFIED = 0
             INVENTORY_REPORT = 1
@@ -183,52 +185,61 @@
         .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
         Attributes:
             yum_package (google.cloud.osconfig_v1.types.Inventory.VersionedPackage):
                 Yum package info. For details about the yum package manager,
                 see
                 https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/6/html/deployment_guide/ch-yum.
+
                 This field is a member of `oneof`_ ``details``.
             apt_package (google.cloud.osconfig_v1.types.Inventory.VersionedPackage):
                 Details of an APT package.
                 For details about the apt package manager, see
                 https://wiki.debian.org/Apt.
+
                 This field is a member of `oneof`_ ``details``.
             zypper_package (google.cloud.osconfig_v1.types.Inventory.VersionedPackage):
                 Details of a Zypper package. For details about the Zypper
                 package manager, see
                 https://en.opensuse.org/SDB:Zypper_manual.
+
                 This field is a member of `oneof`_ ``details``.
             googet_package (google.cloud.osconfig_v1.types.Inventory.VersionedPackage):
                 Details of a Googet package.
                 For details about the googet package manager,
                 see  https://github.com/google/googet.
+
                 This field is a member of `oneof`_ ``details``.
             zypper_patch (google.cloud.osconfig_v1.types.Inventory.ZypperPatch):
                 Details of a Zypper patch. For details about the Zypper
                 package manager, see
                 https://en.opensuse.org/SDB:Zypper_manual.
+
                 This field is a member of `oneof`_ ``details``.
             wua_package (google.cloud.osconfig_v1.types.Inventory.WindowsUpdatePackage):
                 Details of a Windows Update package. See
                 https://docs.microsoft.com/en-us/windows/win32/api/_wua/ for
                 information about Windows Update.
+
                 This field is a member of `oneof`_ ``details``.
             qfe_package (google.cloud.osconfig_v1.types.Inventory.WindowsQuickFixEngineeringPackage):
                 Details of a Windows Quick Fix engineering
                 package. See
                 https://docs.microsoft.com/en-
                 us/windows/win32/cimwin32prov/win32-quickfixengineering
                 for info in Windows Quick Fix Engineering.
+
                 This field is a member of `oneof`_ ``details``.
             cos_package (google.cloud.osconfig_v1.types.Inventory.VersionedPackage):
                 Details of a COS package.
+
                 This field is a member of `oneof`_ ``details``.
             windows_application (google.cloud.osconfig_v1.types.Inventory.WindowsApplication):
                 Details of Windows Application.
+
                 This field is a member of `oneof`_ ``details``.
         """
 
         yum_package = proto.Field(
             proto.MESSAGE,
             number=1,
             oneof="details",
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/os_policy.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/os_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,23 +109,27 @@
                    hyphens.
                 -  Must start with a letter.
                 -  Must be between 1-63 characters.
                 -  Must end with a number or a letter.
                 -  Must be unique within the OS policy.
             pkg (google.cloud.osconfig_v1.types.OSPolicy.Resource.PackageResource):
                 Package resource
+
                 This field is a member of `oneof`_ ``resource_type``.
             repository (google.cloud.osconfig_v1.types.OSPolicy.Resource.RepositoryResource):
                 Package repository resource
+
                 This field is a member of `oneof`_ ``resource_type``.
             exec_ (google.cloud.osconfig_v1.types.OSPolicy.Resource.ExecResource):
                 Exec resource
+
                 This field is a member of `oneof`_ ``resource_type``.
             file (google.cloud.osconfig_v1.types.OSPolicy.Resource.FileResource):
                 File resource
+
                 This field is a member of `oneof`_ ``resource_type``.
         """
 
         class File(proto.Message):
             r"""A remote or local file.
 
             This message has `oneof`_ fields (mutually exclusive fields).
@@ -134,20 +138,23 @@
             members.
 
             .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
             Attributes:
                 remote (google.cloud.osconfig_v1.types.OSPolicy.Resource.File.Remote):
                     A generic remote file.
+
                     This field is a member of `oneof`_ ``type``.
                 gcs (google.cloud.osconfig_v1.types.OSPolicy.Resource.File.Gcs):
                     A Cloud Storage object.
+
                     This field is a member of `oneof`_ ``type``.
                 local_path (str):
                     A local path within the VM to use.
+
                     This field is a member of `oneof`_ ``type``.
                 allow_insecure (bool):
                     Defaults to false. When false, files are
                     subject to validations based on the file type:
                     Remote: A checksum must be specified.
                     Cloud Storage: An object generation number must
                     be specified.
@@ -212,32 +219,39 @@
 
             Attributes:
                 desired_state (google.cloud.osconfig_v1.types.OSPolicy.Resource.PackageResource.DesiredState):
                     Required. The desired state the agent should
                     maintain for this package.
                 apt (google.cloud.osconfig_v1.types.OSPolicy.Resource.PackageResource.APT):
                     A package managed by Apt.
+
                     This field is a member of `oneof`_ ``system_package``.
                 deb (google.cloud.osconfig_v1.types.OSPolicy.Resource.PackageResource.Deb):
                     A deb package file.
+
                     This field is a member of `oneof`_ ``system_package``.
                 yum (google.cloud.osconfig_v1.types.OSPolicy.Resource.PackageResource.YUM):
                     A package managed by YUM.
+
                     This field is a member of `oneof`_ ``system_package``.
                 zypper (google.cloud.osconfig_v1.types.OSPolicy.Resource.PackageResource.Zypper):
                     A package managed by Zypper.
+
                     This field is a member of `oneof`_ ``system_package``.
                 rpm (google.cloud.osconfig_v1.types.OSPolicy.Resource.PackageResource.RPM):
                     An rpm package file.
+
                     This field is a member of `oneof`_ ``system_package``.
                 googet (google.cloud.osconfig_v1.types.OSPolicy.Resource.PackageResource.GooGet):
                     A package managed by GooGet.
+
                     This field is a member of `oneof`_ ``system_package``.
                 msi (google.cloud.osconfig_v1.types.OSPolicy.Resource.PackageResource.MSI):
                     An MSI package.
+
                     This field is a member of `oneof`_ ``system_package``.
             """
 
             class DesiredState(proto.Enum):
                 r"""The desired state that the OS Config agent maintains on the
                 VM.
                 """
@@ -412,23 +426,27 @@
             members.
 
             .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
             Attributes:
                 apt (google.cloud.osconfig_v1.types.OSPolicy.Resource.RepositoryResource.AptRepository):
                     An Apt Repository.
+
                     This field is a member of `oneof`_ ``repository``.
                 yum (google.cloud.osconfig_v1.types.OSPolicy.Resource.RepositoryResource.YumRepository):
                     A Yum Repository.
+
                     This field is a member of `oneof`_ ``repository``.
                 zypper (google.cloud.osconfig_v1.types.OSPolicy.Resource.RepositoryResource.ZypperRepository):
                     A Zypper Repository.
+
                     This field is a member of `oneof`_ ``repository``.
                 goo (google.cloud.osconfig_v1.types.OSPolicy.Resource.RepositoryResource.GooRepository):
                     A Goo Repository.
+
                     This field is a member of `oneof`_ ``repository``.
             """
 
             class AptRepository(proto.Message):
                 r"""Represents a single apt package repository. These will be added to a
                 repo file that will be managed at
                 ``/etc/apt/sources.list.d/google_osconfig.list``.
@@ -611,19 +629,21 @@
                 members.
 
                 .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
                 Attributes:
                     file (google.cloud.osconfig_v1.types.OSPolicy.Resource.File):
                         A remote or local file.
+
                         This field is a member of `oneof`_ ``source``.
                     script (str):
                         An inline script.
                         The size of the script is limited to 1024
                         characters.
+
                         This field is a member of `oneof`_ ``source``.
                     args (Sequence[str]):
                         Optional arguments to pass to the source
                         during execution.
                     interpreter (google.cloud.osconfig_v1.types.OSPolicy.Resource.ExecResource.Exec.Interpreter):
                         Required. The script interpreter to use.
                     output_file_path (str):
@@ -674,19 +694,21 @@
             members.
 
             .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
             Attributes:
                 file (google.cloud.osconfig_v1.types.OSPolicy.Resource.File):
                     A remote or local source.
+
                     This field is a member of `oneof`_ ``source``.
                 content (str):
                     A a file with this content.
                     The size of the content is limited to 1024
                     characters.
+
                     This field is a member of `oneof`_ ``source``.
                 path (str):
                     Required. The absolute path of the file
                     within the VM.
                 state (google.cloud.osconfig_v1.types.OSPolicy.Resource.FileResource.DesiredState):
                     Required. Desired state of the file.
                 permissions (str):
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/os_policy_assignment_reports.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/os_policy_assignment_reports.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,14 +231,15 @@
                        skipped by the agent because errors were encountered
                        while executing prior resources in the OS policy.
                     -  ``os-policy-execution-attempt-failed``: The execution of
                        the OS policy containing this resource failed and the
                        compliance state couldn't be determined.
                 exec_resource_output (google.cloud.osconfig_v1.types.OSPolicyAssignmentReport.OSPolicyCompliance.OSPolicyResourceCompliance.ExecResourceOutput):
                     ExecResource specific output.
+
                     This field is a member of `oneof`_ ``output``.
             """
 
             class ComplianceState(proto.Enum):
                 r"""Possible compliance states for a resource."""
                 UNKNOWN = 0
                 COMPLIANT = 1
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/os_policy_assignments.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/os_policy_assignments.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/osconfig_common.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/osconfig_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,21 @@
     members.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         fixed (int):
             Specifies a fixed value.
+
             This field is a member of `oneof`_ ``mode``.
         percent (int):
             Specifies the relative value defined as a
             percentage, which will be multiplied by a
             reference value.
+
             This field is a member of `oneof`_ ``mode``.
     """
 
     fixed = proto.Field(proto.INT32, number=1, oneof="mode",)
     percent = proto.Field(proto.INT32, number=2, oneof="mode",)
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/osconfig_service.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/osconfig_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/osconfig_zonal_service.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/osconfig_zonal_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/patch_deployments.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/patch_deployments.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,17 +72,19 @@
             Optional. Patch configuration that is
             applied.
         duration (google.protobuf.duration_pb2.Duration):
             Optional. Duration of the patch. After the
             duration ends, the patch times out.
         one_time_schedule (google.cloud.osconfig_v1.types.OneTimeSchedule):
             Required. Schedule a one-time execution.
+
             This field is a member of `oneof`_ ``schedule``.
         recurring_schedule (google.cloud.osconfig_v1.types.RecurringSchedule):
             Required. Schedule recurring executions.
+
             This field is a member of `oneof`_ ``schedule``.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Time the patch deployment was created.
             Timestamp is in
             `RFC3339 <https://www.ietf.org/rfc/rfc3339.txt>`__ text
             format.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
@@ -161,17 +163,19 @@
             Required. Time of the day to run a recurring
             deployment.
         frequency (google.cloud.osconfig_v1.types.RecurringSchedule.Frequency):
             Required. The frequency unit of this
             recurring schedule.
         weekly (google.cloud.osconfig_v1.types.WeeklySchedule):
             Required. Schedule with weekly executions.
+
             This field is a member of `oneof`_ ``schedule_config``.
         monthly (google.cloud.osconfig_v1.types.MonthlySchedule):
             Required. Schedule with monthly executions.
+
             This field is a member of `oneof`_ ``schedule_config``.
         last_execute_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The time the last patch job ran
             successfully.
         next_execute_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The time the next patch job is
             scheduled to run.
@@ -225,22 +229,24 @@
     members.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         week_day_of_month (google.cloud.osconfig_v1.types.WeekDayOfMonth):
             Required. Week day in a month.
+
             This field is a member of `oneof`_ ``day_of_month``.
         month_day (int):
             Required. One day of the month. 1-31
             indicates the 1st to the 31st day. -1 indicates
             the last day of the month. Months without the
             target day will be skipped. For example, a
             schedule to run "every month on the 31st" will
             not run in February, April, June, etc.
+
             This field is a member of `oneof`_ ``day_of_month``.
     """
 
     week_day_of_month = proto.Field(
         proto.MESSAGE, number=1, oneof="day_of_month", message="WeekDayOfMonth",
     )
     month_day = proto.Field(proto.INT32, number=2, oneof="day_of_month",)
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/patch_jobs.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/patch_jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -629,18 +629,20 @@
     members.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         local_path (str):
             An absolute path to the executable on the VM.
+
             This field is a member of `oneof`_ ``executable``.
         gcs_object (google.cloud.osconfig_v1.types.GcsObject):
             A Cloud Storage object containing the
             executable.
+
             This field is a member of `oneof`_ ``executable``.
         allowed_success_codes (Sequence[int]):
             Defaults to [0]. A list of possible return values that the
             execution can return to indicate a success.
         interpreter (google.cloud.osconfig_v1.types.ExecStepConfig.Interpreter):
             The script interpreter to use to run the script. If no
             interpreter is specified the script will be executed
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1/types/vulnerability.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/types/vulnerability.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #
 import proto  # type: ignore
 
 from google.protobuf import timestamp_pb2  # type: ignore
 
 
 __protobuf__ = proto.module(
-    package="google.cloud.osconfig.v1",
+    package="google.cloud.osconfig.v1alpha",
     manifest={
         "VulnerabilityReport",
         "GetVulnerabilityReportRequest",
         "ListVulnerabilityReportsRequest",
         "ListVulnerabilityReportsResponse",
         "CVSSv3",
     },
@@ -40,27 +40,27 @@
 
     Attributes:
         name (str):
             Output only. The ``vulnerabilityReport`` API resource name.
 
             Format:
             ``projects/{project_number}/locations/{location}/instances/{instance_id}/vulnerabilityReport``
-        vulnerabilities (Sequence[google.cloud.osconfig_v1.types.VulnerabilityReport.Vulnerability]):
+        vulnerabilities (Sequence[google.cloud.osconfig_v1alpha.types.VulnerabilityReport.Vulnerability]):
             Output only. List of vulnerabilities
             affecting the VM.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp for when the last
             vulnerability report was generated for the VM.
     """
 
     class Vulnerability(proto.Message):
         r"""A vulnerability affecting the VM instance.
 
         Attributes:
-            details (google.cloud.osconfig_v1.types.VulnerabilityReport.Vulnerability.Details):
+            details (google.cloud.osconfig_v1alpha.types.VulnerabilityReport.Vulnerability.Details):
                 Contains metadata as per the upstream feed of
                 the operating system and NVD.
             installed_inventory_item_ids (Sequence[str]):
                 Corresponds to the ``INSTALLED_PACKAGE`` inventory item on
                 the VM. This field displays the inventory items affected by
                 this vulnerability. If the vulnerability report was not
                 updated after the VM inventory update, these values might
@@ -94,40 +94,37 @@
                     classification> should be unique across
                     vulnerabilities for a VM.
                 cvss_v2_score (float):
                     The CVSS V2 score of this vulnerability. CVSS
                     V2 score is on a scale of 0 - 10 where 0
                     indicates low severity and 10 indicates high
                     severity.
-                cvss_v3 (google.cloud.osconfig_v1.types.CVSSv3):
+                cvss_v3 (google.cloud.osconfig_v1alpha.types.CVSSv3):
                     The full description of the CVSSv3 for this
                     vulnerability from NVD.
                 severity (str):
                     Assigned severity/impact ranking from the
                     distro.
                 description (str):
                     The note or description describing the
                     vulnerability from the distro.
-                references (Sequence[google.cloud.osconfig_v1.types.VulnerabilityReport.Vulnerability.Details.Reference]):
+                references (Sequence[google.cloud.osconfig_v1alpha.types.VulnerabilityReport.Vulnerability.Details.Reference]):
                     Corresponds to the references attached to the
                     ``VulnerabilityDetails``.
             """
 
             class Reference(proto.Message):
                 r"""A reference for this vulnerability.
 
                 Attributes:
                     url (str):
                         The url of the reference.
-                    source (str):
-                        The source of the reference e.g. NVD.
                 """
 
                 url = proto.Field(proto.STRING, number=1,)
-                source = proto.Field(proto.STRING, number=2,)
 
             cve = proto.Field(proto.STRING, number=1,)
             cvss_v2_score = proto.Field(proto.FLOAT, number=2,)
             cvss_v3 = proto.Field(proto.MESSAGE, number=3, message="CVSSv3",)
             severity = proto.Field(proto.STRING, number=4,)
             description = proto.Field(proto.STRING, number=5,)
             references = proto.RepeatedField(
@@ -182,18 +179,20 @@
     VM instances in the specified location.
 
     Attributes:
         parent (str):
             Required. The parent resource name.
 
             Format:
-            ``projects/{project}/locations/{location}/instances/-``
+            ``projects/{project}/locations/{location}/instances/{instance}``
 
             For ``{project}``, either ``project-number`` or
-            ``project-id`` can be provided.
+            ``project-id`` can be provided. For ``{instance}``, only
+            ``-`` character is supported to list vulnerability reports
+            across VMs.
         page_size (int):
             The maximum number of results to return.
         page_token (str):
             A pagination token returned from a previous call to
             ``ListVulnerabilityReports`` that indicates where this
             listing should continue from.
         filter (str):
@@ -209,15 +208,15 @@
 
 
 class ListVulnerabilityReportsResponse(proto.Message):
     r"""A response message for listing vulnerability reports for all
     VM instances in the specified location.
 
     Attributes:
-        vulnerability_reports (Sequence[google.cloud.osconfig_v1.types.VulnerabilityReport]):
+        vulnerability_reports (Sequence[google.cloud.osconfig_v1alpha.types.VulnerabilityReport]):
             List of vulnerabilityReport objects.
         next_page_token (str):
             The pagination token to retrieve the next
             page of vulnerabilityReports object.
     """
 
     @property
@@ -245,44 +244,44 @@
             The Exploitability sub-score equation is
             derived from the Base Exploitability metrics.
             https://www.first.org/cvss/specification-
             document#2-1-Exploitability-Metrics
         impact_score (float):
             The Impact sub-score equation is derived from
             the Base Impact metrics.
-        attack_vector (google.cloud.osconfig_v1.types.CVSSv3.AttackVector):
+        attack_vector (google.cloud.osconfig_v1alpha.types.CVSSv3.AttackVector):
             This metric reflects the context by which
             vulnerability exploitation is possible.
-        attack_complexity (google.cloud.osconfig_v1.types.CVSSv3.AttackComplexity):
+        attack_complexity (google.cloud.osconfig_v1alpha.types.CVSSv3.AttackComplexity):
             This metric describes the conditions beyond
             the attacker's control that must exist in order
             to exploit the vulnerability.
-        privileges_required (google.cloud.osconfig_v1.types.CVSSv3.PrivilegesRequired):
+        privileges_required (google.cloud.osconfig_v1alpha.types.CVSSv3.PrivilegesRequired):
             This metric describes the level of privileges
             an attacker must possess before successfully
             exploiting the vulnerability.
-        user_interaction (google.cloud.osconfig_v1.types.CVSSv3.UserInteraction):
+        user_interaction (google.cloud.osconfig_v1alpha.types.CVSSv3.UserInteraction):
             This metric captures the requirement for a
             human user, other than the attacker, to
             participate in the successful compromise of the
             vulnerable component.
-        scope (google.cloud.osconfig_v1.types.CVSSv3.Scope):
+        scope (google.cloud.osconfig_v1alpha.types.CVSSv3.Scope):
             The Scope metric captures whether a
             vulnerability in one vulnerable component
             impacts resources in components beyond its
             security scope.
-        confidentiality_impact (google.cloud.osconfig_v1.types.CVSSv3.Impact):
+        confidentiality_impact (google.cloud.osconfig_v1alpha.types.CVSSv3.Impact):
             This metric measures the impact to the
             confidentiality of the information resources
             managed by a software component due to a
             successfully exploited vulnerability.
-        integrity_impact (google.cloud.osconfig_v1.types.CVSSv3.Impact):
+        integrity_impact (google.cloud.osconfig_v1alpha.types.CVSSv3.Impact):
             This metric measures the impact to integrity
             of a successfully exploited vulnerability.
-        availability_impact (google.cloud.osconfig_v1.types.CVSSv3.Impact):
+        availability_impact (google.cloud.osconfig_v1alpha.types.CVSSv3.Impact):
             This metric measures the impact to the
             availability of the impacted component resulting
             from a successfully exploited vulnerability.
     """
 
     class AttackVector(proto.Enum):
         r"""This metric reflects the context by which vulnerability
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/__init__.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/gapic_metadata.json` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/services/__init__.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/__init__.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/async_client.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,25 @@
 #
 from collections import OrderedDict
 import functools
 import re
 from typing import Dict, Sequence, Tuple, Type, Union
 import pkg_resources
 
-from google.api_core.client_options import ClientOptions  # type: ignore
-from google.api_core import exceptions as core_exceptions  # type: ignore
-from google.api_core import gapic_v1  # type: ignore
-from google.api_core import retry as retries  # type: ignore
+from google.api_core.client_options import ClientOptions
+from google.api_core import exceptions as core_exceptions
+from google.api_core import gapic_v1
+from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-OptionalRetry = Union[retries.Retry, object]
+try:
+    OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
+except AttributeError:  # pragma: NO COVER
+    OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 from google.cloud.osconfig_v1alpha.services.os_config_zonal_service import pagers
 from google.cloud.osconfig_v1alpha.types import config_common
 from google.cloud.osconfig_v1alpha.types import instance_os_policies_compliance
 from google.cloud.osconfig_v1alpha.types import inventory
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/client.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,31 +10,33 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
-from distutils import util
 import os
 import re
 from typing import Dict, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
-from google.api_core import client_options as client_options_lib  # type: ignore
-from google.api_core import exceptions as core_exceptions  # type: ignore
-from google.api_core import gapic_v1  # type: ignore
-from google.api_core import retry as retries  # type: ignore
+from google.api_core import client_options as client_options_lib
+from google.api_core import exceptions as core_exceptions
+from google.api_core import gapic_v1
+from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-OptionalRetry = Union[retries.Retry, object]
+try:
+    OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
+except AttributeError:  # pragma: NO COVER
+    OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 from google.cloud.osconfig_v1alpha.services.os_config_zonal_service import pagers
 from google.cloud.osconfig_v1alpha.types import config_common
 from google.cloud.osconfig_v1alpha.types import instance_os_policies_compliance
 from google.cloud.osconfig_v1alpha.types import inventory
@@ -365,16 +367,23 @@
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
 
         # Create SSL credentials for mutual TLS if needed.
-        use_client_cert = bool(
-            util.strtobool(os.getenv("GOOGLE_API_USE_CLIENT_CERTIFICATE", "false"))
+        if os.getenv("GOOGLE_API_USE_CLIENT_CERTIFICATE", "false") not in (
+            "true",
+            "false",
+        ):
+            raise ValueError(
+                "Environment variable `GOOGLE_API_USE_CLIENT_CERTIFICATE` must be either `true` or `false`"
+            )
+        use_client_cert = (
+            os.getenv("GOOGLE_API_USE_CLIENT_CERTIFICATE", "false") == "true"
         )
 
         client_cert_source_func = None
         is_mtls = False
         if use_client_cert:
             if client_options.client_cert_source:
                 is_mtls = True
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/pagers.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/transports/__init__.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/transports/base.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/transports/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 # limitations under the License.
 #
 import abc
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Union
 import pkg_resources
 
 import google.auth  # type: ignore
-import google.api_core  # type: ignore
-from google.api_core import exceptions as core_exceptions  # type: ignore
-from google.api_core import gapic_v1  # type: ignore
-from google.api_core import retry as retries  # type: ignore
-from google.api_core import operations_v1  # type: ignore
+import google.api_core
+from google.api_core import exceptions as core_exceptions
+from google.api_core import gapic_v1
+from google.api_core import retry as retries
+from google.api_core import operations_v1
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 from google.cloud.osconfig_v1alpha.types import instance_os_policies_compliance
 from google.cloud.osconfig_v1alpha.types import inventory
 from google.cloud.osconfig_v1alpha.types import os_policy_assignments
 from google.cloud.osconfig_v1alpha.types import vulnerability
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/transports/grpc.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import warnings
 from typing import Callable, Dict, Optional, Sequence, Tuple, Union
 
-from google.api_core import grpc_helpers  # type: ignore
-from google.api_core import operations_v1  # type: ignore
-from google.api_core import gapic_v1  # type: ignore
+from google.api_core import grpc_helpers
+from google.api_core import operations_v1
+from google.api_core import gapic_v1
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
 
 from google.cloud.osconfig_v1alpha.types import instance_os_policies_compliance
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/transports/grpc_asyncio.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/services/os_config_zonal_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import warnings
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
 
-from google.api_core import gapic_v1  # type: ignore
-from google.api_core import grpc_helpers_async  # type: ignore
-from google.api_core import operations_v1  # type: ignore
+from google.api_core import gapic_v1
+from google.api_core import grpc_helpers_async
+from google.api_core import operations_v1
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.cloud.osconfig_v1alpha.types import instance_os_policies_compliance
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/types/__init__.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/types/config_common.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/types/config_common.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,14 +80,15 @@
         config_steps (Sequence[google.cloud.osconfig_v1alpha.types.OSPolicyResourceConfigStep]):
             Ordered list of configuration steps taken by
             the agent for the OS policy resource.
         state (google.cloud.osconfig_v1alpha.types.OSPolicyComplianceState):
             Compliance state of the OS policy resource.
         exec_resource_output (google.cloud.osconfig_v1alpha.types.OSPolicyResourceCompliance.ExecResourceOutput):
             ExecResource specific output.
+
             This field is a member of `oneof`_ ``output``.
     """
 
     class ExecResourceOutput(proto.Message):
         r"""ExecResource specific output.
 
         Attributes:
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/types/instance_os_policies_compliance.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/types/instance_os_policies_compliance.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/types/inventory.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/types/inventory.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,18 +126,20 @@
             update_time (google.protobuf.timestamp_pb2.Timestamp):
                 When this inventory item was last modified.
             type_ (google.cloud.osconfig_v1alpha.types.Inventory.Item.Type):
                 The specific type of inventory, correlating
                 to its specific details.
             installed_package (google.cloud.osconfig_v1alpha.types.Inventory.SoftwarePackage):
                 Software package present on the VM instance.
+
                 This field is a member of `oneof`_ ``details``.
             available_package (google.cloud.osconfig_v1alpha.types.Inventory.SoftwarePackage):
                 Software package available to be installed on
                 the VM instance.
+
                 This field is a member of `oneof`_ ``details``.
         """
 
         class OriginType(proto.Enum):
             r"""The origin of a specific inventory item."""
             ORIGIN_TYPE_UNSPECIFIED = 0
             INVENTORY_REPORT = 1
@@ -183,52 +185,61 @@
         .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
         Attributes:
             yum_package (google.cloud.osconfig_v1alpha.types.Inventory.VersionedPackage):
                 Yum package info. For details about the yum package manager,
                 see
                 https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/6/html/deployment_guide/ch-yum.
+
                 This field is a member of `oneof`_ ``details``.
             apt_package (google.cloud.osconfig_v1alpha.types.Inventory.VersionedPackage):
                 Details of an APT package.
                 For details about the apt package manager, see
                 https://wiki.debian.org/Apt.
+
                 This field is a member of `oneof`_ ``details``.
             zypper_package (google.cloud.osconfig_v1alpha.types.Inventory.VersionedPackage):
                 Details of a Zypper package. For details about the Zypper
                 package manager, see
                 https://en.opensuse.org/SDB:Zypper_manual.
+
                 This field is a member of `oneof`_ ``details``.
             googet_package (google.cloud.osconfig_v1alpha.types.Inventory.VersionedPackage):
                 Details of a Googet package.
                 For details about the googet package manager,
                 see  https://github.com/google/googet.
+
                 This field is a member of `oneof`_ ``details``.
             zypper_patch (google.cloud.osconfig_v1alpha.types.Inventory.ZypperPatch):
                 Details of a Zypper patch. For details about the Zypper
                 package manager, see
                 https://en.opensuse.org/SDB:Zypper_manual.
+
                 This field is a member of `oneof`_ ``details``.
             wua_package (google.cloud.osconfig_v1alpha.types.Inventory.WindowsUpdatePackage):
                 Details of a Windows Update package. See
                 https://docs.microsoft.com/en-us/windows/win32/api/_wua/ for
                 information about Windows Update.
+
                 This field is a member of `oneof`_ ``details``.
             qfe_package (google.cloud.osconfig_v1alpha.types.Inventory.WindowsQuickFixEngineeringPackage):
                 Details of a Windows Quick Fix engineering
                 package. See
                 https://docs.microsoft.com/en-
                 us/windows/win32/cimwin32prov/win32-quickfixengineering
                 for info in Windows Quick Fix Engineering.
+
                 This field is a member of `oneof`_ ``details``.
             cos_package (google.cloud.osconfig_v1alpha.types.Inventory.VersionedPackage):
                 Details of a COS package.
+
                 This field is a member of `oneof`_ ``details``.
             windows_application (google.cloud.osconfig_v1alpha.types.Inventory.WindowsApplication):
                 Details of Windows Application.
+
                 This field is a member of `oneof`_ ``details``.
         """
 
         yum_package = proto.Field(
             proto.MESSAGE,
             number=1,
             oneof="details",
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/types/os_policy.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/types/os_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,23 +111,27 @@
                    hyphens.
                 -  Must start with a letter.
                 -  Must be between 1-63 characters.
                 -  Must end with a number or a letter.
                 -  Must be unique within the OS policy.
             pkg (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.PackageResource):
                 Package resource
+
                 This field is a member of `oneof`_ ``resource_type``.
             repository (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.RepositoryResource):
                 Package repository resource
+
                 This field is a member of `oneof`_ ``resource_type``.
             exec_ (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.ExecResource):
                 Exec resource
+
                 This field is a member of `oneof`_ ``resource_type``.
             file (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.FileResource):
                 File resource
+
                 This field is a member of `oneof`_ ``resource_type``.
         """
 
         class File(proto.Message):
             r"""A remote or local file.
 
             This message has `oneof`_ fields (mutually exclusive fields).
@@ -136,20 +140,23 @@
             members.
 
             .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
             Attributes:
                 remote (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.File.Remote):
                     A generic remote file.
+
                     This field is a member of `oneof`_ ``type``.
                 gcs (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.File.Gcs):
                     A Cloud Storage object.
+
                     This field is a member of `oneof`_ ``type``.
                 local_path (str):
                     A local path within the VM to use.
+
                     This field is a member of `oneof`_ ``type``.
                 allow_insecure (bool):
                     Defaults to false. When false, files are
                     subject to validations based on the file type:
                     Remote: A checksum must be specified.
                     Cloud Storage: An object generation number must
                     be specified.
@@ -214,32 +221,39 @@
 
             Attributes:
                 desired_state (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.PackageResource.DesiredState):
                     Required. The desired state the agent should
                     maintain for this package.
                 apt (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.PackageResource.APT):
                     A package managed by Apt.
+
                     This field is a member of `oneof`_ ``system_package``.
                 deb (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.PackageResource.Deb):
                     A deb package file.
+
                     This field is a member of `oneof`_ ``system_package``.
                 yum (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.PackageResource.YUM):
                     A package managed by YUM.
+
                     This field is a member of `oneof`_ ``system_package``.
                 zypper (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.PackageResource.Zypper):
                     A package managed by Zypper.
+
                     This field is a member of `oneof`_ ``system_package``.
                 rpm (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.PackageResource.RPM):
                     An rpm package file.
+
                     This field is a member of `oneof`_ ``system_package``.
                 googet (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.PackageResource.GooGet):
                     A package managed by GooGet.
+
                     This field is a member of `oneof`_ ``system_package``.
                 msi (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.PackageResource.MSI):
                     An MSI package.
+
                     This field is a member of `oneof`_ ``system_package``.
             """
 
             class DesiredState(proto.Enum):
                 r"""The desired state that the OS Config agent maintains on the
                 VM.
                 """
@@ -414,23 +428,27 @@
             members.
 
             .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
             Attributes:
                 apt (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.RepositoryResource.AptRepository):
                     An Apt Repository.
+
                     This field is a member of `oneof`_ ``repository``.
                 yum (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.RepositoryResource.YumRepository):
                     A Yum Repository.
+
                     This field is a member of `oneof`_ ``repository``.
                 zypper (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.RepositoryResource.ZypperRepository):
                     A Zypper Repository.
+
                     This field is a member of `oneof`_ ``repository``.
                 goo (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.RepositoryResource.GooRepository):
                     A Goo Repository.
+
                     This field is a member of `oneof`_ ``repository``.
             """
 
             class AptRepository(proto.Message):
                 r"""Represents a single apt package repository. These will be added to a
                 repo file that will be managed at
                 ``/etc/apt/sources.list.d/google_osconfig.list``.
@@ -613,19 +631,21 @@
                 members.
 
                 .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
                 Attributes:
                     file (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.File):
                         A remote or local file.
+
                         This field is a member of `oneof`_ ``source``.
                     script (str):
                         An inline script.
                         The size of the script is limited to 1024
                         characters.
+
                         This field is a member of `oneof`_ ``source``.
                     args (Sequence[str]):
                         Optional arguments to pass to the source
                         during execution.
                     interpreter (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.ExecResource.Exec.Interpreter):
                         Required. The script interpreter to use.
                     output_file_path (str):
@@ -676,19 +696,21 @@
             members.
 
             .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
             Attributes:
                 file (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.File):
                     A remote or local source.
+
                     This field is a member of `oneof`_ ``source``.
                 content (str):
                     A a file with this content.
                     The size of the content is limited to 1024
                     characters.
+
                     This field is a member of `oneof`_ ``source``.
                 path (str):
                     Required. The absolute path of the file
                     within the VM.
                 state (google.cloud.osconfig_v1alpha.types.OSPolicy.Resource.FileResource.DesiredState):
                     Required. Desired state of the file.
                 permissions (str):
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/types/os_policy_assignments.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/types/os_policy_assignments.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/types/osconfig_common.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/types/osconfig_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,21 @@
     members.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         fixed (int):
             Specifies a fixed value.
+
             This field is a member of `oneof`_ ``mode``.
         percent (int):
             Specifies the relative value defined as a
             percentage, which will be multiplied by a
             reference value.
+
             This field is a member of `oneof`_ ``mode``.
     """
 
     fixed = proto.Field(proto.INT32, number=1, oneof="mode",)
     percent = proto.Field(proto.INT32, number=2, oneof="mode",)
```

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/types/osconfig_zonal_service.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1alpha/types/osconfig_zonal_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/google/cloud/osconfig_v1alpha/types/vulnerability.py` & `google-cloud-os-config-1.9.0/google/cloud/osconfig_v1/types/vulnerability.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #
 import proto  # type: ignore
 
 from google.protobuf import timestamp_pb2  # type: ignore
 
 
 __protobuf__ = proto.module(
-    package="google.cloud.osconfig.v1alpha",
+    package="google.cloud.osconfig.v1",
     manifest={
         "VulnerabilityReport",
         "GetVulnerabilityReportRequest",
         "ListVulnerabilityReportsRequest",
         "ListVulnerabilityReportsResponse",
         "CVSSv3",
     },
@@ -40,27 +40,27 @@
 
     Attributes:
         name (str):
             Output only. The ``vulnerabilityReport`` API resource name.
 
             Format:
             ``projects/{project_number}/locations/{location}/instances/{instance_id}/vulnerabilityReport``
-        vulnerabilities (Sequence[google.cloud.osconfig_v1alpha.types.VulnerabilityReport.Vulnerability]):
+        vulnerabilities (Sequence[google.cloud.osconfig_v1.types.VulnerabilityReport.Vulnerability]):
             Output only. List of vulnerabilities
             affecting the VM.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp for when the last
             vulnerability report was generated for the VM.
     """
 
     class Vulnerability(proto.Message):
         r"""A vulnerability affecting the VM instance.
 
         Attributes:
-            details (google.cloud.osconfig_v1alpha.types.VulnerabilityReport.Vulnerability.Details):
+            details (google.cloud.osconfig_v1.types.VulnerabilityReport.Vulnerability.Details):
                 Contains metadata as per the upstream feed of
                 the operating system and NVD.
             installed_inventory_item_ids (Sequence[str]):
                 Corresponds to the ``INSTALLED_PACKAGE`` inventory item on
                 the VM. This field displays the inventory items affected by
                 this vulnerability. If the vulnerability report was not
                 updated after the VM inventory update, these values might
@@ -76,14 +76,16 @@
                 vulnerability.
             create_time (google.protobuf.timestamp_pb2.Timestamp):
                 The timestamp for when the vulnerability was
                 first detected.
             update_time (google.protobuf.timestamp_pb2.Timestamp):
                 The timestamp for when the vulnerability was
                 last modified.
+            items (Sequence[google.cloud.osconfig_v1.types.VulnerabilityReport.Vulnerability.Item]):
+                List of items affected by the vulnerability.
         """
 
         class Details(proto.Message):
             r"""Contains metadata information for the vulnerability. This
             information is collected from the upstream feed of the operating
             system.
 
@@ -94,62 +96,102 @@
                     classification> should be unique across
                     vulnerabilities for a VM.
                 cvss_v2_score (float):
                     The CVSS V2 score of this vulnerability. CVSS
                     V2 score is on a scale of 0 - 10 where 0
                     indicates low severity and 10 indicates high
                     severity.
-                cvss_v3 (google.cloud.osconfig_v1alpha.types.CVSSv3):
+                cvss_v3 (google.cloud.osconfig_v1.types.CVSSv3):
                     The full description of the CVSSv3 for this
                     vulnerability from NVD.
                 severity (str):
                     Assigned severity/impact ranking from the
                     distro.
                 description (str):
                     The note or description describing the
                     vulnerability from the distro.
-                references (Sequence[google.cloud.osconfig_v1alpha.types.VulnerabilityReport.Vulnerability.Details.Reference]):
+                references (Sequence[google.cloud.osconfig_v1.types.VulnerabilityReport.Vulnerability.Details.Reference]):
                     Corresponds to the references attached to the
                     ``VulnerabilityDetails``.
             """
 
             class Reference(proto.Message):
                 r"""A reference for this vulnerability.
 
                 Attributes:
                     url (str):
                         The url of the reference.
+                    source (str):
+                        The source of the reference e.g. NVD.
                 """
 
                 url = proto.Field(proto.STRING, number=1,)
+                source = proto.Field(proto.STRING, number=2,)
 
             cve = proto.Field(proto.STRING, number=1,)
             cvss_v2_score = proto.Field(proto.FLOAT, number=2,)
             cvss_v3 = proto.Field(proto.MESSAGE, number=3, message="CVSSv3",)
             severity = proto.Field(proto.STRING, number=4,)
             description = proto.Field(proto.STRING, number=5,)
             references = proto.RepeatedField(
                 proto.MESSAGE,
                 number=6,
                 message="VulnerabilityReport.Vulnerability.Details.Reference",
             )
 
+        class Item(proto.Message):
+            r"""OS inventory item that is affected by a vulnerability or
+            fixed as a result of a vulnerability.
+
+            Attributes:
+                installed_inventory_item_id (str):
+                    Corresponds to the ``INSTALLED_PACKAGE`` inventory item on
+                    the VM. This field displays the inventory items affected by
+                    this vulnerability. If the vulnerability report was not
+                    updated after the VM inventory update, these values might
+                    not display in VM inventory. For some operating systems,
+                    this field might be empty.
+                available_inventory_item_id (str):
+                    Corresponds to the ``AVAILABLE_PACKAGE`` inventory item on
+                    the VM. If the vulnerability report was not updated after
+                    the VM inventory update, these values might not display in
+                    VM inventory. If there is no available fix, the field is
+                    empty. The ``inventory_item`` value specifies the latest
+                    ``SoftwarePackage`` available to the VM that fixes the
+                    vulnerability.
+                fixed_cpe_uri (str):
+                    The recommended `CPE
+                    URI <https://cpe.mitre.org/specification/>`__ update that
+                    contains a fix for this vulnerability.
+                upstream_fix (str):
+                    The upstream OS patch, packages or KB that
+                    fixes the vulnerability.
+            """
+
+            installed_inventory_item_id = proto.Field(proto.STRING, number=1,)
+            available_inventory_item_id = proto.Field(proto.STRING, number=2,)
+            fixed_cpe_uri = proto.Field(proto.STRING, number=3,)
+            upstream_fix = proto.Field(proto.STRING, number=4,)
+
         details = proto.Field(
             proto.MESSAGE,
             number=1,
             message="VulnerabilityReport.Vulnerability.Details",
         )
         installed_inventory_item_ids = proto.RepeatedField(proto.STRING, number=2,)
         available_inventory_item_ids = proto.RepeatedField(proto.STRING, number=3,)
         create_time = proto.Field(
             proto.MESSAGE, number=4, message=timestamp_pb2.Timestamp,
         )
         update_time = proto.Field(
             proto.MESSAGE, number=5, message=timestamp_pb2.Timestamp,
         )
+        items = proto.RepeatedField(
+            proto.MESSAGE, number=6, message="VulnerabilityReport.Vulnerability.Item",
+        )
 
     name = proto.Field(proto.STRING, number=1,)
     vulnerabilities = proto.RepeatedField(
         proto.MESSAGE, number=2, message=Vulnerability,
     )
     update_time = proto.Field(proto.MESSAGE, number=3, message=timestamp_pb2.Timestamp,)
 
@@ -179,20 +221,18 @@
     VM instances in the specified location.
 
     Attributes:
         parent (str):
             Required. The parent resource name.
 
             Format:
-            ``projects/{project}/locations/{location}/instances/{instance}``
+            ``projects/{project}/locations/{location}/instances/-``
 
             For ``{project}``, either ``project-number`` or
-            ``project-id`` can be provided. For ``{instance}``, only
-            ``-`` character is supported to list vulnerability reports
-            across VMs.
+            ``project-id`` can be provided.
         page_size (int):
             The maximum number of results to return.
         page_token (str):
             A pagination token returned from a previous call to
             ``ListVulnerabilityReports`` that indicates where this
             listing should continue from.
         filter (str):
@@ -208,15 +248,15 @@
 
 
 class ListVulnerabilityReportsResponse(proto.Message):
     r"""A response message for listing vulnerability reports for all
     VM instances in the specified location.
 
     Attributes:
-        vulnerability_reports (Sequence[google.cloud.osconfig_v1alpha.types.VulnerabilityReport]):
+        vulnerability_reports (Sequence[google.cloud.osconfig_v1.types.VulnerabilityReport]):
             List of vulnerabilityReport objects.
         next_page_token (str):
             The pagination token to retrieve the next
             page of vulnerabilityReports object.
     """
 
     @property
@@ -244,44 +284,44 @@
             The Exploitability sub-score equation is
             derived from the Base Exploitability metrics.
             https://www.first.org/cvss/specification-
             document#2-1-Exploitability-Metrics
         impact_score (float):
             The Impact sub-score equation is derived from
             the Base Impact metrics.
-        attack_vector (google.cloud.osconfig_v1alpha.types.CVSSv3.AttackVector):
+        attack_vector (google.cloud.osconfig_v1.types.CVSSv3.AttackVector):
             This metric reflects the context by which
             vulnerability exploitation is possible.
-        attack_complexity (google.cloud.osconfig_v1alpha.types.CVSSv3.AttackComplexity):
+        attack_complexity (google.cloud.osconfig_v1.types.CVSSv3.AttackComplexity):
             This metric describes the conditions beyond
             the attacker's control that must exist in order
             to exploit the vulnerability.
-        privileges_required (google.cloud.osconfig_v1alpha.types.CVSSv3.PrivilegesRequired):
+        privileges_required (google.cloud.osconfig_v1.types.CVSSv3.PrivilegesRequired):
             This metric describes the level of privileges
             an attacker must possess before successfully
             exploiting the vulnerability.
-        user_interaction (google.cloud.osconfig_v1alpha.types.CVSSv3.UserInteraction):
+        user_interaction (google.cloud.osconfig_v1.types.CVSSv3.UserInteraction):
             This metric captures the requirement for a
             human user, other than the attacker, to
             participate in the successful compromise of the
             vulnerable component.
-        scope (google.cloud.osconfig_v1alpha.types.CVSSv3.Scope):
+        scope (google.cloud.osconfig_v1.types.CVSSv3.Scope):
             The Scope metric captures whether a
             vulnerability in one vulnerable component
             impacts resources in components beyond its
             security scope.
-        confidentiality_impact (google.cloud.osconfig_v1alpha.types.CVSSv3.Impact):
+        confidentiality_impact (google.cloud.osconfig_v1.types.CVSSv3.Impact):
             This metric measures the impact to the
             confidentiality of the information resources
             managed by a software component due to a
             successfully exploited vulnerability.
-        integrity_impact (google.cloud.osconfig_v1alpha.types.CVSSv3.Impact):
+        integrity_impact (google.cloud.osconfig_v1.types.CVSSv3.Impact):
             This metric measures the impact to integrity
             of a successfully exploited vulnerability.
-        availability_impact (google.cloud.osconfig_v1alpha.types.CVSSv3.Impact):
+        availability_impact (google.cloud.osconfig_v1.types.CVSSv3.Impact):
             This metric measures the impact to the
             availability of the impacted component resulting
             from a successfully exploited vulnerability.
     """
 
     class AttackVector(proto.Enum):
         r"""This metric reflects the context by which vulnerability
```

### Comparing `google-cloud-os-config-1.8.0/google_cloud_os_config.egg-info/PKG-INFO` & `google-cloud-os-config-1.9.0/google_cloud_os_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-os-config
-Version: 1.8.0
+Version: 1.9.0
 Summary: Google Cloud OS Config API client library
 Home-page: https://github.com/googleapis/python-os-config
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-os-config-1.8.0/google_cloud_os_config.egg-info/SOURCES.txt` & `google-cloud-os-config-1.9.0/google_cloud_os_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/scripts/fixup_keywords.py` & `google-cloud-os-config-1.9.0/scripts/fixup_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/setup.py` & `google-cloud-os-config-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import setuptools  # type: ignore
 
 
 # Package metadata.
 
 name = "google-cloud-os-config"
 description = "Google Cloud OS Config API client library"
-version = "1.8.0"
+version = "1.9.0"
 # Should be one of:
 # 'Development Status :: 3 - Alpha'
 # 'Development Status :: 4 - Beta'
 # 'Development Status :: 5 - Production/Stable'
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     # NOTE: Maintainers, please do not require google-api-core>=2.x.x
```

### Comparing `google-cloud-os-config-1.8.0/tests/__init__.py` & `google-cloud-os-config-1.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/tests/system/test_os_config_service_v1.py` & `google-cloud-os-config-1.9.0/tests/system/test_os_config_service_v1.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/tests/unit/__init__.py` & `google-cloud-os-config-1.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/tests/unit/gapic/__init__.py` & `google-cloud-os-config-1.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/tests/unit/gapic/osconfig_v1/__init__.py` & `google-cloud-os-config-1.9.0/tests/unit/gapic/osconfig_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/tests/unit/gapic/osconfig_v1/test_os_config_service.py` & `google-cloud-os-config-1.9.0/tests/unit/gapic/osconfig_v1/test_os_config_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -845,15 +845,17 @@
         # using the keyword arguments to the method.
         client.get_patch_job(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 def test_get_patch_job_flattened_error():
     client = OsConfigServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
@@ -879,15 +881,17 @@
         # using the keyword arguments to the method.
         response = await client.get_patch_job(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_get_patch_job_flattened_error_async():
     client = OsConfigServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -1211,15 +1215,17 @@
         # using the keyword arguments to the method.
         client.list_patch_jobs(parent="parent_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 def test_list_patch_jobs_flattened_error():
     client = OsConfigServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
@@ -1247,15 +1253,17 @@
         # using the keyword arguments to the method.
         response = await client.list_patch_jobs(parent="parent_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_list_patch_jobs_flattened_error_async():
     client = OsConfigServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -1572,15 +1580,17 @@
         # using the keyword arguments to the method.
         client.list_patch_job_instance_details(parent="parent_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 def test_list_patch_job_instance_details_flattened_error():
     client = OsConfigServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
@@ -1610,15 +1620,17 @@
         # using the keyword arguments to the method.
         response = await client.list_patch_job_instance_details(parent="parent_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_list_patch_job_instance_details_flattened_error_async():
     client = OsConfigServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -1979,19 +1991,23 @@
             patch_deployment_id="patch_deployment_id_value",
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
-        assert args[0].patch_deployment == patch_deployments.PatchDeployment(
-            name="name_value"
-        )
-        assert args[0].patch_deployment_id == "patch_deployment_id_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
+        arg = args[0].patch_deployment
+        mock_val = patch_deployments.PatchDeployment(name="name_value")
+        assert arg == mock_val
+        arg = args[0].patch_deployment_id
+        mock_val = "patch_deployment_id_value"
+        assert arg == mock_val
 
 
 def test_create_patch_deployment_flattened_error():
     client = OsConfigServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
@@ -2028,19 +2044,23 @@
             patch_deployment_id="patch_deployment_id_value",
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
-        assert args[0].patch_deployment == patch_deployments.PatchDeployment(
-            name="name_value"
-        )
-        assert args[0].patch_deployment_id == "patch_deployment_id_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
+        arg = args[0].patch_deployment
+        mock_val = patch_deployments.PatchDeployment(name="name_value")
+        assert arg == mock_val
+        arg = args[0].patch_deployment_id
+        mock_val = "patch_deployment_id_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_create_patch_deployment_flattened_error_async():
     client = OsConfigServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -2224,15 +2244,17 @@
         # using the keyword arguments to the method.
         client.get_patch_deployment(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 def test_get_patch_deployment_flattened_error():
     client = OsConfigServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
@@ -2262,15 +2284,17 @@
         # using the keyword arguments to the method.
         response = await client.get_patch_deployment(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_get_patch_deployment_flattened_error_async():
     client = OsConfigServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -2445,15 +2469,17 @@
         # using the keyword arguments to the method.
         client.list_patch_deployments(parent="parent_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 def test_list_patch_deployments_flattened_error():
     client = OsConfigServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
@@ -2483,15 +2509,17 @@
         # using the keyword arguments to the method.
         response = await client.list_patch_deployments(parent="parent_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_list_patch_deployments_flattened_error_async():
     client = OsConfigServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -2830,15 +2858,17 @@
         # using the keyword arguments to the method.
         client.delete_patch_deployment(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 def test_delete_patch_deployment_flattened_error():
     client = OsConfigServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
@@ -2866,15 +2896,17 @@
         # using the keyword arguments to the method.
         response = await client.delete_patch_deployment(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_delete_patch_deployment_flattened_error_async():
     client = OsConfigServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
```

### Comparing `google-cloud-os-config-1.8.0/tests/unit/gapic/osconfig_v1/test_os_config_zonal_service.py` & `google-cloud-os-config-1.9.0/tests/unit/gapic/osconfig_v1/test_os_config_zonal_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -683,19 +683,23 @@
             os_policy_assignment_id="os_policy_assignment_id_value",
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
-        assert args[0].os_policy_assignment == os_policy_assignments.OSPolicyAssignment(
-            name="name_value"
-        )
-        assert args[0].os_policy_assignment_id == "os_policy_assignment_id_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
+        arg = args[0].os_policy_assignment
+        mock_val = os_policy_assignments.OSPolicyAssignment(name="name_value")
+        assert arg == mock_val
+        arg = args[0].os_policy_assignment_id
+        mock_val = "os_policy_assignment_id_value"
+        assert arg == mock_val
 
 
 def test_create_os_policy_assignment_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -738,19 +742,23 @@
             os_policy_assignment_id="os_policy_assignment_id_value",
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
-        assert args[0].os_policy_assignment == os_policy_assignments.OSPolicyAssignment(
-            name="name_value"
-        )
-        assert args[0].os_policy_assignment_id == "os_policy_assignment_id_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
+        arg = args[0].os_policy_assignment
+        mock_val = os_policy_assignments.OSPolicyAssignment(name="name_value")
+        assert arg == mock_val
+        arg = args[0].os_policy_assignment_id
+        mock_val = "os_policy_assignment_id_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_create_os_policy_assignment_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -940,18 +948,20 @@
             update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].os_policy_assignment == os_policy_assignments.OSPolicyAssignment(
-            name="name_value"
-        )
-        assert args[0].update_mask == field_mask_pb2.FieldMask(paths=["paths_value"])
+        arg = args[0].os_policy_assignment
+        mock_val = os_policy_assignments.OSPolicyAssignment(name="name_value")
+        assert arg == mock_val
+        arg = args[0].update_mask
+        mock_val = field_mask_pb2.FieldMask(paths=["paths_value"])
+        assert arg == mock_val
 
 
 def test_update_os_policy_assignment_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -992,18 +1002,20 @@
             update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].os_policy_assignment == os_policy_assignments.OSPolicyAssignment(
-            name="name_value"
-        )
-        assert args[0].update_mask == field_mask_pb2.FieldMask(paths=["paths_value"])
+        arg = args[0].os_policy_assignment
+        mock_val = os_policy_assignments.OSPolicyAssignment(name="name_value")
+        assert arg == mock_val
+        arg = args[0].update_mask
+        mock_val = field_mask_pb2.FieldMask(paths=["paths_value"])
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_update_os_policy_assignment_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -1225,15 +1237,17 @@
         # using the keyword arguments to the method.
         client.get_os_policy_assignment(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 def test_get_os_policy_assignment_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -1265,15 +1279,17 @@
         # using the keyword arguments to the method.
         response = await client.get_os_policy_assignment(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_get_os_policy_assignment_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -1453,15 +1469,17 @@
         # using the keyword arguments to the method.
         client.list_os_policy_assignments(parent="parent_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 def test_list_os_policy_assignments_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -1494,15 +1512,17 @@
         # using the keyword arguments to the method.
         response = await client.list_os_policy_assignments(parent="parent_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_list_os_policy_assignments_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -1869,15 +1889,17 @@
         # using the keyword arguments to the method.
         client.list_os_policy_assignment_revisions(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 def test_list_os_policy_assignment_revisions_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -1912,15 +1934,17 @@
         # using the keyword arguments to the method.
         response = await client.list_os_policy_assignment_revisions(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_list_os_policy_assignment_revisions_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -2279,15 +2303,17 @@
         # using the keyword arguments to the method.
         client.delete_os_policy_assignment(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 def test_delete_os_policy_assignment_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -2319,15 +2345,17 @@
         # using the keyword arguments to the method.
         response = await client.delete_os_policy_assignment(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_delete_os_policy_assignment_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -2525,15 +2553,17 @@
         # using the keyword arguments to the method.
         client.get_os_policy_assignment_report(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 def test_get_os_policy_assignment_report_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -2566,15 +2596,17 @@
         # using the keyword arguments to the method.
         response = await client.get_os_policy_assignment_report(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_get_os_policy_assignment_report_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -2768,15 +2800,17 @@
         # using the keyword arguments to the method.
         client.list_os_policy_assignment_reports(parent="parent_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 def test_list_os_policy_assignment_reports_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -2813,15 +2847,17 @@
             parent="parent_value",
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_list_os_policy_assignment_reports_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -3176,15 +3212,17 @@
         # using the keyword arguments to the method.
         client.get_inventory(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 def test_get_inventory_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -3212,15 +3250,17 @@
         # using the keyword arguments to the method.
         response = await client.get_inventory(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_get_inventory_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -3384,15 +3424,17 @@
         # using the keyword arguments to the method.
         client.list_inventories(parent="parent_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 def test_list_inventories_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -3422,15 +3464,17 @@
         # using the keyword arguments to the method.
         response = await client.list_inventories(parent="parent_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_list_inventories_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -3751,15 +3795,17 @@
         # using the keyword arguments to the method.
         client.get_vulnerability_report(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 def test_get_vulnerability_report_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -3791,15 +3837,17 @@
         # using the keyword arguments to the method.
         response = await client.get_vulnerability_report(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_get_vulnerability_report_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -3978,15 +4026,17 @@
         # using the keyword arguments to the method.
         client.list_vulnerability_reports(parent="parent_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 def test_list_vulnerability_reports_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -4018,15 +4068,17 @@
         # using the keyword arguments to the method.
         response = await client.list_vulnerability_reports(parent="parent_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_list_vulnerability_reports_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
```

### Comparing `google-cloud-os-config-1.8.0/tests/unit/gapic/osconfig_v1alpha/__init__.py` & `google-cloud-os-config-1.9.0/tests/unit/gapic/osconfig_v1alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-config-1.8.0/tests/unit/gapic/osconfig_v1alpha/test_os_config_zonal_service.py` & `google-cloud-os-config-1.9.0/tests/unit/gapic/osconfig_v1alpha/test_os_config_zonal_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -684,19 +684,23 @@
             os_policy_assignment_id="os_policy_assignment_id_value",
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
-        assert args[0].os_policy_assignment == os_policy_assignments.OSPolicyAssignment(
-            name="name_value"
-        )
-        assert args[0].os_policy_assignment_id == "os_policy_assignment_id_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
+        arg = args[0].os_policy_assignment
+        mock_val = os_policy_assignments.OSPolicyAssignment(name="name_value")
+        assert arg == mock_val
+        arg = args[0].os_policy_assignment_id
+        mock_val = "os_policy_assignment_id_value"
+        assert arg == mock_val
 
 
 def test_create_os_policy_assignment_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -739,19 +743,23 @@
             os_policy_assignment_id="os_policy_assignment_id_value",
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
-        assert args[0].os_policy_assignment == os_policy_assignments.OSPolicyAssignment(
-            name="name_value"
-        )
-        assert args[0].os_policy_assignment_id == "os_policy_assignment_id_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
+        arg = args[0].os_policy_assignment
+        mock_val = os_policy_assignments.OSPolicyAssignment(name="name_value")
+        assert arg == mock_val
+        arg = args[0].os_policy_assignment_id
+        mock_val = "os_policy_assignment_id_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_create_os_policy_assignment_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -941,18 +949,20 @@
             update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].os_policy_assignment == os_policy_assignments.OSPolicyAssignment(
-            name="name_value"
-        )
-        assert args[0].update_mask == field_mask_pb2.FieldMask(paths=["paths_value"])
+        arg = args[0].os_policy_assignment
+        mock_val = os_policy_assignments.OSPolicyAssignment(name="name_value")
+        assert arg == mock_val
+        arg = args[0].update_mask
+        mock_val = field_mask_pb2.FieldMask(paths=["paths_value"])
+        assert arg == mock_val
 
 
 def test_update_os_policy_assignment_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -993,18 +1003,20 @@
             update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].os_policy_assignment == os_policy_assignments.OSPolicyAssignment(
-            name="name_value"
-        )
-        assert args[0].update_mask == field_mask_pb2.FieldMask(paths=["paths_value"])
+        arg = args[0].os_policy_assignment
+        mock_val = os_policy_assignments.OSPolicyAssignment(name="name_value")
+        assert arg == mock_val
+        arg = args[0].update_mask
+        mock_val = field_mask_pb2.FieldMask(paths=["paths_value"])
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_update_os_policy_assignment_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -1222,15 +1234,17 @@
         # using the keyword arguments to the method.
         client.get_os_policy_assignment(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 def test_get_os_policy_assignment_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -1262,15 +1276,17 @@
         # using the keyword arguments to the method.
         response = await client.get_os_policy_assignment(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_get_os_policy_assignment_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -1450,15 +1466,17 @@
         # using the keyword arguments to the method.
         client.list_os_policy_assignments(parent="parent_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 def test_list_os_policy_assignments_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -1491,15 +1509,17 @@
         # using the keyword arguments to the method.
         response = await client.list_os_policy_assignments(parent="parent_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_list_os_policy_assignments_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -1866,15 +1886,17 @@
         # using the keyword arguments to the method.
         client.list_os_policy_assignment_revisions(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 def test_list_os_policy_assignment_revisions_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -1909,15 +1931,17 @@
         # using the keyword arguments to the method.
         response = await client.list_os_policy_assignment_revisions(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_list_os_policy_assignment_revisions_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -2276,15 +2300,17 @@
         # using the keyword arguments to the method.
         client.delete_os_policy_assignment(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 def test_delete_os_policy_assignment_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -2316,15 +2342,17 @@
         # using the keyword arguments to the method.
         response = await client.delete_os_policy_assignment(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_delete_os_policy_assignment_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -2541,15 +2569,17 @@
         # using the keyword arguments to the method.
         client.get_instance_os_policies_compliance(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 def test_get_instance_os_policies_compliance_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -2584,15 +2614,17 @@
         # using the keyword arguments to the method.
         response = await client.get_instance_os_policies_compliance(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_get_instance_os_policies_compliance_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -2786,15 +2818,17 @@
         # using the keyword arguments to the method.
         client.list_instance_os_policies_compliances(parent="parent_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 def test_list_instance_os_policies_compliances_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -2831,15 +2865,17 @@
             parent="parent_value",
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_list_instance_os_policies_compliances_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -3194,15 +3230,17 @@
         # using the keyword arguments to the method.
         client.get_inventory(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 def test_get_inventory_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -3230,15 +3268,17 @@
         # using the keyword arguments to the method.
         response = await client.get_inventory(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_get_inventory_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -3402,15 +3442,17 @@
         # using the keyword arguments to the method.
         client.list_inventories(parent="parent_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 def test_list_inventories_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -3440,15 +3482,17 @@
         # using the keyword arguments to the method.
         response = await client.list_inventories(parent="parent_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_list_inventories_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -3769,15 +3813,17 @@
         # using the keyword arguments to the method.
         client.get_vulnerability_report(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 def test_get_vulnerability_report_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -3809,15 +3855,17 @@
         # using the keyword arguments to the method.
         response = await client.get_vulnerability_report(name="name_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].name == "name_value"
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_get_vulnerability_report_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -3996,15 +4044,17 @@
         # using the keyword arguments to the method.
         client.list_vulnerability_reports(parent="parent_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 def test_list_vulnerability_reports_flattened_error():
     client = OsConfigZonalServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -4036,15 +4086,17 @@
         # using the keyword arguments to the method.
         response = await client.list_vulnerability_reports(parent="parent_value",)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0].parent == "parent_value"
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_list_vulnerability_reports_flattened_error_async():
     client = OsConfigZonalServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
```

