# Comparing `tmp/google-cloud-recommendations-ai-0.8.2.tar.gz` & `tmp/google-cloud-recommendations-ai-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-recommendations-ai-0.8.2.tar", last modified: Mon Oct 10 18:13:00 2022, max compression
+gzip compressed data, was "google-cloud-recommendations-ai-0.9.0.tar", last modified: Thu Dec 15 19:47:10 2022, max compression
```

## Comparing `google-cloud-recommendations-ai-0.8.2.tar` & `google-cloud-recommendations-ai-0.9.0.tar`

### file list

```diff
@@ -1,93 +1,95 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:13:00.015494 google-cloud-recommendations-ai-0.8.2/
--rw-rw-r--   0 root         (0)     1003    11358 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4518 2022-10-10 18:13:00.015494 google-cloud-recommendations-ai-0.8.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3774 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:12:59.999493 google-cloud-recommendations-ai-0.8.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:12:59.999493 google-cloud-recommendations-ai-0.8.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:13:00.003493 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine/
--rw-rw-r--   0 root         (0)     1003     7335 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine/__init__.py
--rw-rw-r--   0 root         (0)     1003       92 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:13:00.003493 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/
--rw-rw-r--   0 root         (0)     1003     4958 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8024 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       92 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:13:00.003493 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:13:00.003493 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/catalog_service/
--rw-rw-r--   0 root         (0)     1003      769 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/catalog_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    42061 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/catalog_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    49991 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/catalog_service/client.py
--rw-rw-r--   0 root         (0)     1003     6124 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/catalog_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:13:00.007494 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/
--rw-rw-r--   0 root         (0)     1003     1418 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11323 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18767 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19210 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    38722 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:13:00.007494 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/
--rw-rw-r--   0 root         (0)     1003      809 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/__init__.py
--rw-rw-r--   0 root         (0)     1003    25810 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/async_client.py
--rw-rw-r--   0 root         (0)     1003    35561 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/client.py
--rw-rw-r--   0 root         (0)     1003     7184 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:13:00.007494 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/
--rw-rw-r--   0 root         (0)     1003     1566 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8955 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15587 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15881 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    25105 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:13:00.007494 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_service/
--rw-rw-r--   0 root         (0)     1003      781 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17727 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    26754 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_service/client.py
--rw-rw-r--   0 root         (0)     1003     5912 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:13:00.007494 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/
--rw-rw-r--   0 root         (0)     1003     1460 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6618 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    11985 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12215 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12646 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:13:00.011494 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/user_event_service/
--rw-rw-r--   0 root         (0)     1003      777 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/user_event_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    45739 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/user_event_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    53909 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/user_event_service/client.py
--rw-rw-r--   0 root         (0)     1003     6102 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/user_event_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:13:00.011494 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/
--rw-rw-r--   0 root         (0)     1003     1446 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10524 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18217 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18612 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    36755 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:13:00.011494 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     3146 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    10705 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/types/catalog.py
--rw-rw-r--   0 root         (0)     1003     5227 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/types/catalog_service.py
--rw-rw-r--   0 root         (0)     1003     2835 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/types/common.py
--rw-rw-r--   0 root         (0)     1003    12427 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/types/import_.py
--rw-rw-r--   0 root         (0)     1003     4232 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/types/prediction_apikey_registry_service.py
--rw-rw-r--   0 root         (0)     1003    10133 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/types/prediction_service.py
--rw-rw-r--   0 root         (0)     1003      756 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/types/recommendationengine_resources.py
--rw-rw-r--   0 root         (0)     1003    18877 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/types/user_event.py
--rw-rw-r--   0 root         (0)     1003     9957 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/types/user_event_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:13:00.015494 google-cloud-recommendations-ai-0.8.2/google_cloud_recommendations_ai.egg-info/
--rw-r--r--   0 root         (0)     1003     4518 2022-10-10 18:12:59.000000 google-cloud-recommendations-ai-0.8.2/google_cloud_recommendations_ai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     5053 2022-10-10 18:12:59.000000 google-cloud-recommendations-ai-0.8.2/google_cloud_recommendations_ai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 18:12:59.000000 google-cloud-recommendations-ai-0.8.2/google_cloud_recommendations_ai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-10-10 18:12:59.000000 google-cloud-recommendations-ai-0.8.2/google_cloud_recommendations_ai.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 18:12:59.000000 google-cloud-recommendations-ai-0.8.2/google_cloud_recommendations_ai.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      232 2022-10-10 18:12:59.000000 google-cloud-recommendations-ai-0.8.2/google_cloud_recommendations_ai.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-10-10 18:12:59.000000 google-cloud-recommendations-ai-0.8.2/google_cloud_recommendations_ai.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2022-10-10 18:13:00.015494 google-cloud-recommendations-ai-0.8.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2245 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:13:00.015494 google-cloud-recommendations-ai-0.8.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:13:00.015494 google-cloud-recommendations-ai-0.8.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:13:00.015494 google-cloud-recommendations-ai-0.8.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:13:00.015494 google-cloud-recommendations-ai-0.8.2/tests/unit/gapic/recommendationengine_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/tests/unit/gapic/recommendationengine_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   188149 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/tests/unit/gapic/recommendationengine_v1beta1/test_catalog_service.py
--rw-rw-r--   0 root         (0)     1003   133862 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/tests/unit/gapic/recommendationengine_v1beta1/test_prediction_api_key_registry.py
--rw-rw-r--   0 root         (0)     1003    84692 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/tests/unit/gapic/recommendationengine_v1beta1/test_prediction_service.py
--rw-rw-r--   0 root         (0)     1003   169583 2022-10-10 18:09:40.000000 google-cloud-recommendations-ai-0.8.2/tests/unit/gapic/recommendationengine_v1beta1/test_user_event_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 19:47:10.085149 google-cloud-recommendations-ai-0.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4659 2022-12-15 19:47:10.085149 google-cloud-recommendations-ai-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3774 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 19:47:10.073148 google-cloud-recommendations-ai-0.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 19:47:10.073148 google-cloud-recommendations-ai-0.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 19:47:10.073148 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine/
+-rw-rw-r--   0 root         (0)     1003     7458 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       92 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 19:47:10.073148 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     5081 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8024 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       92 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 19:47:10.077148 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 19:47:10.077148 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/catalog_service/
+-rw-rw-r--   0 root         (0)     1003      769 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/catalog_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    42688 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/catalog_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    51163 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/catalog_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6124 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/catalog_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 19:47:10.077148 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1418 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11210 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18867 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19297 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    39048 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 19:47:10.077148 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/
+-rw-rw-r--   0 root         (0)     1003      809 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26107 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/async_client.py
+-rw-rw-r--   0 root         (0)     1003    35748 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/client.py
+-rw-rw-r--   0 root         (0)     1003     7184 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 19:47:10.077148 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/
+-rw-rw-r--   0 root         (0)     1003     1566 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8842 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15687 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15968 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    25052 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 19:47:10.081148 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_service/
+-rw-rw-r--   0 root         (0)     1003      781 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17772 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    26709 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5912 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 19:47:10.081148 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1460 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6505 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12085 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12302 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12403 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 19:47:10.081148 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/user_event_service/
+-rw-rw-r--   0 root         (0)     1003      777 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/user_event_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    46178 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/user_event_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    54214 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/user_event_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6102 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/user_event_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 19:47:10.081148 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1446 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10411 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18317 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18699 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    37005 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 19:47:10.085149 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     3146 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11086 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/types/catalog.py
+-rw-rw-r--   0 root         (0)     1003     5438 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/types/catalog_service.py
+-rw-rw-r--   0 root         (0)     1003     3026 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/types/common.py
+-rw-rw-r--   0 root         (0)     1003    12991 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/types/import_.py
+-rw-rw-r--   0 root         (0)     1003     4421 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/types/prediction_apikey_registry_service.py
+-rw-rw-r--   0 root         (0)     1003    10500 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/types/prediction_service.py
+-rw-rw-r--   0 root         (0)     1003      756 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/types/recommendationengine_resources.py
+-rw-rw-r--   0 root         (0)     1003    19450 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/types/user_event.py
+-rw-rw-r--   0 root         (0)     1003    10236 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/types/user_event_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 19:47:10.085149 google-cloud-recommendations-ai-0.9.0/google_cloud_recommendations_ai.egg-info/
+-rw-r--r--   0 root         (0)     1003     4659 2022-12-15 19:47:10.000000 google-cloud-recommendations-ai-0.9.0/google_cloud_recommendations_ai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     5163 2022-12-15 19:47:10.000000 google-cloud-recommendations-ai-0.9.0/google_cloud_recommendations_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-12-15 19:47:10.000000 google-cloud-recommendations-ai-0.9.0/google_cloud_recommendations_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-12-15 19:47:10.000000 google-cloud-recommendations-ai-0.9.0/google_cloud_recommendations_ai.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-12-15 19:47:10.000000 google-cloud-recommendations-ai-0.9.0/google_cloud_recommendations_ai.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      257 2022-12-15 19:47:10.000000 google-cloud-recommendations-ai-0.9.0/google_cloud_recommendations_ai.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-12-15 19:47:10.000000 google-cloud-recommendations-ai-0.9.0/google_cloud_recommendations_ai.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2022-12-15 19:47:10.089149 google-cloud-recommendations-ai-0.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2913 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 19:47:10.085149 google-cloud-recommendations-ai-0.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 19:47:10.085149 google-cloud-recommendations-ai-0.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 19:47:10.085149 google-cloud-recommendations-ai-0.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 19:47:10.085149 google-cloud-recommendations-ai-0.9.0/tests/unit/gapic/recommendationengine_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/tests/unit/gapic/recommendationengine_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   189305 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/tests/unit/gapic/recommendationengine_v1beta1/test_catalog_service.py
+-rw-rw-r--   0 root         (0)     1003   133964 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/tests/unit/gapic/recommendationengine_v1beta1/test_prediction_api_key_registry.py
+-rw-rw-r--   0 root         (0)     1003    84726 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/tests/unit/gapic/recommendationengine_v1beta1/test_prediction_service.py
+-rw-rw-r--   0 root         (0)     1003   169771 2022-12-15 19:43:50.000000 google-cloud-recommendations-ai-0.9.0/tests/unit/gapic/recommendationengine_v1beta1/test_user_event_service.py
```

### Comparing `google-cloud-recommendations-ai-0.8.2/LICENSE` & `google-cloud-recommendations-ai-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/MANIFEST.in` & `google-cloud-recommendations-ai-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/PKG-INFO` & `google-cloud-recommendations-ai-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: google-cloud-recommendations-ai
-Version: 0.8.2
+Version: 0.9.0
+Summary: Google Cloud Recommendations Ai API client library
 Home-page: https://github.com/googleapis/python-recommendations-ai
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 License-File: LICENSE
 
 Python Client for Recommendations AI API
 ========================================
 
 |preview| |pypi| |versions|
```

### Comparing `google-cloud-recommendations-ai-0.8.2/README.rst` & `google-cloud-recommendations-ai-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine/__init__.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.recommendationengine import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from google.cloud.recommendationengine_v1beta1.services.catalog_service.client import (
     CatalogServiceClient,
 )
 from google.cloud.recommendationengine_v1beta1.services.catalog_service.async_client import (
     CatalogServiceAsyncClient,
 )
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/__init__.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.recommendationengine import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from .services.catalog_service import CatalogServiceClient
 from .services.catalog_service import CatalogServiceAsyncClient
 from .services.prediction_api_key_registry import PredictionApiKeyRegistryClient
 from .services.prediction_api_key_registry import PredictionApiKeyRegistryAsyncClient
 from .services.prediction_service import PredictionServiceClient
 from .services.prediction_service import PredictionServiceAsyncClient
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/gapic_metadata.json` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/__init__.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/catalog_service/__init__.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/catalog_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/catalog_service/async_client.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/catalog_service/async_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
-import pkg_resources
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
+
+from google.cloud.recommendationengine_v1beta1 import gapic_version as package_version
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
@@ -52,15 +63,18 @@
     _client: CatalogServiceClient
 
     DEFAULT_ENDPOINT = CatalogServiceClient.DEFAULT_ENDPOINT
     DEFAULT_MTLS_ENDPOINT = CatalogServiceClient.DEFAULT_MTLS_ENDPOINT
 
     catalog_path = staticmethod(CatalogServiceClient.catalog_path)
     parse_catalog_path = staticmethod(CatalogServiceClient.parse_catalog_path)
-
+    catalog_item_path_path = staticmethod(CatalogServiceClient.catalog_item_path_path)
+    parse_catalog_item_path_path = staticmethod(
+        CatalogServiceClient.parse_catalog_item_path_path
+    )
     common_billing_account_path = staticmethod(
         CatalogServiceClient.common_billing_account_path
     )
     parse_common_billing_account_path = staticmethod(
         CatalogServiceClient.parse_common_billing_account_path
     )
     common_folder_path = staticmethod(CatalogServiceClient.common_folder_path)
@@ -163,17 +177,17 @@
     get_transport_class = functools.partial(
         type(CatalogServiceClient).get_transport_class, type(CatalogServiceClient)
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, CatalogServiceTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the catalog service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -209,20 +223,20 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def create_catalog_item(
         self,
-        request: Union[catalog_service.CreateCatalogItemRequest, dict] = None,
+        request: Optional[Union[catalog_service.CreateCatalogItemRequest, dict]] = None,
         *,
-        parent: str = None,
-        catalog_item: catalog.CatalogItem = None,
+        parent: Optional[str] = None,
+        catalog_item: Optional[catalog.CatalogItem] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> catalog.CatalogItem:
         r"""Creates a catalog item.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -252,15 +266,15 @@
                 # Make the request
                 response = await client.create_catalog_item(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommendationengine_v1beta1.types.CreateCatalogItemRequest, dict]):
+            request (Optional[Union[google.cloud.recommendationengine_v1beta1.types.CreateCatalogItemRequest, dict]]):
                 The request object. Request message for
                 CreateCatalogItem method.
             parent (:class:`str`):
                 Required. The parent catalog resource name, such as
                 ``projects/*/locations/global/catalogs/default_catalog``.
 
                 This corresponds to the ``parent`` field
@@ -335,19 +349,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_catalog_item(
         self,
-        request: Union[catalog_service.GetCatalogItemRequest, dict] = None,
+        request: Optional[Union[catalog_service.GetCatalogItemRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> catalog.CatalogItem:
         r"""Gets a specific catalog item.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -371,15 +385,15 @@
                 # Make the request
                 response = await client.get_catalog_item(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommendationengine_v1beta1.types.GetCatalogItemRequest, dict]):
+            request (Optional[Union[google.cloud.recommendationengine_v1beta1.types.GetCatalogItemRequest, dict]]):
                 The request object. Request message for GetCatalogItem
                 method.
             name (:class:`str`):
                 Required. Full resource name of catalog item, such as
                 ``projects/*/locations/global/catalogs/default_catalog/catalogitems/some_catalog_item_id``.
 
                 This corresponds to the ``name`` field
@@ -447,20 +461,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def list_catalog_items(
         self,
-        request: Union[catalog_service.ListCatalogItemsRequest, dict] = None,
+        request: Optional[Union[catalog_service.ListCatalogItemsRequest, dict]] = None,
         *,
-        parent: str = None,
-        filter: str = None,
+        parent: Optional[str] = None,
+        filter: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListCatalogItemsAsyncPager:
         r"""Gets a list of catalog items.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -485,15 +499,15 @@
                 page_result = client.list_catalog_items(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.recommendationengine_v1beta1.types.ListCatalogItemsRequest, dict]):
+            request (Optional[Union[google.cloud.recommendationengine_v1beta1.types.ListCatalogItemsRequest, dict]]):
                 The request object. Request message for ListCatalogItems
                 method.
             parent (:class:`str`):
                 Required. The parent catalog resource name, such as
                 ``projects/*/locations/global/catalogs/default_catalog``.
 
                 This corresponds to the ``parent`` field
@@ -582,21 +596,21 @@
         )
 
         # Done; return the response.
         return response
 
     async def update_catalog_item(
         self,
-        request: Union[catalog_service.UpdateCatalogItemRequest, dict] = None,
+        request: Optional[Union[catalog_service.UpdateCatalogItemRequest, dict]] = None,
         *,
-        name: str = None,
-        catalog_item: catalog.CatalogItem = None,
-        update_mask: field_mask_pb2.FieldMask = None,
+        name: Optional[str] = None,
+        catalog_item: Optional[catalog.CatalogItem] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> catalog.CatalogItem:
         r"""Updates a catalog item. Partial updating is
         supported. Non-existing items will be created.
 
         .. code-block:: python
 
@@ -627,20 +641,20 @@
                 # Make the request
                 response = await client.update_catalog_item(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommendationengine_v1beta1.types.UpdateCatalogItemRequest, dict]):
+            request (Optional[Union[google.cloud.recommendationengine_v1beta1.types.UpdateCatalogItemRequest, dict]]):
                 The request object. Request message for
                 UpdateCatalogItem method.
             name (:class:`str`):
                 Required. Full resource name of catalog item, such as
-                ``projects/*/locations/global/catalogs/default_catalog/catalogItems/some_catalog_item_id``
+                ``projects/*/locations/global/catalogs/default_catalog/catalogItems/some_catalog_item_id``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             catalog_item (:class:`google.cloud.recommendationengine_v1beta1.types.CatalogItem`):
                 Required. The catalog item to update/create. The
                 'catalog_item_id' field has to match that in the 'name'.
@@ -722,19 +736,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def delete_catalog_item(
         self,
-        request: Union[catalog_service.DeleteCatalogItemRequest, dict] = None,
+        request: Optional[Union[catalog_service.DeleteCatalogItemRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
         r"""Deletes a catalog item.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -755,15 +769,15 @@
                     name="name_value",
                 )
 
                 # Make the request
                 await client.delete_catalog_item(request=request)
 
         Args:
-            request (Union[google.cloud.recommendationengine_v1beta1.types.DeleteCatalogItemRequest, dict]):
+            request (Optional[Union[google.cloud.recommendationengine_v1beta1.types.DeleteCatalogItemRequest, dict]]):
                 The request object. Request message for
                 DeleteCatalogItem method.
             name (:class:`str`):
                 Required. Full resource name of catalog item, such as
                 ``projects/*/locations/global/catalogs/default_catalog/catalogItems/some_catalog_item_id``.
 
                 This corresponds to the ``name`` field
@@ -822,22 +836,22 @@
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
     async def import_catalog_items(
         self,
-        request: Union[import_.ImportCatalogItemsRequest, dict] = None,
+        request: Optional[Union[import_.ImportCatalogItemsRequest, dict]] = None,
         *,
-        parent: str = None,
-        request_id: str = None,
-        input_config: import_.InputConfig = None,
-        errors_config: import_.ImportErrorsConfig = None,
+        parent: Optional[str] = None,
+        request_id: Optional[str] = None,
+        input_config: Optional[import_.InputConfig] = None,
+        errors_config: Optional[import_.ImportErrorsConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Bulk import of multiple catalog items. Request
         processing may be synchronous. No partial updating
         supported. Non-existing items will be created.
 
         Operation.response is of type ImportResponse. Note that
@@ -865,21 +879,21 @@
                 )
 
                 # Make the request
                 operation = client.import_catalog_items(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommendationengine_v1beta1.types.ImportCatalogItemsRequest, dict]):
+            request (Optional[Union[google.cloud.recommendationengine_v1beta1.types.ImportCatalogItemsRequest, dict]]):
                 The request object. Request message for Import methods.
             parent (:class:`str`):
                 Required.
                 ``projects/1234/locations/global/catalogs/default_catalog``
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -996,18 +1010,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-recommendations-ai",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("CatalogServiceAsyncClient",)
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/catalog_service/client.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/catalog_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
-import pkg_resources
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
+
+from google.cloud.recommendationengine_v1beta1 import gapic_version as package_version
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport import mtls  # type: ignore
@@ -61,15 +73,15 @@
     )  # type: Dict[str, Type[CatalogServiceTransport]]
     _transport_registry["grpc"] = CatalogServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = CatalogServiceGrpcAsyncIOTransport
     _transport_registry["rest"] = CatalogServiceRestTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[CatalogServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -191,14 +203,38 @@
         m = re.match(
             r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)/catalogs/(?P<catalog>.+?)$",
             path,
         )
         return m.groupdict() if m else {}
 
     @staticmethod
+    def catalog_item_path_path(
+        project: str,
+        location: str,
+        catalog: str,
+        catalog_item_path: str,
+    ) -> str:
+        """Returns a fully-qualified catalog_item_path string."""
+        return "projects/{project}/locations/{location}/catalogs/{catalog}/catalogItems/{catalog_item_path}".format(
+            project=project,
+            location=location,
+            catalog=catalog,
+            catalog_item_path=catalog_item_path,
+        )
+
+    @staticmethod
+    def parse_catalog_item_path_path(path: str) -> Dict[str, str]:
+        """Parses a catalog_item_path path into its component segments."""
+        m = re.match(
+            r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)/catalogs/(?P<catalog>.+?)/catalogItems/(?P<catalog_item_path>.+?)$",
+            path,
+        )
+        return m.groupdict() if m else {}
+
+    @staticmethod
     def common_billing_account_path(
         billing_account: str,
     ) -> str:
         """Returns a fully-qualified billing_account string."""
         return "billingAccounts/{billing_account}".format(
             billing_account=billing_account,
         )
@@ -338,33 +374,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, CatalogServiceTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, CatalogServiceTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the catalog service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, CatalogServiceTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
-                NOTE: "rest" transport functionality is currently in a
-                beta state (preview). We welcome your feedback via an
-                issue in this library's source repository.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -386,14 +419,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
@@ -438,20 +472,20 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def create_catalog_item(
         self,
-        request: Union[catalog_service.CreateCatalogItemRequest, dict] = None,
+        request: Optional[Union[catalog_service.CreateCatalogItemRequest, dict]] = None,
         *,
-        parent: str = None,
-        catalog_item: catalog.CatalogItem = None,
+        parent: Optional[str] = None,
+        catalog_item: Optional[catalog.CatalogItem] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> catalog.CatalogItem:
         r"""Creates a catalog item.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -554,19 +588,19 @@
         )
 
         # Done; return the response.
         return response
 
     def get_catalog_item(
         self,
-        request: Union[catalog_service.GetCatalogItemRequest, dict] = None,
+        request: Optional[Union[catalog_service.GetCatalogItemRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> catalog.CatalogItem:
         r"""Gets a specific catalog item.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -656,20 +690,20 @@
         )
 
         # Done; return the response.
         return response
 
     def list_catalog_items(
         self,
-        request: Union[catalog_service.ListCatalogItemsRequest, dict] = None,
+        request: Optional[Union[catalog_service.ListCatalogItemsRequest, dict]] = None,
         *,
-        parent: str = None,
-        filter: str = None,
+        parent: Optional[str] = None,
+        filter: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListCatalogItemsPager:
         r"""Gets a list of catalog items.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -781,21 +815,21 @@
         )
 
         # Done; return the response.
         return response
 
     def update_catalog_item(
         self,
-        request: Union[catalog_service.UpdateCatalogItemRequest, dict] = None,
+        request: Optional[Union[catalog_service.UpdateCatalogItemRequest, dict]] = None,
         *,
-        name: str = None,
-        catalog_item: catalog.CatalogItem = None,
-        update_mask: field_mask_pb2.FieldMask = None,
+        name: Optional[str] = None,
+        catalog_item: Optional[catalog.CatalogItem] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> catalog.CatalogItem:
         r"""Updates a catalog item. Partial updating is
         supported. Non-existing items will be created.
 
         .. code-block:: python
 
@@ -831,15 +865,15 @@
 
         Args:
             request (Union[google.cloud.recommendationengine_v1beta1.types.UpdateCatalogItemRequest, dict]):
                 The request object. Request message for
                 UpdateCatalogItem method.
             name (str):
                 Required. Full resource name of catalog item, such as
-                ``projects/*/locations/global/catalogs/default_catalog/catalogItems/some_catalog_item_id``
+                ``projects/*/locations/global/catalogs/default_catalog/catalogItems/some_catalog_item_id``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             catalog_item (google.cloud.recommendationengine_v1beta1.types.CatalogItem):
                 Required. The catalog item to update/create. The
                 'catalog_item_id' field has to match that in the 'name'.
@@ -911,19 +945,19 @@
         )
 
         # Done; return the response.
         return response
 
     def delete_catalog_item(
         self,
-        request: Union[catalog_service.DeleteCatalogItemRequest, dict] = None,
+        request: Optional[Union[catalog_service.DeleteCatalogItemRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
         r"""Deletes a catalog item.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1001,22 +1035,22 @@
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
     def import_catalog_items(
         self,
-        request: Union[import_.ImportCatalogItemsRequest, dict] = None,
+        request: Optional[Union[import_.ImportCatalogItemsRequest, dict]] = None,
         *,
-        parent: str = None,
-        request_id: str = None,
-        input_config: import_.InputConfig = None,
-        errors_config: import_.ImportErrorsConfig = None,
+        parent: Optional[str] = None,
+        request_id: Optional[str] = None,
+        input_config: Optional[import_.InputConfig] = None,
+        errors_config: Optional[import_.ImportErrorsConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Bulk import of multiple catalog items. Request
         processing may be synchronous. No partial updating
         supported. Non-existing items will be created.
 
         Operation.response is of type ImportResponse. Note that
@@ -1172,18 +1206,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-recommendations-ai",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("CatalogServiceClient",)
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/catalog_service/pagers.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/catalog_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/__init__.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/base.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import abc
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Union
-import pkg_resources
+
+from google.cloud.recommendationengine_v1beta1 import gapic_version as package_version
 
 import google.auth  # type: ignore
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core import operations_v1
@@ -28,36 +29,31 @@
 
 from google.cloud.recommendationengine_v1beta1.types import catalog
 from google.cloud.recommendationengine_v1beta1.types import catalog_service
 from google.cloud.recommendationengine_v1beta1.types import import_
 from google.longrunning import operations_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-recommendations-ai",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class CatalogServiceTransport(abc.ABC):
     """Abstract transport class for CatalogService."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "recommendationengine.googleapis.com"
 
     def __init__(
         self,
         *,
         host: str = DEFAULT_HOST,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
         **kwargs,
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/grpc.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,22 +49,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "recommendationengine.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        channel: grpc.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        channel: Optional[grpc.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
@@ -184,16 +184,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "recommendationengine.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> grpc.Channel:
         """Create and return a gRPC channel object.
         Args:
             host (Optional[str]): The host for the channel to use.
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/grpc_asyncio.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/grpc_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "recommendationengine.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -94,23 +94,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "recommendationengine.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: aio.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
-        quota_project_id=None,
+        channel: Optional[aio.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/rest.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,52 +70,57 @@
     * Stripping extraneous information from responses
 
     These use cases and more can be enabled by injecting an
     instance of a custom subclass when constructing the CatalogServiceRestTransport.
 
     .. code-block:: python
         class MyCustomCatalogServiceInterceptor(CatalogServiceRestInterceptor):
-            def pre_create_catalog_item(request, metadata):
+            def pre_create_catalog_item(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
-            def post_create_catalog_item(response):
+            def post_create_catalog_item(self, response):
                 logging.log(f"Received response: {response}")
+                return response
 
-            def pre_delete_catalog_item(request, metadata):
+            def pre_delete_catalog_item(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
-            def pre_get_catalog_item(request, metadata):
+            def pre_get_catalog_item(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
-            def post_get_catalog_item(response):
+            def post_get_catalog_item(self, response):
                 logging.log(f"Received response: {response}")
+                return response
 
-            def pre_import_catalog_items(request, metadata):
+            def pre_import_catalog_items(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
-            def post_import_catalog_items(response):
+            def post_import_catalog_items(self, response):
                 logging.log(f"Received response: {response}")
+                return response
 
-            def pre_list_catalog_items(request, metadata):
+            def pre_list_catalog_items(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
-            def post_list_catalog_items(response):
+            def post_list_catalog_items(self, response):
                 logging.log(f"Received response: {response}")
+                return response
 
-            def pre_update_catalog_item(request, metadata):
+            def pre_update_catalog_item(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
-            def post_update_catalog_item(response):
+            def post_update_catalog_item(self, response):
                 logging.log(f"Received response: {response}")
+                return response
 
         transport = CatalogServiceRestTransport(interceptor=MyCustomCatalogServiceInterceptor())
         client = CatalogServiceClient(transport=transport)
 
 
     """
 
@@ -262,69 +267,62 @@
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
     and call it.
 
     It sends JSON representations of protocol buffers over HTTP/1.1
 
-    NOTE: This REST transport functionality is currently in a beta
-    state (preview). We welcome your feedback via an issue in this
-    library's source repository. Thank you!
     """
 
     def __init__(
         self,
         *,
         host: str = "recommendationengine.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         url_scheme: str = "https",
         interceptor: Optional[CatalogServiceRestInterceptor] = None,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
-        NOTE: This REST transport functionality is currently in a beta
-        state (preview). We welcome your feedback via a GitHub issue in
-        this library's repository. Thank you!
-
-         Args:
-             host (Optional[str]):
-                  The hostname to connect to.
-             credentials (Optional[google.auth.credentials.Credentials]): The
-                 authorization credentials to attach to requests. These
-                 credentials identify the application to the service; if none
-                 are specified, the client will attempt to ascertain the
-                 credentials from the environment.
-
-             credentials_file (Optional[str]): A file with credentials that can
-                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                 This argument is ignored if ``channel`` is provided.
-             scopes (Optional(Sequence[str])): A list of scopes. This argument is
-                 ignored if ``channel`` is provided.
-             client_cert_source_for_mtls (Callable[[], Tuple[bytes, bytes]]): Client
-                 certificate to configure mutual TLS HTTP channel. It is ignored
-                 if ``channel`` is provided.
-             quota_project_id (Optional[str]): An optional project to use for billing
-                 and quota.
-             client_info (google.api_core.gapic_v1.client_info.ClientInfo):
-                 The client info used to send a user-agent string along with
-                 API requests. If ``None``, then default info will be used.
-                 Generally, you only need to set this if you are developing
-                 your own client library.
-             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
-                 be used for service account credentials.
-             url_scheme: the protocol scheme for the API endpoint.  Normally
-                 "https", but for testing or local servers,
-                 "http" can be specified.
+        Args:
+            host (Optional[str]):
+                 The hostname to connect to.
+            credentials (Optional[google.auth.credentials.Credentials]): The
+                authorization credentials to attach to requests. These
+                credentials identify the application to the service; if none
+                are specified, the client will attempt to ascertain the
+                credentials from the environment.
+
+            credentials_file (Optional[str]): A file with credentials that can
+                be loaded with :func:`google.auth.load_credentials_from_file`.
+                This argument is ignored if ``channel`` is provided.
+            scopes (Optional(Sequence[str])): A list of scopes. This argument is
+                ignored if ``channel`` is provided.
+            client_cert_source_for_mtls (Callable[[], Tuple[bytes, bytes]]): Client
+                certificate to configure mutual TLS HTTP channel. It is ignored
+                if ``channel`` is provided.
+            quota_project_id (Optional[str]): An optional project to use for billing
+                and quota.
+            client_info (google.api_core.gapic_v1.client_info.ClientInfo):
+                The client info used to send a user-agent string along with
+                API requests. If ``None``, then default info will be used.
+                Generally, you only need to set this if you are developing
+                your own client library.
+            always_use_jwt_access (Optional[bool]): Whether self signed JWT should
+                be used for service account credentials.
+            url_scheme: the protocol scheme for the API endpoint.  Normally
+                "https", but for testing or local servers,
+                "http" can be specified.
         """
         # Run the base constructor
         # TODO(yon-mg): resolve other ctor params i.e. scopes, quota, etc.
         # TODO: When custom host (api_endpoint) is set, `scopes` must *also* be set on the
         # credentials object
         maybe_url_match = re.match("^(?P<scheme>http(?:s)?://)?(?P<host>.*)$", host)
         if maybe_url_match is None:
@@ -365,14 +363,15 @@
 
             rest_transport = operations_v1.OperationsRestTransport(
                 host=self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
                 scopes=self._scopes,
                 http_options=http_options,
+                path_prefix="v1beta1",
             )
 
             self._operations_client = operations_v1.AbstractOperationsClient(
                 transport=rest_transport
             )
 
         # Return the client from cache.
@@ -393,15 +392,15 @@
             }
 
         def __call__(
             self,
             request: catalog_service.CreateCatalogItemRequest,
             *,
             retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: float = None,
+            timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> catalog.CatalogItem:
             r"""Call the create catalog item method over HTTP.
 
             Args:
                 request (~.catalog_service.CreateCatalogItemRequest):
                     The request object. Request message for CreateCatalogItem
@@ -434,29 +433,31 @@
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             # Jsonify the request body
 
             body = json_format.MessageToJson(
                 transcoded_request["body"],
                 including_default_value_fields=False,
-                use_integers_for_enums=False,
+                use_integers_for_enums=True,
             )
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(
                 json_format.MessageToJson(
                     transcoded_request["query_params"],
                     including_default_value_fields=False,
-                    use_integers_for_enums=False,
+                    use_integers_for_enums=True,
                 )
             )
             query_params.update(self._get_unset_required_fields(query_params))
 
+            query_params["$alt"] = "json;enum-encoding=int"
+
             # Send the request
             headers = dict(metadata)
             headers["Content-Type"] = "application/json"
             response = getattr(self._session, method)(
                 "{host}{uri}".format(host=self._host, uri=uri),
                 timeout=timeout,
                 headers=headers,
@@ -492,15 +493,15 @@
             }
 
         def __call__(
             self,
             request: catalog_service.DeleteCatalogItemRequest,
             *,
             retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: float = None,
+            timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ):
             r"""Call the delete catalog item method over HTTP.
 
             Args:
                 request (~.catalog_service.DeleteCatalogItemRequest):
                     The request object. Request message for DeleteCatalogItem
@@ -529,19 +530,21 @@
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(
                 json_format.MessageToJson(
                     transcoded_request["query_params"],
                     including_default_value_fields=False,
-                    use_integers_for_enums=False,
+                    use_integers_for_enums=True,
                 )
             )
             query_params.update(self._get_unset_required_fields(query_params))
 
+            query_params["$alt"] = "json;enum-encoding=int"
+
             # Send the request
             headers = dict(metadata)
             headers["Content-Type"] = "application/json"
             response = getattr(self._session, method)(
                 "{host}{uri}".format(host=self._host, uri=uri),
                 timeout=timeout,
                 headers=headers,
@@ -568,15 +571,15 @@
             }
 
         def __call__(
             self,
             request: catalog_service.GetCatalogItemRequest,
             *,
             retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: float = None,
+            timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> catalog.CatalogItem:
             r"""Call the get catalog item method over HTTP.
 
             Args:
                 request (~.catalog_service.GetCatalogItemRequest):
                     The request object. Request message for GetCatalogItem
@@ -611,19 +614,21 @@
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(
                 json_format.MessageToJson(
                     transcoded_request["query_params"],
                     including_default_value_fields=False,
-                    use_integers_for_enums=False,
+                    use_integers_for_enums=True,
                 )
             )
             query_params.update(self._get_unset_required_fields(query_params))
 
+            query_params["$alt"] = "json;enum-encoding=int"
+
             # Send the request
             headers = dict(metadata)
             headers["Content-Type"] = "application/json"
             response = getattr(self._session, method)(
                 "{host}{uri}".format(host=self._host, uri=uri),
                 timeout=timeout,
                 headers=headers,
@@ -658,15 +663,15 @@
             }
 
         def __call__(
             self,
             request: import_.ImportCatalogItemsRequest,
             *,
             retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: float = None,
+            timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> operations_pb2.Operation:
             r"""Call the import catalog items method over HTTP.
 
             Args:
                 request (~.import_.ImportCatalogItemsRequest):
                     The request object. Request message for Import methods.
@@ -698,29 +703,31 @@
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             # Jsonify the request body
 
             body = json_format.MessageToJson(
                 transcoded_request["body"],
                 including_default_value_fields=False,
-                use_integers_for_enums=False,
+                use_integers_for_enums=True,
             )
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(
                 json_format.MessageToJson(
                     transcoded_request["query_params"],
                     including_default_value_fields=False,
-                    use_integers_for_enums=False,
+                    use_integers_for_enums=True,
                 )
             )
             query_params.update(self._get_unset_required_fields(query_params))
 
+            query_params["$alt"] = "json;enum-encoding=int"
+
             # Send the request
             headers = dict(metadata)
             headers["Content-Type"] = "application/json"
             response = getattr(self._session, method)(
                 "{host}{uri}".format(host=self._host, uri=uri),
                 timeout=timeout,
                 headers=headers,
@@ -754,15 +761,15 @@
             }
 
         def __call__(
             self,
             request: catalog_service.ListCatalogItemsRequest,
             *,
             retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: float = None,
+            timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> catalog_service.ListCatalogItemsResponse:
             r"""Call the list catalog items method over HTTP.
 
             Args:
                 request (~.catalog_service.ListCatalogItemsRequest):
                     The request object. Request message for ListCatalogItems
@@ -797,19 +804,21 @@
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(
                 json_format.MessageToJson(
                     transcoded_request["query_params"],
                     including_default_value_fields=False,
-                    use_integers_for_enums=False,
+                    use_integers_for_enums=True,
                 )
             )
             query_params.update(self._get_unset_required_fields(query_params))
 
+            query_params["$alt"] = "json;enum-encoding=int"
+
             # Send the request
             headers = dict(metadata)
             headers["Content-Type"] = "application/json"
             response = getattr(self._session, method)(
                 "{host}{uri}".format(host=self._host, uri=uri),
                 timeout=timeout,
                 headers=headers,
@@ -844,15 +853,15 @@
             }
 
         def __call__(
             self,
             request: catalog_service.UpdateCatalogItemRequest,
             *,
             retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: float = None,
+            timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> catalog.CatalogItem:
             r"""Call the update catalog item method over HTTP.
 
             Args:
                 request (~.catalog_service.UpdateCatalogItemRequest):
                     The request object. Request message for UpdateCatalogItem
@@ -885,29 +894,31 @@
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             # Jsonify the request body
 
             body = json_format.MessageToJson(
                 transcoded_request["body"],
                 including_default_value_fields=False,
-                use_integers_for_enums=False,
+                use_integers_for_enums=True,
             )
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(
                 json_format.MessageToJson(
                     transcoded_request["query_params"],
                     including_default_value_fields=False,
-                    use_integers_for_enums=False,
+                    use_integers_for_enums=True,
                 )
             )
             query_params.update(self._get_unset_required_fields(query_params))
 
+            query_params["$alt"] = "json;enum-encoding=int"
+
             # Send the request
             headers = dict(metadata)
             headers["Content-Type"] = "application/json"
             response = getattr(self._session, method)(
                 "{host}{uri}".format(host=self._host, uri=uri),
                 timeout=timeout,
                 headers=headers,
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/__init__.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/async_client.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/async_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
-import pkg_resources
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
+
+from google.cloud.recommendationengine_v1beta1 import gapic_version as package_version
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
@@ -177,17 +188,17 @@
         type(PredictionApiKeyRegistryClient).get_transport_class,
         type(PredictionApiKeyRegistryClient),
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, PredictionApiKeyRegistryTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the prediction api key registry client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -223,23 +234,27 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def create_prediction_api_key_registration(
         self,
-        request: Union[
-            prediction_apikey_registry_service.CreatePredictionApiKeyRegistrationRequest,
-            dict,
+        request: Optional[
+            Union[
+                prediction_apikey_registry_service.CreatePredictionApiKeyRegistrationRequest,
+                dict,
+            ]
         ] = None,
         *,
-        parent: str = None,
-        prediction_api_key_registration: prediction_apikey_registry_service.PredictionApiKeyRegistration = None,
+        parent: Optional[str] = None,
+        prediction_api_key_registration: Optional[
+            prediction_apikey_registry_service.PredictionApiKeyRegistration
+        ] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> prediction_apikey_registry_service.PredictionApiKeyRegistration:
         r"""Register an API key for use with predict method.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -263,15 +278,15 @@
                 # Make the request
                 response = await client.create_prediction_api_key_registration(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommendationengine_v1beta1.types.CreatePredictionApiKeyRegistrationRequest, dict]):
+            request (Optional[Union[google.cloud.recommendationengine_v1beta1.types.CreatePredictionApiKeyRegistrationRequest, dict]]):
                 The request object. Request message for the
                 `CreatePredictionApiKeyRegistration` method.
             parent (:class:`str`):
                 Required. The parent resource path.
                 ``projects/*/locations/global/catalogs/default_catalog/eventStores/default_event_store``.
 
                 This corresponds to the ``parent`` field
@@ -348,22 +363,24 @@
         )
 
         # Done; return the response.
         return response
 
     async def list_prediction_api_key_registrations(
         self,
-        request: Union[
-            prediction_apikey_registry_service.ListPredictionApiKeyRegistrationsRequest,
-            dict,
+        request: Optional[
+            Union[
+                prediction_apikey_registry_service.ListPredictionApiKeyRegistrationsRequest,
+                dict,
+            ]
         ] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListPredictionApiKeyRegistrationsAsyncPager:
         r"""List the registered apiKeys for use with predict
         method.
 
         .. code-block:: python
 
@@ -389,15 +406,15 @@
                 page_result = client.list_prediction_api_key_registrations(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.recommendationengine_v1beta1.types.ListPredictionApiKeyRegistrationsRequest, dict]):
+            request (Optional[Union[google.cloud.recommendationengine_v1beta1.types.ListPredictionApiKeyRegistrationsRequest, dict]]):
                 The request object. Request message for the
                 `ListPredictionApiKeyRegistrations`.
             parent (:class:`str`):
                 Required. The parent placement resource name such as
                 ``projects/1234/locations/global/catalogs/default_catalog/eventStores/default_event_store``
 
                 This corresponds to the ``parent`` field
@@ -481,22 +498,24 @@
         )
 
         # Done; return the response.
         return response
 
     async def delete_prediction_api_key_registration(
         self,
-        request: Union[
-            prediction_apikey_registry_service.DeletePredictionApiKeyRegistrationRequest,
-            dict,
+        request: Optional[
+            Union[
+                prediction_apikey_registry_service.DeletePredictionApiKeyRegistrationRequest,
+                dict,
+            ]
         ] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
         r"""Unregister an apiKey from using for predict method.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -517,15 +536,15 @@
                     name="name_value",
                 )
 
                 # Make the request
                 await client.delete_prediction_api_key_registration(request=request)
 
         Args:
-            request (Union[google.cloud.recommendationengine_v1beta1.types.DeletePredictionApiKeyRegistrationRequest, dict]):
+            request (Optional[Union[google.cloud.recommendationengine_v1beta1.types.DeletePredictionApiKeyRegistrationRequest, dict]]):
                 The request object. Request message for
                 `DeletePredictionApiKeyRegistration` method.
             name (:class:`str`):
                 Required. The API key to unregister including full
                 resource path.
                 ``projects/*/locations/global/catalogs/default_catalog/eventStores/default_event_store/predictionApiKeyRegistrations/<YOUR_API_KEY>``
 
@@ -592,18 +611,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-recommendations-ai",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("PredictionApiKeyRegistryAsyncClient",)
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/client.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
-import pkg_resources
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
+
+from google.cloud.recommendationengine_v1beta1 import gapic_version as package_version
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport import mtls  # type: ignore
@@ -59,15 +71,15 @@
     )  # type: Dict[str, Type[PredictionApiKeyRegistryTransport]]
     _transport_registry["grpc"] = PredictionApiKeyRegistryGrpcTransport
     _transport_registry["grpc_asyncio"] = PredictionApiKeyRegistryGrpcAsyncIOTransport
     _transport_registry["rest"] = PredictionApiKeyRegistryRestTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[PredictionApiKeyRegistryTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -368,33 +380,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, PredictionApiKeyRegistryTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, PredictionApiKeyRegistryTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the prediction api key registry client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, PredictionApiKeyRegistryTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
-                NOTE: "rest" transport functionality is currently in a
-                beta state (preview). We welcome your feedback via an
-                issue in this library's source repository.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -416,14 +425,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
@@ -468,23 +478,27 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def create_prediction_api_key_registration(
         self,
-        request: Union[
-            prediction_apikey_registry_service.CreatePredictionApiKeyRegistrationRequest,
-            dict,
+        request: Optional[
+            Union[
+                prediction_apikey_registry_service.CreatePredictionApiKeyRegistrationRequest,
+                dict,
+            ]
         ] = None,
         *,
-        parent: str = None,
-        prediction_api_key_registration: prediction_apikey_registry_service.PredictionApiKeyRegistration = None,
+        parent: Optional[str] = None,
+        prediction_api_key_registration: Optional[
+            prediction_apikey_registry_service.PredictionApiKeyRegistration
+        ] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> prediction_apikey_registry_service.PredictionApiKeyRegistration:
         r"""Register an API key for use with predict method.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -590,22 +604,24 @@
         )
 
         # Done; return the response.
         return response
 
     def list_prediction_api_key_registrations(
         self,
-        request: Union[
-            prediction_apikey_registry_service.ListPredictionApiKeyRegistrationsRequest,
-            dict,
+        request: Optional[
+            Union[
+                prediction_apikey_registry_service.ListPredictionApiKeyRegistrationsRequest,
+                dict,
+            ]
         ] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListPredictionApiKeyRegistrationsPager:
         r"""List the registered apiKeys for use with predict
         method.
 
         .. code-block:: python
 
@@ -716,22 +732,24 @@
         )
 
         # Done; return the response.
         return response
 
     def delete_prediction_api_key_registration(
         self,
-        request: Union[
-            prediction_apikey_registry_service.DeletePredictionApiKeyRegistrationRequest,
-            dict,
+        request: Optional[
+            Union[
+                prediction_apikey_registry_service.DeletePredictionApiKeyRegistrationRequest,
+                dict,
+            ]
         ] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
         r"""Unregister an apiKey from using for predict method.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -829,18 +847,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-recommendations-ai",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("PredictionApiKeyRegistryClient",)
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/pagers.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/__init__.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/base.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,51 +11,47 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import abc
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Union
-import pkg_resources
+
+from google.cloud.recommendationengine_v1beta1 import gapic_version as package_version
 
 import google.auth  # type: ignore
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 from google.cloud.recommendationengine_v1beta1.types import (
     prediction_apikey_registry_service,
 )
 from google.protobuf import empty_pb2  # type: ignore
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-recommendations-ai",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class PredictionApiKeyRegistryTransport(abc.ABC):
     """Abstract transport class for PredictionApiKeyRegistry."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "recommendationengine.googleapis.com"
 
     def __init__(
         self,
         *,
         host: str = DEFAULT_HOST,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
         **kwargs,
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/grpc.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,22 +51,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "recommendationengine.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        channel: grpc.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        channel: Optional[grpc.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
@@ -185,16 +185,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "recommendationengine.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> grpc.Channel:
         """Create and return a gRPC channel object.
         Args:
             host (Optional[str]): The host for the channel to use.
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/grpc_asyncio.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/grpc_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "recommendationengine.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -96,23 +96,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "recommendationengine.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: aio.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
-        quota_project_id=None,
+        channel: Optional[aio.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/rest.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_api_key_registry/transports/rest.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,31 +68,33 @@
     * Stripping extraneous information from responses
 
     These use cases and more can be enabled by injecting an
     instance of a custom subclass when constructing the PredictionApiKeyRegistryRestTransport.
 
     .. code-block:: python
         class MyCustomPredictionApiKeyRegistryInterceptor(PredictionApiKeyRegistryRestInterceptor):
-            def pre_create_prediction_api_key_registration(request, metadata):
+            def pre_create_prediction_api_key_registration(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
-            def post_create_prediction_api_key_registration(response):
+            def post_create_prediction_api_key_registration(self, response):
                 logging.log(f"Received response: {response}")
+                return response
 
-            def pre_delete_prediction_api_key_registration(request, metadata):
+            def pre_delete_prediction_api_key_registration(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
-            def pre_list_prediction_api_key_registrations(request, metadata):
+            def pre_list_prediction_api_key_registrations(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
-            def post_list_prediction_api_key_registrations(response):
+            def post_list_prediction_api_key_registrations(self, response):
                 logging.log(f"Received response: {response}")
+                return response
 
         transport = PredictionApiKeyRegistryRestTransport(interceptor=MyCustomPredictionApiKeyRegistryInterceptor())
         client = PredictionApiKeyRegistryClient(transport=transport)
 
 
     """
 
@@ -184,69 +186,62 @@
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
     and call it.
 
     It sends JSON representations of protocol buffers over HTTP/1.1
 
-    NOTE: This REST transport functionality is currently in a beta
-    state (preview). We welcome your feedback via an issue in this
-    library's source repository. Thank you!
     """
 
     def __init__(
         self,
         *,
         host: str = "recommendationengine.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         url_scheme: str = "https",
         interceptor: Optional[PredictionApiKeyRegistryRestInterceptor] = None,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
-        NOTE: This REST transport functionality is currently in a beta
-        state (preview). We welcome your feedback via a GitHub issue in
-        this library's repository. Thank you!
-
-         Args:
-             host (Optional[str]):
-                  The hostname to connect to.
-             credentials (Optional[google.auth.credentials.Credentials]): The
-                 authorization credentials to attach to requests. These
-                 credentials identify the application to the service; if none
-                 are specified, the client will attempt to ascertain the
-                 credentials from the environment.
-
-             credentials_file (Optional[str]): A file with credentials that can
-                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                 This argument is ignored if ``channel`` is provided.
-             scopes (Optional(Sequence[str])): A list of scopes. This argument is
-                 ignored if ``channel`` is provided.
-             client_cert_source_for_mtls (Callable[[], Tuple[bytes, bytes]]): Client
-                 certificate to configure mutual TLS HTTP channel. It is ignored
-                 if ``channel`` is provided.
-             quota_project_id (Optional[str]): An optional project to use for billing
-                 and quota.
-             client_info (google.api_core.gapic_v1.client_info.ClientInfo):
-                 The client info used to send a user-agent string along with
-                 API requests. If ``None``, then default info will be used.
-                 Generally, you only need to set this if you are developing
-                 your own client library.
-             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
-                 be used for service account credentials.
-             url_scheme: the protocol scheme for the API endpoint.  Normally
-                 "https", but for testing or local servers,
-                 "http" can be specified.
+        Args:
+            host (Optional[str]):
+                 The hostname to connect to.
+            credentials (Optional[google.auth.credentials.Credentials]): The
+                authorization credentials to attach to requests. These
+                credentials identify the application to the service; if none
+                are specified, the client will attempt to ascertain the
+                credentials from the environment.
+
+            credentials_file (Optional[str]): A file with credentials that can
+                be loaded with :func:`google.auth.load_credentials_from_file`.
+                This argument is ignored if ``channel`` is provided.
+            scopes (Optional(Sequence[str])): A list of scopes. This argument is
+                ignored if ``channel`` is provided.
+            client_cert_source_for_mtls (Callable[[], Tuple[bytes, bytes]]): Client
+                certificate to configure mutual TLS HTTP channel. It is ignored
+                if ``channel`` is provided.
+            quota_project_id (Optional[str]): An optional project to use for billing
+                and quota.
+            client_info (google.api_core.gapic_v1.client_info.ClientInfo):
+                The client info used to send a user-agent string along with
+                API requests. If ``None``, then default info will be used.
+                Generally, you only need to set this if you are developing
+                your own client library.
+            always_use_jwt_access (Optional[bool]): Whether self signed JWT should
+                be used for service account credentials.
+            url_scheme: the protocol scheme for the API endpoint.  Normally
+                "https", but for testing or local servers,
+                "http" can be specified.
         """
         # Run the base constructor
         # TODO(yon-mg): resolve other ctor params i.e. scopes, quota, etc.
         # TODO: When custom host (api_endpoint) is set, `scopes` must *also* be set on the
         # credentials object
         maybe_url_match = re.match("^(?P<scheme>http(?:s)?://)?(?P<host>.*)$", host)
         if maybe_url_match is None:
@@ -288,15 +283,15 @@
             }
 
         def __call__(
             self,
             request: prediction_apikey_registry_service.CreatePredictionApiKeyRegistrationRequest,
             *,
             retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: float = None,
+            timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> prediction_apikey_registry_service.PredictionApiKeyRegistration:
             r"""Call the create prediction api key
             registration method over HTTP.
 
                 Args:
                     request (~.prediction_apikey_registry_service.CreatePredictionApiKeyRegistrationRequest):
@@ -333,29 +328,31 @@
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             # Jsonify the request body
 
             body = json_format.MessageToJson(
                 transcoded_request["body"],
                 including_default_value_fields=False,
-                use_integers_for_enums=False,
+                use_integers_for_enums=True,
             )
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(
                 json_format.MessageToJson(
                     transcoded_request["query_params"],
                     including_default_value_fields=False,
-                    use_integers_for_enums=False,
+                    use_integers_for_enums=True,
                 )
             )
             query_params.update(self._get_unset_required_fields(query_params))
 
+            query_params["$alt"] = "json;enum-encoding=int"
+
             # Send the request
             headers = dict(metadata)
             headers["Content-Type"] = "application/json"
             response = getattr(self._session, method)(
                 "{host}{uri}".format(host=self._host, uri=uri),
                 timeout=timeout,
                 headers=headers,
@@ -393,15 +390,15 @@
             }
 
         def __call__(
             self,
             request: prediction_apikey_registry_service.DeletePredictionApiKeyRegistrationRequest,
             *,
             retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: float = None,
+            timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ):
             r"""Call the delete prediction api key
             registration method over HTTP.
 
                 Args:
                     request (~.prediction_apikey_registry_service.DeletePredictionApiKeyRegistrationRequest):
@@ -436,19 +433,21 @@
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(
                 json_format.MessageToJson(
                     transcoded_request["query_params"],
                     including_default_value_fields=False,
-                    use_integers_for_enums=False,
+                    use_integers_for_enums=True,
                 )
             )
             query_params.update(self._get_unset_required_fields(query_params))
 
+            query_params["$alt"] = "json;enum-encoding=int"
+
             # Send the request
             headers = dict(metadata)
             headers["Content-Type"] = "application/json"
             response = getattr(self._session, method)(
                 "{host}{uri}".format(host=self._host, uri=uri),
                 timeout=timeout,
                 headers=headers,
@@ -475,15 +474,15 @@
             }
 
         def __call__(
             self,
             request: prediction_apikey_registry_service.ListPredictionApiKeyRegistrationsRequest,
             *,
             retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: float = None,
+            timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> prediction_apikey_registry_service.ListPredictionApiKeyRegistrationsResponse:
             r"""Call the list prediction api key
             registrations method over HTTP.
 
                 Args:
                     request (~.prediction_apikey_registry_service.ListPredictionApiKeyRegistrationsRequest):
@@ -524,19 +523,21 @@
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(
                 json_format.MessageToJson(
                     transcoded_request["query_params"],
                     including_default_value_fields=False,
-                    use_integers_for_enums=False,
+                    use_integers_for_enums=True,
                 )
             )
             query_params.update(self._get_unset_required_fields(query_params))
 
+            query_params["$alt"] = "json;enum-encoding=int"
+
             # Send the request
             headers = dict(metadata)
             headers["Content-Type"] = "application/json"
             response = getattr(self._session, method)(
                 "{host}{uri}".format(host=self._host, uri=uri),
                 timeout=timeout,
                 headers=headers,
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_service/__init__.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_service/async_client.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
-import pkg_resources
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
+
+from google.cloud.recommendationengine_v1beta1 import gapic_version as package_version
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
@@ -155,17 +166,17 @@
     get_transport_class = functools.partial(
         type(PredictionServiceClient).get_transport_class, type(PredictionServiceClient)
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, PredictionServiceTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the prediction service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -201,20 +212,20 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def predict(
         self,
-        request: Union[prediction_service.PredictRequest, dict] = None,
+        request: Optional[Union[prediction_service.PredictRequest, dict]] = None,
         *,
-        name: str = None,
-        user_event: gcr_user_event.UserEvent = None,
+        name: Optional[str] = None,
+        user_event: Optional[gcr_user_event.UserEvent] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.PredictAsyncPager:
         r"""Makes a recommendation prediction. If using API Key based
         authentication, the API Key must be registered using the
         [PredictionApiKeyRegistry][google.cloud.recommendationengine.v1beta1.PredictionApiKeyRegistry]
         service. `Learn
         more </recommendations-ai/docs/setting-up#register-key>`__.
@@ -248,15 +259,15 @@
                 page_result = client.predict(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.recommendationengine_v1beta1.types.PredictRequest, dict]):
+            request (Optional[Union[google.cloud.recommendationengine_v1beta1.types.PredictRequest, dict]]):
                 The request object. Request message for Predict method.
             name (:class:`str`):
                 Required. Full resource name of the format:
                 ``{name=projects/*/locations/global/catalogs/default_catalog/eventStores/default_event_store/placements/*}``
                 The id of the recommendation engine placement. This id
                 is used to identify the set of models that will be used
                 to make the prediction.
@@ -388,18 +399,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-recommendations-ai",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("PredictionServiceAsyncClient",)
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_service/client.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
-import pkg_resources
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
+
+from google.cloud.recommendationengine_v1beta1 import gapic_version as package_version
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport import mtls  # type: ignore
@@ -56,15 +68,15 @@
     )  # type: Dict[str, Type[PredictionServiceTransport]]
     _transport_registry["grpc"] = PredictionServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = PredictionServiceGrpcAsyncIOTransport
     _transport_registry["rest"] = PredictionServiceRestTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[PredictionServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -335,33 +347,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, PredictionServiceTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, PredictionServiceTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the prediction service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, PredictionServiceTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
-                NOTE: "rest" transport functionality is currently in a
-                beta state (preview). We welcome your feedback via an
-                issue in this library's source repository.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -383,14 +392,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
@@ -435,20 +445,20 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def predict(
         self,
-        request: Union[prediction_service.PredictRequest, dict] = None,
+        request: Optional[Union[prediction_service.PredictRequest, dict]] = None,
         *,
-        name: str = None,
-        user_event: gcr_user_event.UserEvent = None,
+        name: Optional[str] = None,
+        user_event: Optional[gcr_user_event.UserEvent] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.PredictPager:
         r"""Makes a recommendation prediction. If using API Key based
         authentication, the API Key must be registered using the
         [PredictionApiKeyRegistry][google.cloud.recommendationengine.v1beta1.PredictionApiKeyRegistry]
         service. `Learn
         more </recommendations-ai/docs/setting-up#register-key>`__.
@@ -619,18 +629,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-recommendations-ai",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("PredictionServiceClient",)
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_service/pagers.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/__init__.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/base.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,48 +11,44 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import abc
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Union
-import pkg_resources
+
+from google.cloud.recommendationengine_v1beta1 import gapic_version as package_version
 
 import google.auth  # type: ignore
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 from google.cloud.recommendationengine_v1beta1.types import prediction_service
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-recommendations-ai",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class PredictionServiceTransport(abc.ABC):
     """Abstract transport class for PredictionService."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "recommendationengine.googleapis.com"
 
     def __init__(
         self,
         *,
         host: str = DEFAULT_HOST,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
         **kwargs,
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/grpc.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,22 +43,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "recommendationengine.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        channel: grpc.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        channel: Optional[grpc.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
@@ -177,16 +177,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "recommendationengine.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> grpc.Channel:
         """Create and return a gRPC channel object.
         Args:
             host (Optional[str]): The host for the channel to use.
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/grpc_asyncio.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/grpc_asyncio.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "recommendationengine.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -88,23 +88,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "recommendationengine.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: aio.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
-        quota_project_id=None,
+        channel: Optional[aio.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/rest.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/prediction_service/transports/rest.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,20 +65,21 @@
     * Stripping extraneous information from responses
 
     These use cases and more can be enabled by injecting an
     instance of a custom subclass when constructing the PredictionServiceRestTransport.
 
     .. code-block:: python
         class MyCustomPredictionServiceInterceptor(PredictionServiceRestInterceptor):
-            def pre_predict(request, metadata):
+            def pre_predict(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
-            def post_predict(response):
+            def post_predict(self, response):
                 logging.log(f"Received response: {response}")
+                return response
 
         transport = PredictionServiceRestTransport(interceptor=MyCustomPredictionServiceInterceptor())
         client = PredictionServiceClient(transport=transport)
 
 
     """
 
@@ -120,69 +121,62 @@
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
     and call it.
 
     It sends JSON representations of protocol buffers over HTTP/1.1
 
-    NOTE: This REST transport functionality is currently in a beta
-    state (preview). We welcome your feedback via an issue in this
-    library's source repository. Thank you!
     """
 
     def __init__(
         self,
         *,
         host: str = "recommendationengine.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         url_scheme: str = "https",
         interceptor: Optional[PredictionServiceRestInterceptor] = None,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
-        NOTE: This REST transport functionality is currently in a beta
-        state (preview). We welcome your feedback via a GitHub issue in
-        this library's repository. Thank you!
-
-         Args:
-             host (Optional[str]):
-                  The hostname to connect to.
-             credentials (Optional[google.auth.credentials.Credentials]): The
-                 authorization credentials to attach to requests. These
-                 credentials identify the application to the service; if none
-                 are specified, the client will attempt to ascertain the
-                 credentials from the environment.
-
-             credentials_file (Optional[str]): A file with credentials that can
-                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                 This argument is ignored if ``channel`` is provided.
-             scopes (Optional(Sequence[str])): A list of scopes. This argument is
-                 ignored if ``channel`` is provided.
-             client_cert_source_for_mtls (Callable[[], Tuple[bytes, bytes]]): Client
-                 certificate to configure mutual TLS HTTP channel. It is ignored
-                 if ``channel`` is provided.
-             quota_project_id (Optional[str]): An optional project to use for billing
-                 and quota.
-             client_info (google.api_core.gapic_v1.client_info.ClientInfo):
-                 The client info used to send a user-agent string along with
-                 API requests. If ``None``, then default info will be used.
-                 Generally, you only need to set this if you are developing
-                 your own client library.
-             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
-                 be used for service account credentials.
-             url_scheme: the protocol scheme for the API endpoint.  Normally
-                 "https", but for testing or local servers,
-                 "http" can be specified.
+        Args:
+            host (Optional[str]):
+                 The hostname to connect to.
+            credentials (Optional[google.auth.credentials.Credentials]): The
+                authorization credentials to attach to requests. These
+                credentials identify the application to the service; if none
+                are specified, the client will attempt to ascertain the
+                credentials from the environment.
+
+            credentials_file (Optional[str]): A file with credentials that can
+                be loaded with :func:`google.auth.load_credentials_from_file`.
+                This argument is ignored if ``channel`` is provided.
+            scopes (Optional(Sequence[str])): A list of scopes. This argument is
+                ignored if ``channel`` is provided.
+            client_cert_source_for_mtls (Callable[[], Tuple[bytes, bytes]]): Client
+                certificate to configure mutual TLS HTTP channel. It is ignored
+                if ``channel`` is provided.
+            quota_project_id (Optional[str]): An optional project to use for billing
+                and quota.
+            client_info (google.api_core.gapic_v1.client_info.ClientInfo):
+                The client info used to send a user-agent string along with
+                API requests. If ``None``, then default info will be used.
+                Generally, you only need to set this if you are developing
+                your own client library.
+            always_use_jwt_access (Optional[bool]): Whether self signed JWT should
+                be used for service account credentials.
+            url_scheme: the protocol scheme for the API endpoint.  Normally
+                "https", but for testing or local servers,
+                "http" can be specified.
         """
         # Run the base constructor
         # TODO(yon-mg): resolve other ctor params i.e. scopes, quota, etc.
         # TODO: When custom host (api_endpoint) is set, `scopes` must *also* be set on the
         # credentials object
         maybe_url_match = re.match("^(?P<scheme>http(?:s)?://)?(?P<host>.*)$", host)
         if maybe_url_match is None:
@@ -224,15 +218,15 @@
             }
 
         def __call__(
             self,
             request: prediction_service.PredictRequest,
             *,
             retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: float = None,
+            timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> prediction_service.PredictResponse:
             r"""Call the predict method over HTTP.
 
             Args:
                 request (~.prediction_service.PredictRequest):
                     The request object. Request message for Predict method.
@@ -259,29 +253,31 @@
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             # Jsonify the request body
 
             body = json_format.MessageToJson(
                 transcoded_request["body"],
                 including_default_value_fields=False,
-                use_integers_for_enums=False,
+                use_integers_for_enums=True,
             )
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(
                 json_format.MessageToJson(
                     transcoded_request["query_params"],
                     including_default_value_fields=False,
-                    use_integers_for_enums=False,
+                    use_integers_for_enums=True,
                 )
             )
             query_params.update(self._get_unset_required_fields(query_params))
 
+            query_params["$alt"] = "json;enum-encoding=int"
+
             # Send the request
             headers = dict(metadata)
             headers["Content-Type"] = "application/json"
             response = getattr(self._session, method)(
                 "{host}{uri}".format(host=self._host, uri=uri),
                 timeout=timeout,
                 headers=headers,
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/user_event_service/__init__.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/user_event_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/user_event_service/async_client.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/user_event_service/async_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
-import pkg_resources
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
+
+from google.cloud.recommendationengine_v1beta1 import gapic_version as package_version
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
@@ -164,17 +175,17 @@
     get_transport_class = functools.partial(
         type(UserEventServiceClient).get_transport_class, type(UserEventServiceClient)
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, UserEventServiceTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the user event service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -210,20 +221,20 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def write_user_event(
         self,
-        request: Union[user_event_service.WriteUserEventRequest, dict] = None,
+        request: Optional[Union[user_event_service.WriteUserEventRequest, dict]] = None,
         *,
-        parent: str = None,
-        user_event: gcr_user_event.UserEvent = None,
+        parent: Optional[str] = None,
+        user_event: Optional[gcr_user_event.UserEvent] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcr_user_event.UserEvent:
         r"""Writes a single user event.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -252,15 +263,15 @@
                 # Make the request
                 response = await client.write_user_event(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommendationengine_v1beta1.types.WriteUserEventRequest, dict]):
+            request (Optional[Union[google.cloud.recommendationengine_v1beta1.types.WriteUserEventRequest, dict]]):
                 The request object. Request message for WriteUserEvent
                 method.
             parent (:class:`str`):
                 Required. The parent eventStore resource name, such as
                 ``projects/1234/locations/global/catalogs/default_catalog/eventStores/default_event_store``.
 
                 This corresponds to the ``parent`` field
@@ -337,22 +348,24 @@
         )
 
         # Done; return the response.
         return response
 
     async def collect_user_event(
         self,
-        request: Union[user_event_service.CollectUserEventRequest, dict] = None,
+        request: Optional[
+            Union[user_event_service.CollectUserEventRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        user_event: str = None,
-        uri: str = None,
-        ets: int = None,
+        parent: Optional[str] = None,
+        user_event: Optional[str] = None,
+        uri: Optional[str] = None,
+        ets: Optional[int] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> httpbody_pb2.HttpBody:
         r"""Writes a single user event from the browser. This
         uses a GET request to due to browser restriction of
         POST-ing to a 3rd party domain.
         This method is used only by the Recommendations AI
         JavaScript pixel. Users should not call this method
@@ -382,15 +395,15 @@
                 # Make the request
                 response = await client.collect_user_event(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommendationengine_v1beta1.types.CollectUserEventRequest, dict]):
+            request (Optional[Union[google.cloud.recommendationengine_v1beta1.types.CollectUserEventRequest, dict]]):
                 The request object. Request message for CollectUserEvent
                 method.
             parent (:class:`str`):
                 Required. The parent eventStore name, such as
                 ``projects/1234/locations/global/catalogs/default_catalog/eventStores/default_event_store``.
 
                 This corresponds to the ``parent`` field
@@ -538,20 +551,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def list_user_events(
         self,
-        request: Union[user_event_service.ListUserEventsRequest, dict] = None,
+        request: Optional[Union[user_event_service.ListUserEventsRequest, dict]] = None,
         *,
-        parent: str = None,
-        filter: str = None,
+        parent: Optional[str] = None,
+        filter: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListUserEventsAsyncPager:
         r"""Gets a list of user events within a time range, with
         potential filtering.
 
         .. code-block:: python
 
@@ -577,15 +590,15 @@
                 page_result = client.list_user_events(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.recommendationengine_v1beta1.types.ListUserEventsRequest, dict]):
+            request (Optional[Union[google.cloud.recommendationengine_v1beta1.types.ListUserEventsRequest, dict]]):
                 The request object. Request message for ListUserEvents
                 method.
             parent (:class:`str`):
                 Required. The parent eventStore resource name, such as
                 ``projects/*/locations/*/catalogs/default_catalog/eventStores/default_event_store``.
 
                 This corresponds to the ``parent`` field
@@ -708,21 +721,23 @@
         )
 
         # Done; return the response.
         return response
 
     async def purge_user_events(
         self,
-        request: Union[user_event_service.PurgeUserEventsRequest, dict] = None,
+        request: Optional[
+            Union[user_event_service.PurgeUserEventsRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        filter: str = None,
-        force: bool = None,
+        parent: Optional[str] = None,
+        filter: Optional[str] = None,
+        force: Optional[bool] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Deletes permanently all user events specified by the
         filter provided. Depending on the number of events
         specified by the filter, this operation could take hours
         or days to complete. To test a filter, use the list
         command first.
@@ -749,21 +764,21 @@
                 )
 
                 # Make the request
                 operation = client.purge_user_events(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommendationengine_v1beta1.types.PurgeUserEventsRequest, dict]):
+            request (Optional[Union[google.cloud.recommendationengine_v1beta1.types.PurgeUserEventsRequest, dict]]):
                 The request object. Request message for PurgeUserEvents
                 method.
             parent (:class:`str`):
                 Required. The resource name of the event_store under
                 which the events are created. The format is
                 ``projects/${projectId}/locations/global/catalogs/${catalogId}/eventStores/${eventStoreId}``
 
@@ -881,22 +896,22 @@
         )
 
         # Done; return the response.
         return response
 
     async def import_user_events(
         self,
-        request: Union[import_.ImportUserEventsRequest, dict] = None,
+        request: Optional[Union[import_.ImportUserEventsRequest, dict]] = None,
         *,
-        parent: str = None,
-        request_id: str = None,
-        input_config: import_.InputConfig = None,
-        errors_config: import_.ImportErrorsConfig = None,
+        parent: Optional[str] = None,
+        request_id: Optional[str] = None,
+        input_config: Optional[import_.InputConfig] = None,
+        errors_config: Optional[import_.ImportErrorsConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Bulk import of User events. Request processing might
         be synchronous. Events that already exist are skipped.
         Use this method for backfilling historical user events.
         Operation.response is of type ImportResponse. Note that
         it is possible for a subset of the items to be
@@ -924,21 +939,21 @@
                 )
 
                 # Make the request
                 operation = client.import_user_events(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommendationengine_v1beta1.types.ImportUserEventsRequest, dict]):
+            request (Optional[Union[google.cloud.recommendationengine_v1beta1.types.ImportUserEventsRequest, dict]]):
                 The request object. Request message for the
                 ImportUserEvents request.
             parent (:class:`str`):
                 Required.
                 ``projects/1234/locations/global/catalogs/default_catalog/eventStores/default_event_store``
 
                 This corresponds to the ``parent`` field
@@ -1056,18 +1071,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-recommendations-ai",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("UserEventServiceAsyncClient",)
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/user_event_service/client.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/user_event_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
-import pkg_resources
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
+
+from google.cloud.recommendationengine_v1beta1 import gapic_version as package_version
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport import mtls  # type: ignore
@@ -63,15 +75,15 @@
     )  # type: Dict[str, Type[UserEventServiceTransport]]
     _transport_registry["grpc"] = UserEventServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = UserEventServiceGrpcAsyncIOTransport
     _transport_registry["rest"] = UserEventServiceRestTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[UserEventServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -342,33 +354,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, UserEventServiceTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, UserEventServiceTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the user event service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, UserEventServiceTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
-                NOTE: "rest" transport functionality is currently in a
-                beta state (preview). We welcome your feedback via an
-                issue in this library's source repository.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -390,14 +399,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
@@ -442,20 +452,20 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def write_user_event(
         self,
-        request: Union[user_event_service.WriteUserEventRequest, dict] = None,
+        request: Optional[Union[user_event_service.WriteUserEventRequest, dict]] = None,
         *,
-        parent: str = None,
-        user_event: gcr_user_event.UserEvent = None,
+        parent: Optional[str] = None,
+        user_event: Optional[gcr_user_event.UserEvent] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcr_user_event.UserEvent:
         r"""Writes a single user event.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -559,22 +569,24 @@
         )
 
         # Done; return the response.
         return response
 
     def collect_user_event(
         self,
-        request: Union[user_event_service.CollectUserEventRequest, dict] = None,
+        request: Optional[
+            Union[user_event_service.CollectUserEventRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        user_event: str = None,
-        uri: str = None,
-        ets: int = None,
+        parent: Optional[str] = None,
+        user_event: Optional[str] = None,
+        uri: Optional[str] = None,
+        ets: Optional[int] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> httpbody_pb2.HttpBody:
         r"""Writes a single user event from the browser. This
         uses a GET request to due to browser restriction of
         POST-ing to a 3rd party domain.
         This method is used only by the Recommendations AI
         JavaScript pixel. Users should not call this method
@@ -750,20 +762,20 @@
         )
 
         # Done; return the response.
         return response
 
     def list_user_events(
         self,
-        request: Union[user_event_service.ListUserEventsRequest, dict] = None,
+        request: Optional[Union[user_event_service.ListUserEventsRequest, dict]] = None,
         *,
-        parent: str = None,
-        filter: str = None,
+        parent: Optional[str] = None,
+        filter: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListUserEventsPager:
         r"""Gets a list of user events within a time range, with
         potential filtering.
 
         .. code-block:: python
 
@@ -910,21 +922,23 @@
         )
 
         # Done; return the response.
         return response
 
     def purge_user_events(
         self,
-        request: Union[user_event_service.PurgeUserEventsRequest, dict] = None,
+        request: Optional[
+            Union[user_event_service.PurgeUserEventsRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        filter: str = None,
-        force: bool = None,
+        parent: Optional[str] = None,
+        filter: Optional[str] = None,
+        force: Optional[bool] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Deletes permanently all user events specified by the
         filter provided. Depending on the number of events
         specified by the filter, this operation could take hours
         or days to complete. To test a filter, use the list
         command first.
@@ -1073,22 +1087,22 @@
         )
 
         # Done; return the response.
         return response
 
     def import_user_events(
         self,
-        request: Union[import_.ImportUserEventsRequest, dict] = None,
+        request: Optional[Union[import_.ImportUserEventsRequest, dict]] = None,
         *,
-        parent: str = None,
-        request_id: str = None,
-        input_config: import_.InputConfig = None,
-        errors_config: import_.ImportErrorsConfig = None,
+        parent: Optional[str] = None,
+        request_id: Optional[str] = None,
+        input_config: Optional[import_.InputConfig] = None,
+        errors_config: Optional[import_.ImportErrorsConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Bulk import of User events. Request processing might
         be synchronous. Events that already exist are skipped.
         Use this method for backfilling historical user events.
         Operation.response is of type ImportResponse. Note that
         it is possible for a subset of the items to be
@@ -1245,18 +1259,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-recommendations-ai",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("UserEventServiceClient",)
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/user_event_service/pagers.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/user_event_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/__init__.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/base.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import abc
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Union
-import pkg_resources
+
+from google.cloud.recommendationengine_v1beta1 import gapic_version as package_version
 
 import google.auth  # type: ignore
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core import operations_v1
@@ -28,36 +29,31 @@
 
 from google.api import httpbody_pb2  # type: ignore
 from google.cloud.recommendationengine_v1beta1.types import import_
 from google.cloud.recommendationengine_v1beta1.types import user_event as gcr_user_event
 from google.cloud.recommendationengine_v1beta1.types import user_event_service
 from google.longrunning import operations_pb2  # type: ignore
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-recommendations-ai",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class UserEventServiceTransport(abc.ABC):
     """Abstract transport class for UserEventService."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "recommendationengine.googleapis.com"
 
     def __init__(
         self,
         *,
         host: str = DEFAULT_HOST,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
         **kwargs,
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/grpc.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/grpc_asyncio.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,61 +10,106 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import warnings
-from typing import Callable, Dict, Optional, Sequence, Tuple, Union
+from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
 
-from google.api_core import grpc_helpers
-from google.api_core import operations_v1
 from google.api_core import gapic_v1
-import google.auth  # type: ignore
+from google.api_core import grpc_helpers_async
+from google.api_core import operations_v1
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
+from grpc.experimental import aio  # type: ignore
 
 from google.api import httpbody_pb2  # type: ignore
 from google.cloud.recommendationengine_v1beta1.types import import_
 from google.cloud.recommendationengine_v1beta1.types import user_event as gcr_user_event
 from google.cloud.recommendationengine_v1beta1.types import user_event_service
 from google.longrunning import operations_pb2  # type: ignore
 from .base import UserEventServiceTransport, DEFAULT_CLIENT_INFO
+from .grpc import UserEventServiceGrpcTransport
 
 
-class UserEventServiceGrpcTransport(UserEventServiceTransport):
-    """gRPC backend transport for UserEventService.
+class UserEventServiceGrpcAsyncIOTransport(UserEventServiceTransport):
+    """gRPC AsyncIO backend transport for UserEventService.
 
     Service for ingesting end user actions on the customer
     website.
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
     and call it.
 
     It sends protocol buffers over the wire using gRPC (which is built on
     top of HTTP/2); the ``grpcio`` package must be installed.
     """
 
-    _stubs: Dict[str, Callable]
+    _grpc_channel: aio.Channel
+    _stubs: Dict[str, Callable] = {}
+
+    @classmethod
+    def create_channel(
+        cls,
+        host: str = "recommendationengine.googleapis.com",
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        quota_project_id: Optional[str] = None,
+        **kwargs,
+    ) -> aio.Channel:
+        """Create and return a gRPC AsyncIO channel object.
+        Args:
+            host (Optional[str]): The host for the channel to use.
+            credentials (Optional[~.Credentials]): The
+                authorization credentials to attach to requests. These
+                credentials identify this application to the service. If
+                none are specified, the client will attempt to ascertain
+                the credentials from the environment.
+            credentials_file (Optional[str]): A file with credentials that can
+                be loaded with :func:`google.auth.load_credentials_from_file`.
+                This argument is ignored if ``channel`` is provided.
+            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
+                service. These are only used when credentials are not specified and
+                are passed to :func:`google.auth.default`.
+            quota_project_id (Optional[str]): An optional project to use for billing
+                and quota.
+            kwargs (Optional[dict]): Keyword arguments, which are passed to the
+                channel creation.
+        Returns:
+            aio.Channel: A gRPC AsyncIO channel object.
+        """
+
+        return grpc_helpers_async.create_channel(
+            host,
+            credentials=credentials,
+            credentials_file=credentials_file,
+            quota_project_id=quota_project_id,
+            default_scopes=cls.AUTH_SCOPES,
+            scopes=scopes,
+            default_host=cls.DEFAULT_HOST,
+            **kwargs,
+        )
 
     def __init__(
         self,
         *,
         host: str = "recommendationengine.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        channel: grpc.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        channel: Optional[aio.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
@@ -76,17 +121,18 @@
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
                 This argument is ignored if ``channel`` is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
                 This argument is ignored if ``channel`` is provided.
-            scopes (Optional(Sequence[str])): A list of scopes. This argument is
-                ignored if ``channel`` is provided.
-            channel (Optional[grpc.Channel]): A ``Channel`` instance through
+            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
+                service. These are only used when credentials are not specified and
+                are passed to :func:`google.auth.default`.
+            channel (Optional[aio.Channel]): A ``Channel`` instance through
                 which to make calls.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
@@ -105,36 +151,35 @@
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
 
         Raises:
-          google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
+            google.auth.exceptions.MutualTlsChannelError: If mutual TLS transport
               creation failed for any reason.
           google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
               and ``credentials_file`` are passed.
         """
         self._grpc_channel = None
         self._ssl_channel_credentials = ssl_channel_credentials
         self._stubs: Dict[str, Callable] = {}
-        self._operations_client: Optional[operations_v1.OperationsClient] = None
+        self._operations_client: Optional[operations_v1.OperationsAsyncClient] = None
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
         if channel:
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
-
         else:
             if api_mtls_endpoint:
                 host = api_mtls_endpoint
 
                 # Create SSL credentials with client_cert_source or application
                 # default SSL credentials.
                 if client_cert_source:
@@ -180,91 +225,53 @@
                     ("grpc.max_receive_message_length", -1),
                 ],
             )
 
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
-    @classmethod
-    def create_channel(
-        cls,
-        host: str = "recommendationengine.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Optional[Sequence[str]] = None,
-        quota_project_id: Optional[str] = None,
-        **kwargs,
-    ) -> grpc.Channel:
-        """Create and return a gRPC channel object.
-        Args:
-            host (Optional[str]): The host for the channel to use.
-            credentials (Optional[~.Credentials]): The
-                authorization credentials to attach to requests. These
-                credentials identify this application to the service. If
-                none are specified, the client will attempt to ascertain
-                the credentials from the environment.
-            credentials_file (Optional[str]): A file with credentials that can
-                be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is mutually exclusive with credentials.
-            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
-                service. These are only used when credentials are not specified and
-                are passed to :func:`google.auth.default`.
-            quota_project_id (Optional[str]): An optional project to use for billing
-                and quota.
-            kwargs (Optional[dict]): Keyword arguments, which are passed to the
-                channel creation.
-        Returns:
-            grpc.Channel: A gRPC channel object.
+    @property
+    def grpc_channel(self) -> aio.Channel:
+        """Create the channel designed to connect to this service.
 
-        Raises:
-            google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
-              and ``credentials_file`` are passed.
+        This property caches on the instance; repeated calls return
+        the same channel.
         """
-
-        return grpc_helpers.create_channel(
-            host,
-            credentials=credentials,
-            credentials_file=credentials_file,
-            quota_project_id=quota_project_id,
-            default_scopes=cls.AUTH_SCOPES,
-            scopes=scopes,
-            default_host=cls.DEFAULT_HOST,
-            **kwargs,
-        )
-
-    @property
-    def grpc_channel(self) -> grpc.Channel:
-        """Return the channel designed to connect to this service."""
+        # Return the channel from cache.
         return self._grpc_channel
 
     @property
-    def operations_client(self) -> operations_v1.OperationsClient:
+    def operations_client(self) -> operations_v1.OperationsAsyncClient:
         """Create the client designed to process long-running operations.
 
         This property caches on the instance; repeated calls return the same
         client.
         """
         # Quick check: Only create a new client if we do not already have one.
         if self._operations_client is None:
-            self._operations_client = operations_v1.OperationsClient(self.grpc_channel)
+            self._operations_client = operations_v1.OperationsAsyncClient(
+                self.grpc_channel
+            )
 
         # Return the client from cache.
         return self._operations_client
 
     @property
     def write_user_event(
         self,
-    ) -> Callable[[user_event_service.WriteUserEventRequest], gcr_user_event.UserEvent]:
+    ) -> Callable[
+        [user_event_service.WriteUserEventRequest], Awaitable[gcr_user_event.UserEvent]
+    ]:
         r"""Return a callable for the write user event method over gRPC.
 
         Writes a single user event.
 
         Returns:
             Callable[[~.WriteUserEventRequest],
-                    ~.UserEvent]:
+                    Awaitable[~.UserEvent]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -275,27 +282,29 @@
                 response_deserializer=gcr_user_event.UserEvent.deserialize,
             )
         return self._stubs["write_user_event"]
 
     @property
     def collect_user_event(
         self,
-    ) -> Callable[[user_event_service.CollectUserEventRequest], httpbody_pb2.HttpBody]:
+    ) -> Callable[
+        [user_event_service.CollectUserEventRequest], Awaitable[httpbody_pb2.HttpBody]
+    ]:
         r"""Return a callable for the collect user event method over gRPC.
 
         Writes a single user event from the browser. This
         uses a GET request to due to browser restriction of
         POST-ing to a 3rd party domain.
         This method is used only by the Recommendations AI
         JavaScript pixel. Users should not call this method
         directly.
 
         Returns:
             Callable[[~.CollectUserEventRequest],
-                    ~.HttpBody]:
+                    Awaitable[~.HttpBody]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -308,24 +317,24 @@
         return self._stubs["collect_user_event"]
 
     @property
     def list_user_events(
         self,
     ) -> Callable[
         [user_event_service.ListUserEventsRequest],
-        user_event_service.ListUserEventsResponse,
+        Awaitable[user_event_service.ListUserEventsResponse],
     ]:
         r"""Return a callable for the list user events method over gRPC.
 
         Gets a list of user events within a time range, with
         potential filtering.
 
         Returns:
             Callable[[~.ListUserEventsRequest],
-                    ~.ListUserEventsResponse]:
+                    Awaitable[~.ListUserEventsResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -337,27 +346,27 @@
             )
         return self._stubs["list_user_events"]
 
     @property
     def purge_user_events(
         self,
     ) -> Callable[
-        [user_event_service.PurgeUserEventsRequest], operations_pb2.Operation
+        [user_event_service.PurgeUserEventsRequest], Awaitable[operations_pb2.Operation]
     ]:
         r"""Return a callable for the purge user events method over gRPC.
 
         Deletes permanently all user events specified by the
         filter provided. Depending on the number of events
         specified by the filter, this operation could take hours
         or days to complete. To test a filter, use the list
         command first.
 
         Returns:
             Callable[[~.PurgeUserEventsRequest],
-                    ~.Operation]:
+                    Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -368,28 +377,30 @@
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["purge_user_events"]
 
     @property
     def import_user_events(
         self,
-    ) -> Callable[[import_.ImportUserEventsRequest], operations_pb2.Operation]:
+    ) -> Callable[
+        [import_.ImportUserEventsRequest], Awaitable[operations_pb2.Operation]
+    ]:
         r"""Return a callable for the import user events method over gRPC.
 
         Bulk import of User events. Request processing might
         be synchronous. Events that already exist are skipped.
         Use this method for backfilling historical user events.
         Operation.response is of type ImportResponse. Note that
         it is possible for a subset of the items to be
         successfully inserted. Operation.metadata is of type
         ImportMetadata.
 
         Returns:
             Callable[[~.ImportUserEventsRequest],
-                    ~.Operation]:
+                    Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -398,15 +409,11 @@
                 "/google.cloud.recommendationengine.v1beta1.UserEventService/ImportUserEvents",
                 request_serializer=import_.ImportUserEventsRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["import_user_events"]
 
     def close(self):
-        self.grpc_channel.close()
-
-    @property
-    def kind(self) -> str:
-        return "grpc"
+        return self.grpc_channel.close()
 
 
-__all__ = ("UserEventServiceGrpcTransport",)
+__all__ = ("UserEventServiceGrpcAsyncIOTransport",)
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/grpc_asyncio.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/grpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,107 +10,62 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import warnings
-from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
+from typing import Callable, Dict, Optional, Sequence, Tuple, Union
 
-from google.api_core import gapic_v1
-from google.api_core import grpc_helpers_async
+from google.api_core import grpc_helpers
 from google.api_core import operations_v1
+from google.api_core import gapic_v1
+import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
-from grpc.experimental import aio  # type: ignore
 
 from google.api import httpbody_pb2  # type: ignore
 from google.cloud.recommendationengine_v1beta1.types import import_
 from google.cloud.recommendationengine_v1beta1.types import user_event as gcr_user_event
 from google.cloud.recommendationengine_v1beta1.types import user_event_service
 from google.longrunning import operations_pb2  # type: ignore
 from .base import UserEventServiceTransport, DEFAULT_CLIENT_INFO
-from .grpc import UserEventServiceGrpcTransport
 
 
-class UserEventServiceGrpcAsyncIOTransport(UserEventServiceTransport):
-    """gRPC AsyncIO backend transport for UserEventService.
+class UserEventServiceGrpcTransport(UserEventServiceTransport):
+    """gRPC backend transport for UserEventService.
 
     Service for ingesting end user actions on the customer
     website.
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
     and call it.
 
     It sends protocol buffers over the wire using gRPC (which is built on
     top of HTTP/2); the ``grpcio`` package must be installed.
     """
 
-    _grpc_channel: aio.Channel
-    _stubs: Dict[str, Callable] = {}
-
-    @classmethod
-    def create_channel(
-        cls,
-        host: str = "recommendationengine.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: Optional[str] = None,
-        scopes: Optional[Sequence[str]] = None,
-        quota_project_id: Optional[str] = None,
-        **kwargs,
-    ) -> aio.Channel:
-        """Create and return a gRPC AsyncIO channel object.
-        Args:
-            host (Optional[str]): The host for the channel to use.
-            credentials (Optional[~.Credentials]): The
-                authorization credentials to attach to requests. These
-                credentials identify this application to the service. If
-                none are specified, the client will attempt to ascertain
-                the credentials from the environment.
-            credentials_file (Optional[str]): A file with credentials that can
-                be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
-            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
-                service. These are only used when credentials are not specified and
-                are passed to :func:`google.auth.default`.
-            quota_project_id (Optional[str]): An optional project to use for billing
-                and quota.
-            kwargs (Optional[dict]): Keyword arguments, which are passed to the
-                channel creation.
-        Returns:
-            aio.Channel: A gRPC AsyncIO channel object.
-        """
-
-        return grpc_helpers_async.create_channel(
-            host,
-            credentials=credentials,
-            credentials_file=credentials_file,
-            quota_project_id=quota_project_id,
-            default_scopes=cls.AUTH_SCOPES,
-            scopes=scopes,
-            default_host=cls.DEFAULT_HOST,
-            **kwargs,
-        )
+    _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "recommendationengine.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: aio.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
-        quota_project_id=None,
+        channel: Optional[grpc.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
@@ -121,18 +76,17 @@
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
                 This argument is ignored if ``channel`` is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
                 This argument is ignored if ``channel`` is provided.
-            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
-                service. These are only used when credentials are not specified and
-                are passed to :func:`google.auth.default`.
-            channel (Optional[aio.Channel]): A ``Channel`` instance through
+            scopes (Optional(Sequence[str])): A list of scopes. This argument is
+                ignored if ``channel`` is provided.
+            channel (Optional[grpc.Channel]): A ``Channel`` instance through
                 which to make calls.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
@@ -151,35 +105,36 @@
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
 
         Raises:
-            google.auth.exceptions.MutualTlsChannelError: If mutual TLS transport
+          google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
               creation failed for any reason.
           google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
               and ``credentials_file`` are passed.
         """
         self._grpc_channel = None
         self._ssl_channel_credentials = ssl_channel_credentials
         self._stubs: Dict[str, Callable] = {}
-        self._operations_client: Optional[operations_v1.OperationsAsyncClient] = None
+        self._operations_client: Optional[operations_v1.OperationsClient] = None
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
         if channel:
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
+
         else:
             if api_mtls_endpoint:
                 host = api_mtls_endpoint
 
                 # Create SSL credentials with client_cert_source or application
                 # default SSL credentials.
                 if client_cert_source:
@@ -225,53 +180,91 @@
                     ("grpc.max_receive_message_length", -1),
                 ],
             )
 
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
-    @property
-    def grpc_channel(self) -> aio.Channel:
-        """Create the channel designed to connect to this service.
+    @classmethod
+    def create_channel(
+        cls,
+        host: str = "recommendationengine.googleapis.com",
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        quota_project_id: Optional[str] = None,
+        **kwargs,
+    ) -> grpc.Channel:
+        """Create and return a gRPC channel object.
+        Args:
+            host (Optional[str]): The host for the channel to use.
+            credentials (Optional[~.Credentials]): The
+                authorization credentials to attach to requests. These
+                credentials identify this application to the service. If
+                none are specified, the client will attempt to ascertain
+                the credentials from the environment.
+            credentials_file (Optional[str]): A file with credentials that can
+                be loaded with :func:`google.auth.load_credentials_from_file`.
+                This argument is mutually exclusive with credentials.
+            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
+                service. These are only used when credentials are not specified and
+                are passed to :func:`google.auth.default`.
+            quota_project_id (Optional[str]): An optional project to use for billing
+                and quota.
+            kwargs (Optional[dict]): Keyword arguments, which are passed to the
+                channel creation.
+        Returns:
+            grpc.Channel: A gRPC channel object.
 
-        This property caches on the instance; repeated calls return
-        the same channel.
+        Raises:
+            google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
+              and ``credentials_file`` are passed.
         """
-        # Return the channel from cache.
+
+        return grpc_helpers.create_channel(
+            host,
+            credentials=credentials,
+            credentials_file=credentials_file,
+            quota_project_id=quota_project_id,
+            default_scopes=cls.AUTH_SCOPES,
+            scopes=scopes,
+            default_host=cls.DEFAULT_HOST,
+            **kwargs,
+        )
+
+    @property
+    def grpc_channel(self) -> grpc.Channel:
+        """Return the channel designed to connect to this service."""
         return self._grpc_channel
 
     @property
-    def operations_client(self) -> operations_v1.OperationsAsyncClient:
+    def operations_client(self) -> operations_v1.OperationsClient:
         """Create the client designed to process long-running operations.
 
         This property caches on the instance; repeated calls return the same
         client.
         """
         # Quick check: Only create a new client if we do not already have one.
         if self._operations_client is None:
-            self._operations_client = operations_v1.OperationsAsyncClient(
-                self.grpc_channel
-            )
+            self._operations_client = operations_v1.OperationsClient(self.grpc_channel)
 
         # Return the client from cache.
         return self._operations_client
 
     @property
     def write_user_event(
         self,
-    ) -> Callable[
-        [user_event_service.WriteUserEventRequest], Awaitable[gcr_user_event.UserEvent]
-    ]:
+    ) -> Callable[[user_event_service.WriteUserEventRequest], gcr_user_event.UserEvent]:
         r"""Return a callable for the write user event method over gRPC.
 
         Writes a single user event.
 
         Returns:
             Callable[[~.WriteUserEventRequest],
-                    Awaitable[~.UserEvent]]:
+                    ~.UserEvent]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -282,29 +275,27 @@
                 response_deserializer=gcr_user_event.UserEvent.deserialize,
             )
         return self._stubs["write_user_event"]
 
     @property
     def collect_user_event(
         self,
-    ) -> Callable[
-        [user_event_service.CollectUserEventRequest], Awaitable[httpbody_pb2.HttpBody]
-    ]:
+    ) -> Callable[[user_event_service.CollectUserEventRequest], httpbody_pb2.HttpBody]:
         r"""Return a callable for the collect user event method over gRPC.
 
         Writes a single user event from the browser. This
         uses a GET request to due to browser restriction of
         POST-ing to a 3rd party domain.
         This method is used only by the Recommendations AI
         JavaScript pixel. Users should not call this method
         directly.
 
         Returns:
             Callable[[~.CollectUserEventRequest],
-                    Awaitable[~.HttpBody]]:
+                    ~.HttpBody]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -317,24 +308,24 @@
         return self._stubs["collect_user_event"]
 
     @property
     def list_user_events(
         self,
     ) -> Callable[
         [user_event_service.ListUserEventsRequest],
-        Awaitable[user_event_service.ListUserEventsResponse],
+        user_event_service.ListUserEventsResponse,
     ]:
         r"""Return a callable for the list user events method over gRPC.
 
         Gets a list of user events within a time range, with
         potential filtering.
 
         Returns:
             Callable[[~.ListUserEventsRequest],
-                    Awaitable[~.ListUserEventsResponse]]:
+                    ~.ListUserEventsResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -346,27 +337,27 @@
             )
         return self._stubs["list_user_events"]
 
     @property
     def purge_user_events(
         self,
     ) -> Callable[
-        [user_event_service.PurgeUserEventsRequest], Awaitable[operations_pb2.Operation]
+        [user_event_service.PurgeUserEventsRequest], operations_pb2.Operation
     ]:
         r"""Return a callable for the purge user events method over gRPC.
 
         Deletes permanently all user events specified by the
         filter provided. Depending on the number of events
         specified by the filter, this operation could take hours
         or days to complete. To test a filter, use the list
         command first.
 
         Returns:
             Callable[[~.PurgeUserEventsRequest],
-                    Awaitable[~.Operation]]:
+                    ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -377,30 +368,28 @@
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["purge_user_events"]
 
     @property
     def import_user_events(
         self,
-    ) -> Callable[
-        [import_.ImportUserEventsRequest], Awaitable[operations_pb2.Operation]
-    ]:
+    ) -> Callable[[import_.ImportUserEventsRequest], operations_pb2.Operation]:
         r"""Return a callable for the import user events method over gRPC.
 
         Bulk import of User events. Request processing might
         be synchronous. Events that already exist are skipped.
         Use this method for backfilling historical user events.
         Operation.response is of type ImportResponse. Note that
         it is possible for a subset of the items to be
         successfully inserted. Operation.metadata is of type
         ImportMetadata.
 
         Returns:
             Callable[[~.ImportUserEventsRequest],
-                    Awaitable[~.Operation]]:
+                    ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -409,11 +398,15 @@
                 "/google.cloud.recommendationengine.v1beta1.UserEventService/ImportUserEvents",
                 request_serializer=import_.ImportUserEventsRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["import_user_events"]
 
     def close(self):
-        return self.grpc_channel.close()
+        self.grpc_channel.close()
+
+    @property
+    def kind(self) -> str:
+        return "grpc"
 
 
-__all__ = ("UserEventServiceGrpcAsyncIOTransport",)
+__all__ = ("UserEventServiceGrpcTransport",)
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/rest.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/services/user_event_service/transports/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,48 +70,53 @@
     * Stripping extraneous information from responses
 
     These use cases and more can be enabled by injecting an
     instance of a custom subclass when constructing the UserEventServiceRestTransport.
 
     .. code-block:: python
         class MyCustomUserEventServiceInterceptor(UserEventServiceRestInterceptor):
-            def pre_collect_user_event(request, metadata):
+            def pre_collect_user_event(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
-            def post_collect_user_event(response):
+            def post_collect_user_event(self, response):
                 logging.log(f"Received response: {response}")
+                return response
 
-            def pre_import_user_events(request, metadata):
+            def pre_import_user_events(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
-            def post_import_user_events(response):
+            def post_import_user_events(self, response):
                 logging.log(f"Received response: {response}")
+                return response
 
-            def pre_list_user_events(request, metadata):
+            def pre_list_user_events(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
-            def post_list_user_events(response):
+            def post_list_user_events(self, response):
                 logging.log(f"Received response: {response}")
+                return response
 
-            def pre_purge_user_events(request, metadata):
+            def pre_purge_user_events(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
-            def post_purge_user_events(response):
+            def post_purge_user_events(self, response):
                 logging.log(f"Received response: {response}")
+                return response
 
-            def pre_write_user_event(request, metadata):
+            def pre_write_user_event(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
-            def post_write_user_event(response):
+            def post_write_user_event(self, response):
                 logging.log(f"Received response: {response}")
+                return response
 
         transport = UserEventServiceRestTransport(interceptor=MyCustomUserEventServiceInterceptor())
         client = UserEventServiceClient(transport=transport)
 
 
     """
 
@@ -246,69 +251,62 @@
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
     and call it.
 
     It sends JSON representations of protocol buffers over HTTP/1.1
 
-    NOTE: This REST transport functionality is currently in a beta
-    state (preview). We welcome your feedback via an issue in this
-    library's source repository. Thank you!
     """
 
     def __init__(
         self,
         *,
         host: str = "recommendationengine.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         url_scheme: str = "https",
         interceptor: Optional[UserEventServiceRestInterceptor] = None,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
-        NOTE: This REST transport functionality is currently in a beta
-        state (preview). We welcome your feedback via a GitHub issue in
-        this library's repository. Thank you!
-
-         Args:
-             host (Optional[str]):
-                  The hostname to connect to.
-             credentials (Optional[google.auth.credentials.Credentials]): The
-                 authorization credentials to attach to requests. These
-                 credentials identify the application to the service; if none
-                 are specified, the client will attempt to ascertain the
-                 credentials from the environment.
-
-             credentials_file (Optional[str]): A file with credentials that can
-                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                 This argument is ignored if ``channel`` is provided.
-             scopes (Optional(Sequence[str])): A list of scopes. This argument is
-                 ignored if ``channel`` is provided.
-             client_cert_source_for_mtls (Callable[[], Tuple[bytes, bytes]]): Client
-                 certificate to configure mutual TLS HTTP channel. It is ignored
-                 if ``channel`` is provided.
-             quota_project_id (Optional[str]): An optional project to use for billing
-                 and quota.
-             client_info (google.api_core.gapic_v1.client_info.ClientInfo):
-                 The client info used to send a user-agent string along with
-                 API requests. If ``None``, then default info will be used.
-                 Generally, you only need to set this if you are developing
-                 your own client library.
-             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
-                 be used for service account credentials.
-             url_scheme: the protocol scheme for the API endpoint.  Normally
-                 "https", but for testing or local servers,
-                 "http" can be specified.
+        Args:
+            host (Optional[str]):
+                 The hostname to connect to.
+            credentials (Optional[google.auth.credentials.Credentials]): The
+                authorization credentials to attach to requests. These
+                credentials identify the application to the service; if none
+                are specified, the client will attempt to ascertain the
+                credentials from the environment.
+
+            credentials_file (Optional[str]): A file with credentials that can
+                be loaded with :func:`google.auth.load_credentials_from_file`.
+                This argument is ignored if ``channel`` is provided.
+            scopes (Optional(Sequence[str])): A list of scopes. This argument is
+                ignored if ``channel`` is provided.
+            client_cert_source_for_mtls (Callable[[], Tuple[bytes, bytes]]): Client
+                certificate to configure mutual TLS HTTP channel. It is ignored
+                if ``channel`` is provided.
+            quota_project_id (Optional[str]): An optional project to use for billing
+                and quota.
+            client_info (google.api_core.gapic_v1.client_info.ClientInfo):
+                The client info used to send a user-agent string along with
+                API requests. If ``None``, then default info will be used.
+                Generally, you only need to set this if you are developing
+                your own client library.
+            always_use_jwt_access (Optional[bool]): Whether self signed JWT should
+                be used for service account credentials.
+            url_scheme: the protocol scheme for the API endpoint.  Normally
+                "https", but for testing or local servers,
+                "http" can be specified.
         """
         # Run the base constructor
         # TODO(yon-mg): resolve other ctor params i.e. scopes, quota, etc.
         # TODO: When custom host (api_endpoint) is set, `scopes` must *also* be set on the
         # credentials object
         maybe_url_match = re.match("^(?P<scheme>http(?:s)?://)?(?P<host>.*)$", host)
         if maybe_url_match is None:
@@ -349,14 +347,15 @@
 
             rest_transport = operations_v1.OperationsRestTransport(
                 host=self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
                 scopes=self._scopes,
                 http_options=http_options,
+                path_prefix="v1beta1",
             )
 
             self._operations_client = operations_v1.AbstractOperationsClient(
                 transport=rest_transport
             )
 
         # Return the client from cache.
@@ -379,15 +378,15 @@
             }
 
         def __call__(
             self,
             request: user_event_service.CollectUserEventRequest,
             *,
             retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: float = None,
+            timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> httpbody_pb2.HttpBody:
             r"""Call the collect user event method over HTTP.
 
             Args:
                 request (~.user_event_service.CollectUserEventRequest):
                     The request object. Request message for CollectUserEvent
@@ -469,19 +468,21 @@
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(
                 json_format.MessageToJson(
                     transcoded_request["query_params"],
                     including_default_value_fields=False,
-                    use_integers_for_enums=False,
+                    use_integers_for_enums=True,
                 )
             )
             query_params.update(self._get_unset_required_fields(query_params))
 
+            query_params["$alt"] = "json;enum-encoding=int"
+
             # Send the request
             headers = dict(metadata)
             headers["Content-Type"] = "application/json"
             response = getattr(self._session, method)(
                 "{host}{uri}".format(host=self._host, uri=uri),
                 timeout=timeout,
                 headers=headers,
@@ -516,15 +517,15 @@
             }
 
         def __call__(
             self,
             request: import_.ImportUserEventsRequest,
             *,
             retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: float = None,
+            timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> operations_pb2.Operation:
             r"""Call the import user events method over HTTP.
 
             Args:
                 request (~.import_.ImportUserEventsRequest):
                     The request object. Request message for the
@@ -558,29 +559,31 @@
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             # Jsonify the request body
 
             body = json_format.MessageToJson(
                 transcoded_request["body"],
                 including_default_value_fields=False,
-                use_integers_for_enums=False,
+                use_integers_for_enums=True,
             )
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(
                 json_format.MessageToJson(
                     transcoded_request["query_params"],
                     including_default_value_fields=False,
-                    use_integers_for_enums=False,
+                    use_integers_for_enums=True,
                 )
             )
             query_params.update(self._get_unset_required_fields(query_params))
 
+            query_params["$alt"] = "json;enum-encoding=int"
+
             # Send the request
             headers = dict(metadata)
             headers["Content-Type"] = "application/json"
             response = getattr(self._session, method)(
                 "{host}{uri}".format(host=self._host, uri=uri),
                 timeout=timeout,
                 headers=headers,
@@ -614,15 +617,15 @@
             }
 
         def __call__(
             self,
             request: user_event_service.ListUserEventsRequest,
             *,
             retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: float = None,
+            timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> user_event_service.ListUserEventsResponse:
             r"""Call the list user events method over HTTP.
 
             Args:
                 request (~.user_event_service.ListUserEventsRequest):
                     The request object. Request message for ListUserEvents
@@ -657,19 +660,21 @@
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(
                 json_format.MessageToJson(
                     transcoded_request["query_params"],
                     including_default_value_fields=False,
-                    use_integers_for_enums=False,
+                    use_integers_for_enums=True,
                 )
             )
             query_params.update(self._get_unset_required_fields(query_params))
 
+            query_params["$alt"] = "json;enum-encoding=int"
+
             # Send the request
             headers = dict(metadata)
             headers["Content-Type"] = "application/json"
             response = getattr(self._session, method)(
                 "{host}{uri}".format(host=self._host, uri=uri),
                 timeout=timeout,
                 headers=headers,
@@ -704,15 +709,15 @@
             }
 
         def __call__(
             self,
             request: user_event_service.PurgeUserEventsRequest,
             *,
             retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: float = None,
+            timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> operations_pb2.Operation:
             r"""Call the purge user events method over HTTP.
 
             Args:
                 request (~.user_event_service.PurgeUserEventsRequest):
                     The request object. Request message for PurgeUserEvents
@@ -746,29 +751,31 @@
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             # Jsonify the request body
 
             body = json_format.MessageToJson(
                 transcoded_request["body"],
                 including_default_value_fields=False,
-                use_integers_for_enums=False,
+                use_integers_for_enums=True,
             )
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(
                 json_format.MessageToJson(
                     transcoded_request["query_params"],
                     including_default_value_fields=False,
-                    use_integers_for_enums=False,
+                    use_integers_for_enums=True,
                 )
             )
             query_params.update(self._get_unset_required_fields(query_params))
 
+            query_params["$alt"] = "json;enum-encoding=int"
+
             # Send the request
             headers = dict(metadata)
             headers["Content-Type"] = "application/json"
             response = getattr(self._session, method)(
                 "{host}{uri}".format(host=self._host, uri=uri),
                 timeout=timeout,
                 headers=headers,
@@ -802,15 +809,15 @@
             }
 
         def __call__(
             self,
             request: user_event_service.WriteUserEventRequest,
             *,
             retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: float = None,
+            timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> gcr_user_event.UserEvent:
             r"""Call the write user event method over HTTP.
 
             Args:
                 request (~.user_event_service.WriteUserEventRequest):
                     The request object. Request message for WriteUserEvent
@@ -845,29 +852,31 @@
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             # Jsonify the request body
 
             body = json_format.MessageToJson(
                 transcoded_request["body"],
                 including_default_value_fields=False,
-                use_integers_for_enums=False,
+                use_integers_for_enums=True,
             )
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(
                 json_format.MessageToJson(
                     transcoded_request["query_params"],
                     including_default_value_fields=False,
-                    use_integers_for_enums=False,
+                    use_integers_for_enums=True,
                 )
             )
             query_params.update(self._get_unset_required_fields(query_params))
 
+            query_params["$alt"] = "json;enum-encoding=int"
+
             # Send the request
             headers = dict(metadata)
             headers["Content-Type"] = "application/json"
             response = getattr(self._session, method)(
                 "{host}{uri}".format(host=self._host, uri=uri),
                 timeout=timeout,
                 headers=headers,
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/types/__init__.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/types/catalog.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/types/catalog.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.recommendationengine_v1beta1.types import common
 
 
 __protobuf__ = proto.module(
     package="google.cloud.recommendationengine.v1beta1",
@@ -39,15 +41,15 @@
         id (str):
             Required. Catalog item identifier. UTF-8
             encoded string with a length limit of 128 bytes.
             This id must be unique among all catalog items
             within the same catalog. It should also be used
             when logging user events in order for the user
             events to be joined with the Catalog.
-        category_hierarchies (Sequence[google.cloud.recommendationengine_v1beta1.types.CatalogItem.CategoryHierarchy]):
+        category_hierarchies (MutableSequence[google.cloud.recommendationengine_v1beta1.types.CatalogItem.CategoryHierarchy]):
             Required. Catalog item categories. This field is repeated
             for supporting one catalog item belonging to several
             parallel category hierarchies.
 
             For example, if a shoes product belongs to both ["Shoes &
             Accessories" -> "Shoes"] and ["Sports & Fitness" ->
             "Athletic Clothing" -> "Shoes"], it could be represented as:
@@ -75,15 +77,15 @@
         language_code (str):
             Optional. Language of the title/description/item_attributes.
             Use language tags defined by BCP 47.
             https://www.rfc-editor.org/rfc/bcp/bcp47.txt. Our supported
             language codes include 'en', 'es', 'fr', 'de', 'ar', 'fa',
             'zh', 'ja', 'ko', 'sv', 'ro', 'nl'. For other languages,
             contact your Google account manager.
-        tags (Sequence[str]):
+        tags (MutableSequence[str]):
             Optional. Filtering tags associated with the
             catalog item. Each tag should be a UTF-8 encoded
             string with a length limit of 1 KiB.
             This tag can be used for filtering
             recommendation results by passing the tag as
             part of the predict request filter.
         item_group_id (str):
@@ -99,62 +101,62 @@
             This field is a member of `oneof`_ ``recommendation_type``.
     """
 
     class CategoryHierarchy(proto.Message):
         r"""Category represents catalog item category hierarchy.
 
         Attributes:
-            categories (Sequence[str]):
+            categories (MutableSequence[str]):
                 Required. Catalog item categories. Each
                 category should be a UTF-8 encoded string with a
                 length limit of 2 KiB.
                 Note that the order in the list denotes the
                 specificity (from least to most specific).
         """
 
-        categories = proto.RepeatedField(
+        categories: MutableSequence[str] = proto.RepeatedField(
             proto.STRING,
             number=1,
         )
 
-    id = proto.Field(
+    id: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    category_hierarchies = proto.RepeatedField(
+    category_hierarchies: MutableSequence[CategoryHierarchy] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message=CategoryHierarchy,
     )
-    title = proto.Field(
+    title: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    description = proto.Field(
+    description: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    item_attributes = proto.Field(
+    item_attributes: common.FeatureMap = proto.Field(
         proto.MESSAGE,
         number=5,
         message=common.FeatureMap,
     )
-    language_code = proto.Field(
+    language_code: str = proto.Field(
         proto.STRING,
         number=6,
     )
-    tags = proto.RepeatedField(
+    tags: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=8,
     )
-    item_group_id = proto.Field(
+    item_group_id: str = proto.Field(
         proto.STRING,
         number=9,
     )
-    product_metadata = proto.Field(
+    product_metadata: "ProductCatalogItem" = proto.Field(
         proto.MESSAGE,
         number=10,
         oneof="recommendation_type",
         message="ProductCatalogItem",
     )
 
 
@@ -174,15 +176,15 @@
             Optional. The exact product price.
 
             This field is a member of `oneof`_ ``price``.
         price_range (google.cloud.recommendationengine_v1beta1.types.ProductCatalogItem.PriceRange):
             Optional. The product price range.
 
             This field is a member of `oneof`_ ``price``.
-        costs (Mapping[str, float]):
+        costs (MutableMapping[str, float]):
             Optional. A map to pass the costs associated with the
             product.
 
             For example: {"manufacturing": 45.5} The profit of selling
             this item is computed like so:
 
             -  If 'exactPrice' is provided, profit = displayPrice -
@@ -198,15 +200,15 @@
             ``IN_STOCK``.
         available_quantity (int):
             Optional. The available quantity of the item.
         canonical_product_uri (str):
             Optional. Canonical URL directly linking to
             the item detail page with a length limit of 5
             KiB..
-        images (Sequence[google.cloud.recommendationengine_v1beta1.types.Image]):
+        images (MutableSequence[google.cloud.recommendationengine_v1beta1.types.Image]):
             Optional. Product images for the catalog
             item.
     """
 
     class StockState(proto.Enum):
         r"""Item stock state. If this field is unspecified, the item is
         assumed to be in stock.
@@ -226,19 +228,19 @@
                 Optional. Display price of the product.
             original_price (float):
                 Optional. Price of the product without any
                 discount. If zero, by default set to be the
                 'displayPrice'.
         """
 
-        display_price = proto.Field(
+        display_price: float = proto.Field(
             proto.FLOAT,
             number=1,
         )
-        original_price = proto.Field(
+        original_price: float = proto.Field(
             proto.FLOAT,
             number=2,
         )
 
     class PriceRange(proto.Message):
         r"""Product price range when there are a range of prices for
         different variations of the same product.
@@ -246,58 +248,58 @@
         Attributes:
             min_ (float):
                 Required. The minimum product price.
             max_ (float):
                 Required. The maximum product price.
         """
 
-        min_ = proto.Field(
+        min_: float = proto.Field(
             proto.FLOAT,
             number=1,
         )
-        max_ = proto.Field(
+        max_: float = proto.Field(
             proto.FLOAT,
             number=2,
         )
 
-    exact_price = proto.Field(
+    exact_price: ExactPrice = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="price",
         message=ExactPrice,
     )
-    price_range = proto.Field(
+    price_range: PriceRange = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="price",
         message=PriceRange,
     )
-    costs = proto.MapField(
+    costs: MutableMapping[str, float] = proto.MapField(
         proto.STRING,
         proto.FLOAT,
         number=3,
     )
-    currency_code = proto.Field(
+    currency_code: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    stock_state = proto.Field(
+    stock_state: StockState = proto.Field(
         proto.ENUM,
         number=5,
         enum=StockState,
     )
-    available_quantity = proto.Field(
+    available_quantity: int = proto.Field(
         proto.INT64,
         number=6,
     )
-    canonical_product_uri = proto.Field(
+    canonical_product_uri: str = proto.Field(
         proto.STRING,
         number=7,
     )
-    images = proto.RepeatedField(
+    images: MutableSequence["Image"] = proto.RepeatedField(
         proto.MESSAGE,
         number=8,
         message="Image",
     )
 
 
 class Image(proto.Message):
@@ -311,22 +313,22 @@
             Optional. Height of the image in number of
             pixels.
         width (int):
             Optional. Width of the image in number of
             pixels.
     """
 
-    uri = proto.Field(
+    uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    height = proto.Field(
+    height: int = proto.Field(
         proto.INT32,
         number=2,
     )
-    width = proto.Field(
+    width: int = proto.Field(
         proto.INT32,
         number=3,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/types/catalog_service.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/types/catalog_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.recommendationengine_v1beta1.types import catalog
 from google.protobuf import field_mask_pb2  # type: ignore
 
 
 __protobuf__ = proto.module(
@@ -39,19 +41,19 @@
         parent (str):
             Required. The parent catalog resource name, such as
             ``projects/*/locations/global/catalogs/default_catalog``.
         catalog_item (google.cloud.recommendationengine_v1beta1.types.CatalogItem):
             Required. The catalog item to create.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    catalog_item = proto.Field(
+    catalog_item: catalog.CatalogItem = proto.Field(
         proto.MESSAGE,
         number=2,
         message=catalog.CatalogItem,
     )
 
 
 class GetCatalogItemRequest(proto.Message):
@@ -59,15 +61,15 @@
 
     Attributes:
         name (str):
             Required. Full resource name of catalog item, such as
             ``projects/*/locations/global/catalogs/default_catalog/catalogitems/some_catalog_item_id``.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ListCatalogItemsRequest(proto.Message):
     r"""Request message for ListCatalogItems method.
@@ -84,85 +86,85 @@
             Optional. The previous
             ListCatalogItemsResponse.next_page_token.
         filter (str):
             Optional. A filter to apply on the list
             results.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    page_size = proto.Field(
+    page_size: int = proto.Field(
         proto.INT32,
         number=2,
     )
-    page_token = proto.Field(
+    page_token: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    filter = proto.Field(
+    filter: str = proto.Field(
         proto.STRING,
         number=4,
     )
 
 
 class ListCatalogItemsResponse(proto.Message):
     r"""Response message for ListCatalogItems method.
 
     Attributes:
-        catalog_items (Sequence[google.cloud.recommendationengine_v1beta1.types.CatalogItem]):
+        catalog_items (MutableSequence[google.cloud.recommendationengine_v1beta1.types.CatalogItem]):
             The catalog items.
         next_page_token (str):
             If empty, the list is complete. If nonempty, the token to
             pass to the next request's
             ListCatalogItemRequest.page_token.
     """
 
     @property
     def raw_page(self):
         return self
 
-    catalog_items = proto.RepeatedField(
+    catalog_items: MutableSequence[catalog.CatalogItem] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=catalog.CatalogItem,
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class UpdateCatalogItemRequest(proto.Message):
     r"""Request message for UpdateCatalogItem method.
 
     Attributes:
         name (str):
             Required. Full resource name of catalog item, such as
-            ``projects/*/locations/global/catalogs/default_catalog/catalogItems/some_catalog_item_id``
+            ``projects/*/locations/global/catalogs/default_catalog/catalogItems/some_catalog_item_id``.
         catalog_item (google.cloud.recommendationengine_v1beta1.types.CatalogItem):
             Required. The catalog item to update/create. The
             'catalog_item_id' field has to match that in the 'name'.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Optional. Indicates which fields in the
             provided 'item' to update. If not set, will by
             default update all fields.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    catalog_item = proto.Field(
+    catalog_item: catalog.CatalogItem = proto.Field(
         proto.MESSAGE,
         number=2,
         message=catalog.CatalogItem,
     )
-    update_mask = proto.Field(
+    update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=3,
         message=field_mask_pb2.FieldMask,
     )
 
 
 class DeleteCatalogItemRequest(proto.Message):
@@ -170,14 +172,14 @@
 
     Attributes:
         name (str):
             Required. Full resource name of catalog item, such as
             ``projects/*/locations/global/catalogs/default_catalog/catalogItems/some_catalog_item_id``.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/types/common.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/types/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.cloud.recommendationengine.v1beta1",
     manifest={
         "FeatureMap",
@@ -26,67 +28,67 @@
 
 class FeatureMap(proto.Message):
     r"""FeatureMap represents extra features that customers want to
     include in the recommendation model for catalogs/user events as
     categorical/numerical features.
 
     Attributes:
-        categorical_features (Mapping[str, google.cloud.recommendationengine_v1beta1.types.FeatureMap.StringList]):
+        categorical_features (MutableMapping[str, google.cloud.recommendationengine_v1beta1.types.FeatureMap.StringList]):
             Categorical features that can take on one of a limited
             number of possible values. Some examples would be the
             brand/maker of a product, or country of a customer.
 
             Feature names and values must be UTF-8 encoded strings.
 
             For example:
             ``{ "colors": {"value": ["yellow", "green"]}, "sizes": {"value":["S", "M"]}``
-        numerical_features (Mapping[str, google.cloud.recommendationengine_v1beta1.types.FeatureMap.FloatList]):
+        numerical_features (MutableMapping[str, google.cloud.recommendationengine_v1beta1.types.FeatureMap.FloatList]):
             Numerical features. Some examples would be the height/weight
             of a product, or age of a customer.
 
             Feature names must be UTF-8 encoded strings.
 
             For example:
             ``{ "lengths_cm": {"value":[2.3, 15.4]}, "heights_cm": {"value":[8.1, 6.4]} }``
     """
 
     class StringList(proto.Message):
         r"""A list of string features.
 
         Attributes:
-            value (Sequence[str]):
+            value (MutableSequence[str]):
                 String feature value with a length limit of
                 128 bytes.
         """
 
-        value = proto.RepeatedField(
+        value: MutableSequence[str] = proto.RepeatedField(
             proto.STRING,
             number=1,
         )
 
     class FloatList(proto.Message):
         r"""A list of float features.
 
         Attributes:
-            value (Sequence[float]):
+            value (MutableSequence[float]):
                 Float feature value.
         """
 
-        value = proto.RepeatedField(
+        value: MutableSequence[float] = proto.RepeatedField(
             proto.FLOAT,
             number=1,
         )
 
-    categorical_features = proto.MapField(
+    categorical_features: MutableMapping[str, StringList] = proto.MapField(
         proto.STRING,
         proto.MESSAGE,
         number=1,
         message=StringList,
     )
-    numerical_features = proto.MapField(
+    numerical_features: MutableMapping[str, FloatList] = proto.MapField(
         proto.STRING,
         proto.MESSAGE,
         number=2,
         message=FloatList,
     )
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/types/import_.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/types/import_.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.recommendationengine_v1beta1.types import catalog
 from google.cloud.recommendationengine_v1beta1.types import user_event
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 
@@ -40,60 +42,60 @@
 
 
 class GcsSource(proto.Message):
     r"""Google Cloud Storage location for input content.
     format.
 
     Attributes:
-        input_uris (Sequence[str]):
+        input_uris (MutableSequence[str]):
             Required. Google Cloud Storage URIs to input files. URI can
             be up to 2000 characters long. URIs can match the full
             object path (for example,
             ``gs://bucket/directory/object.json``) or a pattern matching
-            one or more files, such as ````gs://bucket/directory/*.json````.
+            one or more files, such as ``gs://bucket/directory/*.json``.
             A request can contain at most 100 files, and each file can
             be up to 2 GB. See `Importing catalog
             information </recommendations-ai/docs/upload-catalog>`__ for
             the expected file format and setup instructions.
     """
 
-    input_uris = proto.RepeatedField(
+    input_uris: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=1,
     )
 
 
 class CatalogInlineSource(proto.Message):
     r"""The inline source for the input config for ImportCatalogItems
     method.
 
     Attributes:
-        catalog_items (Sequence[google.cloud.recommendationengine_v1beta1.types.CatalogItem]):
+        catalog_items (MutableSequence[google.cloud.recommendationengine_v1beta1.types.CatalogItem]):
             Optional. A list of catalog items to
             update/create. Recommended max of 10k items.
     """
 
-    catalog_items = proto.RepeatedField(
+    catalog_items: MutableSequence[catalog.CatalogItem] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=catalog.CatalogItem,
     )
 
 
 class UserEventInlineSource(proto.Message):
     r"""The inline source for the input config for ImportUserEvents
     method.
 
     Attributes:
-        user_events (Sequence[google.cloud.recommendationengine_v1beta1.types.UserEvent]):
+        user_events (MutableSequence[google.cloud.recommendationengine_v1beta1.types.UserEvent]):
             Optional. A list of user events to import.
             Recommended max of 10k items.
     """
 
-    user_events = proto.RepeatedField(
+    user_events: MutableSequence[user_event.UserEvent] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=user_event.UserEvent,
     )
 
 
 class ImportErrorsConfig(proto.Message):
@@ -107,15 +109,15 @@
             empty, existing Cloud Storage bucket. Import errors will be
             written to a file in this bucket, one per line, as a
             JSON-encoded ``google.rpc.Status`` message.
 
             This field is a member of `oneof`_ ``destination``.
     """
 
-    gcs_prefix = proto.Field(
+    gcs_prefix: str = proto.Field(
         proto.STRING,
         number=1,
         oneof="destination",
     )
 
 
 class ImportCatalogItemsRequest(proto.Message):
@@ -137,28 +139,28 @@
             Required. The desired input location of the
             data.
         errors_config (google.cloud.recommendationengine_v1beta1.types.ImportErrorsConfig):
             Optional. The desired location of errors
             incurred during the Import.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    request_id = proto.Field(
+    request_id: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    input_config = proto.Field(
+    input_config: "InputConfig" = proto.Field(
         proto.MESSAGE,
         number=3,
         message="InputConfig",
     )
-    errors_config = proto.Field(
+    errors_config: "ImportErrorsConfig" = proto.Field(
         proto.MESSAGE,
         number=4,
         message="ImportErrorsConfig",
     )
 
 
 class ImportUserEventsRequest(proto.Message):
@@ -180,28 +182,28 @@
             Required. The desired input location of the
             data.
         errors_config (google.cloud.recommendationengine_v1beta1.types.ImportErrorsConfig):
             Optional. The desired location of errors
             incurred during the Import.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    request_id = proto.Field(
+    request_id: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    input_config = proto.Field(
+    input_config: "InputConfig" = proto.Field(
         proto.MESSAGE,
         number=3,
         message="InputConfig",
     )
-    errors_config = proto.Field(
+    errors_config: "ImportErrorsConfig" = proto.Field(
         proto.MESSAGE,
         number=4,
         message="ImportErrorsConfig",
     )
 
 
 class InputConfig(proto.Message):
@@ -228,27 +230,27 @@
         user_event_inline_source (google.cloud.recommendationengine_v1beta1.types.UserEventInlineSource):
             The Inline source for the input content for
             UserEvents.
 
             This field is a member of `oneof`_ ``source``.
     """
 
-    catalog_inline_source = proto.Field(
+    catalog_inline_source: "CatalogInlineSource" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="source",
         message="CatalogInlineSource",
     )
-    gcs_source = proto.Field(
+    gcs_source: "GcsSource" = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="source",
         message="GcsSource",
     )
-    user_event_inline_source = proto.Field(
+    user_event_inline_source: "UserEventInlineSource" = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="source",
         message="UserEventInlineSource",
     )
 
 
@@ -273,98 +275,98 @@
             Count of entries that encountered errors
             while processing.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Operation last update time. If the operation
             is done, this is also the finish time.
     """
 
-    operation_name = proto.Field(
+    operation_name: str = proto.Field(
         proto.STRING,
         number=5,
     )
-    request_id = proto.Field(
+    request_id: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    create_time = proto.Field(
+    create_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=4,
         message=timestamp_pb2.Timestamp,
     )
-    success_count = proto.Field(
+    success_count: int = proto.Field(
         proto.INT64,
         number=1,
     )
-    failure_count = proto.Field(
+    failure_count: int = proto.Field(
         proto.INT64,
         number=2,
     )
-    update_time = proto.Field(
+    update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=6,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class ImportCatalogItemsResponse(proto.Message):
     r"""Response of the ImportCatalogItemsRequest. If the long
     running operation is done, then this message is returned by the
     google.longrunning.Operations.response field if the operation
     was successful.
 
     Attributes:
-        error_samples (Sequence[google.rpc.status_pb2.Status]):
+        error_samples (MutableSequence[google.rpc.status_pb2.Status]):
             A sample of errors encountered while
             processing the request.
         errors_config (google.cloud.recommendationengine_v1beta1.types.ImportErrorsConfig):
             Echoes the destination for the complete
             errors in the request if set.
     """
 
-    error_samples = proto.RepeatedField(
+    error_samples: MutableSequence[status_pb2.Status] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=status_pb2.Status,
     )
-    errors_config = proto.Field(
+    errors_config: "ImportErrorsConfig" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="ImportErrorsConfig",
     )
 
 
 class ImportUserEventsResponse(proto.Message):
     r"""Response of the ImportUserEventsRequest. If the long running
     operation was successful, then this message is returned by the
     google.longrunning.Operations.response field if the operation
     was successful.
 
     Attributes:
-        error_samples (Sequence[google.rpc.status_pb2.Status]):
+        error_samples (MutableSequence[google.rpc.status_pb2.Status]):
             A sample of errors encountered while
             processing the request.
         errors_config (google.cloud.recommendationengine_v1beta1.types.ImportErrorsConfig):
             Echoes the destination for the complete
             errors if this field was set in the request.
         import_summary (google.cloud.recommendationengine_v1beta1.types.UserEventImportSummary):
             Aggregated statistics of user event import
             status.
     """
 
-    error_samples = proto.RepeatedField(
+    error_samples: MutableSequence[status_pb2.Status] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=status_pb2.Status,
     )
-    errors_config = proto.Field(
+    errors_config: "ImportErrorsConfig" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="ImportErrorsConfig",
     )
-    import_summary = proto.Field(
+    import_summary: "UserEventImportSummary" = proto.Field(
         proto.MESSAGE,
         number=3,
         message="UserEventImportSummary",
     )
 
 
 class UserEventImportSummary(proto.Message):
@@ -377,18 +379,18 @@
             existing catalog information.
         unjoined_events_count (int):
             Count of user events imported, but with
             catalog information not found in the imported
             catalog.
     """
 
-    joined_events_count = proto.Field(
+    joined_events_count: int = proto.Field(
         proto.INT64,
         number=1,
     )
-    unjoined_events_count = proto.Field(
+    unjoined_events_count: int = proto.Field(
         proto.INT64,
         number=2,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/types/prediction_apikey_registry_service.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/types/prediction_apikey_registry_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.cloud.recommendationengine.v1beta1",
     manifest={
         "PredictionApiKeyRegistration",
@@ -32,15 +34,15 @@
     r"""Registered Api Key.
 
     Attributes:
         api_key (str):
             The API key.
     """
 
-    api_key = proto.Field(
+    api_key: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class CreatePredictionApiKeyRegistrationRequest(proto.Message):
     r"""Request message for the ``CreatePredictionApiKeyRegistration``
@@ -51,19 +53,19 @@
             Required. The parent resource path.
             ``projects/*/locations/global/catalogs/default_catalog/eventStores/default_event_store``.
         prediction_api_key_registration (google.cloud.recommendationengine_v1beta1.types.PredictionApiKeyRegistration):
             Required. The prediction API key
             registration.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    prediction_api_key_registration = proto.Field(
+    prediction_api_key_registration: "PredictionApiKeyRegistration" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="PredictionApiKeyRegistration",
     )
 
 
 class ListPredictionApiKeyRegistrationsRequest(proto.Message):
@@ -78,50 +80,52 @@
             per page. If unset, the service will choose a
             reasonable default.
         page_token (str):
             Optional. The previous
             ``ListPredictionApiKeyRegistration.nextPageToken``.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    page_size = proto.Field(
+    page_size: int = proto.Field(
         proto.INT32,
         number=2,
     )
-    page_token = proto.Field(
+    page_token: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class ListPredictionApiKeyRegistrationsResponse(proto.Message):
     r"""Response message for the ``ListPredictionApiKeyRegistrations``.
 
     Attributes:
-        prediction_api_key_registrations (Sequence[google.cloud.recommendationengine_v1beta1.types.PredictionApiKeyRegistration]):
+        prediction_api_key_registrations (MutableSequence[google.cloud.recommendationengine_v1beta1.types.PredictionApiKeyRegistration]):
             The list of registered API keys.
         next_page_token (str):
             If empty, the list is complete. If nonempty, pass the token
             to the next request's
             ``ListPredictionApiKeysRegistrationsRequest.pageToken``.
     """
 
     @property
     def raw_page(self):
         return self
 
-    prediction_api_key_registrations = proto.RepeatedField(
+    prediction_api_key_registrations: MutableSequence[
+        "PredictionApiKeyRegistration"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="PredictionApiKeyRegistration",
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class DeletePredictionApiKeyRegistrationRequest(proto.Message):
     r"""Request message for ``DeletePredictionApiKeyRegistration`` method.
@@ -129,14 +133,14 @@
     Attributes:
         name (str):
             Required. The API key to unregister including full resource
             path.
             ``projects/*/locations/global/catalogs/default_catalog/eventStores/default_event_store/predictionApiKeyRegistrations/<YOUR_API_KEY>``
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/types/prediction_service.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/types/prediction_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.recommendationengine_v1beta1.types import user_event as gcr_user_event
 from google.protobuf import struct_pb2  # type: ignore
 
 
 __protobuf__ = proto.module(
@@ -105,15 +107,15 @@
             -  filterOutOfStockItems
         dry_run (bool):
             Optional. Use dryRun mode for this prediction
             query. If set to true, a dummy model will be
             used that returns arbitrary catalog items. Note
             that the dryRun mode should only be used for
             testing the API, or if the model is not ready.
-        params (Mapping[str, google.protobuf.struct_pb2.Value]):
+        params (MutableMapping[str, google.protobuf.struct_pb2.Value]):
             Optional. Additional domain specific parameters for the
             predictions.
 
             Allowed values:
 
             -  ``returnCatalogItem``: Boolean. If set to true, the
                associated catalogItem object will be returned in the
@@ -121,15 +123,15 @@
                in the method response.
             -  ``returnItemScore``: Boolean. If set to true, the
                prediction 'score' corresponding to each returned item
                will be set in the ``metadata`` field in the prediction
                response. The given 'score' indicates the probability of
                an item being clicked/purchased given the user's context
                and history.
-        labels (Mapping[str, str]):
+        labels (MutableMapping[str, str]):
             Optional. The labels for the predict request.
 
             -  Label keys can contain lowercase letters, digits and
                hyphens, must start with a letter, and must end with a
                letter or digit.
             -  Non-zero label values can contain lowercase letters,
                digits and hyphens, must start with a letter, and must
@@ -137,137 +139,137 @@
             -  No more than 64 labels can be associated with a given
                request.
 
             See https://goo.gl/xmQnxf for more information on and
             examples of labels.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    user_event = proto.Field(
+    user_event: gcr_user_event.UserEvent = proto.Field(
         proto.MESSAGE,
         number=2,
         message=gcr_user_event.UserEvent,
     )
-    page_size = proto.Field(
+    page_size: int = proto.Field(
         proto.INT32,
         number=7,
     )
-    page_token = proto.Field(
+    page_token: str = proto.Field(
         proto.STRING,
         number=8,
     )
-    filter = proto.Field(
+    filter: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    dry_run = proto.Field(
+    dry_run: bool = proto.Field(
         proto.BOOL,
         number=4,
     )
-    params = proto.MapField(
+    params: MutableMapping[str, struct_pb2.Value] = proto.MapField(
         proto.STRING,
         proto.MESSAGE,
         number=6,
         message=struct_pb2.Value,
     )
-    labels = proto.MapField(
+    labels: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=9,
     )
 
 
 class PredictResponse(proto.Message):
     r"""Response message for predict method.
 
     Attributes:
-        results (Sequence[google.cloud.recommendationengine_v1beta1.types.PredictResponse.PredictionResult]):
+        results (MutableSequence[google.cloud.recommendationengine_v1beta1.types.PredictResponse.PredictionResult]):
             A list of recommended items. The order
             represents the ranking (from the most relevant
             item to the least).
         recommendation_token (str):
             A unique recommendation token. This should be
             included in the user event logs resulting from
             this recommendation, which enables accurate
             attribution of recommendation model performance.
-        items_missing_in_catalog (Sequence[str]):
+        items_missing_in_catalog (MutableSequence[str]):
             IDs of items in the request that were missing
             from the catalog.
         dry_run (bool):
             True if the dryRun property was set in the
             request.
-        metadata (Mapping[str, google.protobuf.struct_pb2.Value]):
+        metadata (MutableMapping[str, google.protobuf.struct_pb2.Value]):
             Additional domain specific prediction
             response metadata.
         next_page_token (str):
             If empty, the list is complete. If nonempty, the token to
             pass to the next request's PredictRequest.page_token.
     """
 
     class PredictionResult(proto.Message):
         r"""PredictionResult represents the recommendation prediction
         results.
 
         Attributes:
             id (str):
                 ID of the recommended catalog item
-            item_metadata (Mapping[str, google.protobuf.struct_pb2.Value]):
+            item_metadata (MutableMapping[str, google.protobuf.struct_pb2.Value]):
                 Additional item metadata / annotations.
 
                 Possible values:
 
                 -  ``catalogItem``: JSON representation of the catalogItem.
                    Will be set if ``returnCatalogItem`` is set to true in
                    ``PredictRequest.params``.
                 -  ``score``: Prediction score in double value. Will be set
                    if ``returnItemScore`` is set to true in
                    ``PredictRequest.params``.
         """
 
-        id = proto.Field(
+        id: str = proto.Field(
             proto.STRING,
             number=1,
         )
-        item_metadata = proto.MapField(
+        item_metadata: MutableMapping[str, struct_pb2.Value] = proto.MapField(
             proto.STRING,
             proto.MESSAGE,
             number=2,
             message=struct_pb2.Value,
         )
 
     @property
     def raw_page(self):
         return self
 
-    results = proto.RepeatedField(
+    results: MutableSequence[PredictionResult] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=PredictionResult,
     )
-    recommendation_token = proto.Field(
+    recommendation_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    items_missing_in_catalog = proto.RepeatedField(
+    items_missing_in_catalog: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=3,
     )
-    dry_run = proto.Field(
+    dry_run: bool = proto.Field(
         proto.BOOL,
         number=4,
     )
-    metadata = proto.MapField(
+    metadata: MutableMapping[str, struct_pb2.Value] = proto.MapField(
         proto.STRING,
         proto.MESSAGE,
         number=5,
         message=struct_pb2.Value,
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=6,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/types/recommendationengine_resources.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/types/recommendationengine_resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/types/user_event.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/types/user_event.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.recommendationengine_v1beta1.types import catalog
 from google.cloud.recommendationengine_v1beta1.types import common
 from google.protobuf import timestamp_pb2  # type: ignore
 
 
@@ -103,39 +105,39 @@
     class EventSource(proto.Enum):
         r"""User event source."""
         EVENT_SOURCE_UNSPECIFIED = 0
         AUTOML = 1
         ECOMMERCE = 2
         BATCH_UPLOAD = 3
 
-    event_type = proto.Field(
+    event_type: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    user_info = proto.Field(
+    user_info: "UserInfo" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="UserInfo",
     )
-    event_detail = proto.Field(
+    event_detail: "EventDetail" = proto.Field(
         proto.MESSAGE,
         number=3,
         message="EventDetail",
     )
-    product_event_detail = proto.Field(
+    product_event_detail: "ProductEventDetail" = proto.Field(
         proto.MESSAGE,
         number=4,
         message="ProductEventDetail",
     )
-    event_time = proto.Field(
+    event_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=5,
         message=timestamp_pb2.Timestamp,
     )
-    event_source = proto.Field(
+    event_source: EventSource = proto.Field(
         proto.ENUM,
         number=6,
         enum=EventSource,
     )
 
 
 class UserInfo(proto.Message):
@@ -175,31 +177,31 @@
             can be populated from the HTTP request. This should *not* be
             set when using the javascript pixel. This flag should be set
             only if the API request is made directly from the end user
             such as a mobile app (and not if a gateway or a server is
             processing and pushing the user events).
     """
 
-    visitor_id = proto.Field(
+    visitor_id: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    user_id = proto.Field(
+    user_id: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    ip_address = proto.Field(
+    ip_address: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    user_agent = proto.Field(
+    user_agent: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    direct_user_request = proto.Field(
+    direct_user_request: bool = proto.Field(
         proto.BOOL,
         number=5,
     )
 
 
 class EventDetail(proto.Message):
     r"""User event details shared by all recommendation types.
@@ -219,15 +221,15 @@
             kept the same for all user events triggered from the same
             pageview. For example, an item detail page view could
             trigger multiple events as the user is browsing the page.
             The ``pageViewId`` property should be kept the same for all
             these events so that they can be grouped together properly.
             This ``pageViewId`` will be automatically generated if using
             the JavaScript pixel.
-        experiment_ids (Sequence[str]):
+        experiment_ids (MutableSequence[str]):
             Optional. A list of identifiers for the
             independent experiment groups this user event
             belongs to. This is used to distinguish between
             user events associated with different experiment
             setups (e.g. using Recommendation Engine system,
             using different recommendation models).
         recommendation_token (str):
@@ -254,35 +256,35 @@
 
             For product recommendation, an example of extra user
             information is traffic_channel, i.e. how user arrives at the
             site. Users can arrive at the site by coming to the site
             directly, or coming through Google search, and etc.
     """
 
-    uri = proto.Field(
+    uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    referrer_uri = proto.Field(
+    referrer_uri: str = proto.Field(
         proto.STRING,
         number=6,
     )
-    page_view_id = proto.Field(
+    page_view_id: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    experiment_ids = proto.RepeatedField(
+    experiment_ids: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=3,
     )
-    recommendation_token = proto.Field(
+    recommendation_token: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    event_attributes = proto.Field(
+    event_attributes: common.FeatureMap = proto.Field(
         proto.MESSAGE,
         number=5,
         message=common.FeatureMap,
     )
 
 
 class ProductEventDetail(proto.Message):
@@ -290,22 +292,22 @@
     to retail products.
 
     Attributes:
         search_query (str):
             Required for ``search`` events. Other event types should not
             set this field. The user's search query as UTF-8 encoded
             text with a length limit of 5 KiB.
-        page_categories (Sequence[google.cloud.recommendationengine_v1beta1.types.CatalogItem.CategoryHierarchy]):
+        page_categories (MutableSequence[google.cloud.recommendationengine_v1beta1.types.CatalogItem.CategoryHierarchy]):
             Required for ``category-page-view`` events. Other event
             types should not set this field. The categories associated
             with a category page. Category pages include special pages
             such as sales or promotions. For instance, a special sale
             page may have the category hierarchy: categories : ["Sales",
             "2017 Black Friday Deals"].
-        product_details (Sequence[google.cloud.recommendationengine_v1beta1.types.ProductDetail]):
+        product_details (MutableSequence[google.cloud.recommendationengine_v1beta1.types.ProductDetail]):
             The main product details related to the event.
 
             This field is required for the following event types:
 
             -  ``add-to-cart``
             -  ``add-to-list``
             -  ``checkout-start``
@@ -343,37 +345,39 @@
         purchase_transaction (google.cloud.recommendationengine_v1beta1.types.PurchaseTransaction):
             Optional. A transaction represents the entire purchase
             transaction. Required for ``purchase-complete`` events.
             Optional for ``checkout-start`` events. Other event types
             should not set this field.
     """
 
-    search_query = proto.Field(
+    search_query: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    page_categories = proto.RepeatedField(
+    page_categories: MutableSequence[
+        catalog.CatalogItem.CategoryHierarchy
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message=catalog.CatalogItem.CategoryHierarchy,
     )
-    product_details = proto.RepeatedField(
+    product_details: MutableSequence["ProductDetail"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="ProductDetail",
     )
-    list_id = proto.Field(
+    list_id: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    cart_id = proto.Field(
+    cart_id: str = proto.Field(
         proto.STRING,
         number=5,
     )
-    purchase_transaction = proto.Field(
+    purchase_transaction: "PurchaseTransaction" = proto.Field(
         proto.MESSAGE,
         number=6,
         message="PurchaseTransaction",
     )
 
 
 class PurchaseTransaction(proto.Message):
@@ -385,18 +389,18 @@
             limit of 128 bytes.
         revenue (float):
             Required. Total revenue or grand total associated with the
             transaction. This value include shipping, tax, or other
             adjustments to total revenue that you want to include as
             part of your revenue calculations. This field is not
             required if the event type is ``refund``.
-        taxes (Mapping[str, float]):
+        taxes (MutableMapping[str, float]):
             Optional. All the taxes associated with the
             transaction.
-        costs (Mapping[str, float]):
+        costs (MutableMapping[str, float]):
             Optional. All the costs associated with the product. These
             can be manufacturing costs, shipping expenses not borne by
             the end user, or any other costs.
 
             Total product cost such that profit = revenue - (sum(taxes)
             + sum(costs)) If product_cost is not set, then profit =
             revenue - tax - shipping - sum(CatalogItem.costs).
@@ -405,33 +409,33 @@
             CatalogItem.cost based profit *cannot* be calculated for
             this Transaction.
         currency_code (str):
             Required. Currency code. Use three-character ISO-4217 code.
             This field is not required if the event type is ``refund``.
     """
 
-    id = proto.Field(
+    id: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    revenue = proto.Field(
+    revenue: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
-    taxes = proto.MapField(
+    taxes: MutableMapping[str, float] = proto.MapField(
         proto.STRING,
         proto.FLOAT,
         number=3,
     )
-    costs = proto.MapField(
+    costs: MutableMapping[str, float] = proto.MapField(
         proto.STRING,
         proto.FLOAT,
         number=4,
     )
-    currency_code = proto.Field(
+    currency_code: str = proto.Field(
         proto.STRING,
         number=6,
     )
 
 
 class ProductDetail(proto.Message):
     r"""Detailed product information associated with a user event.
@@ -475,44 +479,44 @@
             field unspecified / as zero is not sufficient to mark the
             item out of stock.
         item_attributes (google.cloud.recommendationengine_v1beta1.types.FeatureMap):
             Optional. Extra features associated with a
             product in the user event.
     """
 
-    id = proto.Field(
+    id: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    currency_code = proto.Field(
+    currency_code: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    original_price = proto.Field(
+    original_price: float = proto.Field(
         proto.FLOAT,
         number=3,
     )
-    display_price = proto.Field(
+    display_price: float = proto.Field(
         proto.FLOAT,
         number=4,
     )
-    stock_state = proto.Field(
+    stock_state: catalog.ProductCatalogItem.StockState = proto.Field(
         proto.ENUM,
         number=5,
         enum=catalog.ProductCatalogItem.StockState,
     )
-    quantity = proto.Field(
+    quantity: int = proto.Field(
         proto.INT32,
         number=6,
     )
-    available_quantity = proto.Field(
+    available_quantity: int = proto.Field(
         proto.INT32,
         number=7,
     )
-    item_attributes = proto.Field(
+    item_attributes: common.FeatureMap = proto.Field(
         proto.MESSAGE,
         number=8,
         message=common.FeatureMap,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google/cloud/recommendationengine_v1beta1/types/user_event_service.py` & `google-cloud-recommendations-ai-0.9.0/google/cloud/recommendationengine_v1beta1/types/user_event_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.recommendationengine_v1beta1.types import user_event as gcr_user_event
 from google.protobuf import timestamp_pb2  # type: ignore
 
 
 __protobuf__ = proto.module(
@@ -64,23 +66,23 @@
             Optional. The default value is false.
             Override this flag to true to actually perform
             the purge. If the field is not set to true, a
             sampling of events to be deleted will be
             returned.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    filter = proto.Field(
+    filter: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    force = proto.Field(
+    force: bool = proto.Field(
         proto.BOOL,
         number=3,
     )
 
 
 class PurgeUserEventsMetadata(proto.Message):
     r"""Metadata related to the progress of the PurgeUserEvents
@@ -90,19 +92,19 @@
     Attributes:
         operation_name (str):
             The ID of the request / operation.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Operation create time.
     """
 
-    operation_name = proto.Field(
+    operation_name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    create_time = proto.Field(
+    create_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=2,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class PurgeUserEventsResponse(proto.Message):
@@ -110,25 +112,25 @@
     operation is successfully done, then this message is returned by
     the google.longrunning.Operations.response field.
 
     Attributes:
         purged_events_count (int):
             The total count of events purged as a result
             of the operation.
-        user_events_sample (Sequence[google.cloud.recommendationengine_v1beta1.types.UserEvent]):
+        user_events_sample (MutableSequence[google.cloud.recommendationengine_v1beta1.types.UserEvent]):
             A sampling of events deleted (or will be deleted) depending
             on the ``force`` property in the request. Max of 500 items
             will be returned.
     """
 
-    purged_events_count = proto.Field(
+    purged_events_count: int = proto.Field(
         proto.INT64,
         number=1,
     )
-    user_events_sample = proto.RepeatedField(
+    user_events_sample: MutableSequence[gcr_user_event.UserEvent] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message=gcr_user_event.UserEvent,
     )
 
 
 class WriteUserEventRequest(proto.Message):
@@ -138,19 +140,19 @@
         parent (str):
             Required. The parent eventStore resource name, such as
             ``projects/1234/locations/global/catalogs/default_catalog/eventStores/default_event_store``.
         user_event (google.cloud.recommendationengine_v1beta1.types.UserEvent):
             Required. User event to write.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    user_event = proto.Field(
+    user_event: gcr_user_event.UserEvent = proto.Field(
         proto.MESSAGE,
         number=2,
         message=gcr_user_event.UserEvent,
     )
 
 
 class CollectUserEventRequest(proto.Message):
@@ -172,27 +174,27 @@
         ets (int):
             Optional. The event timestamp in
             milliseconds. This prevents browser caching of
             otherwise identical get requests. The name is
             abbreviated to reduce the payload bytes.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    user_event = proto.Field(
+    user_event: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    uri = proto.Field(
+    uri: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    ets = proto.Field(
+    ets: int = proto.Field(
         proto.INT64,
         number=4,
     )
 
 
 class ListUserEventsRequest(proto.Message):
     r"""Request message for ListUserEvents method.
@@ -243,52 +245,52 @@
             -  Example 3: eventsMissingCatalogItems eventType = search
                eventTime < "2018-04-23T18:30:43.511Z"
             -  Example 4: eventTime > "2012-04-23T18:25:43.511Z"
             -  Example 5: eventType = search
             -  Example 6: eventsMissingCatalogItems
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    page_size = proto.Field(
+    page_size: int = proto.Field(
         proto.INT32,
         number=2,
     )
-    page_token = proto.Field(
+    page_token: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    filter = proto.Field(
+    filter: str = proto.Field(
         proto.STRING,
         number=4,
     )
 
 
 class ListUserEventsResponse(proto.Message):
     r"""Response message for ListUserEvents method.
 
     Attributes:
-        user_events (Sequence[google.cloud.recommendationengine_v1beta1.types.UserEvent]):
+        user_events (MutableSequence[google.cloud.recommendationengine_v1beta1.types.UserEvent]):
             The user events.
         next_page_token (str):
             If empty, the list is complete. If nonempty, the token to
             pass to the next request's ListUserEvents.page_token.
     """
 
     @property
     def raw_page(self):
         return self
 
-    user_events = proto.RepeatedField(
+    user_events: MutableSequence[gcr_user_event.UserEvent] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=gcr_user_event.UserEvent,
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google_cloud_recommendations_ai.egg-info/PKG-INFO` & `google-cloud-recommendations-ai-0.9.0/google_cloud_recommendations_ai.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: google-cloud-recommendations-ai
-Version: 0.8.2
+Version: 0.9.0
+Summary: Google Cloud Recommendations Ai API client library
 Home-page: https://github.com/googleapis/python-recommendations-ai
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 License-File: LICENSE
 
 Python Client for Recommendations AI API
 ========================================
 
 |preview| |pypi| |versions|
```

### Comparing `google-cloud-recommendations-ai-0.8.2/google_cloud_recommendations_ai.egg-info/SOURCES.txt` & `google-cloud-recommendations-ai-0.9.0/google_cloud_recommendations_ai.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 google/cloud/recommendationengine/__init__.py
+google/cloud/recommendationengine/gapic_version.py
 google/cloud/recommendationengine/py.typed
 google/cloud/recommendationengine_v1beta1/__init__.py
 google/cloud/recommendationengine_v1beta1/gapic_metadata.json
+google/cloud/recommendationengine_v1beta1/gapic_version.py
 google/cloud/recommendationengine_v1beta1/py.typed
 google/cloud/recommendationengine_v1beta1/services/__init__.py
 google/cloud/recommendationengine_v1beta1/services/catalog_service/__init__.py
 google/cloud/recommendationengine_v1beta1/services/catalog_service/async_client.py
 google/cloud/recommendationengine_v1beta1/services/catalog_service/client.py
 google/cloud/recommendationengine_v1beta1/services/catalog_service/pagers.py
 google/cloud/recommendationengine_v1beta1/services/catalog_service/transports/__init__.py
```

### Comparing `google-cloud-recommendations-ai-0.8.2/setup.py` & `google-cloud-recommendations-ai-0.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,92 @@
 # -*- coding: utf-8 -*-
-
-# Copyright (C) 2019  Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
 import io
 import os
+
 import setuptools  # type: ignore
 
-version = "0.8.2"
+package_root = os.path.abspath(os.path.dirname(__file__))
+
+name = "google-cloud-recommendations-ai"
+
+
+description = "Google Cloud Recommendations Ai API client library"
+
+version = {}
+with open(
+    os.path.join(package_root, "google/cloud/recommendationengine/gapic_version.py")
+) as fp:
+    exec(fp.read(), version)
+version = version["__version__"]
+
+if version[0] == "0":
+    release_status = "Development Status :: 4 - Beta"
+else:
+    release_status = "Development Status :: 5 - Production/Stable"
+
+dependencies = [
+    "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
+    "proto-plus >= 1.22.0, <2.0.0dev",
+    "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
+]
+url = "https://github.com/googleapis/python-recommendations-ai"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
+packages = [
+    package
+    for package in setuptools.PEP420PackageFinder.find()
+    if package.startswith("google")
+]
+
+namespaces = ["google"]
+if "google.cloud" in packages:
+    namespaces.append("google.cloud")
+
 setuptools.setup(
-    name="google-cloud-recommendations-ai",
+    name=name,
     version=version,
+    description=description,
     long_description=readme,
     author="Google LLC",
     author_email="googleapis-packages@google.com",
     license="Apache 2.0",
-    url="https://github.com/googleapis/python-recommendations-ai",
-    packages=[
-        package
-        for package in setuptools.PEP420PackageFinder.find()
-        if package.startswith("google")
-    ],
-    namespace_packages=("google", "google.cloud"),
-    platforms="Posix; MacOS X; Windows",
-    include_package_data=True,
-    install_requires=(
-        "google-api-core[grpc] >= 1.33.2, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
-        "proto-plus >= 1.22.0, <2.0.0dev",
-        "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
-    ),
-    python_requires=">=3.7",
+    url=url,
     classifiers=[
-        "Development Status :: 4 - Beta",
+        release_status,
         "Intended Audience :: Developers",
-        "Operating System :: OS Independent",
+        "License :: OSI Approved :: Apache Software License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Operating System :: OS Independent",
         "Topic :: Internet",
-        "Topic :: Software Development :: Libraries :: Python Modules",
     ],
+    platforms="Posix; MacOS X; Windows",
+    packages=packages,
+    python_requires=">=3.7",
+    namespace_packages=namespaces,
+    install_requires=dependencies,
+    include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `google-cloud-recommendations-ai-0.8.2/tests/__init__.py` & `google-cloud-recommendations-ai-0.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/tests/unit/__init__.py` & `google-cloud-recommendations-ai-0.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/tests/unit/gapic/__init__.py` & `google-cloud-recommendations-ai-0.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/tests/unit/gapic/recommendationengine_v1beta1/__init__.py` & `google-cloud-recommendations-ai-0.9.0/tests/unit/gapic/recommendationengine_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommendations-ai-0.8.2/tests/unit/gapic/recommendationengine_v1beta1/test_catalog_service.py` & `google-cloud-recommendations-ai-0.9.0/tests/unit/gapic/recommendationengine_v1beta1/test_catalog_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -2659,15 +2659,15 @@
             json_return_value = json_format.MessageToJson(pb_return_value)
 
             response_value._content = json_return_value.encode("UTF-8")
             req.return_value = response_value
 
             response = client.create_catalog_item(request)
 
-            expected_params = []
+            expected_params = [("$alt", "json;enum-encoding=int")]
             actual_params = req.call_args.kwargs["params"]
             assert expected_params == actual_params
 
 
 def test_create_catalog_item_rest_unset_required_fields():
     transport = transports.CatalogServiceRestTransport(
         credentials=ga_credentials.AnonymousCredentials
@@ -2974,15 +2974,15 @@
             json_return_value = json_format.MessageToJson(pb_return_value)
 
             response_value._content = json_return_value.encode("UTF-8")
             req.return_value = response_value
 
             response = client.get_catalog_item(request)
 
-            expected_params = []
+            expected_params = [("$alt", "json;enum-encoding=int")]
             actual_params = req.call_args.kwargs["params"]
             assert expected_params == actual_params
 
 
 def test_get_catalog_item_rest_unset_required_fields():
     transport = transports.CatalogServiceRestTransport(
         credentials=ga_credentials.AnonymousCredentials
@@ -3252,15 +3252,15 @@
             json_return_value = json_format.MessageToJson(pb_return_value)
 
             response_value._content = json_return_value.encode("UTF-8")
             req.return_value = response_value
 
             response = client.list_catalog_items(request)
 
-            expected_params = []
+            expected_params = [("$alt", "json;enum-encoding=int")]
             actual_params = req.call_args.kwargs["params"]
             assert expected_params == actual_params
 
 
 def test_list_catalog_items_rest_unset_required_fields():
     transport = transports.CatalogServiceRestTransport(
         credentials=ga_credentials.AnonymousCredentials
@@ -3632,15 +3632,15 @@
             json_return_value = json_format.MessageToJson(pb_return_value)
 
             response_value._content = json_return_value.encode("UTF-8")
             req.return_value = response_value
 
             response = client.update_catalog_item(request)
 
-            expected_params = []
+            expected_params = [("$alt", "json;enum-encoding=int")]
             actual_params = req.call_args.kwargs["params"]
             assert expected_params == actual_params
 
 
 def test_update_catalog_item_rest_unset_required_fields():
     transport = transports.CatalogServiceRestTransport(
         credentials=ga_credentials.AnonymousCredentials
@@ -3932,15 +3932,15 @@
             json_return_value = ""
 
             response_value._content = json_return_value.encode("UTF-8")
             req.return_value = response_value
 
             response = client.delete_catalog_item(request)
 
-            expected_params = []
+            expected_params = [("$alt", "json;enum-encoding=int")]
             actual_params = req.call_args.kwargs["params"]
             assert expected_params == actual_params
 
 
 def test_delete_catalog_item_rest_unset_required_fields():
     transport = transports.CatalogServiceRestTransport(
         credentials=ga_credentials.AnonymousCredentials
@@ -4190,15 +4190,15 @@
             json_return_value = json_format.MessageToJson(return_value)
 
             response_value._content = json_return_value.encode("UTF-8")
             req.return_value = response_value
 
             response = client.import_catalog_items(request)
 
-            expected_params = []
+            expected_params = [("$alt", "json;enum-encoding=int")]
             actual_params = req.call_args.kwargs["params"]
             assert expected_params == actual_params
 
 
 def test_import_catalog_items_rest_unset_required_fields():
     transport = transports.CatalogServiceRestTransport(
         credentials=ga_credentials.AnonymousCredentials
@@ -5003,14 +5003,45 @@
     path = CatalogServiceClient.catalog_path(**expected)
 
     # Check that the path construction is reversible.
     actual = CatalogServiceClient.parse_catalog_path(path)
     assert expected == actual
 
 
+def test_catalog_item_path_path():
+    project = "cuttlefish"
+    location = "mussel"
+    catalog = "winkle"
+    catalog_item_path = "nautilus"
+    expected = "projects/{project}/locations/{location}/catalogs/{catalog}/catalogItems/{catalog_item_path}".format(
+        project=project,
+        location=location,
+        catalog=catalog,
+        catalog_item_path=catalog_item_path,
+    )
+    actual = CatalogServiceClient.catalog_item_path_path(
+        project, location, catalog, catalog_item_path
+    )
+    assert expected == actual
+
+
+def test_parse_catalog_item_path_path():
+    expected = {
+        "project": "scallop",
+        "location": "abalone",
+        "catalog": "squid",
+        "catalog_item_path": "clam",
+    }
+    path = CatalogServiceClient.catalog_item_path_path(**expected)
+
+    # Check that the path construction is reversible.
+    actual = CatalogServiceClient.parse_catalog_item_path_path(path)
+    assert expected == actual
+
+
 def test_common_billing_account_path():
     billing_account = "whelk"
     expected = "billingAccounts/{billing_account}".format(
         billing_account=billing_account,
     )
     actual = CatalogServiceClient.common_billing_account_path(billing_account)
     assert expected == actual
```

### Comparing `google-cloud-recommendations-ai-0.8.2/tests/unit/gapic/recommendationengine_v1beta1/test_prediction_api_key_registry.py` & `google-cloud-recommendations-ai-0.9.0/tests/unit/gapic/recommendationengine_v1beta1/test_prediction_api_key_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1905,15 +1905,15 @@
             json_return_value = json_format.MessageToJson(pb_return_value)
 
             response_value._content = json_return_value.encode("UTF-8")
             req.return_value = response_value
 
             response = client.create_prediction_api_key_registration(request)
 
-            expected_params = []
+            expected_params = [("$alt", "json;enum-encoding=int")]
             actual_params = req.call_args.kwargs["params"]
             assert expected_params == actual_params
 
 
 def test_create_prediction_api_key_registration_rest_unset_required_fields():
     transport = transports.PredictionApiKeyRegistryRestTransport(
         credentials=ga_credentials.AnonymousCredentials
@@ -2227,15 +2227,15 @@
             json_return_value = json_format.MessageToJson(pb_return_value)
 
             response_value._content = json_return_value.encode("UTF-8")
             req.return_value = response_value
 
             response = client.list_prediction_api_key_registrations(request)
 
-            expected_params = []
+            expected_params = [("$alt", "json;enum-encoding=int")]
             actual_params = req.call_args.kwargs["params"]
             assert expected_params == actual_params
 
 
 def test_list_prediction_api_key_registrations_rest_unset_required_fields():
     transport = transports.PredictionApiKeyRegistryRestTransport(
         credentials=ga_credentials.AnonymousCredentials
@@ -2591,15 +2591,15 @@
             json_return_value = ""
 
             response_value._content = json_return_value.encode("UTF-8")
             req.return_value = response_value
 
             response = client.delete_prediction_api_key_registration(request)
 
-            expected_params = []
+            expected_params = [("$alt", "json;enum-encoding=int")]
             actual_params = req.call_args.kwargs["params"]
             assert expected_params == actual_params
 
 
 def test_delete_prediction_api_key_registration_rest_unset_required_fields():
     transport = transports.PredictionApiKeyRegistryRestTransport(
         credentials=ga_credentials.AnonymousCredentials
```

### Comparing `google-cloud-recommendations-ai-0.8.2/tests/unit/gapic/recommendationengine_v1beta1/test_prediction_service.py` & `google-cloud-recommendations-ai-0.9.0/tests/unit/gapic/recommendationengine_v1beta1/test_prediction_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1307,15 +1307,15 @@
             json_return_value = json_format.MessageToJson(pb_return_value)
 
             response_value._content = json_return_value.encode("UTF-8")
             req.return_value = response_value
 
             response = client.predict(request)
 
-            expected_params = []
+            expected_params = [("$alt", "json;enum-encoding=int")]
             actual_params = req.call_args.kwargs["params"]
             assert expected_params == actual_params
 
 
 def test_predict_rest_unset_required_fields():
     transport = transports.PredictionServiceRestTransport(
         credentials=ga_credentials.AnonymousCredentials
```

### Comparing `google-cloud-recommendations-ai-0.8.2/tests/unit/gapic/recommendationengine_v1beta1/test_user_event_service.py` & `google-cloud-recommendations-ai-0.9.0/tests/unit/gapic/recommendationengine_v1beta1/test_user_event_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -2426,15 +2426,15 @@
             json_return_value = json_format.MessageToJson(pb_return_value)
 
             response_value._content = json_return_value.encode("UTF-8")
             req.return_value = response_value
 
             response = client.write_user_event(request)
 
-            expected_params = []
+            expected_params = [("$alt", "json;enum-encoding=int")]
             actual_params = req.call_args.kwargs["params"]
             assert expected_params == actual_params
 
 
 def test_write_user_event_rest_unset_required_fields():
     transport = transports.UserEventServiceRestTransport(
         credentials=ga_credentials.AnonymousCredentials
@@ -2779,14 +2779,15 @@
             response = client.collect_user_event(request)
 
             expected_params = [
                 (
                     "userEvent",
                     "",
                 ),
+                ("$alt", "json;enum-encoding=int"),
             ]
             actual_params = req.call_args.kwargs["params"]
             assert expected_params == actual_params
 
 
 def test_collect_user_event_rest_unset_required_fields():
     transport = transports.UserEventServiceRestTransport(
@@ -3079,15 +3080,15 @@
             json_return_value = json_format.MessageToJson(pb_return_value)
 
             response_value._content = json_return_value.encode("UTF-8")
             req.return_value = response_value
 
             response = client.list_user_events(request)
 
-            expected_params = []
+            expected_params = [("$alt", "json;enum-encoding=int")]
             actual_params = req.call_args.kwargs["params"]
             assert expected_params == actual_params
 
 
 def test_list_user_events_rest_unset_required_fields():
     transport = transports.UserEventServiceRestTransport(
         credentials=ga_credentials.AnonymousCredentials
@@ -3422,15 +3423,15 @@
             json_return_value = json_format.MessageToJson(return_value)
 
             response_value._content = json_return_value.encode("UTF-8")
             req.return_value = response_value
 
             response = client.purge_user_events(request)
 
-            expected_params = []
+            expected_params = [("$alt", "json;enum-encoding=int")]
             actual_params = req.call_args.kwargs["params"]
             assert expected_params == actual_params
 
 
 def test_purge_user_events_rest_unset_required_fields():
     transport = transports.UserEventServiceRestTransport(
         credentials=ga_credentials.AnonymousCredentials
@@ -3704,15 +3705,15 @@
             json_return_value = json_format.MessageToJson(return_value)
 
             response_value._content = json_return_value.encode("UTF-8")
             req.return_value = response_value
 
             response = client.import_user_events(request)
 
-            expected_params = []
+            expected_params = [("$alt", "json;enum-encoding=int")]
             actual_params = req.call_args.kwargs["params"]
             assert expected_params == actual_params
 
 
 def test_import_user_events_rest_unset_required_fields():
     transport = transports.UserEventServiceRestTransport(
         credentials=ga_credentials.AnonymousCredentials
```

