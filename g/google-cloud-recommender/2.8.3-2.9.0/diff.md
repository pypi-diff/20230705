# Comparing `tmp/google-cloud-recommender-2.8.3.tar.gz` & `tmp/google-cloud-recommender-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-recommender-2.8.3.tar", last modified: Mon Oct 10 16:24:12 2022, max compression
+gzip compressed data, was "google-cloud-recommender-2.9.0.tar", last modified: Wed Dec 14 20:02:52 2022, max compression
```

## Comparing `google-cloud-recommender-2.8.3.tar` & `google-cloud-recommender-2.9.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:12.292143 google-cloud-recommender-2.8.3/
--rw-rw-r--   0 root         (0)     1003    11358 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4570 2022-10-10 16:24:12.292143 google-cloud-recommender-2.8.3/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3677 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:12.280142 google-cloud-recommender-2.8.3/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:12.280142 google-cloud-recommender-2.8.3/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:12.284143 google-cloud-recommender-2.8.3/google/cloud/recommender/
--rw-rw-r--   0 root         (0)     1003     2812 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender/__init__.py
--rw-rw-r--   0 root         (0)     1003       85 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:12.284143 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/
--rw-rw-r--   0 root         (0)     1003     2535 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3824 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       85 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:12.284143 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:12.284143 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/services/recommender/
--rw-rw-r--   0 root         (0)     1003      757 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/services/recommender/__init__.py
--rw-rw-r--   0 root         (0)     1003    72793 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/services/recommender/async_client.py
--rw-rw-r--   0 root         (0)     1003    85922 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/services/recommender/client.py
--rw-rw-r--   0 root         (0)     1003    11193 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/services/recommender/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:12.284143 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/services/recommender/transports/
--rw-rw-r--   0 root         (0)     1003     1166 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/services/recommender/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    13778 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/services/recommender/transports/base.py
--rw-rw-r--   0 root         (0)     1003    28414 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/services/recommender/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    28894 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/services/recommender/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:12.284143 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/types/
--rw-rw-r--   0 root         (0)     1003     2373 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     5598 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/types/insight.py
--rw-rw-r--   0 root         (0)     1003     3864 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/types/insight_type_config.py
--rw-rw-r--   0 root         (0)     1003    17133 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/types/recommendation.py
--rw-rw-r--   0 root         (0)     1003     3879 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/types/recommender_config.py
--rw-rw-r--   0 root         (0)     1003    15132 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1/types/recommender_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:12.288143 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/
--rw-rw-r--   0 root         (0)     1003     2597 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3834 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       85 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:12.288143 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:12.288143 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/services/recommender/
--rw-rw-r--   0 root         (0)     1003      757 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/services/recommender/__init__.py
--rw-rw-r--   0 root         (0)     1003    73123 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/services/recommender/async_client.py
--rw-rw-r--   0 root         (0)     1003    86252 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/services/recommender/client.py
--rw-rw-r--   0 root         (0)     1003    11278 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/services/recommender/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:12.288143 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/services/recommender/transports/
--rw-rw-r--   0 root         (0)     1003     1166 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/services/recommender/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    13813 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/services/recommender/transports/base.py
--rw-rw-r--   0 root         (0)     1003    28489 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/services/recommender/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    28969 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/services/recommender/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:12.288143 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     2435 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     5628 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/types/insight.py
--rw-rw-r--   0 root         (0)     1003     3874 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/types/insight_type_config.py
--rw-rw-r--   0 root         (0)     1003    18345 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/types/recommendation.py
--rw-rw-r--   0 root         (0)     1003     3889 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/types/recommender_config.py
--rw-rw-r--   0 root         (0)     1003    15179 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/types/recommender_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:12.292143 google-cloud-recommender-2.8.3/google_cloud_recommender.egg-info/
--rw-r--r--   0 root         (0)     1003     4570 2022-10-10 16:24:12.000000 google-cloud-recommender-2.8.3/google_cloud_recommender.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2942 2022-10-10 16:24:12.000000 google-cloud-recommender-2.8.3/google_cloud_recommender.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:24:12.000000 google-cloud-recommender-2.8.3/google_cloud_recommender.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-10-10 16:24:12.000000 google-cloud-recommender-2.8.3/google_cloud_recommender.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:24:12.000000 google-cloud-recommender-2.8.3/google_cloud_recommender.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      256 2022-10-10 16:24:12.000000 google-cloud-recommender-2.8.3/google_cloud_recommender.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-10-10 16:24:12.000000 google-cloud-recommender-2.8.3/google_cloud_recommender.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:12.292143 google-cloud-recommender-2.8.3/scripts/
--rw-rw-r--   0 root         (0)     1003     6737 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/scripts/fixup_recommender_v1_keywords.py
--rw-rw-r--   0 root         (0)     1003     6737 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/scripts/fixup_recommender_v1beta1_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-10-10 16:24:12.292143 google-cloud-recommender-2.8.3/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2726 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:12.292143 google-cloud-recommender-2.8.3/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:12.292143 google-cloud-recommender-2.8.3/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:12.292143 google-cloud-recommender-2.8.3/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:12.292143 google-cloud-recommender-2.8.3/tests/unit/gapic/recommender_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/tests/unit/gapic/recommender_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   186269 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/tests/unit/gapic/recommender_v1/test_recommender.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:12.292143 google-cloud-recommender-2.8.3/tests/unit/gapic/recommender_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/tests/unit/gapic/recommender_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   186329 2022-10-10 16:20:52.000000 google-cloud-recommender-2.8.3/tests/unit/gapic/recommender_v1beta1/test_recommender.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 20:02:52.363047 google-cloud-recommender-2.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4554 2022-12-14 20:02:52.363047 google-cloud-recommender-2.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3677 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 20:02:52.351047 google-cloud-recommender-2.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 20:02:52.351047 google-cloud-recommender-2.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 20:02:52.355047 google-cloud-recommender-2.9.0/google/cloud/recommender/
+-rw-rw-r--   0 root         (0)     1003     2926 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       85 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 20:02:52.355047 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/
+-rw-rw-r--   0 root         (0)     1003     2649 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3824 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       85 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 20:02:52.355047 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 20:02:52.355047 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/services/recommender/
+-rw-rw-r--   0 root         (0)     1003      757 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/services/recommender/__init__.py
+-rw-rw-r--   0 root         (0)     1003    73845 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/services/recommender/async_client.py
+-rw-rw-r--   0 root         (0)     1003    86974 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/services/recommender/client.py
+-rw-rw-r--   0 root         (0)     1003    11193 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/services/recommender/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 20:02:52.355047 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/services/recommender/transports/
+-rw-rw-r--   0 root         (0)     1003     1166 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/services/recommender/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13657 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/services/recommender/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    28514 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/services/recommender/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    28981 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/services/recommender/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 20:02:52.359047 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2373 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5914 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/types/insight.py
+-rw-rw-r--   0 root         (0)     1003     4044 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/types/insight_type_config.py
+-rw-rw-r--   0 root         (0)     1003    17794 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/types/recommendation.py
+-rw-rw-r--   0 root         (0)     1003     4059 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/types/recommender_config.py
+-rw-rw-r--   0 root         (0)     1003    15685 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1/types/recommender_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 20:02:52.359047 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     2711 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3834 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       85 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 20:02:52.359047 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 20:02:52.359047 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/services/recommender/
+-rw-rw-r--   0 root         (0)     1003      757 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/services/recommender/__init__.py
+-rw-rw-r--   0 root         (0)     1003    74180 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/services/recommender/async_client.py
+-rw-rw-r--   0 root         (0)     1003    87309 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/services/recommender/client.py
+-rw-rw-r--   0 root         (0)     1003    11278 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/services/recommender/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 20:02:52.359047 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/services/recommender/transports/
+-rw-rw-r--   0 root         (0)     1003     1166 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/services/recommender/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13697 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/services/recommender/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    28589 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/services/recommender/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    29056 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/services/recommender/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 20:02:52.359047 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     2435 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5944 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/types/insight.py
+-rw-rw-r--   0 root         (0)     1003     4054 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/types/insight_type_config.py
+-rw-rw-r--   0 root         (0)     1003    19064 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/types/recommendation.py
+-rw-rw-r--   0 root         (0)     1003     4069 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/types/recommender_config.py
+-rw-rw-r--   0 root         (0)     1003    15732 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/types/recommender_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 20:02:52.363047 google-cloud-recommender-2.9.0/google_cloud_recommender.egg-info/
+-rw-r--r--   0 root         (0)     1003     4554 2022-12-14 20:02:52.000000 google-cloud-recommender-2.9.0/google_cloud_recommender.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2992 2022-12-14 20:02:52.000000 google-cloud-recommender-2.9.0/google_cloud_recommender.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-12-14 20:02:52.000000 google-cloud-recommender-2.9.0/google_cloud_recommender.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-12-14 20:02:52.000000 google-cloud-recommender-2.9.0/google_cloud_recommender.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-12-14 20:02:52.000000 google-cloud-recommender-2.9.0/google_cloud_recommender.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      257 2022-12-14 20:02:52.000000 google-cloud-recommender-2.9.0/google_cloud_recommender.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-12-14 20:02:52.000000 google-cloud-recommender-2.9.0/google_cloud_recommender.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2022-12-14 20:02:52.363047 google-cloud-recommender-2.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2883 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 20:02:52.363047 google-cloud-recommender-2.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 20:02:52.363047 google-cloud-recommender-2.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 20:02:52.363047 google-cloud-recommender-2.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 20:02:52.363047 google-cloud-recommender-2.9.0/tests/unit/gapic/recommender_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/tests/unit/gapic/recommender_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   186269 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/tests/unit/gapic/recommender_v1/test_recommender.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 20:02:52.363047 google-cloud-recommender-2.9.0/tests/unit/gapic/recommender_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/tests/unit/gapic/recommender_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   186329 2022-12-14 19:59:36.000000 google-cloud-recommender-2.9.0/tests/unit/gapic/recommender_v1beta1/test_recommender.py
```

### Comparing `google-cloud-recommender-2.8.3/LICENSE` & `google-cloud-recommender-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-recommender-2.8.3/MANIFEST.in` & `google-cloud-recommender-2.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-recommender-2.8.3/PKG-INFO` & `google-cloud-recommender-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: google-cloud-recommender
-Version: 2.8.3
-Summary: Cloud Recommender API client library
+Version: 2.9.0
+Summary: Google Cloud Recommender API client library
 Home-page: https://github.com/googleapis/python-recommender
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -15,15 +15,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
-Provides-Extra: libcst
 License-File: LICENSE
 
 Python Client for Cloud Recommender API
 =======================================
 
 |stable| |pypi| |versions|
```

### Comparing `google-cloud-recommender-2.8.3/README.rst` & `google-cloud-recommender-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender/__init__.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender/__init__.py`

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
+from google.cloud.recommender import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from google.cloud.recommender_v1.services.recommender.async_client import (
     RecommenderAsyncClient,
 )
 from google.cloud.recommender_v1.services.recommender.client import RecommenderClient
 from google.cloud.recommender_v1.types.insight import Insight, InsightStateInfo
 from google.cloud.recommender_v1.types.insight_type_config import (
```

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1/__init__.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.recommender import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from .services.recommender import RecommenderAsyncClient, RecommenderClient
 from .types.insight import Insight, InsightStateInfo
 from .types.insight_type_config import InsightTypeConfig, InsightTypeGenerationConfig
 from .types.recommendation import (
     CostProjection,
     Impact,
```

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1/gapic_metadata.json` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1/services/__init__.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1/services/recommender/__init__.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1/services/recommender/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1/services/recommender/async_client.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1/services/recommender/async_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,23 +12,34 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
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
 
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.recommender_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.protobuf import duration_pb2  # type: ignore
@@ -187,17 +198,17 @@
     get_transport_class = functools.partial(
         type(RecommenderClient).get_transport_class, type(RecommenderClient)
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, RecommenderTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the recommender client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -233,19 +244,19 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def list_insights(
         self,
-        request: Union[recommender_service.ListInsightsRequest, dict] = None,
+        request: Optional[Union[recommender_service.ListInsightsRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListInsightsAsyncPager:
         r"""Lists insights for the specified Cloud Resource. Requires the
         recommender.*.list IAM permission for the specified insight
         type.
 
         .. code-block:: python
@@ -272,15 +283,15 @@
                 page_result = client.list_insights(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1.types.ListInsightsRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1.types.ListInsightsRequest, dict]]):
                 The request object. Request for the `ListInsights`
                 method.
             parent (:class:`str`):
                 Required. The container resource on which to execute the
                 request. Acceptable formats:
 
                 -  ``projects/[PROJECT_NUMBER]/locations/[LOCATION]/insightTypes/[INSIGHT_TYPE_ID]``
@@ -374,19 +385,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_insight(
         self,
-        request: Union[recommender_service.GetInsightRequest, dict] = None,
+        request: Optional[Union[recommender_service.GetInsightRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> insight.Insight:
         r"""Gets the requested insight. Requires the recommender.*.get IAM
         permission for the specified insight type.
 
         .. code-block:: python
 
@@ -411,15 +422,15 @@
                 # Make the request
                 response = await client.get_insight(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1.types.GetInsightRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1.types.GetInsightRequest, dict]]):
                 The request object. Request to the `GetInsight` method.
             name (:class:`str`):
                 Required. Name of the insight.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
@@ -486,21 +497,23 @@
         )
 
         # Done; return the response.
         return response
 
     async def mark_insight_accepted(
         self,
-        request: Union[recommender_service.MarkInsightAcceptedRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.MarkInsightAcceptedRequest, dict]
+        ] = None,
         *,
-        name: str = None,
-        state_metadata: Mapping[str, str] = None,
-        etag: str = None,
+        name: Optional[str] = None,
+        state_metadata: Optional[MutableMapping[str, str]] = None,
+        etag: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> insight.Insight:
         r"""Marks the Insight State as Accepted. Users can use this method
         to indicate to the Recommender API that they have applied some
         action based on the insight. This stops the insight content from
         being updated.
 
@@ -532,23 +545,23 @@
                 # Make the request
                 response = await client.mark_insight_accepted(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1.types.MarkInsightAcceptedRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1.types.MarkInsightAcceptedRequest, dict]]):
                 The request object. Request for the
                 `MarkInsightAccepted` method.
             name (:class:`str`):
                 Required. Name of the insight.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            state_metadata (:class:`Mapping[str, str]`):
+            state_metadata (:class:`MutableMapping[str, str]`):
                 Optional. State properties user wish to include with
                 this state. Full replace of the current state_metadata.
 
                 This corresponds to the ``state_metadata`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             etag (:class:`str`):
@@ -617,20 +630,22 @@
         )
 
         # Done; return the response.
         return response
 
     async def list_recommendations(
         self,
-        request: Union[recommender_service.ListRecommendationsRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.ListRecommendationsRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        filter: str = None,
+        parent: Optional[str] = None,
+        filter: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListRecommendationsAsyncPager:
         r"""Lists recommendations for the specified Cloud Resource. Requires
         the recommender.*.list IAM permission for the specified
         recommender.
 
         .. code-block:: python
@@ -657,15 +672,15 @@
                 page_result = client.list_recommendations(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1.types.ListRecommendationsRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1.types.ListRecommendationsRequest, dict]]):
                 The request object. Request for the
                 `ListRecommendations` method.
             parent (:class:`str`):
                 Required. The container resource on which to execute the
                 request. Acceptable formats:
 
                 -  ``projects/[PROJECT_NUMBER]/locations/[LOCATION]/recommenders/[RECOMMENDER_ID]``
@@ -787,19 +802,21 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_recommendation(
         self,
-        request: Union[recommender_service.GetRecommendationRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.GetRecommendationRequest, dict]
+        ] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> recommendation.Recommendation:
         r"""Gets the requested recommendation. Requires the
         recommender.*.get IAM permission for the specified recommender.
 
         .. code-block:: python
 
@@ -824,15 +841,15 @@
                 # Make the request
                 response = await client.get_recommendation(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1.types.GetRecommendationRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1.types.GetRecommendationRequest, dict]]):
                 The request object. Request to the `GetRecommendation`
                 method.
             name (:class:`str`):
                 Required. Name of the recommendation.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
@@ -900,23 +917,23 @@
         )
 
         # Done; return the response.
         return response
 
     async def mark_recommendation_claimed(
         self,
-        request: Union[
-            recommender_service.MarkRecommendationClaimedRequest, dict
+        request: Optional[
+            Union[recommender_service.MarkRecommendationClaimedRequest, dict]
         ] = None,
         *,
-        name: str = None,
-        state_metadata: Mapping[str, str] = None,
-        etag: str = None,
+        name: Optional[str] = None,
+        state_metadata: Optional[MutableMapping[str, str]] = None,
+        etag: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> recommendation.Recommendation:
         r"""Marks the Recommendation State as Claimed. Users can use this
         method to indicate to the Recommender API that they are starting
         to apply the recommendation themselves. This stops the
         recommendation content from being updated. Associated insights
         are frozen and placed in the ACCEPTED state.
@@ -951,23 +968,23 @@
                 # Make the request
                 response = await client.mark_recommendation_claimed(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1.types.MarkRecommendationClaimedRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1.types.MarkRecommendationClaimedRequest, dict]]):
                 The request object. Request for the
                 `MarkRecommendationClaimed` Method.
             name (:class:`str`):
                 Required. Name of the recommendation.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            state_metadata (:class:`Mapping[str, str]`):
+            state_metadata (:class:`MutableMapping[str, str]`):
                 State properties to include with this state. Overwrites
                 any existing ``state_metadata``. Keys must match the
                 regex ``/^[a-z0-9][a-z0-9_.-]{0,62}$/``. Values must
                 match the regex ``/^[a-zA-Z0-9_./-]{0,255}$/``.
 
                 This corresponds to the ``state_metadata`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1039,23 +1056,23 @@
         )
 
         # Done; return the response.
         return response
 
     async def mark_recommendation_succeeded(
         self,
-        request: Union[
-            recommender_service.MarkRecommendationSucceededRequest, dict
+        request: Optional[
+            Union[recommender_service.MarkRecommendationSucceededRequest, dict]
         ] = None,
         *,
-        name: str = None,
-        state_metadata: Mapping[str, str] = None,
-        etag: str = None,
+        name: Optional[str] = None,
+        state_metadata: Optional[MutableMapping[str, str]] = None,
+        etag: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> recommendation.Recommendation:
         r"""Marks the Recommendation State as Succeeded. Users can use this
         method to indicate to the Recommender API that they have applied
         the recommendation themselves, and the operation was successful.
         This stops the recommendation content from being updated.
         Associated insights are frozen and placed in the ACCEPTED state.
@@ -1090,23 +1107,23 @@
                 # Make the request
                 response = await client.mark_recommendation_succeeded(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1.types.MarkRecommendationSucceededRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1.types.MarkRecommendationSucceededRequest, dict]]):
                 The request object. Request for the
                 `MarkRecommendationSucceeded` Method.
             name (:class:`str`):
                 Required. Name of the recommendation.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            state_metadata (:class:`Mapping[str, str]`):
+            state_metadata (:class:`MutableMapping[str, str]`):
                 State properties to include with this state. Overwrites
                 any existing ``state_metadata``. Keys must match the
                 regex ``/^[a-z0-9][a-z0-9_.-]{0,62}$/``. Values must
                 match the regex ``/^[a-zA-Z0-9_./-]{0,255}$/``.
 
                 This corresponds to the ``state_metadata`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1178,23 +1195,23 @@
         )
 
         # Done; return the response.
         return response
 
     async def mark_recommendation_failed(
         self,
-        request: Union[
-            recommender_service.MarkRecommendationFailedRequest, dict
+        request: Optional[
+            Union[recommender_service.MarkRecommendationFailedRequest, dict]
         ] = None,
         *,
-        name: str = None,
-        state_metadata: Mapping[str, str] = None,
-        etag: str = None,
+        name: Optional[str] = None,
+        state_metadata: Optional[MutableMapping[str, str]] = None,
+        etag: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> recommendation.Recommendation:
         r"""Marks the Recommendation State as Failed. Users can use this
         method to indicate to the Recommender API that they have applied
         the recommendation themselves, and the operation failed. This
         stops the recommendation content from being updated. Associated
         insights are frozen and placed in the ACCEPTED state.
@@ -1229,23 +1246,23 @@
                 # Make the request
                 response = await client.mark_recommendation_failed(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1.types.MarkRecommendationFailedRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1.types.MarkRecommendationFailedRequest, dict]]):
                 The request object. Request for the
                 `MarkRecommendationFailed` Method.
             name (:class:`str`):
                 Required. Name of the recommendation.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            state_metadata (:class:`Mapping[str, str]`):
+            state_metadata (:class:`MutableMapping[str, str]`):
                 State properties to include with this state. Overwrites
                 any existing ``state_metadata``. Keys must match the
                 regex ``/^[a-z0-9][a-z0-9_.-]{0,62}$/``. Values must
                 match the regex ``/^[a-zA-Z0-9_./-]{0,255}$/``.
 
                 This corresponds to the ``state_metadata`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1317,19 +1334,21 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_recommender_config(
         self,
-        request: Union[recommender_service.GetRecommenderConfigRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.GetRecommenderConfigRequest, dict]
+        ] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> recommender_config.RecommenderConfig:
         r"""Gets the requested Recommender Config. There is only
         one instance of the config for each Recommender.
 
         .. code-block:: python
 
@@ -1354,15 +1373,15 @@
                 # Make the request
                 response = await client.get_recommender_config(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1.types.GetRecommenderConfigRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1.types.GetRecommenderConfigRequest, dict]]):
                 The request object. Request for the
                 GetRecommenderConfig` method.
             name (:class:`str`):
                 Required. Name of the Recommendation Config to get.
 
                 Acceptable formats:
 
@@ -1425,20 +1444,22 @@
         )
 
         # Done; return the response.
         return response
 
     async def update_recommender_config(
         self,
-        request: Union[recommender_service.UpdateRecommenderConfigRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.UpdateRecommenderConfigRequest, dict]
+        ] = None,
         *,
-        recommender_config: gcr_recommender_config.RecommenderConfig = None,
-        update_mask: field_mask_pb2.FieldMask = None,
+        recommender_config: Optional[gcr_recommender_config.RecommenderConfig] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcr_recommender_config.RecommenderConfig:
         r"""Updates a Recommender Config. This will create a new
         revision of the config.
 
         .. code-block:: python
 
@@ -1462,15 +1483,15 @@
                 # Make the request
                 response = await client.update_recommender_config(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1.types.UpdateRecommenderConfigRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1.types.UpdateRecommenderConfigRequest, dict]]):
                 The request object. Request for the
                 `UpdateRecommenderConfig` method.
             recommender_config (:class:`google.cloud.recommender_v1.types.RecommenderConfig`):
                 Required. The RecommenderConfig to
                 update.
 
                 This corresponds to the ``recommender_config`` field
@@ -1535,19 +1556,21 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_insight_type_config(
         self,
-        request: Union[recommender_service.GetInsightTypeConfigRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.GetInsightTypeConfigRequest, dict]
+        ] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> insight_type_config.InsightTypeConfig:
         r"""Gets the requested InsightTypeConfig. There is only
         one instance of the config for each InsightType.
 
         .. code-block:: python
 
@@ -1572,15 +1595,15 @@
                 # Make the request
                 response = await client.get_insight_type_config(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1.types.GetInsightTypeConfigRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1.types.GetInsightTypeConfigRequest, dict]]):
                 The request object. Request for the
                 GetInsightTypeConfig` method.
             name (:class:`str`):
                 Required. Name of the InsightTypeConfig to get.
 
                 Acceptable formats:
 
@@ -1643,20 +1666,22 @@
         )
 
         # Done; return the response.
         return response
 
     async def update_insight_type_config(
         self,
-        request: Union[recommender_service.UpdateInsightTypeConfigRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.UpdateInsightTypeConfigRequest, dict]
+        ] = None,
         *,
-        insight_type_config: gcr_insight_type_config.InsightTypeConfig = None,
-        update_mask: field_mask_pb2.FieldMask = None,
+        insight_type_config: Optional[gcr_insight_type_config.InsightTypeConfig] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcr_insight_type_config.InsightTypeConfig:
         r"""Updates an InsightTypeConfig change. This will create
         a new revision of the config.
 
         .. code-block:: python
 
@@ -1680,15 +1705,15 @@
                 # Make the request
                 response = await client.update_insight_type_config(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1.types.UpdateInsightTypeConfigRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1.types.UpdateInsightTypeConfigRequest, dict]]):
                 The request object. Request for the
                 `UpdateInsightTypeConfig` method.
             insight_type_config (:class:`google.cloud.recommender_v1.types.InsightTypeConfig`):
                 Required. The InsightTypeConfig to
                 update.
 
                 This corresponds to the ``insight_type_config`` field
@@ -1758,18 +1783,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-recommender",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("RecommenderAsyncClient",)
```

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1/services/recommender/client.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1/services/recommender/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,26 +12,38 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
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
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.recommender_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.protobuf import duration_pb2  # type: ignore
@@ -67,15 +79,15 @@
 
     _transport_registry = OrderedDict()  # type: Dict[str, Type[RecommenderTransport]]
     _transport_registry["grpc"] = RecommenderGrpcTransport
     _transport_registry["grpc_asyncio"] = RecommenderGrpcAsyncIOTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[RecommenderTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -463,30 +475,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, RecommenderTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, RecommenderTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the recommender client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, RecommenderTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -508,14 +520,15 @@
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
@@ -560,19 +573,19 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def list_insights(
         self,
-        request: Union[recommender_service.ListInsightsRequest, dict] = None,
+        request: Optional[Union[recommender_service.ListInsightsRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListInsightsPager:
         r"""Lists insights for the specified Cloud Resource. Requires the
         recommender.*.list IAM permission for the specified insight
         type.
 
         .. code-block:: python
@@ -691,19 +704,19 @@
         )
 
         # Done; return the response.
         return response
 
     def get_insight(
         self,
-        request: Union[recommender_service.GetInsightRequest, dict] = None,
+        request: Optional[Union[recommender_service.GetInsightRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> insight.Insight:
         r"""Gets the requested insight. Requires the recommender.*.get IAM
         permission for the specified insight type.
 
         .. code-block:: python
 
@@ -793,21 +806,23 @@
         )
 
         # Done; return the response.
         return response
 
     def mark_insight_accepted(
         self,
-        request: Union[recommender_service.MarkInsightAcceptedRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.MarkInsightAcceptedRequest, dict]
+        ] = None,
         *,
-        name: str = None,
-        state_metadata: Mapping[str, str] = None,
-        etag: str = None,
+        name: Optional[str] = None,
+        state_metadata: Optional[MutableMapping[str, str]] = None,
+        etag: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> insight.Insight:
         r"""Marks the Insight State as Accepted. Users can use this method
         to indicate to the Recommender API that they have applied some
         action based on the insight. This stops the insight content from
         being updated.
 
@@ -847,15 +862,15 @@
                 The request object. Request for the
                 `MarkInsightAccepted` method.
             name (str):
                 Required. Name of the insight.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            state_metadata (Mapping[str, str]):
+            state_metadata (MutableMapping[str, str]):
                 Optional. State properties user wish to include with
                 this state. Full replace of the current state_metadata.
 
                 This corresponds to the ``state_metadata`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             etag (str):
@@ -923,20 +938,22 @@
         )
 
         # Done; return the response.
         return response
 
     def list_recommendations(
         self,
-        request: Union[recommender_service.ListRecommendationsRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.ListRecommendationsRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        filter: str = None,
+        parent: Optional[str] = None,
+        filter: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListRecommendationsPager:
         r"""Lists recommendations for the specified Cloud Resource. Requires
         the recommender.*.list IAM permission for the specified
         recommender.
 
         .. code-block:: python
@@ -1083,19 +1100,21 @@
         )
 
         # Done; return the response.
         return response
 
     def get_recommendation(
         self,
-        request: Union[recommender_service.GetRecommendationRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.GetRecommendationRequest, dict]
+        ] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> recommendation.Recommendation:
         r"""Gets the requested recommendation. Requires the
         recommender.*.get IAM permission for the specified recommender.
 
         .. code-block:: python
 
@@ -1186,23 +1205,23 @@
         )
 
         # Done; return the response.
         return response
 
     def mark_recommendation_claimed(
         self,
-        request: Union[
-            recommender_service.MarkRecommendationClaimedRequest, dict
+        request: Optional[
+            Union[recommender_service.MarkRecommendationClaimedRequest, dict]
         ] = None,
         *,
-        name: str = None,
-        state_metadata: Mapping[str, str] = None,
-        etag: str = None,
+        name: Optional[str] = None,
+        state_metadata: Optional[MutableMapping[str, str]] = None,
+        etag: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> recommendation.Recommendation:
         r"""Marks the Recommendation State as Claimed. Users can use this
         method to indicate to the Recommender API that they are starting
         to apply the recommendation themselves. This stops the
         recommendation content from being updated. Associated insights
         are frozen and placed in the ACCEPTED state.
@@ -1245,15 +1264,15 @@
                 The request object. Request for the
                 `MarkRecommendationClaimed` Method.
             name (str):
                 Required. Name of the recommendation.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            state_metadata (Mapping[str, str]):
+            state_metadata (MutableMapping[str, str]):
                 State properties to include with this state. Overwrites
                 any existing ``state_metadata``. Keys must match the
                 regex ``/^[a-z0-9][a-z0-9_.-]{0,62}$/``. Values must
                 match the regex ``/^[a-zA-Z0-9_./-]{0,255}$/``.
 
                 This corresponds to the ``state_metadata`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1328,23 +1347,23 @@
         )
 
         # Done; return the response.
         return response
 
     def mark_recommendation_succeeded(
         self,
-        request: Union[
-            recommender_service.MarkRecommendationSucceededRequest, dict
+        request: Optional[
+            Union[recommender_service.MarkRecommendationSucceededRequest, dict]
         ] = None,
         *,
-        name: str = None,
-        state_metadata: Mapping[str, str] = None,
-        etag: str = None,
+        name: Optional[str] = None,
+        state_metadata: Optional[MutableMapping[str, str]] = None,
+        etag: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> recommendation.Recommendation:
         r"""Marks the Recommendation State as Succeeded. Users can use this
         method to indicate to the Recommender API that they have applied
         the recommendation themselves, and the operation was successful.
         This stops the recommendation content from being updated.
         Associated insights are frozen and placed in the ACCEPTED state.
@@ -1387,15 +1406,15 @@
                 The request object. Request for the
                 `MarkRecommendationSucceeded` Method.
             name (str):
                 Required. Name of the recommendation.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            state_metadata (Mapping[str, str]):
+            state_metadata (MutableMapping[str, str]):
                 State properties to include with this state. Overwrites
                 any existing ``state_metadata``. Keys must match the
                 regex ``/^[a-z0-9][a-z0-9_.-]{0,62}$/``. Values must
                 match the regex ``/^[a-zA-Z0-9_./-]{0,255}$/``.
 
                 This corresponds to the ``state_metadata`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1470,23 +1489,23 @@
         )
 
         # Done; return the response.
         return response
 
     def mark_recommendation_failed(
         self,
-        request: Union[
-            recommender_service.MarkRecommendationFailedRequest, dict
+        request: Optional[
+            Union[recommender_service.MarkRecommendationFailedRequest, dict]
         ] = None,
         *,
-        name: str = None,
-        state_metadata: Mapping[str, str] = None,
-        etag: str = None,
+        name: Optional[str] = None,
+        state_metadata: Optional[MutableMapping[str, str]] = None,
+        etag: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> recommendation.Recommendation:
         r"""Marks the Recommendation State as Failed. Users can use this
         method to indicate to the Recommender API that they have applied
         the recommendation themselves, and the operation failed. This
         stops the recommendation content from being updated. Associated
         insights are frozen and placed in the ACCEPTED state.
@@ -1529,15 +1548,15 @@
                 The request object. Request for the
                 `MarkRecommendationFailed` Method.
             name (str):
                 Required. Name of the recommendation.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            state_metadata (Mapping[str, str]):
+            state_metadata (MutableMapping[str, str]):
                 State properties to include with this state. Overwrites
                 any existing ``state_metadata``. Keys must match the
                 regex ``/^[a-z0-9][a-z0-9_.-]{0,62}$/``. Values must
                 match the regex ``/^[a-zA-Z0-9_./-]{0,255}$/``.
 
                 This corresponds to the ``state_metadata`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1610,19 +1629,21 @@
         )
 
         # Done; return the response.
         return response
 
     def get_recommender_config(
         self,
-        request: Union[recommender_service.GetRecommenderConfigRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.GetRecommenderConfigRequest, dict]
+        ] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> recommender_config.RecommenderConfig:
         r"""Gets the requested Recommender Config. There is only
         one instance of the config for each Recommender.
 
         .. code-block:: python
 
@@ -1718,20 +1739,22 @@
         )
 
         # Done; return the response.
         return response
 
     def update_recommender_config(
         self,
-        request: Union[recommender_service.UpdateRecommenderConfigRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.UpdateRecommenderConfigRequest, dict]
+        ] = None,
         *,
-        recommender_config: gcr_recommender_config.RecommenderConfig = None,
-        update_mask: field_mask_pb2.FieldMask = None,
+        recommender_config: Optional[gcr_recommender_config.RecommenderConfig] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcr_recommender_config.RecommenderConfig:
         r"""Updates a Recommender Config. This will create a new
         revision of the config.
 
         .. code-block:: python
 
@@ -1830,19 +1853,21 @@
         )
 
         # Done; return the response.
         return response
 
     def get_insight_type_config(
         self,
-        request: Union[recommender_service.GetInsightTypeConfigRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.GetInsightTypeConfigRequest, dict]
+        ] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> insight_type_config.InsightTypeConfig:
         r"""Gets the requested InsightTypeConfig. There is only
         one instance of the config for each InsightType.
 
         .. code-block:: python
 
@@ -1938,20 +1963,22 @@
         )
 
         # Done; return the response.
         return response
 
     def update_insight_type_config(
         self,
-        request: Union[recommender_service.UpdateInsightTypeConfigRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.UpdateInsightTypeConfigRequest, dict]
+        ] = None,
         *,
-        insight_type_config: gcr_insight_type_config.InsightTypeConfig = None,
-        update_mask: field_mask_pb2.FieldMask = None,
+        insight_type_config: Optional[gcr_insight_type_config.InsightTypeConfig] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcr_insight_type_config.InsightTypeConfig:
         r"""Updates an InsightTypeConfig change. This will create
         a new revision of the config.
 
         .. code-block:: python
 
@@ -2062,18 +2089,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-recommender",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("RecommenderClient",)
```

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1/services/recommender/pagers.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1/services/recommender/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1/services/recommender/transports/__init__.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1/services/recommender/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1/services/recommender/transports/base.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1/services/recommender/transports/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,50 +19,45 @@
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
 
+from google.cloud.recommender_v1 import gapic_version as package_version
 from google.cloud.recommender_v1.types import (
     insight_type_config as gcr_insight_type_config,
 )
 from google.cloud.recommender_v1.types import (
     recommender_config as gcr_recommender_config,
 )
 from google.cloud.recommender_v1.types import insight
 from google.cloud.recommender_v1.types import insight_type_config
 from google.cloud.recommender_v1.types import recommendation
 from google.cloud.recommender_v1.types import recommender_config
 from google.cloud.recommender_v1.types import recommender_service
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-recommender",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class RecommenderTransport(abc.ABC):
     """Abstract transport class for Recommender."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "recommender.googleapis.com"
 
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

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1/services/recommender/transports/grpc.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1/services/recommender/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,22 +56,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "recommender.googleapis.com",
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
 
@@ -190,16 +190,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "recommender.googleapis.com",
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

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1/services/recommender/transports/grpc_asyncio.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1/services/recommender/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "recommender.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -101,23 +101,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "recommender.googleapis.com",
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

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1/types/__init__.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1/types/insight.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1/types/insight.py`

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
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import struct_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.recommender.v1",
@@ -33,15 +35,15 @@
 
     Attributes:
         name (str):
             Name of the insight.
         description (str):
             Free-form human readable summary in English.
             The maximum length is 500 characters.
-        target_resources (Sequence[str]):
+        target_resources (MutableSequence[str]):
             Fully qualified resource names that this
             insight is targeting.
         insight_subtype (str):
             Insight subtype. Insight content schema will
             be stable for a given subtype.
         content (google.protobuf.struct_pb2.Struct):
             A struct of custom fields to explain the
@@ -59,15 +61,15 @@
         category (google.cloud.recommender_v1.types.Insight.Category):
             Category being targeted by the insight.
         severity (google.cloud.recommender_v1.types.Insight.Severity):
             Insight's severity.
         etag (str):
             Fingerprint of the Insight. Provides
             optimistic locking when updating states.
-        associated_recommendations (Sequence[google.cloud.recommender_v1.types.Insight.RecommendationReference]):
+        associated_recommendations (MutableSequence[google.cloud.recommender_v1.types.Insight.RecommendationReference]):
             Recommendations derived from this insight.
     """
 
     class Category(proto.Enum):
         r"""Insight category."""
         CATEGORY_UNSPECIFIED = 0
         COST = 1
@@ -88,100 +90,102 @@
 
         Attributes:
             recommendation (str):
                 Recommendation resource name, e.g.
                 projects/[PROJECT_NUMBER]/locations/[LOCATION]/recommenders/[RECOMMENDER_ID]/recommendations/[RECOMMENDATION_ID]
         """
 
-        recommendation = proto.Field(
+        recommendation: str = proto.Field(
             proto.STRING,
             number=1,
         )
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    description = proto.Field(
+    description: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    target_resources = proto.RepeatedField(
+    target_resources: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=9,
     )
-    insight_subtype = proto.Field(
+    insight_subtype: str = proto.Field(
         proto.STRING,
         number=10,
     )
-    content = proto.Field(
+    content: struct_pb2.Struct = proto.Field(
         proto.MESSAGE,
         number=3,
         message=struct_pb2.Struct,
     )
-    last_refresh_time = proto.Field(
+    last_refresh_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=4,
         message=timestamp_pb2.Timestamp,
     )
-    observation_period = proto.Field(
+    observation_period: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=5,
         message=duration_pb2.Duration,
     )
-    state_info = proto.Field(
+    state_info: "InsightStateInfo" = proto.Field(
         proto.MESSAGE,
         number=6,
         message="InsightStateInfo",
     )
-    category = proto.Field(
+    category: Category = proto.Field(
         proto.ENUM,
         number=7,
         enum=Category,
     )
-    severity = proto.Field(
+    severity: Severity = proto.Field(
         proto.ENUM,
         number=15,
         enum=Severity,
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=11,
     )
-    associated_recommendations = proto.RepeatedField(
+    associated_recommendations: MutableSequence[
+        RecommendationReference
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=8,
         message=RecommendationReference,
     )
 
 
 class InsightStateInfo(proto.Message):
     r"""Information related to insight state.
 
     Attributes:
         state (google.cloud.recommender_v1.types.InsightStateInfo.State):
             Insight state.
-        state_metadata (Mapping[str, str]):
+        state_metadata (MutableMapping[str, str]):
             A map of metadata for the state, provided by
             user or automations systems.
     """
 
     class State(proto.Enum):
         r"""Represents insight state."""
         STATE_UNSPECIFIED = 0
         ACTIVE = 1
         ACCEPTED = 2
         DISMISSED = 3
 
-    state = proto.Field(
+    state: State = proto.Field(
         proto.ENUM,
         number=1,
         enum=State,
     )
-    state_metadata = proto.MapField(
+    state_metadata: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=2,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1/types/insight_type_config.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1/types/insight_type_config.py`

 * *Files 18% similar despite different names*

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
 from google.protobuf import struct_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.recommender.v1",
     manifest={
@@ -43,57 +45,57 @@
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Last time when the config was updated.
         revision_id (str):
             Output only. Immutable. The revision ID of
             the config. A new revision is committed whenever
             the config is changed in any way. The format is
             an 8-character hexadecimal string.
-        annotations (Mapping[str, str]):
+        annotations (MutableMapping[str, str]):
             Allows clients to store small amounts of arbitrary data.
             Annotations must follow the Kubernetes syntax. The total
             size of all keys and values combined is limited to 256k. Key
             can have 2 segments: prefix (optional) and name (required),
             separated by a slash (/). Prefix must be a DNS subdomain.
             Name must be 63 characters or less, begin and end with
             alphanumerics, with dashes (-), underscores (_), dots (.),
             and alphanumerics between.
         display_name (str):
             A user-settable field to provide a
             human-readable name to be used in user
             interfaces.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    insight_type_generation_config = proto.Field(
+    insight_type_generation_config: "InsightTypeGenerationConfig" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="InsightTypeGenerationConfig",
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    update_time = proto.Field(
+    update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=4,
         message=timestamp_pb2.Timestamp,
     )
-    revision_id = proto.Field(
+    revision_id: str = proto.Field(
         proto.STRING,
         number=5,
     )
-    annotations = proto.MapField(
+    annotations: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=6,
     )
-    display_name = proto.Field(
+    display_name: str = proto.Field(
         proto.STRING,
         number=7,
     )
 
 
 class InsightTypeGenerationConfig(proto.Message):
     r"""A configuration to customize the generation of insights.
@@ -103,15 +105,15 @@
     Attributes:
         params (google.protobuf.struct_pb2.Struct):
             Parameters for this
             InsightTypeGenerationConfig. These configs can
             be used by or are applied to all subtypes.
     """
 
-    params = proto.Field(
+    params: struct_pb2.Struct = proto.Field(
         proto.MESSAGE,
         number=1,
         message=struct_pb2.Struct,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1/types/recommendation.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1/types/recommendation.py`

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
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import struct_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.type import money_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
@@ -62,15 +64,15 @@
             Last time this recommendation was refreshed
             by the system that created it in the first
             place.
         primary_impact (google.cloud.recommender_v1.types.Impact):
             The primary impact that this recommendation
             can have while trying to optimize for one
             category.
-        additional_impact (Sequence[google.cloud.recommender_v1.types.Impact]):
+        additional_impact (MutableSequence[google.cloud.recommender_v1.types.Impact]):
             Optional set of additional impact that this
             recommendation may have when trying to optimize
             for the primary category. These may be positive
             or negative.
         priority (google.cloud.recommender_v1.types.Recommendation.Priority):
             Recommendation's priority.
         content (google.cloud.recommender_v1.types.RecommendationContent):
@@ -78,15 +80,15 @@
             recommended changes to resources.
         state_info (google.cloud.recommender_v1.types.RecommendationStateInfo):
             Information for state. Contains state and
             metadata.
         etag (str):
             Fingerprint of the Recommendation. Provides
             optimistic locking when updating states.
-        associated_insights (Sequence[google.cloud.recommender_v1.types.Recommendation.InsightReference]):
+        associated_insights (MutableSequence[google.cloud.recommender_v1.types.Recommendation.InsightReference]):
             Insights that led to this recommendation.
         xor_group_id (str):
             Corresponds to a mutually exclusive group ID
             within a recommender. A non-empty ID indicates
             that the recommendation belongs to a mutually
             exclusive group. This means that only one
             recommendation within the group is suggested to
@@ -106,115 +108,115 @@
 
         Attributes:
             insight (str):
                 Insight resource name, e.g.
                 projects/[PROJECT_NUMBER]/locations/[LOCATION]/insightTypes/[INSIGHT_TYPE_ID]/insights/[INSIGHT_ID]
         """
 
-        insight = proto.Field(
+        insight: str = proto.Field(
             proto.STRING,
             number=1,
         )
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    description = proto.Field(
+    description: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    recommender_subtype = proto.Field(
+    recommender_subtype: str = proto.Field(
         proto.STRING,
         number=12,
     )
-    last_refresh_time = proto.Field(
+    last_refresh_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=4,
         message=timestamp_pb2.Timestamp,
     )
-    primary_impact = proto.Field(
+    primary_impact: "Impact" = proto.Field(
         proto.MESSAGE,
         number=5,
         message="Impact",
     )
-    additional_impact = proto.RepeatedField(
+    additional_impact: MutableSequence["Impact"] = proto.RepeatedField(
         proto.MESSAGE,
         number=6,
         message="Impact",
     )
-    priority = proto.Field(
+    priority: Priority = proto.Field(
         proto.ENUM,
         number=17,
         enum=Priority,
     )
-    content = proto.Field(
+    content: "RecommendationContent" = proto.Field(
         proto.MESSAGE,
         number=7,
         message="RecommendationContent",
     )
-    state_info = proto.Field(
+    state_info: "RecommendationStateInfo" = proto.Field(
         proto.MESSAGE,
         number=10,
         message="RecommendationStateInfo",
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=11,
     )
-    associated_insights = proto.RepeatedField(
+    associated_insights: MutableSequence[InsightReference] = proto.RepeatedField(
         proto.MESSAGE,
         number=14,
         message=InsightReference,
     )
-    xor_group_id = proto.Field(
+    xor_group_id: str = proto.Field(
         proto.STRING,
         number=18,
     )
 
 
 class RecommendationContent(proto.Message):
     r"""Contains what resources are changing and how they are
     changing.
 
     Attributes:
-        operation_groups (Sequence[google.cloud.recommender_v1.types.OperationGroup]):
+        operation_groups (MutableSequence[google.cloud.recommender_v1.types.OperationGroup]):
             Operations to one or more Google Cloud
             resources grouped in such a way that, all
             operations within one group are expected to be
             performed atomically and in an order.
         overview (google.protobuf.struct_pb2.Struct):
             Condensed overview information about the
             recommendation.
     """
 
-    operation_groups = proto.RepeatedField(
+    operation_groups: MutableSequence["OperationGroup"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="OperationGroup",
     )
-    overview = proto.Field(
+    overview: struct_pb2.Struct = proto.Field(
         proto.MESSAGE,
         number=3,
         message=struct_pb2.Struct,
     )
 
 
 class OperationGroup(proto.Message):
     r"""Group of operations that need to be performed atomically.
 
     Attributes:
-        operations (Sequence[google.cloud.recommender_v1.types.Operation]):
+        operations (MutableSequence[google.cloud.recommender_v1.types.Operation]):
             List of operations across one or more
             resources that belong to this group. Loosely
             based on RFC6902 and should be performed in the
             order they appear.
     """
 
-    operations = proto.RepeatedField(
+    operations: MutableSequence["Operation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="Operation",
     )
 
 
 class Operation(proto.Message):
@@ -275,15 +277,15 @@
             This field is a member of `oneof`_ ``path_value``.
         value_matcher (google.cloud.recommender_v1.types.ValueMatcher):
             Can be set for action 'test' for advanced matching for the
             value of 'path' field. Either this or ``value`` will be set
             for 'test' operation.
 
             This field is a member of `oneof`_ ``path_value``.
-        path_filters (Mapping[str, google.protobuf.struct_pb2.Value]):
+        path_filters (MutableMapping[str, google.protobuf.struct_pb2.Value]):
             Set of filters to apply if ``path`` refers to array elements
             or nested array elements in order to narrow down to a single
             unique element that is being tested/modified. This is
             intended to be an exact match per filter. To perform
             advanced matching, use path_value_matchers.
 
             -  Example:
@@ -311,66 +313,66 @@
                {
                  "/bindings/*/role": "roles/owner"
                  "/bindings/*/members/*" : ["x@example.com", "y@example.com"]
                }
 
             When both path_filters and path_value_matchers are set, an
             implicit AND must be performed.
-        path_value_matchers (Mapping[str, google.cloud.recommender_v1.types.ValueMatcher]):
+        path_value_matchers (MutableMapping[str, google.cloud.recommender_v1.types.ValueMatcher]):
             Similar to path_filters, this contains set of filters to
             apply if ``path`` field refers to array elements. This is
             meant to support value matching beyond exact match. To
             perform exact match, use path_filters. When both
             path_filters and path_value_matchers are set, an implicit
             AND must be performed.
     """
 
-    action = proto.Field(
+    action: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    resource_type = proto.Field(
+    resource_type: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    resource = proto.Field(
+    resource: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    path = proto.Field(
+    path: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    source_resource = proto.Field(
+    source_resource: str = proto.Field(
         proto.STRING,
         number=5,
     )
-    source_path = proto.Field(
+    source_path: str = proto.Field(
         proto.STRING,
         number=6,
     )
-    value = proto.Field(
+    value: struct_pb2.Value = proto.Field(
         proto.MESSAGE,
         number=7,
         oneof="path_value",
         message=struct_pb2.Value,
     )
-    value_matcher = proto.Field(
+    value_matcher: "ValueMatcher" = proto.Field(
         proto.MESSAGE,
         number=10,
         oneof="path_value",
         message="ValueMatcher",
     )
-    path_filters = proto.MapField(
+    path_filters: MutableMapping[str, struct_pb2.Value] = proto.MapField(
         proto.STRING,
         proto.MESSAGE,
         number=8,
         message=struct_pb2.Value,
     )
-    path_value_matchers = proto.MapField(
+    path_value_matchers: MutableMapping[str, "ValueMatcher"] = proto.MapField(
         proto.STRING,
         proto.MESSAGE,
         number=11,
         message="ValueMatcher",
     )
 
 
@@ -388,15 +390,15 @@
             syntax
             (https://github.com/google/re2/wiki/Syntax), so
             to be used with RE2::FullMatch
 
             This field is a member of `oneof`_ ``match_variant``.
     """
 
-    matches_pattern = proto.Field(
+    matches_pattern: str = proto.Field(
         proto.STRING,
         number=1,
         oneof="match_variant",
     )
 
 
 class CostProjection(proto.Message):
@@ -413,20 +415,20 @@
             A user's permissions may affect whether the cost
             is computed using list prices or custom contract
             prices.
         duration (google.protobuf.duration_pb2.Duration):
             Duration for which this cost applies.
     """
 
-    cost = proto.Field(
+    cost: money_pb2.Money = proto.Field(
         proto.MESSAGE,
         number=1,
         message=money_pb2.Money,
     )
-    duration = proto.Field(
+    duration: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
 
 
 class SecurityProjection(proto.Message):
@@ -434,15 +436,15 @@
 
     Attributes:
         details (google.protobuf.struct_pb2.Struct):
             Additional security impact details that is
             provided by the recommender.
     """
 
-    details = proto.Field(
+    details: struct_pb2.Struct = proto.Field(
         proto.MESSAGE,
         number=2,
         message=struct_pb2.Struct,
     )
 
 
 class Impact(proto.Message):
@@ -473,60 +475,60 @@
         r"""The category of the impact."""
         CATEGORY_UNSPECIFIED = 0
         COST = 1
         SECURITY = 2
         PERFORMANCE = 3
         MANAGEABILITY = 4
 
-    category = proto.Field(
+    category: Category = proto.Field(
         proto.ENUM,
         number=1,
         enum=Category,
     )
-    cost_projection = proto.Field(
+    cost_projection: "CostProjection" = proto.Field(
         proto.MESSAGE,
         number=100,
         oneof="projection",
         message="CostProjection",
     )
-    security_projection = proto.Field(
+    security_projection: "SecurityProjection" = proto.Field(
         proto.MESSAGE,
         number=101,
         oneof="projection",
         message="SecurityProjection",
     )
 
 
 class RecommendationStateInfo(proto.Message):
     r"""Information for state. Contains state and metadata.
 
     Attributes:
         state (google.cloud.recommender_v1.types.RecommendationStateInfo.State):
             The state of the recommendation, Eg ACTIVE,
             SUCCEEDED, FAILED.
-        state_metadata (Mapping[str, str]):
+        state_metadata (MutableMapping[str, str]):
             A map of metadata for the state, provided by
             user or automations systems.
     """
 
     class State(proto.Enum):
         r"""Represents Recommendation State."""
         STATE_UNSPECIFIED = 0
         ACTIVE = 1
         CLAIMED = 6
         SUCCEEDED = 3
         FAILED = 4
         DISMISSED = 5
 
-    state = proto.Field(
+    state: State = proto.Field(
         proto.ENUM,
         number=1,
         enum=State,
     )
-    state_metadata = proto.MapField(
+    state_metadata: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=2,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1/types/recommender_config.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1/types/recommender_config.py`

 * *Files 9% similar despite different names*

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
 from google.protobuf import struct_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.recommender.v1",
     manifest={
@@ -43,57 +45,57 @@
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Last time when the config was updated.
         revision_id (str):
             Output only. Immutable. The revision ID of
             the config. A new revision is committed whenever
             the config is changed in any way. The format is
             an 8-character hexadecimal string.
-        annotations (Mapping[str, str]):
+        annotations (MutableMapping[str, str]):
             Allows clients to store small amounts of arbitrary data.
             Annotations must follow the Kubernetes syntax. The total
             size of all keys and values combined is limited to 256k. Key
             can have 2 segments: prefix (optional) and name (required),
             separated by a slash (/). Prefix must be a DNS subdomain.
             Name must be 63 characters or less, begin and end with
             alphanumerics, with dashes (-), underscores (_), dots (.),
             and alphanumerics between.
         display_name (str):
             A user-settable field to provide a
             human-readable name to be used in user
             interfaces.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    recommender_generation_config = proto.Field(
+    recommender_generation_config: "RecommenderGenerationConfig" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="RecommenderGenerationConfig",
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    update_time = proto.Field(
+    update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=4,
         message=timestamp_pb2.Timestamp,
     )
-    revision_id = proto.Field(
+    revision_id: str = proto.Field(
         proto.STRING,
         number=5,
     )
-    annotations = proto.MapField(
+    annotations: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=6,
     )
-    display_name = proto.Field(
+    display_name: str = proto.Field(
         proto.STRING,
         number=7,
     )
 
 
 class RecommenderGenerationConfig(proto.Message):
     r"""A Configuration to customize the generation of
@@ -103,15 +105,15 @@
     Attributes:
         params (google.protobuf.struct_pb2.Struct):
             Parameters for this
             RecommenderGenerationConfig. These configs can
             be used by or are applied to all subtypes.
     """
 
-    params = proto.Field(
+    params: struct_pb2.Struct = proto.Field(
         proto.MESSAGE,
         number=1,
         message=struct_pb2.Struct,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1/types/recommender_service.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/types/recommender_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,28 +9,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 from google.protobuf import field_mask_pb2  # type: ignore
 import proto  # type: ignore
 
-from google.cloud.recommender_v1.types import (
+from google.cloud.recommender_v1beta1.types import (
     insight_type_config as gcr_insight_type_config,
 )
-from google.cloud.recommender_v1.types import (
+from google.cloud.recommender_v1beta1.types import (
     recommender_config as gcr_recommender_config,
 )
-from google.cloud.recommender_v1.types import insight
-from google.cloud.recommender_v1.types import recommendation
+from google.cloud.recommender_v1beta1.types import insight
+from google.cloud.recommender_v1beta1.types import recommendation
 
 __protobuf__ = proto.module(
-    package="google.cloud.recommender.v1",
+    package="google.cloud.recommender.v1beta1",
     manifest={
         "ListInsightsRequest",
         "ListInsightsResponse",
         "GetInsightRequest",
         "MarkInsightAcceptedRequest",
         "ListRecommendationsRequest",
         "ListRecommendationsResponse",
@@ -66,15 +68,15 @@
 
             LOCATION here refers to GCP Locations:
             https://cloud.google.com/about/locations/ INSIGHT_TYPE_ID
             refers to supported insight types:
             https://cloud.google.com/recommender/docs/insights/insight-types.
         page_size (int):
             Optional. The maximum number of results to
-            return from this request. Non-positive values
+            return from this request.  Non-positive values
             are ignored. If not specified, the server will
             determine the number of results to return.
         page_token (str):
             Optional. If present, retrieves the next batch of results
             from the preceding call to this method. ``page_token`` must
             be the value of ``next_page_token`` from the previous
             response. The values of other method parameters must be
@@ -99,97 +101,97 @@
 
             -  ``stateInfo.state = ACTIVE AND (severity = CRITICAL OR severity = HIGH)``
 
             (These expressions are based on the filter language
             described at https://google.aip.dev/160)
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
 
 
 class ListInsightsResponse(proto.Message):
     r"""Response to the ``ListInsights`` method.
 
     Attributes:
-        insights (Sequence[google.cloud.recommender_v1.types.Insight]):
+        insights (MutableSequence[google.cloud.recommender_v1beta1.types.Insight]):
             The set of insights for the ``parent`` resource.
         next_page_token (str):
             A token that can be used to request the next
             page of results. This field is empty if there
             are no additional results.
     """
 
     @property
     def raw_page(self):
         return self
 
-    insights = proto.RepeatedField(
+    insights: MutableSequence[insight.Insight] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=insight.Insight,
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class GetInsightRequest(proto.Message):
     r"""Request to the ``GetInsight`` method.
 
     Attributes:
         name (str):
             Required. Name of the insight.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class MarkInsightAcceptedRequest(proto.Message):
     r"""Request for the ``MarkInsightAccepted`` method.
 
     Attributes:
         name (str):
             Required. Name of the insight.
-        state_metadata (Mapping[str, str]):
+        state_metadata (MutableMapping[str, str]):
             Optional. State properties user wish to include with this
             state. Full replace of the current state_metadata.
         etag (str):
             Required. Fingerprint of the Insight.
             Provides optimistic locking.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    state_metadata = proto.MapField(
+    state_metadata: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=2,
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class ListRecommendationsRequest(proto.Message):
     r"""Request for the ``ListRecommendations`` method.
@@ -211,15 +213,15 @@
 
             LOCATION here refers to GCP Locations:
             https://cloud.google.com/about/locations/ RECOMMENDER_ID
             refers to supported recommenders:
             https://cloud.google.com/recommender/docs/recommenders.
         page_size (int):
             Optional. The maximum number of results to
-            return from this request. Non-positive values
+            return from this request.  Non-positive values
             are ignored. If not specified, the server will
             determine the number of results to return.
         page_token (str):
             Optional. If present, retrieves the next batch of results
             from the preceding call to this method. ``page_token`` must
             be the value of ``next_page_token`` from the previous
             response. The values of other method parameters must be
@@ -244,161 +246,163 @@
 
             -  ``stateInfo.state = ACTIVE AND (priority = P1 OR priority = P2)``
 
             (These expressions are based on the filter language
             described at https://google.aip.dev/160)
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
         number=5,
     )
 
 
 class ListRecommendationsResponse(proto.Message):
     r"""Response to the ``ListRecommendations`` method.
 
     Attributes:
-        recommendations (Sequence[google.cloud.recommender_v1.types.Recommendation]):
+        recommendations (MutableSequence[google.cloud.recommender_v1beta1.types.Recommendation]):
             The set of recommendations for the ``parent`` resource.
         next_page_token (str):
             A token that can be used to request the next
             page of results. This field is empty if there
             are no additional results.
     """
 
     @property
     def raw_page(self):
         return self
 
-    recommendations = proto.RepeatedField(
+    recommendations: MutableSequence[
+        recommendation.Recommendation
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=recommendation.Recommendation,
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class GetRecommendationRequest(proto.Message):
     r"""Request to the ``GetRecommendation`` method.
 
     Attributes:
         name (str):
             Required. Name of the recommendation.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class MarkRecommendationClaimedRequest(proto.Message):
     r"""Request for the ``MarkRecommendationClaimed`` Method.
 
     Attributes:
         name (str):
             Required. Name of the recommendation.
-        state_metadata (Mapping[str, str]):
+        state_metadata (MutableMapping[str, str]):
             State properties to include with this state. Overwrites any
             existing ``state_metadata``. Keys must match the regex
             ``/^[a-z0-9][a-z0-9_.-]{0,62}$/``. Values must match the
             regex ``/^[a-zA-Z0-9_./-]{0,255}$/``.
         etag (str):
             Required. Fingerprint of the Recommendation.
             Provides optimistic locking.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    state_metadata = proto.MapField(
+    state_metadata: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=2,
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class MarkRecommendationSucceededRequest(proto.Message):
     r"""Request for the ``MarkRecommendationSucceeded`` Method.
 
     Attributes:
         name (str):
             Required. Name of the recommendation.
-        state_metadata (Mapping[str, str]):
+        state_metadata (MutableMapping[str, str]):
             State properties to include with this state. Overwrites any
             existing ``state_metadata``. Keys must match the regex
             ``/^[a-z0-9][a-z0-9_.-]{0,62}$/``. Values must match the
             regex ``/^[a-zA-Z0-9_./-]{0,255}$/``.
         etag (str):
             Required. Fingerprint of the Recommendation.
             Provides optimistic locking.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    state_metadata = proto.MapField(
+    state_metadata: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=2,
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class MarkRecommendationFailedRequest(proto.Message):
     r"""Request for the ``MarkRecommendationFailed`` Method.
 
     Attributes:
         name (str):
             Required. Name of the recommendation.
-        state_metadata (Mapping[str, str]):
+        state_metadata (MutableMapping[str, str]):
             State properties to include with this state. Overwrites any
             existing ``state_metadata``. Keys must match the regex
             ``/^[a-z0-9][a-z0-9_.-]{0,62}$/``. Values must match the
             regex ``/^[a-zA-Z0-9_./-]{0,255}$/``.
         etag (str):
             Required. Fingerprint of the Recommendation.
             Provides optimistic locking.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    state_metadata = proto.MapField(
+    state_metadata: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=2,
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class GetRecommenderConfigRequest(proto.Message):
     r"""Request for the GetRecommenderConfig\` method.
@@ -412,44 +416,44 @@
             -  ``projects/[PROJECT_NUMBER]/locations/[LOCATION]/recommenders/[RECOMMENDER_ID]/config``
 
             -  ``projects/[PROJECT_ID]/locations/[LOCATION]/recommenders/[RECOMMENDER_ID]/config``
 
             -  ``organizations/[ORGANIZATION_ID]/locations/[LOCATION]/recommenders/[RECOMMENDER_ID]/config``
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class UpdateRecommenderConfigRequest(proto.Message):
     r"""Request for the ``UpdateRecommenderConfig`` method.
 
     Attributes:
-        recommender_config (google.cloud.recommender_v1.types.RecommenderConfig):
+        recommender_config (google.cloud.recommender_v1beta1.types.RecommenderConfig):
             Required. The RecommenderConfig to update.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             The list of fields to be updated.
         validate_only (bool):
             If true, validate the request and preview the
             change, but do not actually update it.
     """
 
-    recommender_config = proto.Field(
+    recommender_config: gcr_recommender_config.RecommenderConfig = proto.Field(
         proto.MESSAGE,
         number=1,
         message=gcr_recommender_config.RecommenderConfig,
     )
-    update_mask = proto.Field(
+    update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=2,
         message=field_mask_pb2.FieldMask,
     )
-    validate_only = proto.Field(
+    validate_only: bool = proto.Field(
         proto.BOOL,
         number=3,
     )
 
 
 class GetInsightTypeConfigRequest(proto.Message):
     r"""Request for the GetInsightTypeConfig\` method.
@@ -463,43 +467,43 @@
             -  ``projects/[PROJECT_NUMBER]/locations/global/recommenders/[INSIGHT_TYPE_ID]/config``
 
             -  ``projects/[PROJECT_ID]/locations/global/recommenders/[INSIGHT_TYPE_ID]/config``
 
             -  ``organizations/[ORGANIZATION_ID]/locations/global/recommenders/[INSIGHT_TYPE_ID]/config``
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class UpdateInsightTypeConfigRequest(proto.Message):
     r"""Request for the ``UpdateInsightTypeConfig`` method.
 
     Attributes:
-        insight_type_config (google.cloud.recommender_v1.types.InsightTypeConfig):
+        insight_type_config (google.cloud.recommender_v1beta1.types.InsightTypeConfig):
             Required. The InsightTypeConfig to update.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             The list of fields to be updated.
         validate_only (bool):
             If true, validate the request and preview the
             change, but do not actually update it.
     """
 
-    insight_type_config = proto.Field(
+    insight_type_config: gcr_insight_type_config.InsightTypeConfig = proto.Field(
         proto.MESSAGE,
         number=1,
         message=gcr_insight_type_config.InsightTypeConfig,
     )
-    update_mask = proto.Field(
+    update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=2,
         message=field_mask_pb2.FieldMask,
     )
-    validate_only = proto.Field(
+    validate_only: bool = proto.Field(
         proto.BOOL,
         number=3,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/__init__.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.recommender import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from .services.recommender import RecommenderAsyncClient, RecommenderClient
 from .types.insight import Insight, InsightStateInfo
 from .types.insight_type_config import InsightTypeConfig, InsightTypeGenerationConfig
 from .types.recommendation import (
     CostProjection,
     Impact,
```

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/gapic_metadata.json` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/services/__init__.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/services/recommender/__init__.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/services/recommender/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/services/recommender/async_client.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/services/recommender/async_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,23 +12,34 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
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
 
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.recommender_v1beta1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.protobuf import duration_pb2  # type: ignore
@@ -187,17 +198,17 @@
     get_transport_class = functools.partial(
         type(RecommenderClient).get_transport_class, type(RecommenderClient)
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, RecommenderTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the recommender client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -233,19 +244,19 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def list_insights(
         self,
-        request: Union[recommender_service.ListInsightsRequest, dict] = None,
+        request: Optional[Union[recommender_service.ListInsightsRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListInsightsAsyncPager:
         r"""Lists insights for the specified Cloud Resource. Requires the
         recommender.*.list IAM permission for the specified insight
         type.
 
         .. code-block:: python
@@ -272,15 +283,15 @@
                 page_result = client.list_insights(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1beta1.types.ListInsightsRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1beta1.types.ListInsightsRequest, dict]]):
                 The request object. Request for the `ListInsights`
                 method.
             parent (:class:`str`):
                 Required. The container resource on which to execute the
                 request. Acceptable formats:
 
                 -  ``projects/[PROJECT_NUMBER]/locations/[LOCATION]/insightTypes/[INSIGHT_TYPE_ID]``
@@ -374,19 +385,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_insight(
         self,
-        request: Union[recommender_service.GetInsightRequest, dict] = None,
+        request: Optional[Union[recommender_service.GetInsightRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> insight.Insight:
         r"""Gets the requested insight. Requires the recommender.*.get IAM
         permission for the specified insight type.
 
         .. code-block:: python
 
@@ -411,15 +422,15 @@
                 # Make the request
                 response = await client.get_insight(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1beta1.types.GetInsightRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1beta1.types.GetInsightRequest, dict]]):
                 The request object. Request to the `GetInsight` method.
             name (:class:`str`):
                 Required. Name of the insight.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
@@ -486,21 +497,23 @@
         )
 
         # Done; return the response.
         return response
 
     async def mark_insight_accepted(
         self,
-        request: Union[recommender_service.MarkInsightAcceptedRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.MarkInsightAcceptedRequest, dict]
+        ] = None,
         *,
-        name: str = None,
-        state_metadata: Mapping[str, str] = None,
-        etag: str = None,
+        name: Optional[str] = None,
+        state_metadata: Optional[MutableMapping[str, str]] = None,
+        etag: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> insight.Insight:
         r"""Marks the Insight State as Accepted. Users can use this method
         to indicate to the Recommender API that they have applied some
         action based on the insight. This stops the insight content from
         being updated.
 
@@ -532,23 +545,23 @@
                 # Make the request
                 response = await client.mark_insight_accepted(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1beta1.types.MarkInsightAcceptedRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1beta1.types.MarkInsightAcceptedRequest, dict]]):
                 The request object. Request for the
                 `MarkInsightAccepted` method.
             name (:class:`str`):
                 Required. Name of the insight.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            state_metadata (:class:`Mapping[str, str]`):
+            state_metadata (:class:`MutableMapping[str, str]`):
                 Optional. State properties user wish to include with
                 this state. Full replace of the current state_metadata.
 
                 This corresponds to the ``state_metadata`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             etag (:class:`str`):
@@ -617,20 +630,22 @@
         )
 
         # Done; return the response.
         return response
 
     async def list_recommendations(
         self,
-        request: Union[recommender_service.ListRecommendationsRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.ListRecommendationsRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        filter: str = None,
+        parent: Optional[str] = None,
+        filter: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListRecommendationsAsyncPager:
         r"""Lists recommendations for the specified Cloud Resource. Requires
         the recommender.*.list IAM permission for the specified
         recommender.
 
         .. code-block:: python
@@ -657,15 +672,15 @@
                 page_result = client.list_recommendations(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1beta1.types.ListRecommendationsRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1beta1.types.ListRecommendationsRequest, dict]]):
                 The request object. Request for the
                 `ListRecommendations` method.
             parent (:class:`str`):
                 Required. The container resource on which to execute the
                 request. Acceptable formats:
 
                 -  ``projects/[PROJECT_NUMBER]/locations/[LOCATION]/recommenders/[RECOMMENDER_ID]``
@@ -787,19 +802,21 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_recommendation(
         self,
-        request: Union[recommender_service.GetRecommendationRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.GetRecommendationRequest, dict]
+        ] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> recommendation.Recommendation:
         r"""Gets the requested recommendation. Requires the
         recommender.*.get IAM permission for the specified recommender.
 
         .. code-block:: python
 
@@ -824,15 +841,15 @@
                 # Make the request
                 response = await client.get_recommendation(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1beta1.types.GetRecommendationRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1beta1.types.GetRecommendationRequest, dict]]):
                 The request object. Request to the `GetRecommendation`
                 method.
             name (:class:`str`):
                 Required. Name of the recommendation.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
@@ -900,23 +917,23 @@
         )
 
         # Done; return the response.
         return response
 
     async def mark_recommendation_claimed(
         self,
-        request: Union[
-            recommender_service.MarkRecommendationClaimedRequest, dict
+        request: Optional[
+            Union[recommender_service.MarkRecommendationClaimedRequest, dict]
         ] = None,
         *,
-        name: str = None,
-        state_metadata: Mapping[str, str] = None,
-        etag: str = None,
+        name: Optional[str] = None,
+        state_metadata: Optional[MutableMapping[str, str]] = None,
+        etag: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> recommendation.Recommendation:
         r"""Marks the Recommendation State as Claimed. Users can use this
         method to indicate to the Recommender API that they are starting
         to apply the recommendation themselves. This stops the
         recommendation content from being updated. Associated insights
         are frozen and placed in the ACCEPTED state.
@@ -951,23 +968,23 @@
                 # Make the request
                 response = await client.mark_recommendation_claimed(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1beta1.types.MarkRecommendationClaimedRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1beta1.types.MarkRecommendationClaimedRequest, dict]]):
                 The request object. Request for the
                 `MarkRecommendationClaimed` Method.
             name (:class:`str`):
                 Required. Name of the recommendation.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            state_metadata (:class:`Mapping[str, str]`):
+            state_metadata (:class:`MutableMapping[str, str]`):
                 State properties to include with this state. Overwrites
                 any existing ``state_metadata``. Keys must match the
                 regex ``/^[a-z0-9][a-z0-9_.-]{0,62}$/``. Values must
                 match the regex ``/^[a-zA-Z0-9_./-]{0,255}$/``.
 
                 This corresponds to the ``state_metadata`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1039,23 +1056,23 @@
         )
 
         # Done; return the response.
         return response
 
     async def mark_recommendation_succeeded(
         self,
-        request: Union[
-            recommender_service.MarkRecommendationSucceededRequest, dict
+        request: Optional[
+            Union[recommender_service.MarkRecommendationSucceededRequest, dict]
         ] = None,
         *,
-        name: str = None,
-        state_metadata: Mapping[str, str] = None,
-        etag: str = None,
+        name: Optional[str] = None,
+        state_metadata: Optional[MutableMapping[str, str]] = None,
+        etag: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> recommendation.Recommendation:
         r"""Marks the Recommendation State as Succeeded. Users can use this
         method to indicate to the Recommender API that they have applied
         the recommendation themselves, and the operation was successful.
         This stops the recommendation content from being updated.
         Associated insights are frozen and placed in the ACCEPTED state.
@@ -1090,23 +1107,23 @@
                 # Make the request
                 response = await client.mark_recommendation_succeeded(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1beta1.types.MarkRecommendationSucceededRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1beta1.types.MarkRecommendationSucceededRequest, dict]]):
                 The request object. Request for the
                 `MarkRecommendationSucceeded` Method.
             name (:class:`str`):
                 Required. Name of the recommendation.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            state_metadata (:class:`Mapping[str, str]`):
+            state_metadata (:class:`MutableMapping[str, str]`):
                 State properties to include with this state. Overwrites
                 any existing ``state_metadata``. Keys must match the
                 regex ``/^[a-z0-9][a-z0-9_.-]{0,62}$/``. Values must
                 match the regex ``/^[a-zA-Z0-9_./-]{0,255}$/``.
 
                 This corresponds to the ``state_metadata`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1178,23 +1195,23 @@
         )
 
         # Done; return the response.
         return response
 
     async def mark_recommendation_failed(
         self,
-        request: Union[
-            recommender_service.MarkRecommendationFailedRequest, dict
+        request: Optional[
+            Union[recommender_service.MarkRecommendationFailedRequest, dict]
         ] = None,
         *,
-        name: str = None,
-        state_metadata: Mapping[str, str] = None,
-        etag: str = None,
+        name: Optional[str] = None,
+        state_metadata: Optional[MutableMapping[str, str]] = None,
+        etag: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> recommendation.Recommendation:
         r"""Marks the Recommendation State as Failed. Users can use this
         method to indicate to the Recommender API that they have applied
         the recommendation themselves, and the operation failed. This
         stops the recommendation content from being updated. Associated
         insights are frozen and placed in the ACCEPTED state.
@@ -1229,23 +1246,23 @@
                 # Make the request
                 response = await client.mark_recommendation_failed(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1beta1.types.MarkRecommendationFailedRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1beta1.types.MarkRecommendationFailedRequest, dict]]):
                 The request object. Request for the
                 `MarkRecommendationFailed` Method.
             name (:class:`str`):
                 Required. Name of the recommendation.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            state_metadata (:class:`Mapping[str, str]`):
+            state_metadata (:class:`MutableMapping[str, str]`):
                 State properties to include with this state. Overwrites
                 any existing ``state_metadata``. Keys must match the
                 regex ``/^[a-z0-9][a-z0-9_.-]{0,62}$/``. Values must
                 match the regex ``/^[a-zA-Z0-9_./-]{0,255}$/``.
 
                 This corresponds to the ``state_metadata`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1317,19 +1334,21 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_recommender_config(
         self,
-        request: Union[recommender_service.GetRecommenderConfigRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.GetRecommenderConfigRequest, dict]
+        ] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> recommender_config.RecommenderConfig:
         r"""Gets the requested Recommender Config. There is only
         one instance of the config for each Recommender.
 
         .. code-block:: python
 
@@ -1354,15 +1373,15 @@
                 # Make the request
                 response = await client.get_recommender_config(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1beta1.types.GetRecommenderConfigRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1beta1.types.GetRecommenderConfigRequest, dict]]):
                 The request object. Request for the
                 GetRecommenderConfig` method.
             name (:class:`str`):
                 Required. Name of the Recommendation Config to get.
 
                 Acceptable formats:
 
@@ -1425,20 +1444,22 @@
         )
 
         # Done; return the response.
         return response
 
     async def update_recommender_config(
         self,
-        request: Union[recommender_service.UpdateRecommenderConfigRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.UpdateRecommenderConfigRequest, dict]
+        ] = None,
         *,
-        recommender_config: gcr_recommender_config.RecommenderConfig = None,
-        update_mask: field_mask_pb2.FieldMask = None,
+        recommender_config: Optional[gcr_recommender_config.RecommenderConfig] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcr_recommender_config.RecommenderConfig:
         r"""Updates a Recommender Config. This will create a new
         revision of the config.
 
         .. code-block:: python
 
@@ -1462,15 +1483,15 @@
                 # Make the request
                 response = await client.update_recommender_config(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1beta1.types.UpdateRecommenderConfigRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1beta1.types.UpdateRecommenderConfigRequest, dict]]):
                 The request object. Request for the
                 `UpdateRecommenderConfig` method.
             recommender_config (:class:`google.cloud.recommender_v1beta1.types.RecommenderConfig`):
                 Required. The RecommenderConfig to
                 update.
 
                 This corresponds to the ``recommender_config`` field
@@ -1535,19 +1556,21 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_insight_type_config(
         self,
-        request: Union[recommender_service.GetInsightTypeConfigRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.GetInsightTypeConfigRequest, dict]
+        ] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> insight_type_config.InsightTypeConfig:
         r"""Gets the requested InsightTypeConfig. There is only
         one instance of the config for each InsightType.
 
         .. code-block:: python
 
@@ -1572,15 +1595,15 @@
                 # Make the request
                 response = await client.get_insight_type_config(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1beta1.types.GetInsightTypeConfigRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1beta1.types.GetInsightTypeConfigRequest, dict]]):
                 The request object. Request for the
                 GetInsightTypeConfig` method.
             name (:class:`str`):
                 Required. Name of the InsightTypeConfig to get.
 
                 Acceptable formats:
 
@@ -1643,20 +1666,22 @@
         )
 
         # Done; return the response.
         return response
 
     async def update_insight_type_config(
         self,
-        request: Union[recommender_service.UpdateInsightTypeConfigRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.UpdateInsightTypeConfigRequest, dict]
+        ] = None,
         *,
-        insight_type_config: gcr_insight_type_config.InsightTypeConfig = None,
-        update_mask: field_mask_pb2.FieldMask = None,
+        insight_type_config: Optional[gcr_insight_type_config.InsightTypeConfig] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcr_insight_type_config.InsightTypeConfig:
         r"""Updates an InsightTypeConfig change. This will create
         a new revision of the config.
 
         .. code-block:: python
 
@@ -1680,15 +1705,15 @@
                 # Make the request
                 response = await client.update_insight_type_config(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.recommender_v1beta1.types.UpdateInsightTypeConfigRequest, dict]):
+            request (Optional[Union[google.cloud.recommender_v1beta1.types.UpdateInsightTypeConfigRequest, dict]]):
                 The request object. Request for the
                 `UpdateInsightTypeConfig` method.
             insight_type_config (:class:`google.cloud.recommender_v1beta1.types.InsightTypeConfig`):
                 Required. The InsightTypeConfig to
                 update.
 
                 This corresponds to the ``insight_type_config`` field
@@ -1758,18 +1783,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-recommender",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("RecommenderAsyncClient",)
```

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/services/recommender/client.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/services/recommender/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,38 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
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
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.recommender_v1beta1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.protobuf import duration_pb2  # type: ignore
@@ -67,15 +79,15 @@
 
     _transport_registry = OrderedDict()  # type: Dict[str, Type[RecommenderTransport]]
     _transport_registry["grpc"] = RecommenderGrpcTransport
     _transport_registry["grpc_asyncio"] = RecommenderGrpcAsyncIOTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[RecommenderTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -463,30 +475,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, RecommenderTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, RecommenderTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the recommender client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, RecommenderTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -508,14 +520,15 @@
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
@@ -560,19 +573,19 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def list_insights(
         self,
-        request: Union[recommender_service.ListInsightsRequest, dict] = None,
+        request: Optional[Union[recommender_service.ListInsightsRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListInsightsPager:
         r"""Lists insights for the specified Cloud Resource. Requires the
         recommender.*.list IAM permission for the specified insight
         type.
 
         .. code-block:: python
@@ -691,19 +704,19 @@
         )
 
         # Done; return the response.
         return response
 
     def get_insight(
         self,
-        request: Union[recommender_service.GetInsightRequest, dict] = None,
+        request: Optional[Union[recommender_service.GetInsightRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> insight.Insight:
         r"""Gets the requested insight. Requires the recommender.*.get IAM
         permission for the specified insight type.
 
         .. code-block:: python
 
@@ -793,21 +806,23 @@
         )
 
         # Done; return the response.
         return response
 
     def mark_insight_accepted(
         self,
-        request: Union[recommender_service.MarkInsightAcceptedRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.MarkInsightAcceptedRequest, dict]
+        ] = None,
         *,
-        name: str = None,
-        state_metadata: Mapping[str, str] = None,
-        etag: str = None,
+        name: Optional[str] = None,
+        state_metadata: Optional[MutableMapping[str, str]] = None,
+        etag: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> insight.Insight:
         r"""Marks the Insight State as Accepted. Users can use this method
         to indicate to the Recommender API that they have applied some
         action based on the insight. This stops the insight content from
         being updated.
 
@@ -847,15 +862,15 @@
                 The request object. Request for the
                 `MarkInsightAccepted` method.
             name (str):
                 Required. Name of the insight.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            state_metadata (Mapping[str, str]):
+            state_metadata (MutableMapping[str, str]):
                 Optional. State properties user wish to include with
                 this state. Full replace of the current state_metadata.
 
                 This corresponds to the ``state_metadata`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             etag (str):
@@ -923,20 +938,22 @@
         )
 
         # Done; return the response.
         return response
 
     def list_recommendations(
         self,
-        request: Union[recommender_service.ListRecommendationsRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.ListRecommendationsRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        filter: str = None,
+        parent: Optional[str] = None,
+        filter: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListRecommendationsPager:
         r"""Lists recommendations for the specified Cloud Resource. Requires
         the recommender.*.list IAM permission for the specified
         recommender.
 
         .. code-block:: python
@@ -1083,19 +1100,21 @@
         )
 
         # Done; return the response.
         return response
 
     def get_recommendation(
         self,
-        request: Union[recommender_service.GetRecommendationRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.GetRecommendationRequest, dict]
+        ] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> recommendation.Recommendation:
         r"""Gets the requested recommendation. Requires the
         recommender.*.get IAM permission for the specified recommender.
 
         .. code-block:: python
 
@@ -1186,23 +1205,23 @@
         )
 
         # Done; return the response.
         return response
 
     def mark_recommendation_claimed(
         self,
-        request: Union[
-            recommender_service.MarkRecommendationClaimedRequest, dict
+        request: Optional[
+            Union[recommender_service.MarkRecommendationClaimedRequest, dict]
         ] = None,
         *,
-        name: str = None,
-        state_metadata: Mapping[str, str] = None,
-        etag: str = None,
+        name: Optional[str] = None,
+        state_metadata: Optional[MutableMapping[str, str]] = None,
+        etag: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> recommendation.Recommendation:
         r"""Marks the Recommendation State as Claimed. Users can use this
         method to indicate to the Recommender API that they are starting
         to apply the recommendation themselves. This stops the
         recommendation content from being updated. Associated insights
         are frozen and placed in the ACCEPTED state.
@@ -1245,15 +1264,15 @@
                 The request object. Request for the
                 `MarkRecommendationClaimed` Method.
             name (str):
                 Required. Name of the recommendation.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            state_metadata (Mapping[str, str]):
+            state_metadata (MutableMapping[str, str]):
                 State properties to include with this state. Overwrites
                 any existing ``state_metadata``. Keys must match the
                 regex ``/^[a-z0-9][a-z0-9_.-]{0,62}$/``. Values must
                 match the regex ``/^[a-zA-Z0-9_./-]{0,255}$/``.
 
                 This corresponds to the ``state_metadata`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1328,23 +1347,23 @@
         )
 
         # Done; return the response.
         return response
 
     def mark_recommendation_succeeded(
         self,
-        request: Union[
-            recommender_service.MarkRecommendationSucceededRequest, dict
+        request: Optional[
+            Union[recommender_service.MarkRecommendationSucceededRequest, dict]
         ] = None,
         *,
-        name: str = None,
-        state_metadata: Mapping[str, str] = None,
-        etag: str = None,
+        name: Optional[str] = None,
+        state_metadata: Optional[MutableMapping[str, str]] = None,
+        etag: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> recommendation.Recommendation:
         r"""Marks the Recommendation State as Succeeded. Users can use this
         method to indicate to the Recommender API that they have applied
         the recommendation themselves, and the operation was successful.
         This stops the recommendation content from being updated.
         Associated insights are frozen and placed in the ACCEPTED state.
@@ -1387,15 +1406,15 @@
                 The request object. Request for the
                 `MarkRecommendationSucceeded` Method.
             name (str):
                 Required. Name of the recommendation.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            state_metadata (Mapping[str, str]):
+            state_metadata (MutableMapping[str, str]):
                 State properties to include with this state. Overwrites
                 any existing ``state_metadata``. Keys must match the
                 regex ``/^[a-z0-9][a-z0-9_.-]{0,62}$/``. Values must
                 match the regex ``/^[a-zA-Z0-9_./-]{0,255}$/``.
 
                 This corresponds to the ``state_metadata`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1470,23 +1489,23 @@
         )
 
         # Done; return the response.
         return response
 
     def mark_recommendation_failed(
         self,
-        request: Union[
-            recommender_service.MarkRecommendationFailedRequest, dict
+        request: Optional[
+            Union[recommender_service.MarkRecommendationFailedRequest, dict]
         ] = None,
         *,
-        name: str = None,
-        state_metadata: Mapping[str, str] = None,
-        etag: str = None,
+        name: Optional[str] = None,
+        state_metadata: Optional[MutableMapping[str, str]] = None,
+        etag: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> recommendation.Recommendation:
         r"""Marks the Recommendation State as Failed. Users can use this
         method to indicate to the Recommender API that they have applied
         the recommendation themselves, and the operation failed. This
         stops the recommendation content from being updated. Associated
         insights are frozen and placed in the ACCEPTED state.
@@ -1529,15 +1548,15 @@
                 The request object. Request for the
                 `MarkRecommendationFailed` Method.
             name (str):
                 Required. Name of the recommendation.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            state_metadata (Mapping[str, str]):
+            state_metadata (MutableMapping[str, str]):
                 State properties to include with this state. Overwrites
                 any existing ``state_metadata``. Keys must match the
                 regex ``/^[a-z0-9][a-z0-9_.-]{0,62}$/``. Values must
                 match the regex ``/^[a-zA-Z0-9_./-]{0,255}$/``.
 
                 This corresponds to the ``state_metadata`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1610,19 +1629,21 @@
         )
 
         # Done; return the response.
         return response
 
     def get_recommender_config(
         self,
-        request: Union[recommender_service.GetRecommenderConfigRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.GetRecommenderConfigRequest, dict]
+        ] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> recommender_config.RecommenderConfig:
         r"""Gets the requested Recommender Config. There is only
         one instance of the config for each Recommender.
 
         .. code-block:: python
 
@@ -1718,20 +1739,22 @@
         )
 
         # Done; return the response.
         return response
 
     def update_recommender_config(
         self,
-        request: Union[recommender_service.UpdateRecommenderConfigRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.UpdateRecommenderConfigRequest, dict]
+        ] = None,
         *,
-        recommender_config: gcr_recommender_config.RecommenderConfig = None,
-        update_mask: field_mask_pb2.FieldMask = None,
+        recommender_config: Optional[gcr_recommender_config.RecommenderConfig] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcr_recommender_config.RecommenderConfig:
         r"""Updates a Recommender Config. This will create a new
         revision of the config.
 
         .. code-block:: python
 
@@ -1830,19 +1853,21 @@
         )
 
         # Done; return the response.
         return response
 
     def get_insight_type_config(
         self,
-        request: Union[recommender_service.GetInsightTypeConfigRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.GetInsightTypeConfigRequest, dict]
+        ] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> insight_type_config.InsightTypeConfig:
         r"""Gets the requested InsightTypeConfig. There is only
         one instance of the config for each InsightType.
 
         .. code-block:: python
 
@@ -1938,20 +1963,22 @@
         )
 
         # Done; return the response.
         return response
 
     def update_insight_type_config(
         self,
-        request: Union[recommender_service.UpdateInsightTypeConfigRequest, dict] = None,
+        request: Optional[
+            Union[recommender_service.UpdateInsightTypeConfigRequest, dict]
+        ] = None,
         *,
-        insight_type_config: gcr_insight_type_config.InsightTypeConfig = None,
-        update_mask: field_mask_pb2.FieldMask = None,
+        insight_type_config: Optional[gcr_insight_type_config.InsightTypeConfig] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcr_insight_type_config.InsightTypeConfig:
         r"""Updates an InsightTypeConfig change. This will create
         a new revision of the config.
 
         .. code-block:: python
 
@@ -2062,18 +2089,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-recommender",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("RecommenderClient",)
```

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/services/recommender/pagers.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/services/recommender/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/services/recommender/transports/__init__.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/services/recommender/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/services/recommender/transports/base.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/services/recommender/transports/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,50 +19,45 @@
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
 
+from google.cloud.recommender_v1beta1 import gapic_version as package_version
 from google.cloud.recommender_v1beta1.types import (
     insight_type_config as gcr_insight_type_config,
 )
 from google.cloud.recommender_v1beta1.types import (
     recommender_config as gcr_recommender_config,
 )
 from google.cloud.recommender_v1beta1.types import insight
 from google.cloud.recommender_v1beta1.types import insight_type_config
 from google.cloud.recommender_v1beta1.types import recommendation
 from google.cloud.recommender_v1beta1.types import recommender_config
 from google.cloud.recommender_v1beta1.types import recommender_service
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-recommender",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class RecommenderTransport(abc.ABC):
     """Abstract transport class for Recommender."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "recommender.googleapis.com"
 
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

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/services/recommender/transports/grpc.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/services/recommender/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,22 +56,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "recommender.googleapis.com",
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
 
@@ -190,16 +190,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "recommender.googleapis.com",
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

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/services/recommender/transports/grpc_asyncio.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/services/recommender/transports/grpc_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "recommender.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -101,23 +101,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "recommender.googleapis.com",
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

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/types/__init__.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/types/insight.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/types/insight.py`

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
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import struct_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.recommender.v1beta1",
@@ -33,15 +35,15 @@
 
     Attributes:
         name (str):
             Name of the insight.
         description (str):
             Free-form human readable summary in English.
             The maximum length is 500 characters.
-        target_resources (Sequence[str]):
+        target_resources (MutableSequence[str]):
             Fully qualified resource names that this
             insight is targeting.
         insight_subtype (str):
             Insight subtype. Insight content schema will
             be stable for a given subtype.
         content (google.protobuf.struct_pb2.Struct):
             A struct of custom fields to explain the
@@ -59,15 +61,15 @@
         category (google.cloud.recommender_v1beta1.types.Insight.Category):
             Category being targeted by the insight.
         severity (google.cloud.recommender_v1beta1.types.Insight.Severity):
             Insight's severity.
         etag (str):
             Fingerprint of the Insight. Provides
             optimistic locking when updating states.
-        associated_recommendations (Sequence[google.cloud.recommender_v1beta1.types.Insight.RecommendationReference]):
+        associated_recommendations (MutableSequence[google.cloud.recommender_v1beta1.types.Insight.RecommendationReference]):
             Recommendations derived from this insight.
     """
 
     class Category(proto.Enum):
         r"""Insight category."""
         CATEGORY_UNSPECIFIED = 0
         COST = 1
@@ -88,100 +90,102 @@
 
         Attributes:
             recommendation (str):
                 Recommendation resource name, e.g.
                 projects/[PROJECT_NUMBER]/locations/[LOCATION]/recommenders/[RECOMMENDER_ID]/recommendations/[RECOMMENDATION_ID]
         """
 
-        recommendation = proto.Field(
+        recommendation: str = proto.Field(
             proto.STRING,
             number=1,
         )
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    description = proto.Field(
+    description: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    target_resources = proto.RepeatedField(
+    target_resources: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=9,
     )
-    insight_subtype = proto.Field(
+    insight_subtype: str = proto.Field(
         proto.STRING,
         number=10,
     )
-    content = proto.Field(
+    content: struct_pb2.Struct = proto.Field(
         proto.MESSAGE,
         number=3,
         message=struct_pb2.Struct,
     )
-    last_refresh_time = proto.Field(
+    last_refresh_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=4,
         message=timestamp_pb2.Timestamp,
     )
-    observation_period = proto.Field(
+    observation_period: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=5,
         message=duration_pb2.Duration,
     )
-    state_info = proto.Field(
+    state_info: "InsightStateInfo" = proto.Field(
         proto.MESSAGE,
         number=6,
         message="InsightStateInfo",
     )
-    category = proto.Field(
+    category: Category = proto.Field(
         proto.ENUM,
         number=7,
         enum=Category,
     )
-    severity = proto.Field(
+    severity: Severity = proto.Field(
         proto.ENUM,
         number=15,
         enum=Severity,
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=11,
     )
-    associated_recommendations = proto.RepeatedField(
+    associated_recommendations: MutableSequence[
+        RecommendationReference
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=8,
         message=RecommendationReference,
     )
 
 
 class InsightStateInfo(proto.Message):
     r"""Information related to insight state.
 
     Attributes:
         state (google.cloud.recommender_v1beta1.types.InsightStateInfo.State):
             Insight state.
-        state_metadata (Mapping[str, str]):
+        state_metadata (MutableMapping[str, str]):
             A map of metadata for the state, provided by
             user or automations systems.
     """
 
     class State(proto.Enum):
         r"""Represents insight state."""
         STATE_UNSPECIFIED = 0
         ACTIVE = 1
         ACCEPTED = 2
         DISMISSED = 3
 
-    state = proto.Field(
+    state: State = proto.Field(
         proto.ENUM,
         number=1,
         enum=State,
     )
-    state_metadata = proto.MapField(
+    state_metadata: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=2,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/types/insight_type_config.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/types/insight_type_config.py`

 * *Files 15% similar despite different names*

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
 from google.protobuf import struct_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.recommender.v1beta1",
     manifest={
@@ -43,57 +45,57 @@
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Last time when the config was updated.
         revision_id (str):
             Output only. Immutable. The revision ID of
             the config. A new revision is committed whenever
             the config is changed in any way. The format is
             an 8-character hexadecimal string.
-        annotations (Mapping[str, str]):
+        annotations (MutableMapping[str, str]):
             Allows clients to store small amounts of arbitrary data.
             Annotations must follow the Kubernetes syntax. The total
             size of all keys and values combined is limited to 256k. Key
             can have 2 segments: prefix (optional) and name (required),
             separated by a slash (/). Prefix must be a DNS subdomain.
             Name must be 63 characters or less, begin and end with
             alphanumerics, with dashes (-), underscores (_), dots (.),
             and alphanumerics between.
         display_name (str):
             A user-settable field to provide a
             human-readable name to be used in user
             interfaces.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    insight_type_generation_config = proto.Field(
+    insight_type_generation_config: "InsightTypeGenerationConfig" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="InsightTypeGenerationConfig",
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    update_time = proto.Field(
+    update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=4,
         message=timestamp_pb2.Timestamp,
     )
-    revision_id = proto.Field(
+    revision_id: str = proto.Field(
         proto.STRING,
         number=5,
     )
-    annotations = proto.MapField(
+    annotations: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=6,
     )
-    display_name = proto.Field(
+    display_name: str = proto.Field(
         proto.STRING,
         number=7,
     )
 
 
 class InsightTypeGenerationConfig(proto.Message):
     r"""A configuration to customize the generation of insights.
@@ -103,15 +105,15 @@
     Attributes:
         params (google.protobuf.struct_pb2.Struct):
             Parameters for this
             InsightTypeGenerationConfig. These configs can
             be used by or are applied to all subtypes.
     """
 
-    params = proto.Field(
+    params: struct_pb2.Struct = proto.Field(
         proto.MESSAGE,
         number=1,
         message=struct_pb2.Struct,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/types/recommendation.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/types/recommendation.py`

 * *Files 7% similar despite different names*

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
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import struct_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.type import money_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
@@ -63,15 +65,15 @@
             Last time this recommendation was refreshed
             by the system that created it in the first
             place.
         primary_impact (google.cloud.recommender_v1beta1.types.Impact):
             The primary impact that this recommendation
             can have while trying to optimize for one
             category.
-        additional_impact (Sequence[google.cloud.recommender_v1beta1.types.Impact]):
+        additional_impact (MutableSequence[google.cloud.recommender_v1beta1.types.Impact]):
             Optional set of additional impact that this
             recommendation may have when trying to optimize
             for the primary category. These may be positive
             or negative.
         priority (google.cloud.recommender_v1beta1.types.Recommendation.Priority):
             Recommendation's priority.
         content (google.cloud.recommender_v1beta1.types.RecommendationContent):
@@ -79,15 +81,15 @@
             recommended changes to resources.
         state_info (google.cloud.recommender_v1beta1.types.RecommendationStateInfo):
             Information for state. Contains state and
             metadata.
         etag (str):
             Fingerprint of the Recommendation. Provides
             optimistic locking when updating states.
-        associated_insights (Sequence[google.cloud.recommender_v1beta1.types.Recommendation.InsightReference]):
+        associated_insights (MutableSequence[google.cloud.recommender_v1beta1.types.Recommendation.InsightReference]):
             Insights that led to this recommendation.
         xor_group_id (str):
             Corresponds to a mutually exclusive group ID
             within a recommender. A non-empty ID indicates
             that the recommendation belongs to a mutually
             exclusive group. This means that only one
             recommendation within the group is suggested to
@@ -107,115 +109,115 @@
 
         Attributes:
             insight (str):
                 Insight resource name, e.g.
                 projects/[PROJECT_NUMBER]/locations/[LOCATION]/insightTypes/[INSIGHT_TYPE_ID]/insights/[INSIGHT_ID]
         """
 
-        insight = proto.Field(
+        insight: str = proto.Field(
             proto.STRING,
             number=1,
         )
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    description = proto.Field(
+    description: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    recommender_subtype = proto.Field(
+    recommender_subtype: str = proto.Field(
         proto.STRING,
         number=12,
     )
-    last_refresh_time = proto.Field(
+    last_refresh_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=4,
         message=timestamp_pb2.Timestamp,
     )
-    primary_impact = proto.Field(
+    primary_impact: "Impact" = proto.Field(
         proto.MESSAGE,
         number=5,
         message="Impact",
     )
-    additional_impact = proto.RepeatedField(
+    additional_impact: MutableSequence["Impact"] = proto.RepeatedField(
         proto.MESSAGE,
         number=6,
         message="Impact",
     )
-    priority = proto.Field(
+    priority: Priority = proto.Field(
         proto.ENUM,
         number=17,
         enum=Priority,
     )
-    content = proto.Field(
+    content: "RecommendationContent" = proto.Field(
         proto.MESSAGE,
         number=7,
         message="RecommendationContent",
     )
-    state_info = proto.Field(
+    state_info: "RecommendationStateInfo" = proto.Field(
         proto.MESSAGE,
         number=10,
         message="RecommendationStateInfo",
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=11,
     )
-    associated_insights = proto.RepeatedField(
+    associated_insights: MutableSequence[InsightReference] = proto.RepeatedField(
         proto.MESSAGE,
         number=14,
         message=InsightReference,
     )
-    xor_group_id = proto.Field(
+    xor_group_id: str = proto.Field(
         proto.STRING,
         number=18,
     )
 
 
 class RecommendationContent(proto.Message):
     r"""Contains what resources are changing and how they are
     changing.
 
     Attributes:
-        operation_groups (Sequence[google.cloud.recommender_v1beta1.types.OperationGroup]):
+        operation_groups (MutableSequence[google.cloud.recommender_v1beta1.types.OperationGroup]):
             Operations to one or more Google Cloud
             resources grouped in such a way that, all
             operations within one group are expected to be
             performed atomically and in an order.
         overview (google.protobuf.struct_pb2.Struct):
             Condensed overview information about the
             recommendation.
     """
 
-    operation_groups = proto.RepeatedField(
+    operation_groups: MutableSequence["OperationGroup"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="OperationGroup",
     )
-    overview = proto.Field(
+    overview: struct_pb2.Struct = proto.Field(
         proto.MESSAGE,
         number=3,
         message=struct_pb2.Struct,
     )
 
 
 class OperationGroup(proto.Message):
     r"""Group of operations that need to be performed atomically.
 
     Attributes:
-        operations (Sequence[google.cloud.recommender_v1beta1.types.Operation]):
+        operations (MutableSequence[google.cloud.recommender_v1beta1.types.Operation]):
             List of operations across one or more
             resources that belong to this group. Loosely
             based on RFC6902 and should be performed in the
             order they appear.
     """
 
-    operations = proto.RepeatedField(
+    operations: MutableSequence["Operation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="Operation",
     )
 
 
 class Operation(proto.Message):
@@ -276,15 +278,15 @@
             This field is a member of `oneof`_ ``path_value``.
         value_matcher (google.cloud.recommender_v1beta1.types.ValueMatcher):
             Can be set for action 'test' for advanced matching for the
             value of 'path' field. Either this or ``value`` will be set
             for 'test' operation.
 
             This field is a member of `oneof`_ ``path_value``.
-        path_filters (Mapping[str, google.protobuf.struct_pb2.Value]):
+        path_filters (MutableMapping[str, google.protobuf.struct_pb2.Value]):
             Set of filters to apply if ``path`` refers to array elements
             or nested array elements in order to narrow down to a single
             unique element that is being tested/modified. This is
             intended to be an exact match per filter. To perform
             advanced matching, use path_value_matchers.
 
             -  Example:
@@ -312,66 +314,66 @@
                {
                  "/bindings/*/role": "roles/owner"
                  "/bindings/*/members/*" : ["x@example.com", "y@example.com"]
                }
 
             When both path_filters and path_value_matchers are set, an
             implicit AND must be performed.
-        path_value_matchers (Mapping[str, google.cloud.recommender_v1beta1.types.ValueMatcher]):
+        path_value_matchers (MutableMapping[str, google.cloud.recommender_v1beta1.types.ValueMatcher]):
             Similar to path_filters, this contains set of filters to
             apply if ``path`` field refers to array elements. This is
             meant to support value matching beyond exact match. To
             perform exact match, use path_filters. When both
             path_filters and path_value_matchers are set, an implicit
             AND must be performed.
     """
 
-    action = proto.Field(
+    action: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    resource_type = proto.Field(
+    resource_type: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    resource = proto.Field(
+    resource: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    path = proto.Field(
+    path: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    source_resource = proto.Field(
+    source_resource: str = proto.Field(
         proto.STRING,
         number=5,
     )
-    source_path = proto.Field(
+    source_path: str = proto.Field(
         proto.STRING,
         number=6,
     )
-    value = proto.Field(
+    value: struct_pb2.Value = proto.Field(
         proto.MESSAGE,
         number=7,
         oneof="path_value",
         message=struct_pb2.Value,
     )
-    value_matcher = proto.Field(
+    value_matcher: "ValueMatcher" = proto.Field(
         proto.MESSAGE,
         number=10,
         oneof="path_value",
         message="ValueMatcher",
     )
-    path_filters = proto.MapField(
+    path_filters: MutableMapping[str, struct_pb2.Value] = proto.MapField(
         proto.STRING,
         proto.MESSAGE,
         number=8,
         message=struct_pb2.Value,
     )
-    path_value_matchers = proto.MapField(
+    path_value_matchers: MutableMapping[str, "ValueMatcher"] = proto.MapField(
         proto.STRING,
         proto.MESSAGE,
         number=11,
         message="ValueMatcher",
     )
 
 
@@ -389,15 +391,15 @@
             syntax
             (https://github.com/google/re2/wiki/Syntax), so
             to be used with RE2::FullMatch
 
             This field is a member of `oneof`_ ``match_variant``.
     """
 
-    matches_pattern = proto.Field(
+    matches_pattern: str = proto.Field(
         proto.STRING,
         number=1,
         oneof="match_variant",
     )
 
 
 class CostProjection(proto.Message):
@@ -414,20 +416,20 @@
             A user's permissions may affect whether the cost
             is computed using list prices or custom contract
             prices.
         duration (google.protobuf.duration_pb2.Duration):
             Duration for which this cost applies.
     """
 
-    cost = proto.Field(
+    cost: money_pb2.Money = proto.Field(
         proto.MESSAGE,
         number=1,
         message=money_pb2.Money,
     )
-    duration = proto.Field(
+    duration: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
 
 
 class SecurityProjection(proto.Message):
@@ -435,15 +437,15 @@
 
     Attributes:
         details (google.protobuf.struct_pb2.Struct):
             This field can be used by the recommender to
             define details specific to security impact.
     """
 
-    details = proto.Field(
+    details: struct_pb2.Struct = proto.Field(
         proto.MESSAGE,
         number=2,
         message=struct_pb2.Struct,
     )
 
 
 class SustainabilityProjection(proto.Message):
@@ -456,19 +458,19 @@
             kg_c_o2e so that the name renders correctly in camelCase
             (kgCO2e).
         duration (google.protobuf.duration_pb2.Duration):
             Duration for which this sustanability
             applies.
     """
 
-    kg_c_o2e = proto.Field(
+    kg_c_o2e: float = proto.Field(
         proto.DOUBLE,
         number=1,
     )
-    duration = proto.Field(
+    duration: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
 
 
 class Impact(proto.Message):
@@ -504,66 +506,66 @@
         CATEGORY_UNSPECIFIED = 0
         COST = 1
         SECURITY = 2
         PERFORMANCE = 3
         MANAGEABILITY = 4
         SUSTAINABILITY = 5
 
-    category = proto.Field(
+    category: Category = proto.Field(
         proto.ENUM,
         number=1,
         enum=Category,
     )
-    cost_projection = proto.Field(
+    cost_projection: "CostProjection" = proto.Field(
         proto.MESSAGE,
         number=100,
         oneof="projection",
         message="CostProjection",
     )
-    security_projection = proto.Field(
+    security_projection: "SecurityProjection" = proto.Field(
         proto.MESSAGE,
         number=101,
         oneof="projection",
         message="SecurityProjection",
     )
-    sustainability_projection = proto.Field(
+    sustainability_projection: "SustainabilityProjection" = proto.Field(
         proto.MESSAGE,
         number=102,
         oneof="projection",
         message="SustainabilityProjection",
     )
 
 
 class RecommendationStateInfo(proto.Message):
     r"""Information for state. Contains state and metadata.
 
     Attributes:
         state (google.cloud.recommender_v1beta1.types.RecommendationStateInfo.State):
             The state of the recommendation, Eg ACTIVE,
             SUCCEEDED, FAILED.
-        state_metadata (Mapping[str, str]):
+        state_metadata (MutableMapping[str, str]):
             A map of metadata for the state, provided by
             user or automations systems.
     """
 
     class State(proto.Enum):
         r"""Represents Recommendation State."""
         STATE_UNSPECIFIED = 0
         ACTIVE = 1
         CLAIMED = 6
         SUCCEEDED = 3
         FAILED = 4
         DISMISSED = 5
 
-    state = proto.Field(
+    state: State = proto.Field(
         proto.ENUM,
         number=1,
         enum=State,
     )
-    state_metadata = proto.MapField(
+    state_metadata: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=2,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/types/recommender_config.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1beta1/types/recommender_config.py`

 * *Files 9% similar despite different names*

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
 from google.protobuf import struct_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.recommender.v1beta1",
     manifest={
@@ -43,57 +45,57 @@
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Last time when the config was updated.
         revision_id (str):
             Output only. Immutable. The revision ID of
             the config. A new revision is committed whenever
             the config is changed in any way. The format is
             an 8-character hexadecimal string.
-        annotations (Mapping[str, str]):
+        annotations (MutableMapping[str, str]):
             Allows clients to store small amounts of arbitrary data.
             Annotations must follow the Kubernetes syntax. The total
             size of all keys and values combined is limited to 256k. Key
             can have 2 segments: prefix (optional) and name (required),
             separated by a slash (/). Prefix must be a DNS subdomain.
             Name must be 63 characters or less, begin and end with
             alphanumerics, with dashes (-), underscores (_), dots (.),
             and alphanumerics between.
         display_name (str):
             A user-settable field to provide a
             human-readable name to be used in user
             interfaces.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    recommender_generation_config = proto.Field(
+    recommender_generation_config: "RecommenderGenerationConfig" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="RecommenderGenerationConfig",
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    update_time = proto.Field(
+    update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=4,
         message=timestamp_pb2.Timestamp,
     )
-    revision_id = proto.Field(
+    revision_id: str = proto.Field(
         proto.STRING,
         number=5,
     )
-    annotations = proto.MapField(
+    annotations: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=6,
     )
-    display_name = proto.Field(
+    display_name: str = proto.Field(
         proto.STRING,
         number=7,
     )
 
 
 class RecommenderGenerationConfig(proto.Message):
     r"""A Configuration to customize the generation of
@@ -103,15 +105,15 @@
     Attributes:
         params (google.protobuf.struct_pb2.Struct):
             Parameters for this
             RecommenderGenerationConfig. These configs can
             be used by or are applied to all subtypes.
     """
 
-    params = proto.Field(
+    params: struct_pb2.Struct = proto.Field(
         proto.MESSAGE,
         number=1,
         message=struct_pb2.Struct,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-recommender-2.8.3/google/cloud/recommender_v1beta1/types/recommender_service.py` & `google-cloud-recommender-2.9.0/google/cloud/recommender_v1/types/recommender_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,28 +9,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 from google.protobuf import field_mask_pb2  # type: ignore
 import proto  # type: ignore
 
-from google.cloud.recommender_v1beta1.types import (
+from google.cloud.recommender_v1.types import (
     insight_type_config as gcr_insight_type_config,
 )
-from google.cloud.recommender_v1beta1.types import (
+from google.cloud.recommender_v1.types import (
     recommender_config as gcr_recommender_config,
 )
-from google.cloud.recommender_v1beta1.types import insight
-from google.cloud.recommender_v1beta1.types import recommendation
+from google.cloud.recommender_v1.types import insight
+from google.cloud.recommender_v1.types import recommendation
 
 __protobuf__ = proto.module(
-    package="google.cloud.recommender.v1beta1",
+    package="google.cloud.recommender.v1",
     manifest={
         "ListInsightsRequest",
         "ListInsightsResponse",
         "GetInsightRequest",
         "MarkInsightAcceptedRequest",
         "ListRecommendationsRequest",
         "ListRecommendationsResponse",
@@ -66,15 +68,15 @@
 
             LOCATION here refers to GCP Locations:
             https://cloud.google.com/about/locations/ INSIGHT_TYPE_ID
             refers to supported insight types:
             https://cloud.google.com/recommender/docs/insights/insight-types.
         page_size (int):
             Optional. The maximum number of results to
-            return from this request.  Non-positive values
+            return from this request. Non-positive values
             are ignored. If not specified, the server will
             determine the number of results to return.
         page_token (str):
             Optional. If present, retrieves the next batch of results
             from the preceding call to this method. ``page_token`` must
             be the value of ``next_page_token`` from the previous
             response. The values of other method parameters must be
@@ -99,97 +101,97 @@
 
             -  ``stateInfo.state = ACTIVE AND (severity = CRITICAL OR severity = HIGH)``
 
             (These expressions are based on the filter language
             described at https://google.aip.dev/160)
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
 
 
 class ListInsightsResponse(proto.Message):
     r"""Response to the ``ListInsights`` method.
 
     Attributes:
-        insights (Sequence[google.cloud.recommender_v1beta1.types.Insight]):
+        insights (MutableSequence[google.cloud.recommender_v1.types.Insight]):
             The set of insights for the ``parent`` resource.
         next_page_token (str):
             A token that can be used to request the next
             page of results. This field is empty if there
             are no additional results.
     """
 
     @property
     def raw_page(self):
         return self
 
-    insights = proto.RepeatedField(
+    insights: MutableSequence[insight.Insight] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=insight.Insight,
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class GetInsightRequest(proto.Message):
     r"""Request to the ``GetInsight`` method.
 
     Attributes:
         name (str):
             Required. Name of the insight.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class MarkInsightAcceptedRequest(proto.Message):
     r"""Request for the ``MarkInsightAccepted`` method.
 
     Attributes:
         name (str):
             Required. Name of the insight.
-        state_metadata (Mapping[str, str]):
+        state_metadata (MutableMapping[str, str]):
             Optional. State properties user wish to include with this
             state. Full replace of the current state_metadata.
         etag (str):
             Required. Fingerprint of the Insight.
             Provides optimistic locking.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    state_metadata = proto.MapField(
+    state_metadata: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=2,
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class ListRecommendationsRequest(proto.Message):
     r"""Request for the ``ListRecommendations`` method.
@@ -211,15 +213,15 @@
 
             LOCATION here refers to GCP Locations:
             https://cloud.google.com/about/locations/ RECOMMENDER_ID
             refers to supported recommenders:
             https://cloud.google.com/recommender/docs/recommenders.
         page_size (int):
             Optional. The maximum number of results to
-            return from this request.  Non-positive values
+            return from this request. Non-positive values
             are ignored. If not specified, the server will
             determine the number of results to return.
         page_token (str):
             Optional. If present, retrieves the next batch of results
             from the preceding call to this method. ``page_token`` must
             be the value of ``next_page_token`` from the previous
             response. The values of other method parameters must be
@@ -244,161 +246,163 @@
 
             -  ``stateInfo.state = ACTIVE AND (priority = P1 OR priority = P2)``
 
             (These expressions are based on the filter language
             described at https://google.aip.dev/160)
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
         number=5,
     )
 
 
 class ListRecommendationsResponse(proto.Message):
     r"""Response to the ``ListRecommendations`` method.
 
     Attributes:
-        recommendations (Sequence[google.cloud.recommender_v1beta1.types.Recommendation]):
+        recommendations (MutableSequence[google.cloud.recommender_v1.types.Recommendation]):
             The set of recommendations for the ``parent`` resource.
         next_page_token (str):
             A token that can be used to request the next
             page of results. This field is empty if there
             are no additional results.
     """
 
     @property
     def raw_page(self):
         return self
 
-    recommendations = proto.RepeatedField(
+    recommendations: MutableSequence[
+        recommendation.Recommendation
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=recommendation.Recommendation,
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class GetRecommendationRequest(proto.Message):
     r"""Request to the ``GetRecommendation`` method.
 
     Attributes:
         name (str):
             Required. Name of the recommendation.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class MarkRecommendationClaimedRequest(proto.Message):
     r"""Request for the ``MarkRecommendationClaimed`` Method.
 
     Attributes:
         name (str):
             Required. Name of the recommendation.
-        state_metadata (Mapping[str, str]):
+        state_metadata (MutableMapping[str, str]):
             State properties to include with this state. Overwrites any
             existing ``state_metadata``. Keys must match the regex
             ``/^[a-z0-9][a-z0-9_.-]{0,62}$/``. Values must match the
             regex ``/^[a-zA-Z0-9_./-]{0,255}$/``.
         etag (str):
             Required. Fingerprint of the Recommendation.
             Provides optimistic locking.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    state_metadata = proto.MapField(
+    state_metadata: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=2,
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class MarkRecommendationSucceededRequest(proto.Message):
     r"""Request for the ``MarkRecommendationSucceeded`` Method.
 
     Attributes:
         name (str):
             Required. Name of the recommendation.
-        state_metadata (Mapping[str, str]):
+        state_metadata (MutableMapping[str, str]):
             State properties to include with this state. Overwrites any
             existing ``state_metadata``. Keys must match the regex
             ``/^[a-z0-9][a-z0-9_.-]{0,62}$/``. Values must match the
             regex ``/^[a-zA-Z0-9_./-]{0,255}$/``.
         etag (str):
             Required. Fingerprint of the Recommendation.
             Provides optimistic locking.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    state_metadata = proto.MapField(
+    state_metadata: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=2,
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class MarkRecommendationFailedRequest(proto.Message):
     r"""Request for the ``MarkRecommendationFailed`` Method.
 
     Attributes:
         name (str):
             Required. Name of the recommendation.
-        state_metadata (Mapping[str, str]):
+        state_metadata (MutableMapping[str, str]):
             State properties to include with this state. Overwrites any
             existing ``state_metadata``. Keys must match the regex
             ``/^[a-z0-9][a-z0-9_.-]{0,62}$/``. Values must match the
             regex ``/^[a-zA-Z0-9_./-]{0,255}$/``.
         etag (str):
             Required. Fingerprint of the Recommendation.
             Provides optimistic locking.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    state_metadata = proto.MapField(
+    state_metadata: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=2,
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class GetRecommenderConfigRequest(proto.Message):
     r"""Request for the GetRecommenderConfig\` method.
@@ -412,44 +416,44 @@
             -  ``projects/[PROJECT_NUMBER]/locations/[LOCATION]/recommenders/[RECOMMENDER_ID]/config``
 
             -  ``projects/[PROJECT_ID]/locations/[LOCATION]/recommenders/[RECOMMENDER_ID]/config``
 
             -  ``organizations/[ORGANIZATION_ID]/locations/[LOCATION]/recommenders/[RECOMMENDER_ID]/config``
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class UpdateRecommenderConfigRequest(proto.Message):
     r"""Request for the ``UpdateRecommenderConfig`` method.
 
     Attributes:
-        recommender_config (google.cloud.recommender_v1beta1.types.RecommenderConfig):
+        recommender_config (google.cloud.recommender_v1.types.RecommenderConfig):
             Required. The RecommenderConfig to update.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             The list of fields to be updated.
         validate_only (bool):
             If true, validate the request and preview the
             change, but do not actually update it.
     """
 
-    recommender_config = proto.Field(
+    recommender_config: gcr_recommender_config.RecommenderConfig = proto.Field(
         proto.MESSAGE,
         number=1,
         message=gcr_recommender_config.RecommenderConfig,
     )
-    update_mask = proto.Field(
+    update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=2,
         message=field_mask_pb2.FieldMask,
     )
-    validate_only = proto.Field(
+    validate_only: bool = proto.Field(
         proto.BOOL,
         number=3,
     )
 
 
 class GetInsightTypeConfigRequest(proto.Message):
     r"""Request for the GetInsightTypeConfig\` method.
@@ -463,43 +467,43 @@
             -  ``projects/[PROJECT_NUMBER]/locations/global/recommenders/[INSIGHT_TYPE_ID]/config``
 
             -  ``projects/[PROJECT_ID]/locations/global/recommenders/[INSIGHT_TYPE_ID]/config``
 
             -  ``organizations/[ORGANIZATION_ID]/locations/global/recommenders/[INSIGHT_TYPE_ID]/config``
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class UpdateInsightTypeConfigRequest(proto.Message):
     r"""Request for the ``UpdateInsightTypeConfig`` method.
 
     Attributes:
-        insight_type_config (google.cloud.recommender_v1beta1.types.InsightTypeConfig):
+        insight_type_config (google.cloud.recommender_v1.types.InsightTypeConfig):
             Required. The InsightTypeConfig to update.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             The list of fields to be updated.
         validate_only (bool):
             If true, validate the request and preview the
             change, but do not actually update it.
     """
 
-    insight_type_config = proto.Field(
+    insight_type_config: gcr_insight_type_config.InsightTypeConfig = proto.Field(
         proto.MESSAGE,
         number=1,
         message=gcr_insight_type_config.InsightTypeConfig,
     )
-    update_mask = proto.Field(
+    update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=2,
         message=field_mask_pb2.FieldMask,
     )
-    validate_only = proto.Field(
+    validate_only: bool = proto.Field(
         proto.BOOL,
         number=3,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-recommender-2.8.3/google_cloud_recommender.egg-info/PKG-INFO` & `google-cloud-recommender-2.9.0/google_cloud_recommender.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: google-cloud-recommender
-Version: 2.8.3
-Summary: Cloud Recommender API client library
+Version: 2.9.0
+Summary: Google Cloud Recommender API client library
 Home-page: https://github.com/googleapis/python-recommender
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -15,15 +15,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
-Provides-Extra: libcst
 License-File: LICENSE
 
 Python Client for Cloud Recommender API
 =======================================
 
 |stable| |pypi| |versions|
```

### Comparing `google-cloud-recommender-2.8.3/google_cloud_recommender.egg-info/SOURCES.txt` & `google-cloud-recommender-2.9.0/google_cloud_recommender.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 google/cloud/recommender/__init__.py
+google/cloud/recommender/gapic_version.py
 google/cloud/recommender/py.typed
 google/cloud/recommender_v1/__init__.py
 google/cloud/recommender_v1/gapic_metadata.json
+google/cloud/recommender_v1/gapic_version.py
 google/cloud/recommender_v1/py.typed
 google/cloud/recommender_v1/services/__init__.py
 google/cloud/recommender_v1/services/recommender/__init__.py
 google/cloud/recommender_v1/services/recommender/async_client.py
 google/cloud/recommender_v1/services/recommender/client.py
 google/cloud/recommender_v1/services/recommender/pagers.py
 google/cloud/recommender_v1/services/recommender/transports/__init__.py
@@ -21,14 +23,15 @@
 google/cloud/recommender_v1/types/insight.py
 google/cloud/recommender_v1/types/insight_type_config.py
 google/cloud/recommender_v1/types/recommendation.py
 google/cloud/recommender_v1/types/recommender_config.py
 google/cloud/recommender_v1/types/recommender_service.py
 google/cloud/recommender_v1beta1/__init__.py
 google/cloud/recommender_v1beta1/gapic_metadata.json
+google/cloud/recommender_v1beta1/gapic_version.py
 google/cloud/recommender_v1beta1/py.typed
 google/cloud/recommender_v1beta1/services/__init__.py
 google/cloud/recommender_v1beta1/services/recommender/__init__.py
 google/cloud/recommender_v1beta1/services/recommender/async_client.py
 google/cloud/recommender_v1beta1/services/recommender/client.py
 google/cloud/recommender_v1beta1/services/recommender/pagers.py
 google/cloud/recommender_v1beta1/services/recommender/transports/__init__.py
@@ -44,16 +47,14 @@
 google_cloud_recommender.egg-info/PKG-INFO
 google_cloud_recommender.egg-info/SOURCES.txt
 google_cloud_recommender.egg-info/dependency_links.txt
 google_cloud_recommender.egg-info/namespace_packages.txt
 google_cloud_recommender.egg-info/not-zip-safe
 google_cloud_recommender.egg-info/requires.txt
 google_cloud_recommender.egg-info/top_level.txt
-scripts/fixup_recommender_v1_keywords.py
-scripts/fixup_recommender_v1beta1_keywords.py
 tests/__init__.py
 tests/unit/__init__.py
 tests/unit/gapic/__init__.py
 tests/unit/gapic/recommender_v1/__init__.py
 tests/unit/gapic/recommender_v1/test_recommender.py
 tests/unit/gapic/recommender_v1beta1/__init__.py
 tests/unit/gapic/recommender_v1beta1/test_recommender.py
```

### Comparing `google-cloud-recommender-2.8.3/setup.py` & `google-cloud-recommender-2.9.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 # -*- coding: utf-8 -*-
-#
-# Copyright 2018 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     https://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+#
 import io
 import os
 
-import setuptools
+import setuptools  # type: ignore
+
+package_root = os.path.abspath(os.path.dirname(__file__))
 
 name = "google-cloud-recommender"
-description = "Cloud Recommender API client library"
-version = "2.8.3"
-release_status = "Development Status :: 5 - Production/Stable"
+
+
+description = "Google Cloud Recommender API client library"
+
+version = {}
+with open(
+    os.path.join(package_root, "google/cloud/recommender/gapic_version.py")
+) as fp:
+    exec(fp.read(), version)
+version = version["__version__"]
+
+if version[0] == "0":
+    release_status = "Development Status :: 4 - Beta"
+else:
+    release_status = "Development Status :: 5 - Production/Stable"
+
 dependencies = [
-    "google-api-core[grpc] >= 1.32.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
+    "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-extras = {"libcst": "libcst >= 0.2.5"}
-scripts = [
-    "scripts/fixup_recommender_v1_keywords.py",
-    "scripts/fixup_recommender_v1beta1_keywords.py",
-]
+url = "https://github.com/googleapis/python-recommender"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
@@ -54,15 +64,15 @@
     name=name,
     version=version,
     description=description,
     long_description=readme,
     author="Google LLC",
     author_email="googleapis-packages@google.com",
     license="Apache 2.0",
-    url="https://github.com/googleapis/python-recommender",
+    url=url,
     classifiers=[
         release_status,
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
@@ -70,15 +80,13 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
         "Topic :: Internet",
     ],
     platforms="Posix; MacOS X; Windows",
     packages=packages,
+    python_requires=">=3.7",
     namespace_packages=namespaces,
     install_requires=dependencies,
-    extras_require=extras,
-    python_requires=">=3.7",
-    scripts=scripts,
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `google-cloud-recommender-2.8.3/tests/__init__.py` & `google-cloud-recommender-2.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommender-2.8.3/tests/unit/__init__.py` & `google-cloud-recommender-2.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommender-2.8.3/tests/unit/gapic/__init__.py` & `google-cloud-recommender-2.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommender-2.8.3/tests/unit/gapic/recommender_v1/__init__.py` & `google-cloud-recommender-2.9.0/tests/unit/gapic/recommender_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommender-2.8.3/tests/unit/gapic/recommender_v1/test_recommender.py` & `google-cloud-recommender-2.9.0/tests/unit/gapic/recommender_v1/test_recommender.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommender-2.8.3/tests/unit/gapic/recommender_v1beta1/__init__.py` & `google-cloud-recommender-2.9.0/tests/unit/gapic/recommender_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recommender-2.8.3/tests/unit/gapic/recommender_v1beta1/test_recommender.py` & `google-cloud-recommender-2.9.0/tests/unit/gapic/recommender_v1beta1/test_recommender.py`

 * *Files identical despite different names*

