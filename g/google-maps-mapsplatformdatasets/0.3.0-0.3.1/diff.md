# Comparing `tmp/google-maps-mapsplatformdatasets-0.3.0.tar.gz` & `tmp/google-maps-mapsplatformdatasets-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-maps-mapsplatformdatasets-0.3.0.tar", last modified: Mon Jun  5 14:00:13 2023, max compression
+gzip compressed data, was "google-maps-mapsplatformdatasets-0.3.1.tar", last modified: Wed Jul  5 15:57:08 2023, max compression
```

## Comparing `google-maps-mapsplatformdatasets-0.3.0.tar` & `google-maps-mapsplatformdatasets-0.3.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:13.859798 google-maps-mapsplatformdatasets-0.3.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4655 2023-06-05 14:00:13.859798 google-maps-mapsplatformdatasets-0.3.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3723 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:13.843797 google-maps-mapsplatformdatasets-0.3.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:13.847797 google-maps-mapsplatformdatasets-0.3.0/google/maps/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:13.847797 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets/
--rw-rw-r--   0 root         (0)     1003     2059 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:13.847797 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/
--rw-rw-r--   0 root         (0)     1003     1530 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2561 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:13.847797 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:13.851797 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/
--rw-rw-r--   0 root         (0)     1003      793 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/__init__.py
--rw-rw-r--   0 root         (0)     1003    32143 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/async_client.py
--rw-rw-r--   0 root         (0)     1003    41226 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/client.py
--rw-rw-r--   0 root         (0)     1003     5952 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:13.851797 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/
--rw-rw-r--   0 root         (0)     1003     1492 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8756 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/base.py
--rw-rw-r--   0 root         (0)     1003    16605 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16955 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    32138 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:13.851797 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/types/
--rw-rw-r--   0 root         (0)     1003     1195 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2554 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/types/data_source.py
--rw-rw-r--   0 root         (0)     1003     7560 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/types/dataset.py
--rw-rw-r--   0 root         (0)     1003     4790 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/types/maps_platform_datasets.py
--rw-rw-r--   0 root         (0)     1003      778 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/types/maps_platform_datasets_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:13.851797 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/
--rw-rw-r--   0 root         (0)     1003     1772 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003     3415 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:13.851797 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:13.851797 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/
--rw-rw-r--   0 root         (0)     1003      821 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003    41865 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/async_client.py
--rw-rw-r--   0 root         (0)     1003    50915 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/client.py
--rw-rw-r--   0 root         (0)     1003    11389 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:13.855798 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/
--rw-rw-r--   0 root         (0)     1003     1603 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10148 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/base.py
--rw-rw-r--   0 root         (0)     1003    19355 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19762 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    42037 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:13.855798 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/types/
--rw-rw-r--   0 root         (0)     1003     1395 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2754 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/types/data_source.py
--rw-rw-r--   0 root         (0)     1003     6072 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/types/dataset.py
--rw-rw-r--   0 root         (0)     1003     8144 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/types/maps_platform_datasets.py
--rw-rw-r--   0 root         (0)     1003      783 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/types/maps_platform_datasets_alpha_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:13.855798 google-maps-mapsplatformdatasets-0.3.0/google_maps_mapsplatformdatasets.egg-info/
--rw-r--r--   0 root         (0)     1003     4655 2023-06-05 14:00:13.000000 google-maps-mapsplatformdatasets-0.3.0/google_maps_mapsplatformdatasets.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3764 2023-06-05 14:00:13.000000 google-maps-mapsplatformdatasets-0.3.0/google_maps_mapsplatformdatasets.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-05 14:00:13.000000 google-maps-mapsplatformdatasets-0.3.0/google_maps_mapsplatformdatasets.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       19 2023-06-05 14:00:13.000000 google-maps-mapsplatformdatasets-0.3.0/google_maps_mapsplatformdatasets.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-05 14:00:13.000000 google-maps-mapsplatformdatasets-0.3.0/google_maps_mapsplatformdatasets.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-06-05 14:00:13.000000 google-maps-mapsplatformdatasets-0.3.0/google_maps_mapsplatformdatasets.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-05 14:00:13.000000 google-maps-mapsplatformdatasets-0.3.0/google_maps_mapsplatformdatasets.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-06-05 14:00:13.859798 google-maps-mapsplatformdatasets-0.3.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2967 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:13.855798 google-maps-mapsplatformdatasets-0.3.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:13.855798 google-maps-mapsplatformdatasets-0.3.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:13.855798 google-maps-mapsplatformdatasets-0.3.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:13.859798 google-maps-mapsplatformdatasets-0.3.0/tests/unit/gapic/mapsplatformdatasets_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/tests/unit/gapic/mapsplatformdatasets_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   162948 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/tests/unit/gapic/mapsplatformdatasets_v1/test_maps_platform_datasets.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:13.859798 google-maps-mapsplatformdatasets-0.3.0/tests/unit/gapic/mapsplatformdatasets_v1alpha/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/tests/unit/gapic/mapsplatformdatasets_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003   212591 2023-06-05 13:56:51.000000 google-maps-mapsplatformdatasets-0.3.0/tests/unit/gapic/mapsplatformdatasets_v1alpha/test_maps_platform_datasets_v1_alpha.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:08.431838 google-maps-mapsplatformdatasets-0.3.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4655 2023-07-05 15:57:08.431838 google-maps-mapsplatformdatasets-0.3.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3723 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:08.415831 google-maps-mapsplatformdatasets-0.3.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:08.419833 google-maps-mapsplatformdatasets-0.3.1/google/maps/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:08.419833 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets/
+-rw-rw-r--   0 root         (0)     1003     2059 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:08.419833 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/
+-rw-rw-r--   0 root         (0)     1003     1530 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2561 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:08.419833 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:08.423835 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/
+-rw-rw-r--   0 root         (0)     1003      793 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/__init__.py
+-rw-rw-r--   0 root         (0)     1003    32180 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/async_client.py
+-rw-rw-r--   0 root         (0)     1003    41226 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/client.py
+-rw-rw-r--   0 root         (0)     1003     5952 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:08.423835 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/
+-rw-rw-r--   0 root         (0)     1003     1492 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8756 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    16605 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16955 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    32138 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:08.423835 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1195 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2554 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/types/data_source.py
+-rw-rw-r--   0 root         (0)     1003     7560 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/types/dataset.py
+-rw-rw-r--   0 root         (0)     1003     4790 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/types/maps_platform_datasets.py
+-rw-rw-r--   0 root         (0)     1003      778 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/types/maps_platform_datasets_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:08.423835 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/
+-rw-rw-r--   0 root         (0)     1003     1772 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3415 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:08.423835 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:08.427837 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/
+-rw-rw-r--   0 root         (0)     1003      821 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003    41909 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/async_client.py
+-rw-rw-r--   0 root         (0)     1003    50915 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/client.py
+-rw-rw-r--   0 root         (0)     1003    11389 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:08.427837 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/
+-rw-rw-r--   0 root         (0)     1003     1603 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10148 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    19355 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19762 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    42037 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:08.427837 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/types/
+-rw-rw-r--   0 root         (0)     1003     1395 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2754 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/types/data_source.py
+-rw-rw-r--   0 root         (0)     1003     6072 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/types/dataset.py
+-rw-rw-r--   0 root         (0)     1003     8144 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/types/maps_platform_datasets.py
+-rw-rw-r--   0 root         (0)     1003      783 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/types/maps_platform_datasets_alpha_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:08.427837 google-maps-mapsplatformdatasets-0.3.1/google_maps_mapsplatformdatasets.egg-info/
+-rw-r--r--   0 root         (0)     1003     4655 2023-07-05 15:57:08.000000 google-maps-mapsplatformdatasets-0.3.1/google_maps_mapsplatformdatasets.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3764 2023-07-05 15:57:08.000000 google-maps-mapsplatformdatasets-0.3.1/google_maps_mapsplatformdatasets.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:57:08.000000 google-maps-mapsplatformdatasets-0.3.1/google_maps_mapsplatformdatasets.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       19 2023-07-05 15:57:08.000000 google-maps-mapsplatformdatasets-0.3.1/google_maps_mapsplatformdatasets.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:57:08.000000 google-maps-mapsplatformdatasets-0.3.1/google_maps_mapsplatformdatasets.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:57:08.000000 google-maps-mapsplatformdatasets-0.3.1/google_maps_mapsplatformdatasets.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:57:08.000000 google-maps-mapsplatformdatasets-0.3.1/google_maps_mapsplatformdatasets.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:57:08.431838 google-maps-mapsplatformdatasets-0.3.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2967 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:08.427837 google-maps-mapsplatformdatasets-0.3.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:08.431838 google-maps-mapsplatformdatasets-0.3.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:08.431838 google-maps-mapsplatformdatasets-0.3.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:08.431838 google-maps-mapsplatformdatasets-0.3.1/tests/unit/gapic/mapsplatformdatasets_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/tests/unit/gapic/mapsplatformdatasets_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   162631 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/tests/unit/gapic/mapsplatformdatasets_v1/test_maps_platform_datasets.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:08.431838 google-maps-mapsplatformdatasets-0.3.1/tests/unit/gapic/mapsplatformdatasets_v1alpha/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/tests/unit/gapic/mapsplatformdatasets_v1alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003   212473 2023-07-05 15:46:59.000000 google-maps-mapsplatformdatasets-0.3.1/tests/unit/gapic/mapsplatformdatasets_v1alpha/test_maps_platform_datasets_v1_alpha.py
```

### Comparing `google-maps-mapsplatformdatasets-0.3.0/LICENSE` & `google-maps-mapsplatformdatasets-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/MANIFEST.in` & `google-maps-mapsplatformdatasets-0.3.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/PKG-INFO` & `google-maps-mapsplatformdatasets-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-mapsplatformdatasets
-Version: 0.3.0
+Version: 0.3.1
 Summary: Google Maps Mapsplatformdatasets API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-mapsplatformdatasets-0.3.0/README.rst` & `google-maps-mapsplatformdatasets-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets/__init__.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets/gapic_version.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets/gapic_version.py`

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
-__version__ = "0.3.0"  # {x-release-please-version}
+__version__ = "0.3.1"  # {x-release-please-version}
```

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/__init__.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/gapic_metadata.json` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/gapic_version.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.3.1"  # {x-release-please-version}
```

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/__init__.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/__init__.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/async_client.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -775,15 +775,15 @@
         await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "MapsPlatformDatasetsAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/client.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/client.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/pagers.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/pagers.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/__init__.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/base.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/grpc.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/grpc_asyncio.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/rest.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/types/__init__.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/types/data_source.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/types/data_source.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/types/dataset.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/types/dataset.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/types/maps_platform_datasets.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/types/maps_platform_datasets.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1/types/maps_platform_datasets_service.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1/types/maps_platform_datasets_service.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/__init__.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/gapic_metadata.json` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/gapic_version.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/gapic_version.py`

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
-__version__ = "0.3.0"  # {x-release-please-version}
+__version__ = "0.3.1"  # {x-release-please-version}
```

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/__init__.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/__init__.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/async_client.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1009,15 +1009,15 @@
         await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "MapsPlatformDatasetsV1AlphaAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/client.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/client.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/pagers.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/pagers.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/__init__.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/base.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/grpc.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/grpc_asyncio.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/rest.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/types/__init__.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/types/data_source.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/types/data_source.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/types/dataset.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/types/dataset.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/types/maps_platform_datasets.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/types/maps_platform_datasets.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google/maps/mapsplatformdatasets_v1alpha/types/maps_platform_datasets_alpha_service.py` & `google-maps-mapsplatformdatasets-0.3.1/google/maps/mapsplatformdatasets_v1alpha/types/maps_platform_datasets_alpha_service.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google_maps_mapsplatformdatasets.egg-info/PKG-INFO` & `google-maps-mapsplatformdatasets-0.3.1/google_maps_mapsplatformdatasets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-mapsplatformdatasets
-Version: 0.3.0
+Version: 0.3.1
 Summary: Google Maps Mapsplatformdatasets API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-mapsplatformdatasets-0.3.0/google_maps_mapsplatformdatasets.egg-info/SOURCES.txt` & `google-maps-mapsplatformdatasets-0.3.1/google_maps_mapsplatformdatasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/setup.py` & `google-maps-mapsplatformdatasets-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/tests/__init__.py` & `google-maps-mapsplatformdatasets-0.3.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/tests/unit/__init__.py` & `google-maps-mapsplatformdatasets-0.3.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/tests/unit/gapic/__init__.py` & `google-maps-mapsplatformdatasets-0.3.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/tests/unit/gapic/mapsplatformdatasets_v1/__init__.py` & `google-maps-mapsplatformdatasets-0.3.1/tests/unit/gapic/mapsplatformdatasets_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/tests/unit/gapic/mapsplatformdatasets_v1/test_maps_platform_datasets.py` & `google-maps-mapsplatformdatasets-0.3.1/tests/unit/gapic/mapsplatformdatasets_v1/test_maps_platform_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -776,15 +776,14 @@
         call.return_value = gmm_dataset.Dataset(
             name="name_value",
             display_name="display_name_value",
             description="description_value",
             version_id="version_id_value",
             usage=[gmm_dataset.Usage.USAGE_DATA_DRIVEN_STYLING],
             version_description="version_description_value",
-            local_file_source=data_source.LocalFileSource(filename="filename_value"),
         )
         response = client.create_dataset(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == maps_platform_datasets.CreateDatasetRequest()
@@ -1038,15 +1037,14 @@
         call.return_value = gmm_dataset.Dataset(
             name="name_value",
             display_name="display_name_value",
             description="description_value",
             version_id="version_id_value",
             usage=[gmm_dataset.Usage.USAGE_DATA_DRIVEN_STYLING],
             version_description="version_description_value",
-            local_file_source=data_source.LocalFileSource(filename="filename_value"),
         )
         response = client.update_dataset_metadata(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == maps_platform_datasets.UpdateDatasetMetadataRequest()
@@ -1310,15 +1308,14 @@
         call.return_value = dataset.Dataset(
             name="name_value",
             display_name="display_name_value",
             description="description_value",
             version_id="version_id_value",
             usage=[dataset.Usage.USAGE_DATA_DRIVEN_STYLING],
             version_description="version_description_value",
-            local_file_source=data_source.LocalFileSource(filename="filename_value"),
         )
         response = client.get_dataset(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == maps_platform_datasets.GetDatasetRequest()
@@ -1946,17 +1943,19 @@
                     dataset.Dataset(),
                     dataset.Dataset(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_datasets(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2216,15 +2215,14 @@
         return_value = gmm_dataset.Dataset(
             name="name_value",
             display_name="display_name_value",
             description="description_value",
             version_id="version_id_value",
             usage=[gmm_dataset.Usage.USAGE_DATA_DRIVEN_STYLING],
             version_description="version_description_value",
-            local_file_source=data_source.LocalFileSource(filename="filename_value"),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = gmm_dataset.Dataset.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -2530,15 +2528,14 @@
         return_value = gmm_dataset.Dataset(
             name="name_value",
             display_name="display_name_value",
             description="description_value",
             version_id="version_id_value",
             usage=[gmm_dataset.Usage.USAGE_DATA_DRIVEN_STYLING],
             version_description="version_description_value",
-            local_file_source=data_source.LocalFileSource(filename="filename_value"),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = gmm_dataset.Dataset.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -2821,15 +2818,14 @@
         return_value = dataset.Dataset(
             name="name_value",
             display_name="display_name_value",
             description="description_value",
             version_id="version_id_value",
             usage=[dataset.Usage.USAGE_DATA_DRIVEN_STYLING],
             version_description="version_description_value",
-            local_file_source=data_source.LocalFileSource(filename="filename_value"),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = dataset.Dataset.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

### Comparing `google-maps-mapsplatformdatasets-0.3.0/tests/unit/gapic/mapsplatformdatasets_v1alpha/__init__.py` & `google-maps-mapsplatformdatasets-0.3.1/tests/unit/gapic/mapsplatformdatasets_v1alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.0/tests/unit/gapic/mapsplatformdatasets_v1alpha/test_maps_platform_datasets_v1_alpha.py` & `google-maps-mapsplatformdatasets-0.3.1/tests/unit/gapic/mapsplatformdatasets_v1alpha/test_maps_platform_datasets_v1_alpha.py`

 * *Files 1% similar despite different names*

```diff
@@ -786,15 +786,14 @@
             name="name_value",
             display_name="display_name_value",
             description="description_value",
             version_id="version_id_value",
             usage=[gmm_dataset.Usage.USAGE_DATA_DRIVEN_STYLING],
             status=gmm_dataset.State.STATE_IMPORTING,
             version_description="version_description_value",
-            local_file_source=data_source.LocalFileSource(filename="filename_value"),
         )
         response = client.create_dataset(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == maps_platform_datasets.CreateDatasetRequest()
@@ -1052,15 +1051,14 @@
             name="name_value",
             display_name="display_name_value",
             description="description_value",
             version_id="version_id_value",
             usage=[gmm_dataset.Usage.USAGE_DATA_DRIVEN_STYLING],
             status=gmm_dataset.State.STATE_IMPORTING,
             version_description="version_description_value",
-            local_file_source=data_source.LocalFileSource(filename="filename_value"),
         )
         response = client.update_dataset_metadata(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == maps_platform_datasets.UpdateDatasetMetadataRequest()
@@ -1328,15 +1326,14 @@
             name="name_value",
             display_name="display_name_value",
             description="description_value",
             version_id="version_id_value",
             usage=[dataset.Usage.USAGE_DATA_DRIVEN_STYLING],
             status=dataset.State.STATE_IMPORTING,
             version_description="version_description_value",
-            local_file_source=data_source.LocalFileSource(filename="filename_value"),
         )
         response = client.get_dataset(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == maps_platform_datasets.GetDatasetRequest()
@@ -1989,17 +1986,19 @@
                     dataset.Dataset(),
                     dataset.Dataset(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_dataset_versions(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2410,17 +2409,19 @@
                     dataset.Dataset(),
                     dataset.Dataset(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_datasets(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2916,15 +2917,14 @@
             name="name_value",
             display_name="display_name_value",
             description="description_value",
             version_id="version_id_value",
             usage=[gmm_dataset.Usage.USAGE_DATA_DRIVEN_STYLING],
             status=gmm_dataset.State.STATE_IMPORTING,
             version_description="version_description_value",
-            local_file_source=data_source.LocalFileSource(filename="filename_value"),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = gmm_dataset.Dataset.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -3232,15 +3232,14 @@
             name="name_value",
             display_name="display_name_value",
             description="description_value",
             version_id="version_id_value",
             usage=[gmm_dataset.Usage.USAGE_DATA_DRIVEN_STYLING],
             status=gmm_dataset.State.STATE_IMPORTING,
             version_description="version_description_value",
-            local_file_source=data_source.LocalFileSource(filename="filename_value"),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = gmm_dataset.Dataset.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -3527,15 +3526,14 @@
             name="name_value",
             display_name="display_name_value",
             description="description_value",
             version_id="version_id_value",
             usage=[dataset.Usage.USAGE_DATA_DRIVEN_STYLING],
             status=dataset.State.STATE_IMPORTING,
             version_description="version_description_value",
-            local_file_source=data_source.LocalFileSource(filename="filename_value"),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = dataset.Dataset.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

