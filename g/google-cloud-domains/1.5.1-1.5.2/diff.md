# Comparing `tmp/google-cloud-domains-1.5.1.tar.gz` & `tmp/google-cloud-domains-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-domains-1.5.1.tar", last modified: Mon Mar 27 16:06:05 2023, max compression
+gzip compressed data, was "google-cloud-domains-1.5.2.tar", last modified: Wed Jul  5 15:52:48 2023, max compression
```

## Comparing `google-cloud-domains-1.5.1.tar` & `google-cloud-domains-1.5.2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:05.268424 google-cloud-domains-1.5.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4516 2023-03-27 16:06:05.268424 google-cloud-domains-1.5.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3600 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:05.256422 google-cloud-domains-1.5.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:05.256422 google-cloud-domains-1.5.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:05.260423 google-cloud-domains-1.5.1/google/cloud/domains/
--rw-rw-r--   0 root         (0)     1003     2816 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       81 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:05.260423 google-cloud-domains-1.5.1/google/cloud/domains_v1/
--rw-rw-r--   0 root         (0)     1003     2701 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     6751 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       81 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:05.260423 google-cloud-domains-1.5.1/google/cloud/domains_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:05.260423 google-cloud-domains-1.5.1/google/cloud/domains_v1/services/domains/
--rw-rw-r--   0 root         (0)     1003      741 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1/services/domains/__init__.py
--rw-rw-r--   0 root         (0)     1003   100408 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1/services/domains/async_client.py
--rw-rw-r--   0 root         (0)     1003   111874 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1/services/domains/client.py
--rw-rw-r--   0 root         (0)     1003     5830 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1/services/domains/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:05.260423 google-cloud-domains-1.5.1/google/cloud/domains_v1/services/domains/transports/
--rw-rw-r--   0 root         (0)     1003     1302 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1/services/domains/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12805 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1/services/domains/transports/base.py
--rw-rw-r--   0 root         (0)     1003    33547 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1/services/domains/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    34205 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1/services/domains/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    88944 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1/services/domains/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:05.260423 google-cloud-domains-1.5.1/google/cloud/domains_v1/types/
--rw-rw-r--   0 root         (0)     1003     2470 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    53578 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1/types/domains.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:05.264423 google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/
--rw-rw-r--   0 root         (0)     1003     2706 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     6761 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       81 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:05.264423 google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:05.264423 google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/domains/
--rw-rw-r--   0 root         (0)     1003      741 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/domains/__init__.py
--rw-rw-r--   0 root         (0)     1003   100838 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/domains/async_client.py
--rw-rw-r--   0 root         (0)     1003   112304 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/domains/client.py
--rw-rw-r--   0 root         (0)     1003     5875 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/domains/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:05.264423 google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/domains/transports/
--rw-rw-r--   0 root         (0)     1003     1302 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/domains/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12815 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/domains/transports/base.py
--rw-rw-r--   0 root         (0)     1003    33627 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/domains/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    34285 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/domains/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    89039 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/domains/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:05.264423 google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     2470 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    53788 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/types/domains.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:05.268424 google-cloud-domains-1.5.1/google_cloud_domains.egg-info/
--rw-r--r--   0 root         (0)     1003     4516 2023-03-27 16:06:05.000000 google-cloud-domains-1.5.1/google_cloud_domains.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2405 2023-03-27 16:06:05.000000 google-cloud-domains-1.5.1/google_cloud_domains.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:06:05.000000 google-cloud-domains-1.5.1/google_cloud_domains.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 16:06:05.000000 google-cloud-domains-1.5.1/google_cloud_domains.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:06:05.000000 google-cloud-domains-1.5.1/google_cloud_domains.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 16:06:05.000000 google-cloud-domains-1.5.1/google_cloud_domains.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 16:06:05.000000 google-cloud-domains-1.5.1/google_cloud_domains.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 16:06:05.268424 google-cloud-domains-1.5.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2921 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:05.268424 google-cloud-domains-1.5.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:05.268424 google-cloud-domains-1.5.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:05.268424 google-cloud-domains-1.5.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:05.268424 google-cloud-domains-1.5.1/tests/unit/gapic/domains_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/tests/unit/gapic/domains_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   356928 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/tests/unit/gapic/domains_v1/test_domains.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:05.268424 google-cloud-domains-1.5.1/tests/unit/gapic/domains_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/tests/unit/gapic/domains_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   357033 2023-03-27 16:03:30.000000 google-cloud-domains-1.5.1/tests/unit/gapic/domains_v1beta1/test_domains.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:48.093384 google-cloud-domains-1.5.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4485 2023-07-05 15:52:48.093384 google-cloud-domains-1.5.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3564 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:48.081385 google-cloud-domains-1.5.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:48.081385 google-cloud-domains-1.5.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:48.085384 google-cloud-domains-1.5.2/google/cloud/domains/
+-rw-rw-r--   0 root         (0)     1003     2816 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       81 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:48.085384 google-cloud-domains-1.5.2/google/cloud/domains_v1/
+-rw-rw-r--   0 root         (0)     1003     2701 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6751 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       81 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:48.085384 google-cloud-domains-1.5.2/google/cloud/domains_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:48.085384 google-cloud-domains-1.5.2/google/cloud/domains_v1/services/domains/
+-rw-rw-r--   0 root         (0)     1003      741 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1/services/domains/__init__.py
+-rw-rw-r--   0 root         (0)     1003   100432 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1/services/domains/async_client.py
+-rw-rw-r--   0 root         (0)     1003   111874 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1/services/domains/client.py
+-rw-rw-r--   0 root         (0)     1003     5830 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1/services/domains/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:48.085384 google-cloud-domains-1.5.2/google/cloud/domains_v1/services/domains/transports/
+-rw-rw-r--   0 root         (0)     1003     1302 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1/services/domains/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12805 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1/services/domains/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    33547 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1/services/domains/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    34205 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1/services/domains/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    88944 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1/services/domains/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:48.085384 google-cloud-domains-1.5.2/google/cloud/domains_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2470 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    53578 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1/types/domains.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:48.085384 google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     2706 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6761 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       81 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:48.085384 google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:48.089384 google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/domains/
+-rw-rw-r--   0 root         (0)     1003      741 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/domains/__init__.py
+-rw-rw-r--   0 root         (0)     1003   100862 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/domains/async_client.py
+-rw-rw-r--   0 root         (0)     1003   112304 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/domains/client.py
+-rw-rw-r--   0 root         (0)     1003     5875 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/domains/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:48.089384 google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/domains/transports/
+-rw-rw-r--   0 root         (0)     1003     1302 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/domains/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12815 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/domains/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    33627 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/domains/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    34285 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/domains/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    89039 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/domains/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:48.089384 google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     2470 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    53788 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/types/domains.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:48.089384 google-cloud-domains-1.5.2/google_cloud_domains.egg-info/
+-rw-r--r--   0 root         (0)     1003     4485 2023-07-05 15:52:48.000000 google-cloud-domains-1.5.2/google_cloud_domains.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2405 2023-07-05 15:52:48.000000 google-cloud-domains-1.5.2/google_cloud_domains.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:48.000000 google-cloud-domains-1.5.2/google_cloud_domains.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:52:48.000000 google-cloud-domains-1.5.2/google_cloud_domains.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:48.000000 google-cloud-domains-1.5.2/google_cloud_domains.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:52:48.000000 google-cloud-domains-1.5.2/google_cloud_domains.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:52:48.000000 google-cloud-domains-1.5.2/google_cloud_domains.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:52:48.093384 google-cloud-domains-1.5.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2926 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:48.089384 google-cloud-domains-1.5.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:48.093384 google-cloud-domains-1.5.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:48.093384 google-cloud-domains-1.5.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:48.093384 google-cloud-domains-1.5.2/tests/unit/gapic/domains_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/tests/unit/gapic/domains_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   357127 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/tests/unit/gapic/domains_v1/test_domains.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:48.093384 google-cloud-domains-1.5.2/tests/unit/gapic/domains_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/tests/unit/gapic/domains_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   357232 2023-07-05 15:46:58.000000 google-cloud-domains-1.5.2/tests/unit/gapic/domains_v1beta1/test_domains.py
```

### Comparing `google-cloud-domains-1.5.1/LICENSE` & `google-cloud-domains-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/MANIFEST.in` & `google-cloud-domains-1.5.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/PKG-INFO` & `google-cloud-domains-1.5.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-domains
-Version: 1.5.1
+Version: 1.5.2
 Summary: Google Cloud Domains API client library
-Home-page: https://github.com/googleapis/python-domains
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
 
-Python Client for Cloud Domains API
-===================================
+Python Client for Cloud Domains
+===============================
 
 |stable| |pypi| |versions|
 
-`Cloud Domains API`_: allows you to register and manage domains by using Cloud Domains.
+`Cloud Domains`_: allows you to register and manage domains by using Cloud Domains.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-domains.svg
    :target: https://pypi.org/project/google-cloud-domains/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-domains.svg
    :target: https://pypi.org/project/google-cloud-domains/
-.. _Cloud Domains API: https://cloud.google.com/domains
+.. _Cloud Domains: https://cloud.google.com/domains
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/domains/latest
 .. _Product Documentation:  https://cloud.google.com/domains
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Domains API.`_
+3. `Enable the Cloud Domains.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Domains API.:  https://cloud.google.com/domains
+.. _Enable the Cloud Domains.:  https://cloud.google.com/domains
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-domains
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Domains API
+-  Read the `Client Library Documentation`_ for Cloud Domains
    to see other available methods on the client.
--  Read the `Cloud Domains API Product documentation`_ to learn
+-  Read the `Cloud Domains Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Domains API Product documentation:  https://cloud.google.com/domains
+.. _Cloud Domains Product documentation:  https://cloud.google.com/domains
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-domains-1.5.1/README.rst` & `google-cloud-domains-1.5.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Cloud Domains API
-===================================
+Python Client for Cloud Domains
+===============================
 
 |stable| |pypi| |versions|
 
-`Cloud Domains API`_: allows you to register and manage domains by using Cloud Domains.
+`Cloud Domains`_: allows you to register and manage domains by using Cloud Domains.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-domains.svg
    :target: https://pypi.org/project/google-cloud-domains/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-domains.svg
    :target: https://pypi.org/project/google-cloud-domains/
-.. _Cloud Domains API: https://cloud.google.com/domains
+.. _Cloud Domains: https://cloud.google.com/domains
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/domains/latest
 .. _Product Documentation:  https://cloud.google.com/domains
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Domains API.`_
+3. `Enable the Cloud Domains.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Domains API.:  https://cloud.google.com/domains
+.. _Enable the Cloud Domains.:  https://cloud.google.com/domains
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-domains
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Domains API
+-  Read the `Client Library Documentation`_ for Cloud Domains
    to see other available methods on the client.
--  Read the `Cloud Domains API Product documentation`_ to learn
+-  Read the `Cloud Domains Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Domains API Product documentation:  https://cloud.google.com/domains
+.. _Cloud Domains Product documentation:  https://cloud.google.com/domains
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains/__init__.py` & `google-cloud-domains-1.5.2/google/cloud/domains/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains/gapic_version.py` & `google-cloud-domains-1.5.2/google/cloud/domains/gapic_version.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.5.1"  # {x-release-please-version}
+__version__ = "1.5.2"  # {x-release-please-version}
```

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1/__init__.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1/gapic_metadata.json` & `google-cloud-domains-1.5.2/google/cloud/domains_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1/gapic_version.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1/gapic_version.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.5.1"  # {x-release-please-version}
+__version__ = "1.5.2"  # {x-release-please-version}
```

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1/services/__init__.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1/services/domains/__init__.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1/services/domains/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1/services/domains/async_client.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1/services/domains/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2324,15 +2324,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "DomainsAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1/services/domains/client.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1/services/domains/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1/services/domains/pagers.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1/services/domains/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1/services/domains/transports/__init__.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1/services/domains/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1/services/domains/transports/base.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1/services/domains/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1/services/domains/transports/grpc.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1/services/domains/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1/services/domains/transports/grpc_asyncio.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1/services/domains/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1/services/domains/transports/rest.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1/services/domains/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1/types/__init__.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1/types/domains.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1/types/domains.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/__init__.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/gapic_metadata.json` & `google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/gapic_version.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/gapic_version.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.5.1"  # {x-release-please-version}
+__version__ = "1.5.2"  # {x-release-please-version}
```

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/__init__.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/domains/__init__.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/domains/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/domains/async_client.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/domains/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2324,15 +2324,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "DomainsAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/domains/client.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/domains/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/domains/pagers.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/domains/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/domains/transports/__init__.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/domains/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/domains/transports/base.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/domains/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/domains/transports/grpc.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/domains/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/domains/transports/grpc_asyncio.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/domains/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/services/domains/transports/rest.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/services/domains/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/types/__init__.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google/cloud/domains_v1beta1/types/domains.py` & `google-cloud-domains-1.5.2/google/cloud/domains_v1beta1/types/domains.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/google_cloud_domains.egg-info/PKG-INFO` & `google-cloud-domains-1.5.2/google_cloud_domains.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-domains
-Version: 1.5.1
+Version: 1.5.2
 Summary: Google Cloud Domains API client library
-Home-page: https://github.com/googleapis/python-domains
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
 
-Python Client for Cloud Domains API
-===================================
+Python Client for Cloud Domains
+===============================
 
 |stable| |pypi| |versions|
 
-`Cloud Domains API`_: allows you to register and manage domains by using Cloud Domains.
+`Cloud Domains`_: allows you to register and manage domains by using Cloud Domains.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-domains.svg
    :target: https://pypi.org/project/google-cloud-domains/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-domains.svg
    :target: https://pypi.org/project/google-cloud-domains/
-.. _Cloud Domains API: https://cloud.google.com/domains
+.. _Cloud Domains: https://cloud.google.com/domains
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/domains/latest
 .. _Product Documentation:  https://cloud.google.com/domains
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Domains API.`_
+3. `Enable the Cloud Domains.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Domains API.:  https://cloud.google.com/domains
+.. _Enable the Cloud Domains.:  https://cloud.google.com/domains
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-domains
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Domains API
+-  Read the `Client Library Documentation`_ for Cloud Domains
    to see other available methods on the client.
--  Read the `Cloud Domains API Product documentation`_ to learn
+-  Read the `Cloud Domains Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Domains API Product documentation:  https://cloud.google.com/domains
+.. _Cloud Domains Product documentation:  https://cloud.google.com/domains
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-domains-1.5.1/google_cloud_domains.egg-info/SOURCES.txt` & `google-cloud-domains-1.5.2/google_cloud_domains.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/setup.py` & `google-cloud-domains-1.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-domains"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-domains-1.5.1/tests/__init__.py` & `google-cloud-domains-1.5.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/tests/unit/__init__.py` & `google-cloud-domains-1.5.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/tests/unit/gapic/__init__.py` & `google-cloud-domains-1.5.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/tests/unit/gapic/domains_v1/__init__.py` & `google-cloud-domains-1.5.2/tests/unit/gapic/domains_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/tests/unit/gapic/domains_v1/test_domains.py` & `google-cloud-domains-1.5.2/tests/unit/gapic/domains_v1/test_domains.py`

 * *Files 0% similar despite different names*

```diff
@@ -2343,17 +2343,19 @@
                     domains.Registration(),
                     domains.Registration(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_registrations(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-domains-1.5.1/tests/unit/gapic/domains_v1beta1/__init__.py` & `google-cloud-domains-1.5.2/tests/unit/gapic/domains_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-domains-1.5.1/tests/unit/gapic/domains_v1beta1/test_domains.py` & `google-cloud-domains-1.5.2/tests/unit/gapic/domains_v1beta1/test_domains.py`

 * *Files 0% similar despite different names*

```diff
@@ -2343,17 +2343,19 @@
                     domains.Registration(),
                     domains.Registration(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_registrations(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

