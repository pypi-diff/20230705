# Comparing `tmp/google-cloud-bigquery-migration-0.9.0.tar.gz` & `tmp/google-cloud-bigquery-migration-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-bigquery-migration-0.9.0.tar", last modified: Wed Jan 11 15:56:41 2023, max compression
+gzip compressed data, was "google-cloud-bigquery-migration-0.9.1.tar", last modified: Mon Jan 23 16:17:02 2023, max compression
```

## Comparing `google-cloud-bigquery-migration-0.9.0.tar` & `google-cloud-bigquery-migration-0.9.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:56:41.918554 google-cloud-bigquery-migration-0.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4768 2023-01-11 15:56:41.918554 google-cloud-bigquery-migration-0.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3832 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:56:41.902554 google-cloud-bigquery-migration-0.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:56:41.906554 google-cloud-bigquery-migration-0.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:56:41.906554 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration/
--rw-rw-r--   0 root         (0)     1003     3380 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       92 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:56:41.906554 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/
--rw-rw-r--   0 root         (0)     1003     3040 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     2531 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       92 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:56:41.906554 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:56:41.910554 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/services/migration_service/
--rw-rw-r--   0 root         (0)     1003      777 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/services/migration_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    41608 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/services/migration_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    51477 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/services/migration_service/client.py
--rw-rw-r--   0 root         (0)     1003    11728 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/services/migration_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:56:41.910554 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/services/migration_service/transports/
--rw-rw-r--   0 root         (0)     1003     1211 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/services/migration_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10341 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/services/migration_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    19663 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/services/migration_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20030 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/services/migration_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:56:41.910554 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/types/
--rw-rw-r--   0 root         (0)     1003     2701 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    10024 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/types/migration_entities.py
--rw-rw-r--   0 root         (0)     1003     3455 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/types/migration_error_details.py
--rw-rw-r--   0 root         (0)     1003     7170 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/types/migration_metrics.py
--rw-rw-r--   0 root         (0)     1003     8820 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/types/migration_service.py
--rw-rw-r--   0 root         (0)     1003    15128 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/types/translation_config.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:56:41.910554 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/
--rw-rw-r--   0 root         (0)     1003     2708 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003     2541 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       92 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:56:41.910554 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:56:41.914554 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/services/migration_service/
--rw-rw-r--   0 root         (0)     1003      777 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/services/migration_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    42415 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/services/migration_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    51662 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/services/migration_service/client.py
--rw-rw-r--   0 root         (0)     1003    11813 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/services/migration_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:56:41.914554 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/services/migration_service/transports/
--rw-rw-r--   0 root         (0)     1003     1211 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/services/migration_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11045 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/services/migration_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    19703 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/services/migration_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20070 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/services/migration_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:56:41.914554 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/types/
--rw-rw-r--   0 root         (0)     1003     2350 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2294 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/types/assessment_task.py
--rw-rw-r--   0 root         (0)     1003    11946 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/types/migration_entities.py
--rw-rw-r--   0 root         (0)     1003     3470 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/types/migration_error_details.py
--rw-rw-r--   0 root         (0)     1003     7194 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/types/migration_metrics.py
--rw-rw-r--   0 root         (0)     1003     8845 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/types/migration_service.py
--rw-rw-r--   0 root         (0)     1003     9909 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/types/translation_task.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:56:41.914554 google-cloud-bigquery-migration-0.9.0/google_cloud_bigquery_migration.egg-info/
--rw-r--r--   0 root         (0)     1003     4768 2023-01-11 15:56:41.000000 google-cloud-bigquery-migration-0.9.0/google_cloud_bigquery_migration.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3559 2023-01-11 15:56:41.000000 google-cloud-bigquery-migration-0.9.0/google_cloud_bigquery_migration.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-11 15:56:41.000000 google-cloud-bigquery-migration-0.9.0/google_cloud_bigquery_migration.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-11 15:56:41.000000 google-cloud-bigquery-migration-0.9.0/google_cloud_bigquery_migration.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-11 15:56:41.000000 google-cloud-bigquery-migration-0.9.0/google_cloud_bigquery_migration.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-01-11 15:56:41.000000 google-cloud-bigquery-migration-0.9.0/google_cloud_bigquery_migration.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-11 15:56:41.000000 google-cloud-bigquery-migration-0.9.0/google_cloud_bigquery_migration.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-01-11 15:56:41.918554 google-cloud-bigquery-migration-0.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3024 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:56:41.914554 google-cloud-bigquery-migration-0.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:56:41.914554 google-cloud-bigquery-migration-0.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:56:41.914554 google-cloud-bigquery-migration-0.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:56:41.918554 google-cloud-bigquery-migration-0.9.0/tests/unit/gapic/bigquery_migration_v2/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/tests/unit/gapic/bigquery_migration_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003   130005 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/tests/unit/gapic/bigquery_migration_v2/test_migration_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:56:41.918554 google-cloud-bigquery-migration-0.9.0/tests/unit/gapic/bigquery_migration_v2alpha/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/tests/unit/gapic/bigquery_migration_v2alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003   130106 2023-01-11 15:53:15.000000 google-cloud-bigquery-migration-0.9.0/tests/unit/gapic/bigquery_migration_v2alpha/test_migration_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:02.990083 google-cloud-bigquery-migration-0.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4768 2023-01-23 16:17:02.990083 google-cloud-bigquery-migration-0.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3832 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:02.974075 google-cloud-bigquery-migration-0.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:02.974075 google-cloud-bigquery-migration-0.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:02.978077 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration/
+-rw-rw-r--   0 root         (0)     1003     3380 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       92 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:02.978077 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/
+-rw-rw-r--   0 root         (0)     1003     3040 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2531 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       92 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:02.978077 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:02.982079 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/services/migration_service/
+-rw-rw-r--   0 root         (0)     1003      777 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/services/migration_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    41608 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/services/migration_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    51505 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/services/migration_service/client.py
+-rw-rw-r--   0 root         (0)     1003    11728 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/services/migration_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:02.982079 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/services/migration_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1211 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/services/migration_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10341 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/services/migration_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    19663 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/services/migration_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    20030 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/services/migration_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:02.982079 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/types/
+-rw-rw-r--   0 root         (0)     1003     2701 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12212 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/types/migration_entities.py
+-rw-rw-r--   0 root         (0)     1003     3455 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/types/migration_error_details.py
+-rw-rw-r--   0 root         (0)     1003     7170 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/types/migration_metrics.py
+-rw-rw-r--   0 root         (0)     1003     8820 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/types/migration_service.py
+-rw-rw-r--   0 root         (0)     1003    16066 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/types/translation_config.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:02.982079 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/
+-rw-rw-r--   0 root         (0)     1003     2708 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2541 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       92 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:02.982079 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:02.982079 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/services/migration_service/
+-rw-rw-r--   0 root         (0)     1003      777 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/services/migration_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    42415 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/services/migration_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    51690 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/services/migration_service/client.py
+-rw-rw-r--   0 root         (0)     1003    11813 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/services/migration_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:02.986081 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/services/migration_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1211 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/services/migration_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11045 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/services/migration_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    19703 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/services/migration_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    20070 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/services/migration_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:02.986081 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/types/
+-rw-rw-r--   0 root         (0)     1003     2350 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2294 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/types/assessment_task.py
+-rw-rw-r--   0 root         (0)     1003    14134 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/types/migration_entities.py
+-rw-rw-r--   0 root         (0)     1003     3470 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/types/migration_error_details.py
+-rw-rw-r--   0 root         (0)     1003     7194 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/types/migration_metrics.py
+-rw-rw-r--   0 root         (0)     1003     8845 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/types/migration_service.py
+-rw-rw-r--   0 root         (0)     1003    11671 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/types/translation_task.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:02.986081 google-cloud-bigquery-migration-0.9.1/google_cloud_bigquery_migration.egg-info/
+-rw-r--r--   0 root         (0)     1003     4768 2023-01-23 16:17:02.000000 google-cloud-bigquery-migration-0.9.1/google_cloud_bigquery_migration.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3559 2023-01-23 16:17:02.000000 google-cloud-bigquery-migration-0.9.1/google_cloud_bigquery_migration.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 16:17:02.000000 google-cloud-bigquery-migration-0.9.1/google_cloud_bigquery_migration.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-01-23 16:17:02.000000 google-cloud-bigquery-migration-0.9.1/google_cloud_bigquery_migration.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 16:17:02.000000 google-cloud-bigquery-migration-0.9.1/google_cloud_bigquery_migration.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-01-23 16:17:02.000000 google-cloud-bigquery-migration-0.9.1/google_cloud_bigquery_migration.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-01-23 16:17:02.000000 google-cloud-bigquery-migration-0.9.1/google_cloud_bigquery_migration.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-01-23 16:17:02.990083 google-cloud-bigquery-migration-0.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3024 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:02.986081 google-cloud-bigquery-migration-0.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:02.986081 google-cloud-bigquery-migration-0.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:02.986081 google-cloud-bigquery-migration-0.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:02.990083 google-cloud-bigquery-migration-0.9.1/tests/unit/gapic/bigquery_migration_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/tests/unit/gapic/bigquery_migration_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   130005 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/tests/unit/gapic/bigquery_migration_v2/test_migration_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:02.990083 google-cloud-bigquery-migration-0.9.1/tests/unit/gapic/bigquery_migration_v2alpha/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/tests/unit/gapic/bigquery_migration_v2alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003   130106 2023-01-23 16:13:48.000000 google-cloud-bigquery-migration-0.9.1/tests/unit/gapic/bigquery_migration_v2alpha/test_migration_service.py
```

### Comparing `google-cloud-bigquery-migration-0.9.0/LICENSE` & `google-cloud-bigquery-migration-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/MANIFEST.in` & `google-cloud-bigquery-migration-0.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/PKG-INFO` & `google-cloud-bigquery-migration-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-migration
-Version: 0.9.0
+Version: 0.9.1
 Summary: Google Cloud Bigquery Migration API client library
 Home-page: https://github.com/googleapis/python-bigquery-migration
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-bigquery-migration-0.9.0/README.rst` & `google-cloud-bigquery-migration-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration/__init__.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration/gapic_version.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration/gapic_version.py`

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
-__version__ = "0.9.0"  # {x-release-please-version}
+__version__ = "0.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/__init__.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/gapic_metadata.json` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/gapic_version.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/gapic_version.py`

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
-__version__ = "0.9.0"  # {x-release-please-version}
+__version__ = "0.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/services/__init__.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/services/migration_service/__init__.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/services/migration_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/services/migration_service/async_client.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/services/migration_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/services/migration_service/client.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/services/migration_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1227,15 +1227,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "MigrationServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/services/migration_service/pagers.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/services/migration_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/services/migration_service/transports/__init__.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/services/migration_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/services/migration_service/transports/base.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/services/migration_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/services/migration_service/transports/grpc.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/services/migration_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/services/migration_service/transports/grpc_asyncio.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/services/migration_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/types/__init__.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/types/migration_entities.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/types/migration_entities.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,15 +59,35 @@
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Time when the workflow was created.
         last_update_time (google.protobuf.timestamp_pb2.Timestamp):
             Time when the workflow was last updated.
     """
 
     class State(proto.Enum):
-        r"""Possible migration workflow states."""
+        r"""Possible migration workflow states.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                Workflow state is unspecified.
+            DRAFT (1):
+                Workflow is in draft status, i.e. tasks are
+                not yet eligible for execution.
+            RUNNING (2):
+                Workflow is running (i.e. tasks are eligible
+                for execution).
+            PAUSED (3):
+                Workflow is paused. Tasks currently in
+                progress may continue, but no further tasks will
+                be scheduled.
+            COMPLETED (4):
+                Workflow is complete. There should not be any
+                task in a non-terminal state, but if they are
+                (e.g. forced termination), they will not be
+                scheduled.
+        """
         STATE_UNSPECIFIED = 0
         DRAFT = 1
         RUNNING = 2
         PAUSED = 3
         COMPLETED = 4
 
     name: str = proto.Field(
@@ -134,15 +154,34 @@
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Time when the task was created.
         last_update_time (google.protobuf.timestamp_pb2.Timestamp):
             Time when the task was last updated.
     """
 
     class State(proto.Enum):
-        r"""Possible states of a migration task."""
+        r"""Possible states of a migration task.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state is unspecified.
+            PENDING (1):
+                The task is waiting for orchestration.
+            ORCHESTRATING (2):
+                The task is assigned to an orchestrator.
+            RUNNING (3):
+                The task is running, i.e. its subtasks are
+                ready for execution.
+            PAUSED (4):
+                Tha task is paused. Assigned subtasks can
+                continue, but no new subtasks will be scheduled.
+            SUCCEEDED (5):
+                The task finished successfully.
+            FAILED (6):
+                The task finished unsuccessfully.
+        """
         STATE_UNSPECIFIED = 0
         PENDING = 1
         ORCHESTRATING = 2
         RUNNING = 3
         PAUSED = 4
         SUCCEEDED = 5
         FAILED = 6
@@ -230,15 +269,35 @@
         last_update_time (google.protobuf.timestamp_pb2.Timestamp):
             Time when the subtask was last updated.
         metrics (MutableSequence[google.cloud.bigquery_migration_v2.types.TimeSeries]):
             The metrics for the subtask.
     """
 
     class State(proto.Enum):
-        r"""Possible states of a migration subtask."""
+        r"""Possible states of a migration subtask.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state is unspecified.
+            ACTIVE (1):
+                The subtask is ready, i.e. it is ready for
+                execution.
+            RUNNING (2):
+                The subtask is running, i.e. it is assigned
+                to a worker for execution.
+            SUCCEEDED (3):
+                The subtask finished successfully.
+            FAILED (4):
+                The subtask finished unsuccessfully.
+            PAUSED (5):
+                The subtask is paused, i.e., it will not be
+                scheduled. If it was already assigned,it might
+                still finish but no new lease renewals will be
+                granted.
+        """
         STATE_UNSPECIFIED = 0
         ACTIVE = 1
         RUNNING = 2
         SUCCEEDED = 3
         FAILED = 4
         PAUSED = 5
```

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/types/migration_error_details.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/types/migration_error_details.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/types/migration_metrics.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/types/migration_metrics.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/types/migration_service.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/types/migration_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2/types/translation_config.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2/types/translation_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -284,15 +284,24 @@
     Attributes:
         mode (google.cloud.bigquery_migration_v2.types.TeradataDialect.Mode):
             Which Teradata sub-dialect mode the user
             specifies.
     """
 
     class Mode(proto.Enum):
-        r"""The sub-dialect options for Teradata."""
+        r"""The sub-dialect options for Teradata.
+
+        Values:
+            MODE_UNSPECIFIED (0):
+                Unspecified mode.
+            SQL (1):
+                Teradata SQL mode.
+            BTEQ (2):
+                BTEQ mode (which includes SQL).
+        """
         MODE_UNSPECIFIED = 0
         SQL = 1
         BTEQ = 2
 
     mode: Mode = proto.Field(
         proto.ENUM,
         number=1,
@@ -400,15 +409,35 @@
             equivalent in the source data warehouse).
         attribute (str):
             The attribute name (BigQuery column
             equivalent in the source data warehouse).
     """
 
     class Type(proto.Enum):
-        r"""The type of the object that is being mapped."""
+        r"""The type of the object that is being mapped.
+
+        Values:
+            TYPE_UNSPECIFIED (0):
+                Unspecified name mapping type.
+            DATABASE (1):
+                The object being mapped is a database.
+            SCHEMA (2):
+                The object being mapped is a schema.
+            RELATION (3):
+                The object being mapped is a relation.
+            ATTRIBUTE (4):
+                The object being mapped is an attribute.
+            RELATION_ALIAS (5):
+                The object being mapped is a relation alias.
+            ATTRIBUTE_ALIAS (6):
+                The object being mapped is a an attribute
+                alias.
+            FUNCTION (7):
+                The object being mapped is a function.
+        """
         TYPE_UNSPECIFIED = 0
         DATABASE = 1
         SCHEMA = 2
         RELATION = 3
         ATTRIBUTE = 4
         RELATION_ALIAS = 5
         ATTRIBUTE_ALIAS = 6
```

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/__init__.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/gapic_metadata.json` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/gapic_version.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/gapic_version.py`

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
-__version__ = "0.9.0"  # {x-release-please-version}
+__version__ = "0.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/services/__init__.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/services/migration_service/__init__.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/services/migration_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/services/migration_service/async_client.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/services/migration_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/services/migration_service/client.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/services/migration_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1227,15 +1227,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "MigrationServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/services/migration_service/pagers.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/services/migration_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/services/migration_service/transports/__init__.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/services/migration_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/services/migration_service/transports/base.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/services/migration_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/services/migration_service/transports/grpc.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/services/migration_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/services/migration_service/transports/grpc_asyncio.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/services/migration_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/types/__init__.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/types/assessment_task.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/types/assessment_task.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/types/migration_entities.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/types/migration_entities.py`

 * *Files 15% similar despite different names*

```diff
@@ -62,15 +62,35 @@
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Time when the workflow was created.
         last_update_time (google.protobuf.timestamp_pb2.Timestamp):
             Time when the workflow was last updated.
     """
 
     class State(proto.Enum):
-        r"""Possible migration workflow states."""
+        r"""Possible migration workflow states.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                Workflow state is unspecified.
+            DRAFT (1):
+                Workflow is in draft status, i.e. tasks are
+                not yet eligible for execution.
+            RUNNING (2):
+                Workflow is running (i.e. tasks are eligible
+                for execution).
+            PAUSED (3):
+                Workflow is paused. Tasks currently in
+                progress may continue, but no further tasks will
+                be scheduled.
+            COMPLETED (4):
+                Workflow is complete. There should not be any
+                task in a non-terminal state, but if they are
+                (e.g. forced termination), they will not be
+                scheduled.
+        """
         STATE_UNSPECIFIED = 0
         DRAFT = 1
         RUNNING = 2
         PAUSED = 3
         COMPLETED = 4
 
     name: str = proto.Field(
@@ -147,15 +167,34 @@
             Time when the task was last updated.
         orchestration_result (google.cloud.bigquery_migration_v2alpha.types.MigrationTaskOrchestrationResult):
             Output only. Additional information about the
             orchestration.
     """
 
     class State(proto.Enum):
-        r"""Possible states of a migration task."""
+        r"""Possible states of a migration task.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state is unspecified.
+            PENDING (1):
+                The task is waiting for orchestration.
+            ORCHESTRATING (2):
+                The task is assigned to an orchestrator.
+            RUNNING (3):
+                The task is running, i.e. its subtasks are
+                ready for execution.
+            PAUSED (4):
+                Tha task is paused. Assigned subtasks can
+                continue, but no new subtasks will be scheduled.
+            SUCCEEDED (5):
+                The task finished successfully.
+            FAILED (6):
+                The task finished unsuccessfully.
+        """
         STATE_UNSPECIFIED = 0
         PENDING = 1
         ORCHESTRATING = 2
         RUNNING = 3
         PAUSED = 4
         SUCCEEDED = 5
         FAILED = 6
@@ -257,15 +296,35 @@
         last_update_time (google.protobuf.timestamp_pb2.Timestamp):
             Time when the subtask was last updated.
         metrics (MutableSequence[google.cloud.bigquery_migration_v2alpha.types.TimeSeries]):
             The metrics for the subtask.
     """
 
     class State(proto.Enum):
-        r"""Possible states of a migration subtask."""
+        r"""Possible states of a migration subtask.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state is unspecified.
+            ACTIVE (1):
+                The subtask is ready, i.e. it is ready for
+                execution.
+            RUNNING (2):
+                The subtask is running, i.e. it is assigned
+                to a worker for execution.
+            SUCCEEDED (3):
+                The subtask finished successfully.
+            FAILED (4):
+                The subtask finished unsuccessfully.
+            PAUSED (5):
+                The subtask is paused, i.e., it will not be
+                scheduled. If it was already assigned,it might
+                still finish but no new lease renewals will be
+                granted.
+        """
         STATE_UNSPECIFIED = 0
         ACTIVE = 1
         RUNNING = 2
         SUCCEEDED = 3
         FAILED = 4
         PAUSED = 5
```

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/types/migration_error_details.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/types/migration_error_details.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/types/migration_metrics.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/types/migration_metrics.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/types/migration_service.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/types/migration_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/google/cloud/bigquery_migration_v2alpha/types/translation_task.py` & `google-cloud-bigquery-migration-0.9.1/google/cloud/bigquery_migration_v2alpha/types/translation_task.py`

 * *Files 19% similar despite different names*

```diff
@@ -112,25 +112,61 @@
             exist, we will create it. If it already exists
             and the schema is the same, we will re-use. If
             the table exists and the schema is different, we
             will throw an error.
     """
 
     class FileEncoding(proto.Enum):
-        r"""The file encoding types."""
+        r"""The file encoding types.
+
+        Values:
+            FILE_ENCODING_UNSPECIFIED (0):
+                File encoding setting is not specified.
+            UTF_8 (1):
+                File encoding is UTF_8.
+            ISO_8859_1 (2):
+                File encoding is ISO_8859_1.
+            US_ASCII (3):
+                File encoding is US_ASCII.
+            UTF_16 (4):
+                File encoding is UTF_16.
+            UTF_16LE (5):
+                File encoding is UTF_16LE.
+            UTF_16BE (6):
+                File encoding is UTF_16BE.
+        """
         FILE_ENCODING_UNSPECIFIED = 0
         UTF_8 = 1
         ISO_8859_1 = 2
         US_ASCII = 3
         UTF_16 = 4
         UTF_16LE = 5
         UTF_16BE = 6
 
     class TokenType(proto.Enum):
-        r"""The special token data type."""
+        r"""The special token data type.
+
+        Values:
+            TOKEN_TYPE_UNSPECIFIED (0):
+                Token type is not specified.
+            STRING (1):
+                Token type as string.
+            INT64 (2):
+                Token type as integer.
+            NUMERIC (3):
+                Token type as numeric.
+            BOOL (4):
+                Token type as boolean.
+            FLOAT64 (5):
+                Token type as float.
+            DATE (6):
+                Token type as date.
+            TIMESTAMP (7):
+                Token type as timestamp.
+        """
         TOKEN_TYPE_UNSPECIFIED = 0
         STRING = 1
         INT64 = 2
         NUMERIC = 3
         BOOL = 4
         FLOAT64 = 5
         DATE = 6
@@ -216,22 +252,43 @@
             identifier case.
         identifier_rewrite_mode (google.cloud.bigquery_migration_v2alpha.types.IdentifierSettings.IdentifierRewriteMode):
             Specifies the rewrite mode for SQL
             identifiers.
     """
 
     class IdentifierCase(proto.Enum):
-        r"""The identifier case type."""
+        r"""The identifier case type.
+
+        Values:
+            IDENTIFIER_CASE_UNSPECIFIED (0):
+                The identifier case is not specified.
+            ORIGINAL (1):
+                Identifiers' cases will be kept as the
+                original cases.
+            UPPER (2):
+                Identifiers will be in upper cases.
+            LOWER (3):
+                Identifiers will be in lower cases.
+        """
         IDENTIFIER_CASE_UNSPECIFIED = 0
         ORIGINAL = 1
         UPPER = 2
         LOWER = 3
 
     class IdentifierRewriteMode(proto.Enum):
-        r"""The SQL identifier rewrite mode."""
+        r"""The SQL identifier rewrite mode.
+
+        Values:
+            IDENTIFIER_REWRITE_MODE_UNSPECIFIED (0):
+                SQL Identifier rewrite mode is unspecified.
+            NONE (1):
+                SQL identifiers won't be rewrite.
+            REWRITE_ALL (2):
+                All SQL identifiers will be rewrite.
+        """
         IDENTIFIER_REWRITE_MODE_UNSPECIFIED = 0
         NONE = 1
         REWRITE_ALL = 2
 
     output_identifier_case: IdentifierCase = proto.Field(
         proto.ENUM,
         number=1,
```

### Comparing `google-cloud-bigquery-migration-0.9.0/google_cloud_bigquery_migration.egg-info/PKG-INFO` & `google-cloud-bigquery-migration-0.9.1/google_cloud_bigquery_migration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-migration
-Version: 0.9.0
+Version: 0.9.1
 Summary: Google Cloud Bigquery Migration API client library
 Home-page: https://github.com/googleapis/python-bigquery-migration
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-bigquery-migration-0.9.0/google_cloud_bigquery_migration.egg-info/SOURCES.txt` & `google-cloud-bigquery-migration-0.9.1/google_cloud_bigquery_migration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/setup.py` & `google-cloud-bigquery-migration-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/tests/__init__.py` & `google-cloud-bigquery-migration-0.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/tests/unit/__init__.py` & `google-cloud-bigquery-migration-0.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/tests/unit/gapic/__init__.py` & `google-cloud-bigquery-migration-0.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/tests/unit/gapic/bigquery_migration_v2/__init__.py` & `google-cloud-bigquery-migration-0.9.1/tests/unit/gapic/bigquery_migration_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/tests/unit/gapic/bigquery_migration_v2/test_migration_service.py` & `google-cloud-bigquery-migration-0.9.1/tests/unit/gapic/bigquery_migration_v2/test_migration_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/tests/unit/gapic/bigquery_migration_v2alpha/__init__.py` & `google-cloud-bigquery-migration-0.9.1/tests/unit/gapic/bigquery_migration_v2alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-migration-0.9.0/tests/unit/gapic/bigquery_migration_v2alpha/test_migration_service.py` & `google-cloud-bigquery-migration-0.9.1/tests/unit/gapic/bigquery_migration_v2alpha/test_migration_service.py`

 * *Files identical despite different names*

