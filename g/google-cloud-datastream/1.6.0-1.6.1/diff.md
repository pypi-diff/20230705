# Comparing `tmp/google-cloud-datastream-1.6.0.tar.gz` & `tmp/google-cloud-datastream-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-datastream-1.6.0.tar", last modified: Wed May 31 18:40:40 2023, max compression
+gzip compressed data, was "google-cloud-datastream-1.6.1.tar", last modified: Wed Jul  5 15:52:24 2023, max compression
```

## Comparing `google-cloud-datastream-1.6.0.tar` & `google-cloud-datastream-1.6.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.058371 google-cloud-datastream-1.6.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4683 2023-05-31 18:40:40.058371 google-cloud-datastream-1.6.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3758 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.042370 google-cloud-datastream-1.6.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.042370 google-cloud-datastream-1.6.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.046371 google-cloud-datastream-1.6.0/google/cloud/datastream/
--rw-rw-r--   0 root         (0)     1003     5078 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.046371 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/
--rw-rw-r--   0 root         (0)     1003     4916 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    10384 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.046371 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.050371 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/
--rw-rw-r--   0 root         (0)     1003      753 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/__init__.py
--rw-rw-r--   0 root         (0)     1003   141640 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/async_client.py
--rw-rw-r--   0 root         (0)     1003   157494 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/client.py
--rw-rw-r--   0 root         (0)     1003    31348 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.050371 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/
--rw-rw-r--   0 root         (0)     1003     1344 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    19242 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/base.py
--rw-rw-r--   0 root         (0)     1003    46386 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    47307 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   160720 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.050371 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/types/
--rw-rw-r--   0 root         (0)     1003     4661 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    44898 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/types/datastream.py
--rw-rw-r--   0 root         (0)     1003    64096 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/types/datastream_resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.050371 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/
--rw-rw-r--   0 root         (0)     1003     4154 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8809 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.050371 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.050371 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/
--rw-rw-r--   0 root         (0)     1003      753 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/__init__.py
--rw-rw-r--   0 root         (0)     1003   111029 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/async_client.py
--rw-rw-r--   0 root         (0)     1003   125201 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/client.py
--rw-rw-r--   0 root         (0)     1003    26460 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.054371 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/
--rw-rw-r--   0 root         (0)     1003     1344 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    15616 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/base.py
--rw-rw-r--   0 root         (0)     1003    36520 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    37308 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   116775 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.054371 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/types/
--rw-rw-r--   0 root         (0)     1003     3893 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    38294 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/types/datastream.py
--rw-rw-r--   0 root         (0)     1003    40603 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/types/datastream_resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.054371 google-cloud-datastream-1.6.0/google_cloud_datastream.egg-info/
--rw-r--r--   0 root         (0)     1003     4683 2023-05-31 18:40:39.000000 google-cloud-datastream-1.6.0/google_cloud_datastream.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2747 2023-05-31 18:40:40.000000 google-cloud-datastream-1.6.0/google_cloud_datastream.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-31 18:40:39.000000 google-cloud-datastream-1.6.0/google_cloud_datastream.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-05-31 18:40:39.000000 google-cloud-datastream-1.6.0/google_cloud_datastream.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-31 18:40:39.000000 google-cloud-datastream-1.6.0/google_cloud_datastream.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-05-31 18:40:39.000000 google-cloud-datastream-1.6.0/google_cloud_datastream.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-05-31 18:40:39.000000 google-cloud-datastream-1.6.0/google_cloud_datastream.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-05-31 18:40:40.058371 google-cloud-datastream-1.6.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2980 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.054371 google-cloud-datastream-1.6.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.054371 google-cloud-datastream-1.6.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.054371 google-cloud-datastream-1.6.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.054371 google-cloud-datastream-1.6.0/tests/unit/gapic/datastream_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/tests/unit/gapic/datastream_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   654798 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/tests/unit/gapic/datastream_v1/test_datastream.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.058371 google-cloud-datastream-1.6.0/tests/unit/gapic/datastream_v1alpha1/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/tests/unit/gapic/datastream_v1alpha1/__init__.py
--rw-rw-r--   0 root         (0)     1003   511456 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/tests/unit/gapic/datastream_v1alpha1/test_datastream.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.085279 google-cloud-datastream-1.6.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4649 2023-07-05 15:52:24.085279 google-cloud-datastream-1.6.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3722 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.069279 google-cloud-datastream-1.6.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.073279 google-cloud-datastream-1.6.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.073279 google-cloud-datastream-1.6.1/google/cloud/datastream/
+-rw-rw-r--   0 root         (0)     1003     5078 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.073279 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/
+-rw-rw-r--   0 root         (0)     1003     4916 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10384 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.073279 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.077279 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/
+-rw-rw-r--   0 root         (0)     1003      753 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/__init__.py
+-rw-rw-r--   0 root         (0)     1003   141667 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/async_client.py
+-rw-rw-r--   0 root         (0)     1003   157494 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/client.py
+-rw-rw-r--   0 root         (0)     1003    31348 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.077279 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/
+-rw-rw-r--   0 root         (0)     1003     1344 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19242 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    46386 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    47307 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   160708 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.077279 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/types/
+-rw-rw-r--   0 root         (0)     1003     4661 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    44898 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/types/datastream.py
+-rw-rw-r--   0 root         (0)     1003    64096 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/types/datastream_resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.077279 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/
+-rw-rw-r--   0 root         (0)     1003     4154 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8809 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.077279 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.081279 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/
+-rw-rw-r--   0 root         (0)     1003      753 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/__init__.py
+-rw-rw-r--   0 root         (0)     1003   111056 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/async_client.py
+-rw-rw-r--   0 root         (0)     1003   125201 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/client.py
+-rw-rw-r--   0 root         (0)     1003    26460 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.081279 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/
+-rw-rw-r--   0 root         (0)     1003     1344 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15616 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    36520 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    37308 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   116775 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.081279 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/types/
+-rw-rw-r--   0 root         (0)     1003     3893 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    38294 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/types/datastream.py
+-rw-rw-r--   0 root         (0)     1003    40603 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/types/datastream_resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.085279 google-cloud-datastream-1.6.1/google_cloud_datastream.egg-info/
+-rw-r--r--   0 root         (0)     1003     4649 2023-07-05 15:52:24.000000 google-cloud-datastream-1.6.1/google_cloud_datastream.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2747 2023-07-05 15:52:24.000000 google-cloud-datastream-1.6.1/google_cloud_datastream.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:24.000000 google-cloud-datastream-1.6.1/google_cloud_datastream.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:52:24.000000 google-cloud-datastream-1.6.1/google_cloud_datastream.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:24.000000 google-cloud-datastream-1.6.1/google_cloud_datastream.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:52:24.000000 google-cloud-datastream-1.6.1/google_cloud_datastream.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:52:24.000000 google-cloud-datastream-1.6.1/google_cloud_datastream.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:52:24.085279 google-cloud-datastream-1.6.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2982 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.085279 google-cloud-datastream-1.6.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.085279 google-cloud-datastream-1.6.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.085279 google-cloud-datastream-1.6.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.085279 google-cloud-datastream-1.6.1/tests/unit/gapic/datastream_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/tests/unit/gapic/datastream_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   654590 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/tests/unit/gapic/datastream_v1/test_datastream.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.085279 google-cloud-datastream-1.6.1/tests/unit/gapic/datastream_v1alpha1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/tests/unit/gapic/datastream_v1alpha1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   510931 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/tests/unit/gapic/datastream_v1alpha1/test_datastream.py
```

### Comparing `google-cloud-datastream-1.6.0/LICENSE` & `google-cloud-datastream-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/MANIFEST.in` & `google-cloud-datastream-1.6.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/PKG-INFO` & `google-cloud-datastream-1.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-datastream
-Version: 1.6.0
+Version: 1.6.1
 Summary: Google Cloud Datastream API client library
-Home-page: https://github.com/googleapis/python-datastream
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
 
-Python Client for Datastream API
-================================
+Python Client for Datastream
+============================
 
 |stable| |pypi| |versions|
 
-`Datastream API`_: is a serverless and easy-to-use change data capture (CDC) and replication service. It allows you to synchronize data across heterogeneous databases and applications reliably, and with minimal latency and downtime.
+`Datastream`_: is a serverless and easy-to-use change data capture (CDC) and replication service. It allows you to synchronize data across heterogeneous databases and applications reliably, and with minimal latency and downtime.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-datastream.svg
    :target: https://pypi.org/project/google-cloud-datastream/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-datastream.svg
    :target: https://pypi.org/project/google-cloud-datastream/
-.. _Datastream API: https://cloud.google.com/datastream/
+.. _Datastream: https://cloud.google.com/datastream/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/datastream/latest
 .. _Product Documentation:  https://cloud.google.com/datastream/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Datastream API.`_
+3. `Enable the Datastream.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Datastream API.:  https://cloud.google.com/datastream/
+.. _Enable the Datastream.:  https://cloud.google.com/datastream/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-datastream
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Datastream API
+-  Read the `Client Library Documentation`_ for Datastream
    to see other available methods on the client.
--  Read the `Datastream API Product documentation`_ to learn
+-  Read the `Datastream Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Datastream API Product documentation:  https://cloud.google.com/datastream/
+.. _Datastream Product documentation:  https://cloud.google.com/datastream/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-datastream-1.6.0/README.rst` & `google-cloud-datastream-1.6.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Datastream API
-================================
+Python Client for Datastream
+============================
 
 |stable| |pypi| |versions|
 
-`Datastream API`_: is a serverless and easy-to-use change data capture (CDC) and replication service. It allows you to synchronize data across heterogeneous databases and applications reliably, and with minimal latency and downtime.
+`Datastream`_: is a serverless and easy-to-use change data capture (CDC) and replication service. It allows you to synchronize data across heterogeneous databases and applications reliably, and with minimal latency and downtime.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-datastream.svg
    :target: https://pypi.org/project/google-cloud-datastream/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-datastream.svg
    :target: https://pypi.org/project/google-cloud-datastream/
-.. _Datastream API: https://cloud.google.com/datastream/
+.. _Datastream: https://cloud.google.com/datastream/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/datastream/latest
 .. _Product Documentation:  https://cloud.google.com/datastream/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Datastream API.`_
+3. `Enable the Datastream.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Datastream API.:  https://cloud.google.com/datastream/
+.. _Enable the Datastream.:  https://cloud.google.com/datastream/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-datastream
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Datastream API
+-  Read the `Client Library Documentation`_ for Datastream
    to see other available methods on the client.
--  Read the `Datastream API Product documentation`_ to learn
+-  Read the `Datastream Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Datastream API Product documentation:  https://cloud.google.com/datastream/
+.. _Datastream Product documentation:  https://cloud.google.com/datastream/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream/__init__.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream/gapic_version.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream/gapic_version.py`

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
-__version__ = "1.6.0"  # {x-release-please-version}
+__version__ = "1.6.1"  # {x-release-please-version}
```

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/__init__.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/gapic_metadata.json` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/gapic_version.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/gapic_version.py`

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
-__version__ = "1.6.0"  # {x-release-please-version}
+__version__ = "1.6.1"  # {x-release-please-version}
```

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/__init__.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/__init__.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/async_client.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3510,15 +3510,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "DatastreamAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/client.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/pagers.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/__init__.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/base.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/grpc.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/grpc_asyncio.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/rest.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -3882,15 +3882,15 @@
 
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

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/types/__init__.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/types/datastream.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/types/datastream.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/types/datastream_resources.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/types/datastream_resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/__init__.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/gapic_metadata.json` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/gapic_version.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/gapic_version.py`

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
-__version__ = "1.6.0"  # {x-release-please-version}
+__version__ = "1.6.1"  # {x-release-please-version}
```

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/__init__.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/__init__.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/async_client.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2733,15 +2733,15 @@
             empty_pb2.Empty,
             metadata_type=datastream.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "DatastreamAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/client.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/pagers.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/__init__.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/base.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc_asyncio.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/rest.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/types/__init__.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/types/datastream.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/types/datastream.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/types/datastream_resources.py` & `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/types/datastream_resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/google_cloud_datastream.egg-info/PKG-INFO` & `google-cloud-datastream-1.6.1/google_cloud_datastream.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-datastream
-Version: 1.6.0
+Version: 1.6.1
 Summary: Google Cloud Datastream API client library
-Home-page: https://github.com/googleapis/python-datastream
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
 
-Python Client for Datastream API
-================================
+Python Client for Datastream
+============================
 
 |stable| |pypi| |versions|
 
-`Datastream API`_: is a serverless and easy-to-use change data capture (CDC) and replication service. It allows you to synchronize data across heterogeneous databases and applications reliably, and with minimal latency and downtime.
+`Datastream`_: is a serverless and easy-to-use change data capture (CDC) and replication service. It allows you to synchronize data across heterogeneous databases and applications reliably, and with minimal latency and downtime.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-datastream.svg
    :target: https://pypi.org/project/google-cloud-datastream/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-datastream.svg
    :target: https://pypi.org/project/google-cloud-datastream/
-.. _Datastream API: https://cloud.google.com/datastream/
+.. _Datastream: https://cloud.google.com/datastream/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/datastream/latest
 .. _Product Documentation:  https://cloud.google.com/datastream/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Datastream API.`_
+3. `Enable the Datastream.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Datastream API.:  https://cloud.google.com/datastream/
+.. _Enable the Datastream.:  https://cloud.google.com/datastream/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-datastream
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Datastream API
+-  Read the `Client Library Documentation`_ for Datastream
    to see other available methods on the client.
--  Read the `Datastream API Product documentation`_ to learn
+-  Read the `Datastream Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Datastream API Product documentation:  https://cloud.google.com/datastream/
+.. _Datastream Product documentation:  https://cloud.google.com/datastream/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-datastream-1.6.0/google_cloud_datastream.egg-info/SOURCES.txt` & `google-cloud-datastream-1.6.1/google_cloud_datastream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/setup.py` & `google-cloud-datastream-1.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
-url = "https://github.com/googleapis/python-datastream"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-datastream-1.6.0/tests/__init__.py` & `google-cloud-datastream-1.6.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/tests/unit/__init__.py` & `google-cloud-datastream-1.6.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/tests/unit/gapic/__init__.py` & `google-cloud-datastream-1.6.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/tests/unit/gapic/datastream_v1/__init__.py` & `google-cloud-datastream-1.6.1/tests/unit/gapic/datastream_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/tests/unit/gapic/datastream_v1/test_datastream.py` & `google-cloud-datastream-1.6.1/tests/unit/gapic/datastream_v1/test_datastream.py`

 * *Files 0% similar despite different names*

```diff
@@ -1136,17 +1136,19 @@
                     datastream_resources.ConnectionProfile(),
                     datastream_resources.ConnectionProfile(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_connection_profiles(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1169,18 +1171,14 @@
     with mock.patch.object(
         type(client.transport.get_connection_profile), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = datastream_resources.ConnectionProfile(
             name="name_value",
             display_name="display_name_value",
-            oracle_profile=datastream_resources.OracleProfile(
-                hostname="hostname_value"
-            ),
-            static_service_ip_connectivity=None,
         )
         response = client.get_connection_profile(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == datastream.GetConnectionProfileRequest()
@@ -2189,21 +2187,15 @@
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.discover_connection_profile), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
-        call.return_value = datastream.DiscoverConnectionProfileResponse(
-            oracle_rdbms=datastream_resources.OracleRdbms(
-                oracle_schemas=[
-                    datastream_resources.OracleSchema(schema="schema_value")
-                ]
-            ),
-        )
+        call.return_value = datastream.DiscoverConnectionProfileResponse()
         response = client.discover_connection_profile(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == datastream.DiscoverConnectionProfileRequest()
 
@@ -2744,17 +2736,19 @@
                     datastream_resources.Stream(),
                     datastream_resources.Stream(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_streams(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2777,21 +2771,14 @@
     with mock.patch.object(type(client.transport.get_stream), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = datastream_resources.Stream(
             name="name_value",
             display_name="display_name_value",
             state=datastream_resources.Stream.State.NOT_STARTED,
             customer_managed_encryption_key="customer_managed_encryption_key_value",
-            backfill_all=datastream_resources.Stream.BackfillAllStrategy(
-                oracle_excluded_objects=datastream_resources.OracleRdbms(
-                    oracle_schemas=[
-                        datastream_resources.OracleSchema(schema="schema_value")
-                    ]
-                )
-            ),
         )
         response = client.get_stream(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == datastream.GetStreamRequest()
@@ -4565,17 +4552,19 @@
                     datastream_resources.StreamObject(),
                     datastream_resources.StreamObject(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_stream_objects(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5469,17 +5458,19 @@
                     str(),
                     str(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.fetch_static_ips(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -6443,17 +6434,19 @@
                     datastream_resources.PrivateConnection(),
                     datastream_resources.PrivateConnection(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_private_connections(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -7598,17 +7591,19 @@
                     datastream_resources.Route(),
                     datastream_resources.Route(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_routes(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -8205,18 +8200,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = datastream_resources.ConnectionProfile(
             name="name_value",
             display_name="display_name_value",
-            oracle_profile=datastream_resources.OracleProfile(
-                hostname="hostname_value"
-            ),
-            static_service_ip_connectivity=None,
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = datastream_resources.ConnectionProfile.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -9548,21 +9539,15 @@
     # send a request that will satisfy transcoding
     request_init = {"parent": "projects/sample1/locations/sample2"}
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
-        return_value = datastream.DiscoverConnectionProfileResponse(
-            oracle_rdbms=datastream_resources.OracleRdbms(
-                oracle_schemas=[
-                    datastream_resources.OracleSchema(schema="schema_value")
-                ]
-            ),
-        )
+        return_value = datastream.DiscoverConnectionProfileResponse()
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = datastream.DiscoverConnectionProfileResponse.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
 
@@ -10112,21 +10097,14 @@
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = datastream_resources.Stream(
             name="name_value",
             display_name="display_name_value",
             state=datastream_resources.Stream.State.NOT_STARTED,
             customer_managed_encryption_key="customer_managed_encryption_key_value",
-            backfill_all=datastream_resources.Stream.BackfillAllStrategy(
-                oracle_excluded_objects=datastream_resources.OracleRdbms(
-                    oracle_schemas=[
-                        datastream_resources.OracleSchema(schema="schema_value")
-                    ]
-                )
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = datastream_resources.Stream.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

### Comparing `google-cloud-datastream-1.6.0/tests/unit/gapic/datastream_v1alpha1/__init__.py` & `google-cloud-datastream-1.6.1/tests/unit/gapic/datastream_v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.0/tests/unit/gapic/datastream_v1alpha1/test_datastream.py` & `google-cloud-datastream-1.6.1/tests/unit/gapic/datastream_v1alpha1/test_datastream.py`

 * *Files 0% similar despite different names*

```diff
@@ -1132,17 +1132,19 @@
                     datastream_resources.ConnectionProfile(),
                     datastream_resources.ConnectionProfile(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_connection_profiles(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1165,18 +1167,14 @@
     with mock.patch.object(
         type(client.transport.get_connection_profile), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = datastream_resources.ConnectionProfile(
             name="name_value",
             display_name="display_name_value",
-            oracle_profile=datastream_resources.OracleProfile(
-                hostname="hostname_value"
-            ),
-            no_connectivity=None,
         )
         response = client.get_connection_profile(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == datastream.GetConnectionProfileRequest()
@@ -2185,21 +2183,15 @@
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.discover_connection_profile), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
-        call.return_value = datastream.DiscoverConnectionProfileResponse(
-            oracle_rdbms=datastream_resources.OracleRdbms(
-                oracle_schemas=[
-                    datastream_resources.OracleSchema(schema_name="schema_name_value")
-                ]
-            ),
-        )
+        call.return_value = datastream.DiscoverConnectionProfileResponse()
         response = client.discover_connection_profile(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == datastream.DiscoverConnectionProfileRequest()
 
@@ -2740,17 +2732,19 @@
                     datastream_resources.Stream(),
                     datastream_resources.Stream(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_streams(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2772,23 +2766,14 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_stream), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = datastream_resources.Stream(
             name="name_value",
             display_name="display_name_value",
             state=datastream_resources.Stream.State.CREATED,
-            backfill_all=datastream_resources.Stream.BackfillAllStrategy(
-                oracle_excluded_objects=datastream_resources.OracleRdbms(
-                    oracle_schemas=[
-                        datastream_resources.OracleSchema(
-                            schema_name="schema_name_value"
-                        )
-                    ]
-                )
-            ),
         )
         response = client.get_stream(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == datastream.GetStreamRequest()
@@ -4265,17 +4250,19 @@
                     str(),
                     str(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.fetch_static_ips(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5239,17 +5226,19 @@
                     datastream_resources.PrivateConnection(),
                     datastream_resources.PrivateConnection(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_private_connections(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -6394,17 +6383,19 @@
                     datastream_resources.Route(),
                     datastream_resources.Route(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_routes(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -7001,18 +6992,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = datastream_resources.ConnectionProfile(
             name="name_value",
             display_name="display_name_value",
-            oracle_profile=datastream_resources.OracleProfile(
-                hostname="hostname_value"
-            ),
-            no_connectivity=None,
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = datastream_resources.ConnectionProfile.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -8328,21 +8315,15 @@
     # send a request that will satisfy transcoding
     request_init = {"parent": "projects/sample1/locations/sample2"}
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
-        return_value = datastream.DiscoverConnectionProfileResponse(
-            oracle_rdbms=datastream_resources.OracleRdbms(
-                oracle_schemas=[
-                    datastream_resources.OracleSchema(schema_name="schema_name_value")
-                ]
-            ),
-        )
+        return_value = datastream.DiscoverConnectionProfileResponse()
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = datastream.DiscoverConnectionProfileResponse.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
 
@@ -8892,23 +8873,14 @@
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = datastream_resources.Stream(
             name="name_value",
             display_name="display_name_value",
             state=datastream_resources.Stream.State.CREATED,
-            backfill_all=datastream_resources.Stream.BackfillAllStrategy(
-                oracle_excluded_objects=datastream_resources.OracleRdbms(
-                    oracle_schemas=[
-                        datastream_resources.OracleSchema(
-                            schema_name="schema_name_value"
-                        )
-                    ]
-                )
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = datastream_resources.Stream.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

