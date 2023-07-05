# Comparing `tmp/google-cloud-beyondcorp-appconnections-0.4.2.tar.gz` & `tmp/google-cloud-beyondcorp-appconnections-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-beyondcorp-appconnections-0.4.2.tar", last modified: Mon Mar 27 16:10:17 2023, max compression
+gzip compressed data, was "google-cloud-beyondcorp-appconnections-0.4.3.tar", last modified: Wed Jul  5 15:50:31 2023, max compression
```

## Comparing `google-cloud-beyondcorp-appconnections-0.4.2.tar` & `google-cloud-beyondcorp-appconnections-0.4.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:10:17.587649 google-cloud-beyondcorp-appconnections-0.4.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5027 2023-03-27 16:10:17.587649 google-cloud-beyondcorp-appconnections-0.4.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4070 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:10:17.575652 google-cloud-beyondcorp-appconnections-0.4.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:10:17.579651 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:10:17.579651 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections/
--rw-rw-r--   0 root         (0)     1003     1824 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       99 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:10:17.579651 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/
--rw-rw-r--   0 root         (0)     1003     1634 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3138 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       99 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:10:17.579651 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:10:17.583650 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/
--rw-rw-r--   0 root         (0)     1003      797 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    68340 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    79284 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/client.py
--rw-rw-r--   0 root         (0)     1003    11982 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:10:17.583650 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/
--rw-rw-r--   0 root         (0)     1003     1519 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11257 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    28308 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    28702 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    77073 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:10:17.583650 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/types/
--rw-rw-r--   0 root         (0)     1003     1300 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    23418 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/types/app_connections_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:10:17.583650 google-cloud-beyondcorp-appconnections-0.4.2/google_cloud_beyondcorp_appconnections.egg-info/
--rw-r--r--   0 root         (0)     1003     5027 2023-03-27 16:10:17.000000 google-cloud-beyondcorp-appconnections-0.4.2/google_cloud_beyondcorp_appconnections.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2105 2023-03-27 16:10:17.000000 google-cloud-beyondcorp-appconnections-0.4.2/google_cloud_beyondcorp_appconnections.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:10:17.000000 google-cloud-beyondcorp-appconnections-0.4.2/google_cloud_beyondcorp_appconnections.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 16:10:17.000000 google-cloud-beyondcorp-appconnections-0.4.2/google_cloud_beyondcorp_appconnections.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:10:17.000000 google-cloud-beyondcorp-appconnections-0.4.2/google_cloud_beyondcorp_appconnections.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 16:10:17.000000 google-cloud-beyondcorp-appconnections-0.4.2/google_cloud_beyondcorp_appconnections.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 16:10:17.000000 google-cloud-beyondcorp-appconnections-0.4.2/google_cloud_beyondcorp_appconnections.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 16:10:17.587649 google-cloud-beyondcorp-appconnections-0.4.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3060 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:10:17.583650 google-cloud-beyondcorp-appconnections-0.4.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:10:17.587649 google-cloud-beyondcorp-appconnections-0.4.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:10:17.587649 google-cloud-beyondcorp-appconnections-0.4.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:10:17.587649 google-cloud-beyondcorp-appconnections-0.4.2/tests/unit/gapic/beyondcorp_appconnections_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/tests/unit/gapic/beyondcorp_appconnections_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   272623 2023-03-27 16:07:40.000000 google-cloud-beyondcorp-appconnections-0.4.2/tests/unit/gapic/beyondcorp_appconnections_v1/test_app_connections_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:31.456778 google-cloud-beyondcorp-appconnections-0.4.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4978 2023-07-05 15:50:31.460778 google-cloud-beyondcorp-appconnections-0.4.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4034 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:31.448777 google-cloud-beyondcorp-appconnections-0.4.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:31.448777 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:31.452777 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections/
+-rw-rw-r--   0 root         (0)     1003     1824 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       99 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:31.452777 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/
+-rw-rw-r--   0 root         (0)     1003     1634 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3138 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       99 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:31.452777 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:31.452777 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/
+-rw-rw-r--   0 root         (0)     1003      797 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    68378 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    79284 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/client.py
+-rw-rw-r--   0 root         (0)     1003    11982 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:31.456778 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1519 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11257 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    28308 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    28702 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    77037 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:31.456778 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1300 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    23418 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/types/app_connections_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:31.456778 google-cloud-beyondcorp-appconnections-0.4.3/google_cloud_beyondcorp_appconnections.egg-info/
+-rw-r--r--   0 root         (0)     1003     4978 2023-07-05 15:50:31.000000 google-cloud-beyondcorp-appconnections-0.4.3/google_cloud_beyondcorp_appconnections.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2105 2023-07-05 15:50:31.000000 google-cloud-beyondcorp-appconnections-0.4.3/google_cloud_beyondcorp_appconnections.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:31.000000 google-cloud-beyondcorp-appconnections-0.4.3/google_cloud_beyondcorp_appconnections.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:50:31.000000 google-cloud-beyondcorp-appconnections-0.4.3/google_cloud_beyondcorp_appconnections.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:31.000000 google-cloud-beyondcorp-appconnections-0.4.3/google_cloud_beyondcorp_appconnections.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:50:31.000000 google-cloud-beyondcorp-appconnections-0.4.3/google_cloud_beyondcorp_appconnections.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:50:31.000000 google-cloud-beyondcorp-appconnections-0.4.3/google_cloud_beyondcorp_appconnections.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:50:31.460778 google-cloud-beyondcorp-appconnections-0.4.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3047 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:31.456778 google-cloud-beyondcorp-appconnections-0.4.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:31.456778 google-cloud-beyondcorp-appconnections-0.4.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:31.456778 google-cloud-beyondcorp-appconnections-0.4.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:31.456778 google-cloud-beyondcorp-appconnections-0.4.3/tests/unit/gapic/beyondcorp_appconnections_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/tests/unit/gapic/beyondcorp_appconnections_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   273021 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-appconnections-0.4.3/tests/unit/gapic/beyondcorp_appconnections_v1/test_app_connections_service.py
```

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/LICENSE` & `google-cloud-beyondcorp-appconnections-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/MANIFEST.in` & `google-cloud-beyondcorp-appconnections-0.4.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/PKG-INFO` & `google-cloud-beyondcorp-appconnections-0.4.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-beyondcorp-appconnections
-Version: 0.4.2
+Version: 0.4.3
 Summary: Google Cloud Beyondcorp Appconnections API client library
-Home-page: https://github.com/googleapis/python-beyondcorp-appconnections
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
 
-Python Client for BeyondCorp AppConnections API
-===============================================
+Python Client for BeyondCorp AppConnections
+===========================================
 
 |preview| |pypi| |versions|
 
-`BeyondCorp AppConnections API`_: Beyondcorp Enterprise provides identity and context aware access controls for enterprise resources and enables zero-trust access. Using the Beyondcorp Enterprise APIs, enterprises can set up multi-cloud and on-prem connectivity using the App Connector hybrid connectivity solution.
+`BeyondCorp AppConnections`_: Beyondcorp Enterprise provides identity and context aware access controls for enterprise resources and enables zero-trust access. Using the Beyondcorp Enterprise APIs, enterprises can set up multi-cloud and on-prem connectivity using the App Connector hybrid connectivity solution.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-beyondcorp-appconnections.svg
    :target: https://pypi.org/project/google-cloud-beyondcorp-appconnections/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-beyondcorp-appconnections.svg
    :target: https://pypi.org/project/google-cloud-beyondcorp-appconnections/
-.. _BeyondCorp AppConnections API: https://cloud.google.com/beyondcorp/
+.. _BeyondCorp AppConnections: https://cloud.google.com/beyondcorp/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/beyondcorpappconnections/latest
 .. _Product Documentation:  https://cloud.google.com/beyondcorp/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the BeyondCorp AppConnections API.`_
+3. `Enable the BeyondCorp AppConnections.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the BeyondCorp AppConnections API.:  https://cloud.google.com/beyondcorp/
+.. _Enable the BeyondCorp AppConnections.:  https://cloud.google.com/beyondcorp/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-beyondcorp-appconnections
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for BeyondCorp AppConnections API
+-  Read the `Client Library Documentation`_ for BeyondCorp AppConnections
    to see other available methods on the client.
--  Read the `BeyondCorp AppConnections API Product documentation`_ to learn
+-  Read the `BeyondCorp AppConnections Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _BeyondCorp AppConnections API Product documentation:  https://cloud.google.com/beyondcorp/
+.. _BeyondCorp AppConnections Product documentation:  https://cloud.google.com/beyondcorp/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/README.rst` & `google-cloud-beyondcorp-appconnections-0.4.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for BeyondCorp AppConnections API
-===============================================
+Python Client for BeyondCorp AppConnections
+===========================================
 
 |preview| |pypi| |versions|
 
-`BeyondCorp AppConnections API`_: Beyondcorp Enterprise provides identity and context aware access controls for enterprise resources and enables zero-trust access. Using the Beyondcorp Enterprise APIs, enterprises can set up multi-cloud and on-prem connectivity using the App Connector hybrid connectivity solution.
+`BeyondCorp AppConnections`_: Beyondcorp Enterprise provides identity and context aware access controls for enterprise resources and enables zero-trust access. Using the Beyondcorp Enterprise APIs, enterprises can set up multi-cloud and on-prem connectivity using the App Connector hybrid connectivity solution.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-beyondcorp-appconnections.svg
    :target: https://pypi.org/project/google-cloud-beyondcorp-appconnections/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-beyondcorp-appconnections.svg
    :target: https://pypi.org/project/google-cloud-beyondcorp-appconnections/
-.. _BeyondCorp AppConnections API: https://cloud.google.com/beyondcorp/
+.. _BeyondCorp AppConnections: https://cloud.google.com/beyondcorp/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/beyondcorpappconnections/latest
 .. _Product Documentation:  https://cloud.google.com/beyondcorp/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the BeyondCorp AppConnections API.`_
+3. `Enable the BeyondCorp AppConnections.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the BeyondCorp AppConnections API.:  https://cloud.google.com/beyondcorp/
+.. _Enable the BeyondCorp AppConnections.:  https://cloud.google.com/beyondcorp/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-beyondcorp-appconnections
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for BeyondCorp AppConnections API
+-  Read the `Client Library Documentation`_ for BeyondCorp AppConnections
    to see other available methods on the client.
--  Read the `BeyondCorp AppConnections API Product documentation`_ to learn
+-  Read the `BeyondCorp AppConnections Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _BeyondCorp AppConnections API Product documentation:  https://cloud.google.com/beyondcorp/
+.. _BeyondCorp AppConnections Product documentation:  https://cloud.google.com/beyondcorp/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections/__init__.py` & `google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections/gapic_version.py` & `google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections/gapic_version.py`

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
-__version__ = "0.4.2"  # {x-release-please-version}
+__version__ = "0.4.3"  # {x-release-please-version}
```

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/__init__.py` & `google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/gapic_metadata.json` & `google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/gapic_version.py` & `google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/gapic_version.py`

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
-__version__ = "0.4.2"  # {x-release-please-version}
+__version__ = "0.4.3"  # {x-release-please-version}
```

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/__init__.py` & `google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/__init__.py` & `google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/async_client.py` & `google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1652,15 +1652,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "AppConnectionsServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/client.py` & `google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/pagers.py` & `google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/__init__.py` & `google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/base.py` & `google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/grpc.py` & `google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/grpc_asyncio.py` & `google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/rest.py` & `google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/services/app_connections_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1552,15 +1552,15 @@
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
@@ -1644,15 +1644,15 @@
 
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
@@ -1713,15 +1713,15 @@
 
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

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/types/__init__.py` & `google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/google/cloud/beyondcorp_appconnections_v1/types/app_connections_service.py` & `google-cloud-beyondcorp-appconnections-0.4.3/google/cloud/beyondcorp_appconnections_v1/types/app_connections_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/google_cloud_beyondcorp_appconnections.egg-info/PKG-INFO` & `google-cloud-beyondcorp-appconnections-0.4.3/google_cloud_beyondcorp_appconnections.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-beyondcorp-appconnections
-Version: 0.4.2
+Version: 0.4.3
 Summary: Google Cloud Beyondcorp Appconnections API client library
-Home-page: https://github.com/googleapis/python-beyondcorp-appconnections
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
 
-Python Client for BeyondCorp AppConnections API
-===============================================
+Python Client for BeyondCorp AppConnections
+===========================================
 
 |preview| |pypi| |versions|
 
-`BeyondCorp AppConnections API`_: Beyondcorp Enterprise provides identity and context aware access controls for enterprise resources and enables zero-trust access. Using the Beyondcorp Enterprise APIs, enterprises can set up multi-cloud and on-prem connectivity using the App Connector hybrid connectivity solution.
+`BeyondCorp AppConnections`_: Beyondcorp Enterprise provides identity and context aware access controls for enterprise resources and enables zero-trust access. Using the Beyondcorp Enterprise APIs, enterprises can set up multi-cloud and on-prem connectivity using the App Connector hybrid connectivity solution.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-beyondcorp-appconnections.svg
    :target: https://pypi.org/project/google-cloud-beyondcorp-appconnections/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-beyondcorp-appconnections.svg
    :target: https://pypi.org/project/google-cloud-beyondcorp-appconnections/
-.. _BeyondCorp AppConnections API: https://cloud.google.com/beyondcorp/
+.. _BeyondCorp AppConnections: https://cloud.google.com/beyondcorp/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/beyondcorpappconnections/latest
 .. _Product Documentation:  https://cloud.google.com/beyondcorp/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the BeyondCorp AppConnections API.`_
+3. `Enable the BeyondCorp AppConnections.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the BeyondCorp AppConnections API.:  https://cloud.google.com/beyondcorp/
+.. _Enable the BeyondCorp AppConnections.:  https://cloud.google.com/beyondcorp/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-beyondcorp-appconnections
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for BeyondCorp AppConnections API
+-  Read the `Client Library Documentation`_ for BeyondCorp AppConnections
    to see other available methods on the client.
--  Read the `BeyondCorp AppConnections API Product documentation`_ to learn
+-  Read the `BeyondCorp AppConnections Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _BeyondCorp AppConnections API Product documentation:  https://cloud.google.com/beyondcorp/
+.. _BeyondCorp AppConnections Product documentation:  https://cloud.google.com/beyondcorp/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/google_cloud_beyondcorp_appconnections.egg-info/SOURCES.txt` & `google-cloud-beyondcorp-appconnections-0.4.3/google_cloud_beyondcorp_appconnections.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/setup.py` & `google-cloud-beyondcorp-appconnections-0.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
-url = "https://github.com/googleapis/python-beyondcorp-appconnections"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/tests/__init__.py` & `google-cloud-beyondcorp-appconnections-0.4.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/tests/unit/__init__.py` & `google-cloud-beyondcorp-appconnections-0.4.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/tests/unit/gapic/__init__.py` & `google-cloud-beyondcorp-appconnections-0.4.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/tests/unit/gapic/beyondcorp_appconnections_v1/__init__.py` & `google-cloud-beyondcorp-appconnections-0.4.3/tests/unit/gapic/beyondcorp_appconnections_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-appconnections-0.4.2/tests/unit/gapic/beyondcorp_appconnections_v1/test_app_connections_service.py` & `google-cloud-beyondcorp-appconnections-0.4.3/tests/unit/gapic/beyondcorp_appconnections_v1/test_app_connections_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1204,17 +1204,19 @@
                     app_connections_service.AppConnection(),
                     app_connections_service.AppConnection(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_app_connections(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2683,17 +2685,19 @@
                     app_connections_service.ResolveAppConnectionsResponse.AppConnectionDetails(),
                     app_connections_service.ResolveAppConnectionsResponse.AppConnectionDetails(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.resolve_app_connections(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

