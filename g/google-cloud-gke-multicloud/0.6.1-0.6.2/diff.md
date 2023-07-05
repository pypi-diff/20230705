# Comparing `tmp/google-cloud-gke-multicloud-0.6.1.tar.gz` & `tmp/google-cloud-gke-multicloud-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-gke-multicloud-0.6.1.tar", last modified: Mon Mar 27 14:59:55 2023, max compression
+gzip compressed data, was "google-cloud-gke-multicloud-0.6.2.tar", last modified: Wed Jul  5 15:53:22 2023, max compression
```

## Comparing `google-cloud-gke-multicloud-0.6.1.tar` & `google-cloud-gke-multicloud-0.6.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:55.401819 google-cloud-gke-multicloud-0.6.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4794 2023-03-27 14:59:55.401819 google-cloud-gke-multicloud-0.6.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3870 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:55.385818 google-cloud-gke-multicloud-0.6.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:55.385818 google-cloud-gke-multicloud-0.6.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:55.385818 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud/
--rw-rw-r--   0 root         (0)     1003     7853 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       88 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:55.385818 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/
--rw-rw-r--   0 root         (0)     1003     7256 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    15980 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       88 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:55.389818 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:55.389818 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/attached_clusters/
--rw-rw-r--   0 root         (0)     1003      777 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/attached_clusters/__init__.py
--rw-rw-r--   0 root         (0)     1003    66037 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/attached_clusters/async_client.py
--rw-rw-r--   0 root         (0)     1003    75856 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/attached_clusters/client.py
--rw-rw-r--   0 root         (0)     1003     6153 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/attached_clusters/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:55.389818 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12225 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/base.py
--rw-rw-r--   0 root         (0)     1003    26237 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    26688 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    67547 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:55.389818 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/aws_clusters/
--rw-rw-r--   0 root         (0)     1003      757 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/aws_clusters/__init__.py
--rw-rw-r--   0 root         (0)     1003    89025 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/aws_clusters/async_client.py
--rw-rw-r--   0 root         (0)     1003    99401 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/aws_clusters/client.py
--rw-rw-r--   0 root         (0)     1003    11046 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/aws_clusters/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:55.393818 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14325 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/base.py
--rw-rw-r--   0 root         (0)     1003    30447 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    31075 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    85415 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:55.393818 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/azure_clusters/
--rw-rw-r--   0 root         (0)     1003      765 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/azure_clusters/__init__.py
--rw-rw-r--   0 root         (0)     1003   112727 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/azure_clusters/async_client.py
--rw-rw-r--   0 root         (0)     1003   123684 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/azure_clusters/client.py
--rw-rw-r--   0 root         (0)     1003    16380 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/azure_clusters/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:55.393818 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    17079 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/base.py
--rw-rw-r--   0 root         (0)     1003    36579 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    37325 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   107962 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:55.397819 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/types/
--rw-rw-r--   0 root         (0)     1003     6649 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    12694 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/types/attached_resources.py
--rw-rw-r--   0 root         (0)     1003    15455 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/types/attached_service.py
--rw-rw-r--   0 root         (0)     1003    36717 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/types/aws_resources.py
--rw-rw-r--   0 root         (0)     1003    21899 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/types/aws_service.py
--rw-rw-r--   0 root         (0)     1003    41341 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/types/azure_resources.py
--rw-rw-r--   0 root         (0)     1003    27564 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/types/azure_service.py
--rw-rw-r--   0 root         (0)     1003     9285 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/types/common_resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:55.397819 google-cloud-gke-multicloud-0.6.1/google_cloud_gke_multicloud.egg-info/
--rw-r--r--   0 root         (0)     1003     4794 2023-03-27 14:59:55.000000 google-cloud-gke-multicloud-0.6.1/google_cloud_gke_multicloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3458 2023-03-27 14:59:55.000000 google-cloud-gke-multicloud-0.6.1/google_cloud_gke_multicloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:59:55.000000 google-cloud-gke-multicloud-0.6.1/google_cloud_gke_multicloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:59:55.000000 google-cloud-gke-multicloud-0.6.1/google_cloud_gke_multicloud.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:59:55.000000 google-cloud-gke-multicloud-0.6.1/google_cloud_gke_multicloud.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 14:59:55.000000 google-cloud-gke-multicloud-0.6.1/google_cloud_gke_multicloud.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:59:55.000000 google-cloud-gke-multicloud-0.6.1/google_cloud_gke_multicloud.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 14:59:55.401819 google-cloud-gke-multicloud-0.6.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2955 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:55.397819 google-cloud-gke-multicloud-0.6.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:55.397819 google-cloud-gke-multicloud-0.6.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:55.397819 google-cloud-gke-multicloud-0.6.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:55.401819 google-cloud-gke-multicloud-0.6.1/tests/unit/gapic/gke_multicloud_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/tests/unit/gapic/gke_multicloud_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   263229 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/tests/unit/gapic/gke_multicloud_v1/test_attached_clusters.py
--rw-rw-r--   0 root         (0)     1003   346759 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/tests/unit/gapic/gke_multicloud_v1/test_aws_clusters.py
--rw-rw-r--   0 root         (0)     1003   439829 2023-03-27 14:57:44.000000 google-cloud-gke-multicloud-0.6.1/tests/unit/gapic/gke_multicloud_v1/test_azure_clusters.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:22.057213 google-cloud-gke-multicloud-0.6.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4756 2023-07-05 15:53:22.057213 google-cloud-gke-multicloud-0.6.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3834 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:22.041213 google-cloud-gke-multicloud-0.6.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:22.041213 google-cloud-gke-multicloud-0.6.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:22.045213 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud/
+-rw-rw-r--   0 root         (0)     1003     7853 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       88 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:22.045213 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/
+-rw-rw-r--   0 root         (0)     1003     7256 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15980 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       88 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:22.045213 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:22.045213 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/attached_clusters/
+-rw-rw-r--   0 root         (0)     1003      777 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/attached_clusters/__init__.py
+-rw-rw-r--   0 root         (0)     1003    66070 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/attached_clusters/async_client.py
+-rw-rw-r--   0 root         (0)     1003    75856 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/attached_clusters/client.py
+-rw-rw-r--   0 root         (0)     1003     6153 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/attached_clusters/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:22.045213 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12225 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    26237 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    26688 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    67535 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:22.049213 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/aws_clusters/
+-rw-rw-r--   0 root         (0)     1003      757 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/aws_clusters/__init__.py
+-rw-rw-r--   0 root         (0)     1003    89053 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/aws_clusters/async_client.py
+-rw-rw-r--   0 root         (0)     1003    99401 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/aws_clusters/client.py
+-rw-rw-r--   0 root         (0)     1003    11046 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/aws_clusters/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:22.049213 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14325 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    30447 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    31075 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    85403 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:22.049213 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/azure_clusters/
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/azure_clusters/__init__.py
+-rw-rw-r--   0 root         (0)     1003   112757 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/azure_clusters/async_client.py
+-rw-rw-r--   0 root         (0)     1003   123684 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/azure_clusters/client.py
+-rw-rw-r--   0 root         (0)     1003    16380 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/azure_clusters/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:22.053213 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17079 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    36579 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    37325 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   107950 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:22.053213 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/types/
+-rw-rw-r--   0 root         (0)     1003     6649 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12694 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/types/attached_resources.py
+-rw-rw-r--   0 root         (0)     1003    15455 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/types/attached_service.py
+-rw-rw-r--   0 root         (0)     1003    36717 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/types/aws_resources.py
+-rw-rw-r--   0 root         (0)     1003    21899 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/types/aws_service.py
+-rw-rw-r--   0 root         (0)     1003    41341 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/types/azure_resources.py
+-rw-rw-r--   0 root         (0)     1003    27564 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/types/azure_service.py
+-rw-rw-r--   0 root         (0)     1003     9285 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/types/common_resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:22.053213 google-cloud-gke-multicloud-0.6.2/google_cloud_gke_multicloud.egg-info/
+-rw-r--r--   0 root         (0)     1003     4756 2023-07-05 15:53:21.000000 google-cloud-gke-multicloud-0.6.2/google_cloud_gke_multicloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3458 2023-07-05 15:53:22.000000 google-cloud-gke-multicloud-0.6.2/google_cloud_gke_multicloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:21.000000 google-cloud-gke-multicloud-0.6.2/google_cloud_gke_multicloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:53:21.000000 google-cloud-gke-multicloud-0.6.2/google_cloud_gke_multicloud.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:21.000000 google-cloud-gke-multicloud-0.6.2/google_cloud_gke_multicloud.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:53:21.000000 google-cloud-gke-multicloud-0.6.2/google_cloud_gke_multicloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:53:21.000000 google-cloud-gke-multicloud-0.6.2/google_cloud_gke_multicloud.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:53:22.057213 google-cloud-gke-multicloud-0.6.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2953 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:22.053213 google-cloud-gke-multicloud-0.6.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:22.053213 google-cloud-gke-multicloud-0.6.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:22.053213 google-cloud-gke-multicloud-0.6.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:22.057213 google-cloud-gke-multicloud-0.6.2/tests/unit/gapic/gke_multicloud_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/tests/unit/gapic/gke_multicloud_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   263428 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/tests/unit/gapic/gke_multicloud_v1/test_attached_clusters.py
+-rw-rw-r--   0 root         (0)     1003   347157 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/tests/unit/gapic/gke_multicloud_v1/test_aws_clusters.py
+-rw-rw-r--   0 root         (0)     1003   440426 2023-07-05 15:46:59.000000 google-cloud-gke-multicloud-0.6.2/tests/unit/gapic/gke_multicloud_v1/test_azure_clusters.py
```

### Comparing `google-cloud-gke-multicloud-0.6.1/LICENSE` & `google-cloud-gke-multicloud-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/MANIFEST.in` & `google-cloud-gke-multicloud-0.6.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/PKG-INFO` & `google-cloud-gke-multicloud-0.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-gke-multicloud
-Version: 0.6.1
+Version: 0.6.2
 Summary: Google Cloud Gke Multicloud API client library
-Home-page: https://github.com/googleapis/python-gke-multicloud
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
 
-Python Client for Anthos Multicloud API
-=======================================
+Python Client for Anthos Multicloud
+===================================
 
 |preview| |pypi| |versions|
 
-`Anthos Multicloud API`_: An API for provisioning and managing GKE clusters running on AWS and Azure infrastructure through a centralized Google Cloud backed control plane.
+`Anthos Multicloud`_: An API for provisioning and managing GKE clusters running on AWS and Azure infrastructure through a centralized Google Cloud backed control plane.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-gke-multicloud.svg
    :target: https://pypi.org/project/google-cloud-gke-multicloud/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-gke-multicloud.svg
    :target: https://pypi.org/project/google-cloud-gke-multicloud/
-.. _Anthos Multicloud API: https://cloud.google.com/anthos/clusters/docs/multi-cloud
+.. _Anthos Multicloud: https://cloud.google.com/anthos/clusters/docs/multi-cloud
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/gkemulticloud/latest
 .. _Product Documentation:  https://cloud.google.com/anthos/clusters/docs/multi-cloud
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Anthos Multicloud API.`_
+3. `Enable the Anthos Multicloud.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Anthos Multicloud API.:  https://cloud.google.com/anthos/clusters/docs/multi-cloud
+.. _Enable the Anthos Multicloud.:  https://cloud.google.com/anthos/clusters/docs/multi-cloud
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-gke-multicloud
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Anthos Multicloud API
+-  Read the `Client Library Documentation`_ for Anthos Multicloud
    to see other available methods on the client.
--  Read the `Anthos Multicloud API Product documentation`_ to learn
+-  Read the `Anthos Multicloud Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Anthos Multicloud API Product documentation:  https://cloud.google.com/anthos/clusters/docs/multi-cloud
+.. _Anthos Multicloud Product documentation:  https://cloud.google.com/anthos/clusters/docs/multi-cloud
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-gke-multicloud-0.6.1/README.rst` & `google-cloud-gke-multicloud-0.6.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Anthos Multicloud API
-=======================================
+Python Client for Anthos Multicloud
+===================================
 
 |preview| |pypi| |versions|
 
-`Anthos Multicloud API`_: An API for provisioning and managing GKE clusters running on AWS and Azure infrastructure through a centralized Google Cloud backed control plane.
+`Anthos Multicloud`_: An API for provisioning and managing GKE clusters running on AWS and Azure infrastructure through a centralized Google Cloud backed control plane.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-gke-multicloud.svg
    :target: https://pypi.org/project/google-cloud-gke-multicloud/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-gke-multicloud.svg
    :target: https://pypi.org/project/google-cloud-gke-multicloud/
-.. _Anthos Multicloud API: https://cloud.google.com/anthos/clusters/docs/multi-cloud
+.. _Anthos Multicloud: https://cloud.google.com/anthos/clusters/docs/multi-cloud
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/gkemulticloud/latest
 .. _Product Documentation:  https://cloud.google.com/anthos/clusters/docs/multi-cloud
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Anthos Multicloud API.`_
+3. `Enable the Anthos Multicloud.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Anthos Multicloud API.:  https://cloud.google.com/anthos/clusters/docs/multi-cloud
+.. _Enable the Anthos Multicloud.:  https://cloud.google.com/anthos/clusters/docs/multi-cloud
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-gke-multicloud
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Anthos Multicloud API
+-  Read the `Client Library Documentation`_ for Anthos Multicloud
    to see other available methods on the client.
--  Read the `Anthos Multicloud API Product documentation`_ to learn
+-  Read the `Anthos Multicloud Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Anthos Multicloud API Product documentation:  https://cloud.google.com/anthos/clusters/docs/multi-cloud
+.. _Anthos Multicloud Product documentation:  https://cloud.google.com/anthos/clusters/docs/multi-cloud
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud/__init__.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud/gapic_version.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud/gapic_version.py`

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
-__version__ = "0.6.1"  # {x-release-please-version}
+__version__ = "0.6.2"  # {x-release-please-version}
```

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/__init__.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/gapic_metadata.json` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/gapic_version.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/gapic_version.py`

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
-__version__ = "0.6.1"  # {x-release-please-version}
+__version__ = "0.6.2"  # {x-release-please-version}
```

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/__init__.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/attached_clusters/__init__.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/attached_clusters/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/attached_clusters/async_client.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/attached_clusters/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1596,15 +1596,15 @@
         await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "AttachedClustersAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/attached_clusters/client.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/attached_clusters/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/attached_clusters/pagers.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/attached_clusters/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/__init__.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/base.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/grpc.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/grpc_asyncio.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/rest.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1464,15 +1464,15 @@
 
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

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/aws_clusters/__init__.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/aws_clusters/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/aws_clusters/async_client.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/aws_clusters/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2130,15 +2130,15 @@
         await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "AwsClustersAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/aws_clusters/client.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/aws_clusters/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/aws_clusters/pagers.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/aws_clusters/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/__init__.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/base.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/grpc.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/grpc_asyncio.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/rest.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1939,15 +1939,15 @@
 
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

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/azure_clusters/__init__.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/azure_clusters/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/azure_clusters/async_client.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/azure_clusters/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2717,15 +2717,15 @@
         await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "AzureClustersAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/azure_clusters/client.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/azure_clusters/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/azure_clusters/pagers.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/azure_clusters/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/__init__.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/base.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/grpc.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/grpc_asyncio.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/rest.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -2487,15 +2487,15 @@
 
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

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/types/__init__.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/types/attached_resources.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/types/attached_resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/types/attached_service.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/types/attached_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/types/aws_resources.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/types/aws_resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/types/aws_service.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/types/aws_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/types/azure_resources.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/types/azure_resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/types/azure_service.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/types/azure_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google/cloud/gke_multicloud_v1/types/common_resources.py` & `google-cloud-gke-multicloud-0.6.2/google/cloud/gke_multicloud_v1/types/common_resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/google_cloud_gke_multicloud.egg-info/PKG-INFO` & `google-cloud-gke-multicloud-0.6.2/google_cloud_gke_multicloud.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-gke-multicloud
-Version: 0.6.1
+Version: 0.6.2
 Summary: Google Cloud Gke Multicloud API client library
-Home-page: https://github.com/googleapis/python-gke-multicloud
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
 
-Python Client for Anthos Multicloud API
-=======================================
+Python Client for Anthos Multicloud
+===================================
 
 |preview| |pypi| |versions|
 
-`Anthos Multicloud API`_: An API for provisioning and managing GKE clusters running on AWS and Azure infrastructure through a centralized Google Cloud backed control plane.
+`Anthos Multicloud`_: An API for provisioning and managing GKE clusters running on AWS and Azure infrastructure through a centralized Google Cloud backed control plane.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-gke-multicloud.svg
    :target: https://pypi.org/project/google-cloud-gke-multicloud/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-gke-multicloud.svg
    :target: https://pypi.org/project/google-cloud-gke-multicloud/
-.. _Anthos Multicloud API: https://cloud.google.com/anthos/clusters/docs/multi-cloud
+.. _Anthos Multicloud: https://cloud.google.com/anthos/clusters/docs/multi-cloud
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/gkemulticloud/latest
 .. _Product Documentation:  https://cloud.google.com/anthos/clusters/docs/multi-cloud
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Anthos Multicloud API.`_
+3. `Enable the Anthos Multicloud.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Anthos Multicloud API.:  https://cloud.google.com/anthos/clusters/docs/multi-cloud
+.. _Enable the Anthos Multicloud.:  https://cloud.google.com/anthos/clusters/docs/multi-cloud
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-gke-multicloud
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Anthos Multicloud API
+-  Read the `Client Library Documentation`_ for Anthos Multicloud
    to see other available methods on the client.
--  Read the `Anthos Multicloud API Product documentation`_ to learn
+-  Read the `Anthos Multicloud Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Anthos Multicloud API Product documentation:  https://cloud.google.com/anthos/clusters/docs/multi-cloud
+.. _Anthos Multicloud Product documentation:  https://cloud.google.com/anthos/clusters/docs/multi-cloud
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-gke-multicloud-0.6.1/google_cloud_gke_multicloud.egg-info/SOURCES.txt` & `google-cloud-gke-multicloud-0.6.2/google_cloud_gke_multicloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/setup.py` & `google-cloud-gke-multicloud-0.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-gke-multicloud"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-gke-multicloud-0.6.1/tests/__init__.py` & `google-cloud-gke-multicloud-0.6.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/tests/unit/__init__.py` & `google-cloud-gke-multicloud-0.6.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/tests/unit/gapic/__init__.py` & `google-cloud-gke-multicloud-0.6.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/tests/unit/gapic/gke_multicloud_v1/__init__.py` & `google-cloud-gke-multicloud-0.6.2/tests/unit/gapic/gke_multicloud_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.1/tests/unit/gapic/gke_multicloud_v1/test_attached_clusters.py` & `google-cloud-gke-multicloud-0.6.2/tests/unit/gapic/gke_multicloud_v1/test_attached_clusters.py`

 * *Files 0% similar despite different names*

```diff
@@ -2226,17 +2226,19 @@
                     attached_resources.AttachedCluster(),
                     attached_resources.AttachedCluster(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_attached_clusters(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-gke-multicloud-0.6.1/tests/unit/gapic/gke_multicloud_v1/test_aws_clusters.py` & `google-cloud-gke-multicloud-0.6.2/tests/unit/gapic/gke_multicloud_v1/test_aws_clusters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1900,17 +1900,19 @@
                     aws_resources.AwsCluster(),
                     aws_resources.AwsCluster(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_aws_clusters(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3523,17 +3525,19 @@
                     aws_resources.AwsNodePool(),
                     aws_resources.AwsNodePool(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_aws_node_pools(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-gke-multicloud-0.6.1/tests/unit/gapic/gke_multicloud_v1/test_azure_clusters.py` & `google-cloud-gke-multicloud-0.6.2/tests/unit/gapic/gke_multicloud_v1/test_azure_clusters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1661,17 +1661,19 @@
                     azure_resources.AzureClient(),
                     azure_resources.AzureClient(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_azure_clients(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3141,17 +3143,19 @@
                     azure_resources.AzureCluster(),
                     azure_resources.AzureCluster(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_azure_clusters(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4772,17 +4776,19 @@
                     azure_resources.AzureNodePool(),
                     azure_resources.AzureNodePool(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_azure_node_pools(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

