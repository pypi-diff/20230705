# Comparing `tmp/google-cloud-memcache-1.7.1.tar.gz` & `tmp/google-cloud-memcache-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-memcache-1.7.1.tar", last modified: Mon Mar 27 14:58:44 2023, max compression
+gzip compressed data, was "google-cloud-memcache-1.7.2.tar", last modified: Wed Jul  5 15:53:57 2023, max compression
```

## Comparing `google-cloud-memcache-1.7.1.tar` & `google-cloud-memcache-1.7.2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:44.798513 google-cloud-memcache-1.7.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4732 2023-03-27 14:58:44.798513 google-cloud-memcache-1.7.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3813 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:44.786512 google-cloud-memcache-1.7.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:44.786512 google-cloud-memcache-1.7.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:44.786512 google-cloud-memcache-1.7.1/google/cloud/memcache/
--rw-rw-r--   0 root         (0)     1003     1976 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:44.790512 google-cloud-memcache-1.7.1/google/cloud/memcache_v1/
--rw-rw-r--   0 root         (0)     1003     1842 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3666 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:44.790512 google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:44.790512 google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/cloud_memcache/
--rw-rw-r--   0 root         (0)     1003      765 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/cloud_memcache/__init__.py
--rw-rw-r--   0 root         (0)     1003    66362 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/cloud_memcache/async_client.py
--rw-rw-r--   0 root         (0)     1003    76351 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/cloud_memcache/client.py
--rw-rw-r--   0 root         (0)     1003     5802 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/cloud_memcache/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:44.790512 google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/cloud_memcache/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/cloud_memcache/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10854 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/cloud_memcache/transports/base.py
--rw-rw-r--   0 root         (0)     1003    26537 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/cloud_memcache/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    27042 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/cloud_memcache/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    72955 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/cloud_memcache/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:44.790512 google-cloud-memcache-1.7.1/google/cloud/memcache_v1/types/
--rw-rw-r--   0 root         (0)     1003     1579 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    29886 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1/types/cloud_memcache.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:44.790512 google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/
--rw-rw-r--   0 root         (0)     1003     1913 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003     4081 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:44.790512 google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:44.794512 google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/cloud_memcache/
--rw-rw-r--   0 root         (0)     1003      765 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/cloud_memcache/__init__.py
--rw-rw-r--   0 root         (0)     1003    72601 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/cloud_memcache/async_client.py
--rw-rw-r--   0 root         (0)     1003    82738 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/cloud_memcache/client.py
--rw-rw-r--   0 root         (0)     1003     5847 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/cloud_memcache/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:44.794512 google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11326 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/base.py
--rw-rw-r--   0 root         (0)     1003    27813 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    28340 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    78620 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:44.794512 google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/types/
--rw-rw-r--   0 root         (0)     1003     1645 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    31623 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/types/cloud_memcache.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:44.794512 google-cloud-memcache-1.7.1/google_cloud_memcache.egg-info/
--rw-r--r--   0 root         (0)     1003     4732 2023-03-27 14:58:44.000000 google-cloud-memcache-1.7.1/google_cloud_memcache.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2605 2023-03-27 14:58:44.000000 google-cloud-memcache-1.7.1/google_cloud_memcache.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:58:44.000000 google-cloud-memcache-1.7.1/google_cloud_memcache.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:58:44.000000 google-cloud-memcache-1.7.1/google_cloud_memcache.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:58:44.000000 google-cloud-memcache-1.7.1/google_cloud_memcache.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 14:58:44.000000 google-cloud-memcache-1.7.1/google_cloud_memcache.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:58:44.000000 google-cloud-memcache-1.7.1/google_cloud_memcache.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 14:58:44.798513 google-cloud-memcache-1.7.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2925 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:44.794512 google-cloud-memcache-1.7.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:44.798513 google-cloud-memcache-1.7.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:44.798513 google-cloud-memcache-1.7.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:44.798513 google-cloud-memcache-1.7.1/tests/unit/gapic/memcache_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/tests/unit/gapic/memcache_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   268469 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/tests/unit/gapic/memcache_v1/test_cloud_memcache.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:44.798513 google-cloud-memcache-1.7.1/tests/unit/gapic/memcache_v1beta2/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/tests/unit/gapic/memcache_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003   288288 2023-03-27 14:56:02.000000 google-cloud-memcache-1.7.1/tests/unit/gapic/memcache_v1beta2/test_cloud_memcache.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:57.052727 google-cloud-memcache-1.7.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4700 2023-07-05 15:53:57.052727 google-cloud-memcache-1.7.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3777 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:57.036728 google-cloud-memcache-1.7.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:57.036728 google-cloud-memcache-1.7.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:57.040727 google-cloud-memcache-1.7.2/google/cloud/memcache/
+-rw-rw-r--   0 root         (0)     1003     1976 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:57.040727 google-cloud-memcache-1.7.2/google/cloud/memcache_v1/
+-rw-rw-r--   0 root         (0)     1003     1842 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3666 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:57.040727 google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:57.044727 google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/cloud_memcache/
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/cloud_memcache/__init__.py
+-rw-rw-r--   0 root         (0)     1003    66392 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/cloud_memcache/async_client.py
+-rw-rw-r--   0 root         (0)     1003    76351 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/cloud_memcache/client.py
+-rw-rw-r--   0 root         (0)     1003     5802 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/cloud_memcache/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:57.044727 google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/cloud_memcache/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/cloud_memcache/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10854 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/cloud_memcache/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    26537 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/cloud_memcache/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    27042 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/cloud_memcache/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    72943 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/cloud_memcache/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:57.044727 google-cloud-memcache-1.7.2/google/cloud/memcache_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1579 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    29886 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1/types/cloud_memcache.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:57.044727 google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/
+-rw-rw-r--   0 root         (0)     1003     1913 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4081 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:57.044727 google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:57.044727 google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/cloud_memcache/
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/cloud_memcache/__init__.py
+-rw-rw-r--   0 root         (0)     1003    72631 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/cloud_memcache/async_client.py
+-rw-rw-r--   0 root         (0)     1003    82738 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/cloud_memcache/client.py
+-rw-rw-r--   0 root         (0)     1003     5847 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/cloud_memcache/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:57.048727 google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11326 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    27813 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    28340 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    78608 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:57.048727 google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/types/
+-rw-rw-r--   0 root         (0)     1003     1645 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    31623 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/types/cloud_memcache.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:57.048727 google-cloud-memcache-1.7.2/google_cloud_memcache.egg-info/
+-rw-r--r--   0 root         (0)     1003     4700 2023-07-05 15:53:56.000000 google-cloud-memcache-1.7.2/google_cloud_memcache.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2605 2023-07-05 15:53:57.000000 google-cloud-memcache-1.7.2/google_cloud_memcache.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:56.000000 google-cloud-memcache-1.7.2/google_cloud_memcache.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:53:56.000000 google-cloud-memcache-1.7.2/google_cloud_memcache.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:56.000000 google-cloud-memcache-1.7.2/google_cloud_memcache.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:53:56.000000 google-cloud-memcache-1.7.2/google_cloud_memcache.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:53:56.000000 google-cloud-memcache-1.7.2/google_cloud_memcache.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:53:57.052727 google-cloud-memcache-1.7.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2929 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:57.048727 google-cloud-memcache-1.7.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:57.048727 google-cloud-memcache-1.7.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:57.048727 google-cloud-memcache-1.7.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:57.048727 google-cloud-memcache-1.7.2/tests/unit/gapic/memcache_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/tests/unit/gapic/memcache_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   268668 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/tests/unit/gapic/memcache_v1/test_cloud_memcache.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:57.052727 google-cloud-memcache-1.7.2/tests/unit/gapic/memcache_v1beta2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/tests/unit/gapic/memcache_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   288487 2023-07-05 15:46:59.000000 google-cloud-memcache-1.7.2/tests/unit/gapic/memcache_v1beta2/test_cloud_memcache.py
```

### Comparing `google-cloud-memcache-1.7.1/LICENSE` & `google-cloud-memcache-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/MANIFEST.in` & `google-cloud-memcache-1.7.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/PKG-INFO` & `google-cloud-memcache-1.7.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-memcache
-Version: 1.7.1
+Version: 1.7.2
 Summary: Google Cloud Memcache API client library
-Home-page: https://github.com/googleapis/python-memcache
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
 
-Python Client for Cloud Memorystore for Memcached API
-=====================================================
+Python Client for Cloud Memorystore for Memcached
+=================================================
 
 |stable| |pypi| |versions|
 
-`Cloud Memorystore for Memcached API`_: is a fully-managed in-memory data store service for Memcache.
+`Cloud Memorystore for Memcached`_: is a fully-managed in-memory data store service for Memcache.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-memcache.svg
    :target: https://pypi.org/project/google-cloud-memcache/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-memcache.svg
    :target: https://pypi.org/project/google-cloud-memcache/
-.. _Cloud Memorystore for Memcached API: cloud.google.com/memorystore/docs/memcached/
+.. _Cloud Memorystore for Memcached: cloud.google.com/memorystore/docs/memcached/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/memcache/latest
 .. _Product Documentation:  cloud.google.com/memorystore/docs/memcached/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Memorystore for Memcached API.`_
+3. `Enable the Cloud Memorystore for Memcached.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Memorystore for Memcached API.:  cloud.google.com/memorystore/docs/memcached/
+.. _Enable the Cloud Memorystore for Memcached.:  cloud.google.com/memorystore/docs/memcached/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-memcache
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Memorystore for Memcached API
+-  Read the `Client Library Documentation`_ for Cloud Memorystore for Memcached
    to see other available methods on the client.
--  Read the `Cloud Memorystore for Memcached API Product documentation`_ to learn
+-  Read the `Cloud Memorystore for Memcached Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Memorystore for Memcached API Product documentation:  cloud.google.com/memorystore/docs/memcached/
+.. _Cloud Memorystore for Memcached Product documentation:  cloud.google.com/memorystore/docs/memcached/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-memcache-1.7.1/README.rst` & `google-cloud-memcache-1.7.2/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Cloud Memorystore for Memcached API
-=====================================================
+Python Client for Cloud Memorystore for Memcached
+=================================================
 
 |stable| |pypi| |versions|
 
-`Cloud Memorystore for Memcached API`_: is a fully-managed in-memory data store service for Memcache.
+`Cloud Memorystore for Memcached`_: is a fully-managed in-memory data store service for Memcache.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-memcache.svg
    :target: https://pypi.org/project/google-cloud-memcache/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-memcache.svg
    :target: https://pypi.org/project/google-cloud-memcache/
-.. _Cloud Memorystore for Memcached API: cloud.google.com/memorystore/docs/memcached/
+.. _Cloud Memorystore for Memcached: cloud.google.com/memorystore/docs/memcached/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/memcache/latest
 .. _Product Documentation:  cloud.google.com/memorystore/docs/memcached/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Memorystore for Memcached API.`_
+3. `Enable the Cloud Memorystore for Memcached.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Memorystore for Memcached API.:  cloud.google.com/memorystore/docs/memcached/
+.. _Enable the Cloud Memorystore for Memcached.:  cloud.google.com/memorystore/docs/memcached/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-memcache
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Memorystore for Memcached API
+-  Read the `Client Library Documentation`_ for Cloud Memorystore for Memcached
    to see other available methods on the client.
--  Read the `Cloud Memorystore for Memcached API Product documentation`_ to learn
+-  Read the `Cloud Memorystore for Memcached Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Memorystore for Memcached API Product documentation:  cloud.google.com/memorystore/docs/memcached/
+.. _Cloud Memorystore for Memcached Product documentation:  cloud.google.com/memorystore/docs/memcached/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache/__init__.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache/gapic_version.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache/gapic_version.py`

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
-__version__ = "1.7.1"  # {x-release-please-version}
+__version__ = "1.7.2"  # {x-release-please-version}
```

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1/__init__.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1/gapic_metadata.json` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1/gapic_version.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1/gapic_version.py`

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
-__version__ = "1.7.1"  # {x-release-please-version}
+__version__ = "1.7.2"  # {x-release-please-version}
```

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/__init__.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/cloud_memcache/__init__.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/cloud_memcache/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/cloud_memcache/async_client.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/cloud_memcache/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1625,15 +1625,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "CloudMemcacheAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/cloud_memcache/client.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/cloud_memcache/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/cloud_memcache/pagers.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/cloud_memcache/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/cloud_memcache/transports/__init__.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/cloud_memcache/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/cloud_memcache/transports/base.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/cloud_memcache/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/cloud_memcache/transports/grpc.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/cloud_memcache/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/cloud_memcache/transports/grpc_asyncio.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/cloud_memcache/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1/services/cloud_memcache/transports/rest.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1/services/cloud_memcache/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1627,15 +1627,15 @@
 
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

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1/types/__init__.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1/types/cloud_memcache.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1/types/cloud_memcache.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/__init__.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/gapic_metadata.json` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/gapic_version.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/gapic_version.py`

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
-__version__ = "1.7.1"  # {x-release-please-version}
+__version__ = "1.7.2"  # {x-release-please-version}
```

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/__init__.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/cloud_memcache/__init__.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/cloud_memcache/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/cloud_memcache/async_client.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/cloud_memcache/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1772,15 +1772,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "CloudMemcacheAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/cloud_memcache/client.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/cloud_memcache/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/cloud_memcache/pagers.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/cloud_memcache/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/__init__.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/base.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/grpc.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/grpc_asyncio.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/rest.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/services/cloud_memcache/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1767,15 +1767,15 @@
 
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

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/types/__init__.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google/cloud/memcache_v1beta2/types/cloud_memcache.py` & `google-cloud-memcache-1.7.2/google/cloud/memcache_v1beta2/types/cloud_memcache.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/google_cloud_memcache.egg-info/PKG-INFO` & `google-cloud-memcache-1.7.2/google_cloud_memcache.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-memcache
-Version: 1.7.1
+Version: 1.7.2
 Summary: Google Cloud Memcache API client library
-Home-page: https://github.com/googleapis/python-memcache
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
 
-Python Client for Cloud Memorystore for Memcached API
-=====================================================
+Python Client for Cloud Memorystore for Memcached
+=================================================
 
 |stable| |pypi| |versions|
 
-`Cloud Memorystore for Memcached API`_: is a fully-managed in-memory data store service for Memcache.
+`Cloud Memorystore for Memcached`_: is a fully-managed in-memory data store service for Memcache.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-memcache.svg
    :target: https://pypi.org/project/google-cloud-memcache/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-memcache.svg
    :target: https://pypi.org/project/google-cloud-memcache/
-.. _Cloud Memorystore for Memcached API: cloud.google.com/memorystore/docs/memcached/
+.. _Cloud Memorystore for Memcached: cloud.google.com/memorystore/docs/memcached/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/memcache/latest
 .. _Product Documentation:  cloud.google.com/memorystore/docs/memcached/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Memorystore for Memcached API.`_
+3. `Enable the Cloud Memorystore for Memcached.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Memorystore for Memcached API.:  cloud.google.com/memorystore/docs/memcached/
+.. _Enable the Cloud Memorystore for Memcached.:  cloud.google.com/memorystore/docs/memcached/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-memcache
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Memorystore for Memcached API
+-  Read the `Client Library Documentation`_ for Cloud Memorystore for Memcached
    to see other available methods on the client.
--  Read the `Cloud Memorystore for Memcached API Product documentation`_ to learn
+-  Read the `Cloud Memorystore for Memcached Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Memorystore for Memcached API Product documentation:  cloud.google.com/memorystore/docs/memcached/
+.. _Cloud Memorystore for Memcached Product documentation:  cloud.google.com/memorystore/docs/memcached/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-memcache-1.7.1/google_cloud_memcache.egg-info/SOURCES.txt` & `google-cloud-memcache-1.7.2/google_cloud_memcache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/setup.py` & `google-cloud-memcache-1.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-memcache"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-memcache-1.7.1/tests/__init__.py` & `google-cloud-memcache-1.7.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/tests/unit/__init__.py` & `google-cloud-memcache-1.7.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/tests/unit/gapic/__init__.py` & `google-cloud-memcache-1.7.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/tests/unit/gapic/memcache_v1/__init__.py` & `google-cloud-memcache-1.7.2/tests/unit/gapic/memcache_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/tests/unit/gapic/memcache_v1/test_cloud_memcache.py` & `google-cloud-memcache-1.7.2/tests/unit/gapic/memcache_v1/test_cloud_memcache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1131,17 +1131,19 @@
                     cloud_memcache.Instance(),
                     cloud_memcache.Instance(),
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
```

### Comparing `google-cloud-memcache-1.7.1/tests/unit/gapic/memcache_v1beta2/__init__.py` & `google-cloud-memcache-1.7.2/tests/unit/gapic/memcache_v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-memcache-1.7.1/tests/unit/gapic/memcache_v1beta2/test_cloud_memcache.py` & `google-cloud-memcache-1.7.2/tests/unit/gapic/memcache_v1beta2/test_cloud_memcache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1131,17 +1131,19 @@
                     cloud_memcache.Instance(),
                     cloud_memcache.Instance(),
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
```

