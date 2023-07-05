# Comparing `tmp/google-cloud-rapidmigrationassessment-0.1.0.tar.gz` & `tmp/google-cloud-rapidmigrationassessment-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-rapidmigrationassessment-0.1.0.tar", last modified: Mon May 29 16:32:57 2023, max compression
+gzip compressed data, was "google-cloud-rapidmigrationassessment-0.1.1.tar", last modified: Wed Jul  5 15:54:53 2023, max compression
```

## Comparing `google-cloud-rapidmigrationassessment-0.1.0.tar` & `google-cloud-rapidmigrationassessment-0.1.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-29 16:32:57.563210 google-cloud-rapidmigrationassessment-0.1.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4871 2023-05-29 16:32:57.563210 google-cloud-rapidmigrationassessment-0.1.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3929 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-29 16:32:57.555209 google-cloud-rapidmigrationassessment-0.1.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-29 16:32:57.555209 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-29 16:32:57.559210 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment/
--rw-rw-r--   0 root         (0)     1003     2087 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       98 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-29 16:32:57.559210 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/
--rw-rw-r--   0 root         (0)     1003     1836 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4486 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       98 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-29 16:32:57.559210 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-29 16:32:57.559210 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/
--rw-rw-r--   0 root         (0)     1003      809 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/__init__.py
--rw-rw-r--   0 root         (0)     1003    71138 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/async_client.py
--rw-rw-r--   0 root         (0)     1003    81012 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/client.py
--rw-rw-r--   0 root         (0)     1003     6148 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-29 16:32:57.563210 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/
--rw-rw-r--   0 root         (0)     1003     1561 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    13148 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/base.py
--rw-rw-r--   0 root         (0)     1003    28414 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    28953 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    83561 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-29 16:32:57.563210 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/types/
--rw-rw-r--   0 root         (0)     1003     1482 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     8088 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/types/api_entities.py
--rw-rw-r--   0 root         (0)     1003    14805 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/types/rapidmigrationassessment.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-29 16:32:57.563210 google-cloud-rapidmigrationassessment-0.1.0/google_cloud_rapidmigrationassessment.egg-info/
--rw-r--r--   0 root         (0)     1003     4871 2023-05-29 16:32:57.000000 google-cloud-rapidmigrationassessment-0.1.0/google_cloud_rapidmigrationassessment.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2161 2023-05-29 16:32:57.000000 google-cloud-rapidmigrationassessment-0.1.0/google_cloud_rapidmigrationassessment.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-29 16:32:57.000000 google-cloud-rapidmigrationassessment-0.1.0/google_cloud_rapidmigrationassessment.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-05-29 16:32:57.000000 google-cloud-rapidmigrationassessment-0.1.0/google_cloud_rapidmigrationassessment.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-29 16:32:57.000000 google-cloud-rapidmigrationassessment-0.1.0/google_cloud_rapidmigrationassessment.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-05-29 16:32:57.000000 google-cloud-rapidmigrationassessment-0.1.0/google_cloud_rapidmigrationassessment.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-05-29 16:32:57.000000 google-cloud-rapidmigrationassessment-0.1.0/google_cloud_rapidmigrationassessment.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-05-29 16:32:57.567210 google-cloud-rapidmigrationassessment-0.1.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2983 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-29 16:32:57.563210 google-cloud-rapidmigrationassessment-0.1.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-29 16:32:57.563210 google-cloud-rapidmigrationassessment-0.1.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-29 16:32:57.563210 google-cloud-rapidmigrationassessment-0.1.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-29 16:32:57.563210 google-cloud-rapidmigrationassessment-0.1.0/tests/unit/gapic/rapidmigrationassessment_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/tests/unit/gapic/rapidmigrationassessment_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   306900 2023-05-29 16:30:25.000000 google-cloud-rapidmigrationassessment-0.1.0/tests/unit/gapic/rapidmigrationassessment_v1/test_rapid_migration_assessment.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:53.807458 google-cloud-rapidmigrationassessment-0.1.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4871 2023-07-05 15:54:53.807458 google-cloud-rapidmigrationassessment-0.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3929 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:53.799459 google-cloud-rapidmigrationassessment-0.1.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:53.799459 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:53.799459 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment/
+-rw-rw-r--   0 root         (0)     1003     2087 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       98 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:53.803459 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/
+-rw-rw-r--   0 root         (0)     1003     1836 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4486 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       98 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:53.803459 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:53.803459 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/
+-rw-rw-r--   0 root         (0)     1003      809 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/__init__.py
+-rw-rw-r--   0 root         (0)     1003    71179 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/async_client.py
+-rw-rw-r--   0 root         (0)     1003    81012 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/client.py
+-rw-rw-r--   0 root         (0)     1003     6148 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:53.803459 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/
+-rw-rw-r--   0 root         (0)     1003     1561 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13148 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    28414 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    28953 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    83549 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:53.803459 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1482 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8088 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/types/api_entities.py
+-rw-rw-r--   0 root         (0)     1003    14805 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/types/rapidmigrationassessment.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:53.807458 google-cloud-rapidmigrationassessment-0.1.1/google_cloud_rapidmigrationassessment.egg-info/
+-rw-r--r--   0 root         (0)     1003     4871 2023-07-05 15:54:53.000000 google-cloud-rapidmigrationassessment-0.1.1/google_cloud_rapidmigrationassessment.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2161 2023-07-05 15:54:53.000000 google-cloud-rapidmigrationassessment-0.1.1/google_cloud_rapidmigrationassessment.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:53.000000 google-cloud-rapidmigrationassessment-0.1.1/google_cloud_rapidmigrationassessment.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:54:53.000000 google-cloud-rapidmigrationassessment-0.1.1/google_cloud_rapidmigrationassessment.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:53.000000 google-cloud-rapidmigrationassessment-0.1.1/google_cloud_rapidmigrationassessment.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:54:53.000000 google-cloud-rapidmigrationassessment-0.1.1/google_cloud_rapidmigrationassessment.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:54:53.000000 google-cloud-rapidmigrationassessment-0.1.1/google_cloud_rapidmigrationassessment.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:54:53.807458 google-cloud-rapidmigrationassessment-0.1.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2983 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:53.807458 google-cloud-rapidmigrationassessment-0.1.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:53.807458 google-cloud-rapidmigrationassessment-0.1.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:53.807458 google-cloud-rapidmigrationassessment-0.1.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:53.807458 google-cloud-rapidmigrationassessment-0.1.1/tests/unit/gapic/rapidmigrationassessment_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/tests/unit/gapic/rapidmigrationassessment_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   307099 2023-07-05 15:46:59.000000 google-cloud-rapidmigrationassessment-0.1.1/tests/unit/gapic/rapidmigrationassessment_v1/test_rapid_migration_assessment.py
```

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/LICENSE` & `google-cloud-rapidmigrationassessment-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/MANIFEST.in` & `google-cloud-rapidmigrationassessment-0.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/PKG-INFO` & `google-cloud-rapidmigrationassessment-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-rapidmigrationassessment
-Version: 0.1.0
+Version: 0.1.1
 Summary: Google Cloud Rapidmigrationassessment API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/README.rst` & `google-cloud-rapidmigrationassessment-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment/__init__.py` & `google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment/gapic_version.py` & `google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.1.1"  # {x-release-please-version}
```

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/__init__.py` & `google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/gapic_metadata.json` & `google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/gapic_version.py` & `google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/gapic_version.py`

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
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.1.1"  # {x-release-please-version}
```

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/__init__.py` & `google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/__init__.py` & `google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/async_client.py` & `google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1765,15 +1765,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "RapidMigrationAssessmentAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/client.py` & `google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/pagers.py` & `google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/__init__.py` & `google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/base.py` & `google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/grpc.py` & `google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/grpc_asyncio.py` & `google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/rest.py` & `google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/services/rapid_migration_assessment/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1908,15 +1908,15 @@
 
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

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/types/__init__.py` & `google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/types/api_entities.py` & `google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/types/api_entities.py`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/google/cloud/rapidmigrationassessment_v1/types/rapidmigrationassessment.py` & `google-cloud-rapidmigrationassessment-0.1.1/google/cloud/rapidmigrationassessment_v1/types/rapidmigrationassessment.py`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/google_cloud_rapidmigrationassessment.egg-info/PKG-INFO` & `google-cloud-rapidmigrationassessment-0.1.1/google_cloud_rapidmigrationassessment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-rapidmigrationassessment
-Version: 0.1.0
+Version: 0.1.1
 Summary: Google Cloud Rapidmigrationassessment API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/google_cloud_rapidmigrationassessment.egg-info/SOURCES.txt` & `google-cloud-rapidmigrationassessment-0.1.1/google_cloud_rapidmigrationassessment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/setup.py` & `google-cloud-rapidmigrationassessment-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/tests/__init__.py` & `google-cloud-rapidmigrationassessment-0.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/tests/unit/__init__.py` & `google-cloud-rapidmigrationassessment-0.1.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/tests/unit/gapic/__init__.py` & `google-cloud-rapidmigrationassessment-0.1.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/tests/unit/gapic/rapidmigrationassessment_v1/__init__.py` & `google-cloud-rapidmigrationassessment-0.1.1/tests/unit/gapic/rapidmigrationassessment_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-rapidmigrationassessment-0.1.0/tests/unit/gapic/rapidmigrationassessment_v1/test_rapid_migration_assessment.py` & `google-cloud-rapidmigrationassessment-0.1.1/tests/unit/gapic/rapidmigrationassessment_v1/test_rapid_migration_assessment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1919,17 +1919,19 @@
                     api_entities.Collector(),
                     api_entities.Collector(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_collectors(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

