# Comparing `tmp/google-cloud-translate-3.8.4.tar.gz` & `tmp/google-cloud-translate-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-translate-3.8.4.tar", last modified: Mon Oct 10 16:24:14 2022, max compression
+gzip compressed data, was "google-cloud-translate-3.9.0.tar", last modified: Thu Dec 15 23:17:39 2022, max compression
```

## Comparing `google-cloud-translate-3.8.4.tar` & `google-cloud-translate-3.9.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.212258 google-cloud-translate-3.8.4/
--rw-rw-r--   0 root         (0)     1003    11358 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4653 2022-10-10 16:24:14.212258 google-cloud-translate-3.8.4/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3780 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.200257 google-cloud-translate-3.8.4/google/
--rw-rw-r--   0 root         (0)     1003      774 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.200257 google-cloud-translate-3.8.4/google/cloud/
--rw-rw-r--   0 root         (0)     1003      774 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.200257 google-cloud-translate-3.8.4/google/cloud/translate/
--rw-rw-r--   0 root         (0)     1003     5200 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate/__init__.py
--rw-rw-r--   0 root         (0)     1003       83 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.200257 google-cloud-translate-3.8.4/google/cloud/translate_v2/
--rw-rw-r--   0 root         (0)     1003      821 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     1731 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v2/_http.py
--rw-rw-r--   0 root         (0)     1003    10818 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v2/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.200257 google-cloud-translate-3.8.4/google/cloud/translate_v3/
--rw-rw-r--   0 root         (0)     1003     4115 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3/__init__.py
--rw-rw-r--   0 root         (0)     1003     3121 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       83 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.204258 google-cloud-translate-3.8.4/google/cloud/translate_v3/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.204258 google-cloud-translate-3.8.4/google/cloud/translate_v3/services/translation_service/
--rw-rw-r--   0 root         (0)     1003      785 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3/services/translation_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    67128 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3/services/translation_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    76127 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3/services/translation_service/client.py
--rw-rw-r--   0 root         (0)     1003     5906 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3/services/translation_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.204258 google-cloud-translate-3.8.4/google/cloud/translate_v3/services/translation_service/transports/
--rw-rw-r--   0 root         (0)     1003     1238 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3/services/translation_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12533 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3/services/translation_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    24359 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3/services/translation_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    24851 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3/services/translation_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.204258 google-cloud-translate-3.8.4/google/cloud/translate_v3/types/
--rw-rw-r--   0 root         (0)     1003     2684 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    71068 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3/types/translation_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.204258 google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/
--rw-rw-r--   0 root         (0)     1003     4115 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3131 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       83 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.204258 google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.204258 google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/services/translation_service/
--rw-rw-r--   0 root         (0)     1003      785 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/services/translation_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    63545 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/services/translation_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    72537 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/services/translation_service/client.py
--rw-rw-r--   0 root         (0)     1003     5951 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/services/translation_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.208258 google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/services/translation_service/transports/
--rw-rw-r--   0 root         (0)     1003     1238 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/services/translation_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12538 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/services/translation_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    24415 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/services/translation_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    24907 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/services/translation_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.208258 google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/types/
--rw-rw-r--   0 root         (0)     1003     2684 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    70895 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/types/translation_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.208258 google-cloud-translate-3.8.4/google_cloud_translate.egg-info/
--rw-r--r--   0 root         (0)     1003     4653 2022-10-10 16:24:14.000000 google-cloud-translate-3.8.4/google_cloud_translate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2813 2022-10-10 16:24:14.000000 google-cloud-translate-3.8.4/google_cloud_translate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:24:14.000000 google-cloud-translate-3.8.4/google_cloud_translate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-10-10 16:24:14.000000 google-cloud-translate-3.8.4/google_cloud_translate.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:24:14.000000 google-cloud-translate-3.8.4/google_cloud_translate.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      267 2022-10-10 16:24:14.000000 google-cloud-translate-3.8.4/google_cloud_translate.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-10-10 16:24:14.000000 google-cloud-translate-3.8.4/google_cloud_translate.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.208258 google-cloud-translate-3.8.4/scripts/
--rw-rw-r--   0 root         (0)     1003     6954 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/scripts/fixup_translate_v3_keywords.py
--rw-rw-r--   0 root         (0)     1003     6954 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/scripts/fixup_translate_v3beta1_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-10-10 16:24:14.212258 google-cloud-translate-3.8.4/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3047 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.208258 google-cloud-translate-3.8.4/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.208258 google-cloud-translate-3.8.4/tests/system/
--rw-rw-r--   0 root         (0)     1003     5603 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/tests/system/test_vpcsc.py
--rw-rw-r--   0 root         (0)     1003     5443 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/tests/system.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.208258 google-cloud-translate-3.8.4/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.208258 google-cloud-translate-3.8.4/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.208258 google-cloud-translate-3.8.4/tests/unit/gapic/translate_v3/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/tests/unit/gapic/translate_v3/__init__.py
--rw-rw-r--   0 root         (0)     1003   147410 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/tests/unit/gapic/translate_v3/test_translation_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.212258 google-cloud-translate-3.8.4/tests/unit/gapic/translate_v3beta1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/tests/unit/gapic/translate_v3beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   142597 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/tests/unit/gapic/translate_v3beta1/test_translation_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:14.212258 google-cloud-translate-3.8.4/tests/unit/v2/
--rw-rw-r--   0 root         (0)     1003     4689 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/tests/unit/v2/test__http.py
--rw-rw-r--   0 root         (0)     1003    13223 2022-10-10 16:21:03.000000 google-cloud-translate-3.8.4/tests/unit/v2/test_client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.309299 google-cloud-translate-3.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4651 2022-12-15 23:17:39.309299 google-cloud-translate-3.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3780 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.297295 google-cloud-translate-3.9.0/google/
+-rw-rw-r--   0 root         (0)     1003      774 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.297295 google-cloud-translate-3.9.0/google/cloud/
+-rw-rw-r--   0 root         (0)     1003      774 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.297295 google-cloud-translate-3.9.0/google/cloud/translate/
+-rw-rw-r--   0 root         (0)     1003     5312 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       83 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.297295 google-cloud-translate-3.9.0/google/cloud/translate_v2/
+-rw-rw-r--   0 root         (0)     1003      821 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1731 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v2/_http.py
+-rw-rw-r--   0 root         (0)     1003    10818 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v2/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.301297 google-cloud-translate-3.9.0/google/cloud/translate_v3/
+-rw-rw-r--   0 root         (0)     1003     4227 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3121 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       83 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.301297 google-cloud-translate-3.9.0/google/cloud/translate_v3/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.301297 google-cloud-translate-3.9.0/google/cloud/translate_v3/services/translation_service/
+-rw-rw-r--   0 root         (0)     1003      785 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3/services/translation_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    68110 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3/services/translation_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    77121 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3/services/translation_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5906 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3/services/translation_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.301297 google-cloud-translate-3.9.0/google/cloud/translate_v3/services/translation_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1238 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3/services/translation_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12413 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3/services/translation_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    24459 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3/services/translation_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    24938 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3/services/translation_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.301297 google-cloud-translate-3.9.0/google/cloud/translate_v3/types/
+-rw-rw-r--   0 root         (0)     1003     2684 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    73073 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3/types/translation_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.301297 google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/
+-rw-rw-r--   0 root         (0)     1003     4227 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3131 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       83 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.301297 google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.305298 google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/services/translation_service/
+-rw-rw-r--   0 root         (0)     1003      785 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/services/translation_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    64458 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/services/translation_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    73462 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/services/translation_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5951 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/services/translation_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.305298 google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/services/translation_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1238 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/services/translation_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12423 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/services/translation_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    24515 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/services/translation_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    24994 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/services/translation_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.305298 google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/types/
+-rw-rw-r--   0 root         (0)     1003     2684 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    72900 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/types/translation_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.305298 google-cloud-translate-3.9.0/google_cloud_translate.egg-info/
+-rw-r--r--   0 root         (0)     1003     4651 2022-12-15 23:17:39.000000 google-cloud-translate-3.9.0/google_cloud_translate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2861 2022-12-15 23:17:39.000000 google-cloud-translate-3.9.0/google_cloud_translate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-12-15 23:17:39.000000 google-cloud-translate-3.9.0/google_cloud_translate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-12-15 23:17:39.000000 google-cloud-translate-3.9.0/google_cloud_translate.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-12-15 23:17:39.000000 google-cloud-translate-3.9.0/google_cloud_translate.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      292 2022-12-15 23:17:39.000000 google-cloud-translate-3.9.0/google_cloud_translate.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-12-15 23:17:39.000000 google-cloud-translate-3.9.0/google_cloud_translate.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2022-12-15 23:17:39.309299 google-cloud-translate-3.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2914 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.305298 google-cloud-translate-3.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.305298 google-cloud-translate-3.9.0/tests/system/
+-rw-rw-r--   0 root         (0)     1003     5603 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/tests/system/test_vpcsc.py
+-rw-rw-r--   0 root         (0)     1003     5443 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/tests/system.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.305298 google-cloud-translate-3.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.305298 google-cloud-translate-3.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.305298 google-cloud-translate-3.9.0/tests/unit/gapic/translate_v3/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/tests/unit/gapic/translate_v3/__init__.py
+-rw-rw-r--   0 root         (0)     1003   147410 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/tests/unit/gapic/translate_v3/test_translation_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.309299 google-cloud-translate-3.9.0/tests/unit/gapic/translate_v3beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/tests/unit/gapic/translate_v3beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   142597 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/tests/unit/gapic/translate_v3beta1/test_translation_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 23:17:39.309299 google-cloud-translate-3.9.0/tests/unit/v2/
+-rw-rw-r--   0 root         (0)     1003     4689 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/tests/unit/v2/test__http.py
+-rw-rw-r--   0 root         (0)     1003    13223 2022-12-15 23:14:21.000000 google-cloud-translate-3.9.0/tests/unit/v2/test_client.py
```

### Comparing `google-cloud-translate-3.8.4/LICENSE` & `google-cloud-translate-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/MANIFEST.in` & `google-cloud-translate-3.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/PKG-INFO` & `google-cloud-translate-3.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: google-cloud-translate
-Version: 3.8.4
-Summary: Google Cloud Translation API client library
+Version: 3.9.0
+Summary: Google Cloud Translate API client library
 Home-page: https://github.com/googleapis/python-translate
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `google-cloud-translate-3.8.4/README.rst` & `google-cloud-translate-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/google/__init__.py` & `google-cloud-translate-3.9.0/google/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/google/cloud/__init__.py` & `google-cloud-translate-3.9.0/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate/__init__.py` & `google-cloud-translate-3.9.0/google/cloud/translate/__init__.py`

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
+from google.cloud.translate import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from google.cloud.translate_v3.services.translation_service.client import (
     TranslationServiceClient,
 )
 from google.cloud.translate_v3.services.translation_service.async_client import (
     TranslationServiceAsyncClient,
 )
```

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v2/__init__.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v2/_http.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v2/_http.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v2/client.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v2/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3/__init__.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.translate import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from .services.translation_service import TranslationServiceClient
 from .services.translation_service import TranslationServiceAsyncClient
 
 from .types.translation_service import BatchDocumentInputConfig
 from .types.translation_service import BatchDocumentOutputConfig
 from .types.translation_service import BatchTranslateDocumentMetadata
```

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3/gapic_metadata.json` & `google-cloud-translate-3.9.0/google/cloud/translate_v3/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3/services/__init__.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3/services/translation_service/__init__.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3/services/translation_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3/services/translation_service/async_client.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3/services/translation_service/async_client.py`

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
+from google.cloud.translate_v3 import gapic_version as package_version
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
@@ -158,17 +169,17 @@
         type(TranslationServiceClient).get_transport_class,
         type(TranslationServiceClient),
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, TranslationServiceTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the translation service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -204,24 +215,24 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def translate_text(
         self,
-        request: Union[translation_service.TranslateTextRequest, dict] = None,
+        request: Optional[Union[translation_service.TranslateTextRequest, dict]] = None,
         *,
-        parent: str = None,
-        target_language_code: str = None,
-        contents: Sequence[str] = None,
-        model: str = None,
-        mime_type: str = None,
-        source_language_code: str = None,
+        parent: Optional[str] = None,
+        target_language_code: Optional[str] = None,
+        contents: Optional[MutableSequence[str]] = None,
+        model: Optional[str] = None,
+        mime_type: Optional[str] = None,
+        source_language_code: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> translation_service.TranslateTextResponse:
         r"""Translates input text and returns translated text.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -247,15 +258,15 @@
                 # Make the request
                 response = await client.translate_text(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.translate_v3.types.TranslateTextRequest, dict]):
+            request (Optional[Union[google.cloud.translate_v3.types.TranslateTextRequest, dict]]):
                 The request object. The request message for synchronous
                 translation.
             parent (:class:`str`):
                 Required. Project or location to make a call. Must refer
                 to a caller's project.
 
                 Format: ``projects/{project-number-or-id}`` or
@@ -280,15 +291,15 @@
                 use for translation of the input text,
                 set to one of the language codes listed
                 in Language Support.
 
                 This corresponds to the ``target_language_code`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            contents (:class:`Sequence[str]`):
+            contents (:class:`MutableSequence[str]`):
                 Required. The content of the input in
                 string format. We recommend the total
                 content be less than 30k codepoints. The
                 max length of this field is 1024.
                 Use BatchTranslateText for larger text.
 
                 This corresponds to the ``contents`` field
@@ -407,22 +418,24 @@
         )
 
         # Done; return the response.
         return response
 
     async def detect_language(
         self,
-        request: Union[translation_service.DetectLanguageRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.DetectLanguageRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        model: str = None,
-        mime_type: str = None,
-        content: str = None,
+        parent: Optional[str] = None,
+        model: Optional[str] = None,
+        mime_type: Optional[str] = None,
+        content: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> translation_service.DetectLanguageResponse:
         r"""Detects the language of text within a request.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -447,15 +460,15 @@
                 # Make the request
                 response = await client.detect_language(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.translate_v3.types.DetectLanguageRequest, dict]):
+            request (Optional[Union[google.cloud.translate_v3.types.DetectLanguageRequest, dict]]):
                 The request object. The request message for language
                 detection.
             parent (:class:`str`):
                 Required. Project or location to make a call. Must refer
                 to a caller's project.
 
                 Format:
@@ -562,21 +575,23 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_supported_languages(
         self,
-        request: Union[translation_service.GetSupportedLanguagesRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.GetSupportedLanguagesRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        model: str = None,
-        display_language_code: str = None,
+        parent: Optional[str] = None,
+        model: Optional[str] = None,
+        display_language_code: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> translation_service.SupportedLanguages:
         r"""Returns a list of supported languages for
         translation.
 
         .. code-block:: python
 
@@ -601,15 +616,15 @@
                 # Make the request
                 response = await client.get_supported_languages(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.translate_v3.types.GetSupportedLanguagesRequest, dict]):
+            request (Optional[Union[google.cloud.translate_v3.types.GetSupportedLanguagesRequest, dict]]):
                 The request object. The request message for discovering
                 supported languages.
             parent (:class:`str`):
                 Required. Project or location to make a call. Must refer
                 to a caller's project.
 
                 Format: ``projects/{project-number-or-id}`` or
@@ -722,18 +737,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def translate_document(
         self,
-        request: Union[translation_service.TranslateDocumentRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.TranslateDocumentRequest, dict]
+        ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> translation_service.TranslateDocumentResponse:
         r"""Translates documents in synchronous mode.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -762,15 +779,15 @@
                 # Make the request
                 response = await client.translate_document(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.translate_v3.types.TranslateDocumentRequest, dict]):
+            request (Optional[Union[google.cloud.translate_v3.types.TranslateDocumentRequest, dict]]):
                 The request object. A document translation request.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
@@ -806,18 +823,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def batch_translate_text(
         self,
-        request: Union[translation_service.BatchTranslateTextRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.BatchTranslateTextRequest, dict]
+        ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Translates a large volume of text in asynchronous
         batch mode. This function provides real-time output as
         the inputs are being processed. If caller cancels a
         request, the partial results (for an input file, it's
         all or nothing) may still be available on the specified
@@ -857,21 +876,21 @@
                 )
 
                 # Make the request
                 operation = client.batch_translate_text(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.translate_v3.types.BatchTranslateTextRequest, dict]):
+            request (Optional[Union[google.cloud.translate_v3.types.BatchTranslateTextRequest, dict]]):
                 The request object. The batch translation request.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
@@ -919,23 +938,27 @@
         )
 
         # Done; return the response.
         return response
 
     async def batch_translate_document(
         self,
-        request: Union[translation_service.BatchTranslateDocumentRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.BatchTranslateDocumentRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        source_language_code: str = None,
-        target_language_codes: Sequence[str] = None,
-        input_configs: Sequence[translation_service.BatchDocumentInputConfig] = None,
-        output_config: translation_service.BatchDocumentOutputConfig = None,
+        parent: Optional[str] = None,
+        source_language_code: Optional[str] = None,
+        target_language_codes: Optional[MutableSequence[str]] = None,
+        input_configs: Optional[
+            MutableSequence[translation_service.BatchDocumentInputConfig]
+        ] = None,
+        output_config: Optional[translation_service.BatchDocumentOutputConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Translates a large volume of document in asynchronous
         batch mode. This function provides real-time output as
         the inputs are being processed. If caller cancels a
         request, the partial results (for an input file, it's
         all or nothing) may still be available on the specified
@@ -975,21 +998,21 @@
                 )
 
                 # Make the request
                 operation = client.batch_translate_document(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.translate_v3.types.BatchTranslateDocumentRequest, dict]):
+            request (Optional[Union[google.cloud.translate_v3.types.BatchTranslateDocumentRequest, dict]]):
                 The request object. The BatchTranslateDocument request.
             parent (:class:`str`):
                 Required. Location to make a regional call.
 
                 Format:
                 ``projects/{project-number-or-id}/locations/{location-id}``.
 
@@ -1010,24 +1033,24 @@
                 language codes are listed in Language
                 Support
                 (https://cloud.google.com/translate/docs/languages).
 
                 This corresponds to the ``source_language_code`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            target_language_codes (:class:`Sequence[str]`):
+            target_language_codes (:class:`MutableSequence[str]`):
                 Required. The BCP-47 language code to
                 use for translation of the input
                 document. Specify up to 10 language
                 codes here.
 
                 This corresponds to the ``target_language_codes`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            input_configs (:class:`Sequence[google.cloud.translate_v3.types.BatchDocumentInputConfig]`):
+            input_configs (:class:`MutableSequence[google.cloud.translate_v3.types.BatchDocumentInputConfig]`):
                 Required. Input configurations.
                 The total number of files matched should
                 be <= 100. The total content size to
                 translate should be <= 100M Unicode
                 codepoints. The files must use UTF-8
                 encoding.
 
@@ -1124,20 +1147,22 @@
         )
 
         # Done; return the response.
         return response
 
     async def create_glossary(
         self,
-        request: Union[translation_service.CreateGlossaryRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.CreateGlossaryRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        glossary: translation_service.Glossary = None,
+        parent: Optional[str] = None,
+        glossary: Optional[translation_service.Glossary] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Creates a glossary and returns the long-running operation.
         Returns NOT_FOUND, if the project doesn't exist.
 
         .. code-block:: python
 
@@ -1164,21 +1189,21 @@
                 )
 
                 # Make the request
                 operation = client.create_glossary(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.translate_v3.types.CreateGlossaryRequest, dict]):
+            request (Optional[Union[google.cloud.translate_v3.types.CreateGlossaryRequest, dict]]):
                 The request object. Request message for CreateGlossary.
             parent (:class:`str`):
                 Required. The project name.
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             glossary (:class:`google.cloud.translate_v3.types.Glossary`):
@@ -1251,19 +1276,21 @@
         )
 
         # Done; return the response.
         return response
 
     async def list_glossaries(
         self,
-        request: Union[translation_service.ListGlossariesRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.ListGlossariesRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListGlossariesAsyncPager:
         r"""Lists glossaries in a project. Returns NOT_FOUND, if the project
         doesn't exist.
 
         .. code-block:: python
 
@@ -1289,15 +1316,15 @@
                 page_result = client.list_glossaries(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.translate_v3.types.ListGlossariesRequest, dict]):
+            request (Optional[Union[google.cloud.translate_v3.types.ListGlossariesRequest, dict]]):
                 The request object. Request message for ListGlossaries.
             parent (:class:`str`):
                 Required. The name of the project
                 from which to list all of the
                 glossaries.
 
                 This corresponds to the ``parent`` field
@@ -1376,19 +1403,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_glossary(
         self,
-        request: Union[translation_service.GetGlossaryRequest, dict] = None,
+        request: Optional[Union[translation_service.GetGlossaryRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> translation_service.Glossary:
         r"""Gets a glossary. Returns NOT_FOUND, if the glossary doesn't
         exist.
 
         .. code-block:: python
 
@@ -1413,15 +1440,15 @@
                 # Make the request
                 response = await client.get_glossary(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.translate_v3.types.GetGlossaryRequest, dict]):
+            request (Optional[Union[google.cloud.translate_v3.types.GetGlossaryRequest, dict]]):
                 The request object. Request message for GetGlossary.
             name (:class:`str`):
                 Required. The name of the glossary to
                 retrieve.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1488,19 +1515,21 @@
         )
 
         # Done; return the response.
         return response
 
     async def delete_glossary(
         self,
-        request: Union[translation_service.DeleteGlossaryRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.DeleteGlossaryRequest, dict]
+        ] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Deletes a glossary, or cancels glossary construction if the
         glossary isn't created yet. Returns NOT_FOUND, if the glossary
         doesn't exist.
 
         .. code-block:: python
@@ -1524,21 +1553,21 @@
                 )
 
                 # Make the request
                 operation = client.delete_glossary(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.translate_v3.types.DeleteGlossaryRequest, dict]):
+            request (Optional[Union[google.cloud.translate_v3.types.DeleteGlossaryRequest, dict]]):
                 The request object. Request message for DeleteGlossary.
             name (:class:`str`):
                 Required. The name of the glossary to
                 delete.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1621,18 +1650,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-translate",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("TranslationServiceAsyncClient",)
```

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3/services/translation_service/client.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3/services/translation_service/client.py`

 * *Files 8% similar despite different names*

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
+from google.cloud.translate_v3 import gapic_version as package_version
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport import mtls  # type: ignore
@@ -56,15 +68,15 @@
         OrderedDict()
     )  # type: Dict[str, Type[TranslationServiceTransport]]
     _transport_registry["grpc"] = TranslationServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = TranslationServiceGrpcAsyncIOTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[TranslationServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -331,30 +343,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, TranslationServiceTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, TranslationServiceTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the translation service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, TranslationServiceTransport]): The
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
@@ -376,14 +388,15 @@
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
@@ -428,24 +441,24 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def translate_text(
         self,
-        request: Union[translation_service.TranslateTextRequest, dict] = None,
+        request: Optional[Union[translation_service.TranslateTextRequest, dict]] = None,
         *,
-        parent: str = None,
-        target_language_code: str = None,
-        contents: Sequence[str] = None,
-        model: str = None,
-        mime_type: str = None,
-        source_language_code: str = None,
+        parent: Optional[str] = None,
+        target_language_code: Optional[str] = None,
+        contents: Optional[MutableSequence[str]] = None,
+        model: Optional[str] = None,
+        mime_type: Optional[str] = None,
+        source_language_code: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> translation_service.TranslateTextResponse:
         r"""Translates input text and returns translated text.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -504,15 +517,15 @@
                 use for translation of the input text,
                 set to one of the language codes listed
                 in Language Support.
 
                 This corresponds to the ``target_language_code`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            contents (Sequence[str]):
+            contents (MutableSequence[str]):
                 Required. The content of the input in
                 string format. We recommend the total
                 content be less than 30k codepoints. The
                 max length of this field is 1024.
                 Use BatchTranslateText for larger text.
 
                 This corresponds to the ``contents`` field
@@ -631,22 +644,24 @@
         )
 
         # Done; return the response.
         return response
 
     def detect_language(
         self,
-        request: Union[translation_service.DetectLanguageRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.DetectLanguageRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        model: str = None,
-        mime_type: str = None,
-        content: str = None,
+        parent: Optional[str] = None,
+        model: Optional[str] = None,
+        mime_type: Optional[str] = None,
+        content: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> translation_service.DetectLanguageResponse:
         r"""Detects the language of text within a request.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -786,21 +801,23 @@
         )
 
         # Done; return the response.
         return response
 
     def get_supported_languages(
         self,
-        request: Union[translation_service.GetSupportedLanguagesRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.GetSupportedLanguagesRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        model: str = None,
-        display_language_code: str = None,
+        parent: Optional[str] = None,
+        model: Optional[str] = None,
+        display_language_code: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> translation_service.SupportedLanguages:
         r"""Returns a list of supported languages for
         translation.
 
         .. code-block:: python
 
@@ -936,18 +953,20 @@
         )
 
         # Done; return the response.
         return response
 
     def translate_document(
         self,
-        request: Union[translation_service.TranslateDocumentRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.TranslateDocumentRequest, dict]
+        ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> translation_service.TranslateDocumentResponse:
         r"""Translates documents in synchronous mode.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1021,18 +1040,20 @@
         )
 
         # Done; return the response.
         return response
 
     def batch_translate_text(
         self,
-        request: Union[translation_service.BatchTranslateTextRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.BatchTranslateTextRequest, dict]
+        ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Translates a large volume of text in asynchronous
         batch mode. This function provides real-time output as
         the inputs are being processed. If caller cancels a
         request, the partial results (for an input file, it's
         all or nothing) may still be available on the specified
@@ -1135,23 +1156,27 @@
         )
 
         # Done; return the response.
         return response
 
     def batch_translate_document(
         self,
-        request: Union[translation_service.BatchTranslateDocumentRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.BatchTranslateDocumentRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        source_language_code: str = None,
-        target_language_codes: Sequence[str] = None,
-        input_configs: Sequence[translation_service.BatchDocumentInputConfig] = None,
-        output_config: translation_service.BatchDocumentOutputConfig = None,
+        parent: Optional[str] = None,
+        source_language_code: Optional[str] = None,
+        target_language_codes: Optional[MutableSequence[str]] = None,
+        input_configs: Optional[
+            MutableSequence[translation_service.BatchDocumentInputConfig]
+        ] = None,
+        output_config: Optional[translation_service.BatchDocumentOutputConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Translates a large volume of document in asynchronous
         batch mode. This function provides real-time output as
         the inputs are being processed. If caller cancels a
         request, the partial results (for an input file, it's
         all or nothing) may still be available on the specified
@@ -1226,24 +1251,24 @@
                 language codes are listed in Language
                 Support
                 (https://cloud.google.com/translate/docs/languages).
 
                 This corresponds to the ``source_language_code`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            target_language_codes (Sequence[str]):
+            target_language_codes (MutableSequence[str]):
                 Required. The BCP-47 language code to
                 use for translation of the input
                 document. Specify up to 10 language
                 codes here.
 
                 This corresponds to the ``target_language_codes`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            input_configs (Sequence[google.cloud.translate_v3.types.BatchDocumentInputConfig]):
+            input_configs (MutableSequence[google.cloud.translate_v3.types.BatchDocumentInputConfig]):
                 Required. Input configurations.
                 The total number of files matched should
                 be <= 100. The total content size to
                 translate should be <= 100M Unicode
                 codepoints. The files must use UTF-8
                 encoding.
 
@@ -1340,20 +1365,22 @@
         )
 
         # Done; return the response.
         return response
 
     def create_glossary(
         self,
-        request: Union[translation_service.CreateGlossaryRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.CreateGlossaryRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        glossary: translation_service.Glossary = None,
+        parent: Optional[str] = None,
+        glossary: Optional[translation_service.Glossary] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Creates a glossary and returns the long-running operation.
         Returns NOT_FOUND, if the project doesn't exist.
 
         .. code-block:: python
 
@@ -1467,19 +1494,21 @@
         )
 
         # Done; return the response.
         return response
 
     def list_glossaries(
         self,
-        request: Union[translation_service.ListGlossariesRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.ListGlossariesRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListGlossariesPager:
         r"""Lists glossaries in a project. Returns NOT_FOUND, if the project
         doesn't exist.
 
         .. code-block:: python
 
@@ -1582,19 +1611,19 @@
         )
 
         # Done; return the response.
         return response
 
     def get_glossary(
         self,
-        request: Union[translation_service.GetGlossaryRequest, dict] = None,
+        request: Optional[Union[translation_service.GetGlossaryRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> translation_service.Glossary:
         r"""Gets a glossary. Returns NOT_FOUND, if the glossary doesn't
         exist.
 
         .. code-block:: python
 
@@ -1684,19 +1713,21 @@
         )
 
         # Done; return the response.
         return response
 
     def delete_glossary(
         self,
-        request: Union[translation_service.DeleteGlossaryRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.DeleteGlossaryRequest, dict]
+        ] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Deletes a glossary, or cancels glossary construction if the
         glossary isn't created yet. Returns NOT_FOUND, if the glossary
         doesn't exist.
 
         .. code-block:: python
@@ -1814,18 +1845,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-translate",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("TranslationServiceClient",)
```

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3/services/translation_service/pagers.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3/services/translation_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3/services/translation_service/transports/__init__.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3/services/translation_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3/services/translation_service/transports/base.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/services/translation_service/transports/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,36 +11,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import abc
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Union
-import pkg_resources
+
+from google.cloud.translate_v3beta1 import gapic_version as package_version
 
 import google.auth  # type: ignore
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core import operations_v1
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-from google.cloud.translate_v3.types import translation_service
+from google.cloud.translate_v3beta1.types import translation_service
 from google.longrunning import operations_pb2  # type: ignore
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-translate",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class TranslationServiceTransport(abc.ABC):
     """Abstract transport class for TranslationService."""
 
     AUTH_SCOPES = (
         "https://www.googleapis.com/auth/cloud-platform",
@@ -49,15 +45,15 @@
 
     DEFAULT_HOST: str = "translate.googleapis.com"
 
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

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3/services/translation_service/transports/grpc.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3/services/translation_service/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,22 +45,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "translate.googleapis.com",
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
 
@@ -180,16 +180,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "translate.googleapis.com",
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

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3/services/translation_service/transports/grpc_asyncio.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3/services/translation_service/transports/grpc_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "translate.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -90,23 +90,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "translate.googleapis.com",
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

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3/types/__init__.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3/types/translation_service.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3/types/translation_service.py`

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
 
 from google.protobuf import timestamp_pb2  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.cloud.translation.v3",
@@ -77,29 +79,29 @@
                ``projects/{project-number-or-id}/locations/{location-id}/glossaries/{glossary-id}``
         ignore_case (bool):
             Optional. Indicates match is
             case-insensitive. Default value is false if
             missing.
     """
 
-    glossary = proto.Field(
+    glossary: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    ignore_case = proto.Field(
+    ignore_case: bool = proto.Field(
         proto.BOOL,
         number=2,
     )
 
 
 class TranslateTextRequest(proto.Message):
     r"""The request message for synchronous translation.
 
     Attributes:
-        contents (Sequence[str]):
+        contents (MutableSequence[str]):
             Required. The content of the input in string
             format. We recommend the total content be less
             than 30k codepoints. The max length of this
             field is 1024.
             Use BatchTranslateText for larger text.
         mime_type (str):
             Optional. The format of the source text, for
@@ -152,86 +154,86 @@
             If not provided, the default Google model (NMT) will be
             used.
         glossary_config (google.cloud.translate_v3.types.TranslateTextGlossaryConfig):
             Optional. Glossary to be applied. The glossary must be
             within the same region (have the same location-id) as the
             model, otherwise an INVALID_ARGUMENT (400) error is
             returned.
-        labels (Mapping[str, str]):
+        labels (MutableMapping[str, str]):
             Optional. The labels with user-defined
             metadata for the request.
             Label keys and values can be no longer than 63
             characters (Unicode codepoints), can only
             contain lowercase letters, numeric characters,
             underscores and dashes. International characters
             are allowed. Label values are optional. Label
             keys must start with a letter.
             See
             https://cloud.google.com/translate/docs/advanced/labels
             for more information.
     """
 
-    contents = proto.RepeatedField(
+    contents: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=1,
     )
-    mime_type = proto.Field(
+    mime_type: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    source_language_code = proto.Field(
+    source_language_code: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    target_language_code = proto.Field(
+    target_language_code: str = proto.Field(
         proto.STRING,
         number=5,
     )
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=8,
     )
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=6,
     )
-    glossary_config = proto.Field(
+    glossary_config: "TranslateTextGlossaryConfig" = proto.Field(
         proto.MESSAGE,
         number=7,
         message="TranslateTextGlossaryConfig",
     )
-    labels = proto.MapField(
+    labels: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=10,
     )
 
 
 class TranslateTextResponse(proto.Message):
     r"""
 
     Attributes:
-        translations (Sequence[google.cloud.translate_v3.types.Translation]):
+        translations (MutableSequence[google.cloud.translate_v3.types.Translation]):
             Text translation responses with no glossary applied. This
             field has the same length as
             [``contents``][google.cloud.translation.v3.TranslateTextRequest.contents].
-        glossary_translations (Sequence[google.cloud.translate_v3.types.Translation]):
+        glossary_translations (MutableSequence[google.cloud.translate_v3.types.Translation]):
             Text translation responses if a glossary is provided in the
             request. This can be the same as
             [``translations``][google.cloud.translation.v3.TranslateTextResponse.translations]
             if no terms apply. This field has the same length as
             [``contents``][google.cloud.translation.v3.TranslateTextRequest.contents].
     """
 
-    translations = proto.RepeatedField(
+    translations: MutableSequence["Translation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="Translation",
     )
-    glossary_translations = proto.RepeatedField(
+    glossary_translations: MutableSequence["Translation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="Translation",
     )
 
 
 class Translation(proto.Message):
@@ -258,27 +260,27 @@
             request. If the source language was passed,
             auto-detection of the language does not occur
             and this field is empty.
         glossary_config (google.cloud.translate_v3.types.TranslateTextGlossaryConfig):
             The ``glossary_config`` used for this translation.
     """
 
-    translated_text = proto.Field(
+    translated_text: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    detected_language_code = proto.Field(
+    detected_language_code: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    glossary_config = proto.Field(
+    glossary_config: "TranslateTextGlossaryConfig" = proto.Field(
         proto.MESSAGE,
         number=3,
         message="TranslateTextGlossaryConfig",
     )
 
 
 class DetectLanguageRequest(proto.Message):
@@ -316,46 +318,46 @@
             The content of the input stored as a string.
 
             This field is a member of `oneof`_ ``source``.
         mime_type (str):
             Optional. The format of the source text, for
             example, "text/html", "text/plain". If left
             blank, the MIME type defaults to "text/html".
-        labels (Mapping[str, str]):
+        labels (MutableMapping[str, str]):
             Optional. The labels with user-defined
             metadata for the request.
             Label keys and values can be no longer than 63
             characters (Unicode codepoints), can only
             contain lowercase letters, numeric characters,
             underscores and dashes. International characters
             are allowed. Label values are optional. Label
             keys must start with a letter.
             See
             https://cloud.google.com/translate/docs/advanced/labels
             for more information.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=5,
     )
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    content = proto.Field(
+    content: str = proto.Field(
         proto.STRING,
         number=1,
         oneof="source",
     )
-    mime_type = proto.Field(
+    mime_type: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    labels = proto.MapField(
+    labels: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=6,
     )
 
 
 class DetectedLanguage(proto.Message):
@@ -366,36 +368,36 @@
             The BCP-47 language code of source content in
             the request, detected automatically.
         confidence (float):
             The confidence of the detection result for
             this language.
     """
 
-    language_code = proto.Field(
+    language_code: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
 
 
 class DetectLanguageResponse(proto.Message):
     r"""The response message for language detection.
 
     Attributes:
-        languages (Sequence[google.cloud.translate_v3.types.DetectedLanguage]):
+        languages (MutableSequence[google.cloud.translate_v3.types.DetectedLanguage]):
             The most probable language detected by the
             Translation API. For each request, the
             Translation API will always return only one
             result.
     """
 
-    languages = proto.RepeatedField(
+    languages: MutableSequence["DetectedLanguage"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="DetectedLanguage",
     )
 
 
 class GetSupportedLanguagesRequest(proto.Message):
@@ -435,39 +437,39 @@
                ``projects/{project-number-or-id}/locations/{location-id}/models/general/nmt``,
 
             Returns languages supported by the specified model. If
             missing, we get supported languages of Google general NMT
             model.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    display_language_code = proto.Field(
+    display_language_code: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class SupportedLanguages(proto.Message):
     r"""The response message for discovering supported languages.
 
     Attributes:
-        languages (Sequence[google.cloud.translate_v3.types.SupportedLanguage]):
+        languages (MutableSequence[google.cloud.translate_v3.types.SupportedLanguage]):
             A list of supported language responses. This
             list contains an entry for each language the
             Translation API supports.
     """
 
-    languages = proto.RepeatedField(
+    languages: MutableSequence["SupportedLanguage"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="SupportedLanguage",
     )
 
 
 class SupportedLanguage(proto.Message):
@@ -487,42 +489,42 @@
             request.
         support_source (bool):
             Can be used as source language.
         support_target (bool):
             Can be used as target language.
     """
 
-    language_code = proto.Field(
+    language_code: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    display_name = proto.Field(
+    display_name: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    support_source = proto.Field(
+    support_source: bool = proto.Field(
         proto.BOOL,
         number=3,
     )
-    support_target = proto.Field(
+    support_target: bool = proto.Field(
         proto.BOOL,
         number=4,
     )
 
 
 class GcsSource(proto.Message):
     r"""The Google Cloud Storage location for the input content.
 
     Attributes:
         input_uri (str):
             Required. Source data URI. For example,
             ``gs://my_bucket/my_object``.
     """
 
-    input_uri = proto.Field(
+    input_uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class InputConfig(proto.Message):
     r"""Input configuration for BatchTranslateText request.
@@ -555,19 +557,19 @@
 
             The other supported file extensions are ``.txt`` or
             ``.html``, which is treated as a single large chunk of text.
 
             This field is a member of `oneof`_ ``source``.
     """
 
-    mime_type = proto.Field(
+    mime_type: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    gcs_source = proto.Field(
+    gcs_source: "GcsSource" = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="source",
         message="GcsSource",
     )
 
 
@@ -580,15 +582,15 @@
             and there must be no files under 'output_uri_prefix'.
             'output_uri_prefix' must end with "/" and start with
             "gs://". One 'output_uri_prefix' can only be used by one
             batch translation job at a time. Otherwise an
             INVALID_ARGUMENT (400) error is returned.
     """
 
-    output_uri_prefix = proto.Field(
+    output_uri_prefix: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class OutputConfig(proto.Message):
     r"""Output configuration for BatchTranslateText request.
@@ -635,15 +637,15 @@
             Since index.csv will be keeping updated during the process,
             please make sure there is no custom retention policy applied
             on the output bucket that may avoid file updating.
             (https://cloud.google.com/storage/docs/bucket-lock?hl=en#retention-policy)
 
             The format of translations_file (for target language code
             'trg') is:
-            gs://translation_test/a_b_c\_'trg'_translations.[extension]
+            ``gs://translation_test/a_b_c\_'trg'_translations.[extension]``
 
             If the input file extension is tsv, the output has the
             following columns: Column 1: ID of the request provided in
             the input, if it's not provided in the input, then the input
             row number is used (0-based). Column 2: source sentence.
             Column 3: translation without applying a glossary. Empty
             string if there is an error. Column 4 (only present if a
@@ -673,15 +675,15 @@
             glossary_error_file will be generated that contains error
             details. glossary_error_file has format of
             gs://translation_test/a_b_c\_'trg'_glossary_errors.[extension]
 
             This field is a member of `oneof`_ ``destination``.
     """
 
-    gcs_destination = proto.Field(
+    gcs_destination: "GcsDestination" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="destination",
         message="GcsDestination",
     )
 
 
@@ -716,26 +718,26 @@
 
             -  application/pdf
             -  application/vnd.openxmlformats-officedocument.wordprocessingml.document
             -  application/vnd.openxmlformats-officedocument.presentationml.presentation
             -  application/vnd.openxmlformats-officedocument.spreadsheetml.sheet
     """
 
-    content = proto.Field(
+    content: bytes = proto.Field(
         proto.BYTES,
         number=1,
         oneof="source",
     )
-    gcs_source = proto.Field(
+    gcs_source: "GcsSource" = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="source",
         message="GcsSource",
     )
-    mime_type = proto.Field(
+    mime_type: str = proto.Field(
         proto.STRING,
         number=4,
     )
 
 
 class DocumentOutputConfig(proto.Message):
     r"""A document translation request output config.
@@ -803,21 +805,21 @@
 
             -  application/pdf
             -  application/vnd.openxmlformats-officedocument.wordprocessingml.document
             -  application/vnd.openxmlformats-officedocument.presentationml.presentation
             -  application/vnd.openxmlformats-officedocument.spreadsheetml.sheet
     """
 
-    gcs_destination = proto.Field(
+    gcs_destination: "GcsDestination" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="destination",
         message="GcsDestination",
     )
-    mime_type = proto.Field(
+    mime_type: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class TranslateDocumentRequest(proto.Message):
     r"""A document translation request.
@@ -877,71 +879,71 @@
             If not provided, the default Google model (NMT) will be used
             for translation.
         glossary_config (google.cloud.translate_v3.types.TranslateTextGlossaryConfig):
             Optional. Glossary to be applied. The glossary must be
             within the same region (have the same location-id) as the
             model, otherwise an INVALID_ARGUMENT (400) error is
             returned.
-        labels (Mapping[str, str]):
+        labels (MutableMapping[str, str]):
             Optional. The labels with user-defined
             metadata for the request.
             Label keys and values can be no longer than 63
             characters (Unicode codepoints), can only
             contain lowercase letters, numeric characters,
             underscores and dashes. International characters
             are allowed. Label values are optional. Label
             keys must start with a letter.
             See
             https://cloud.google.com/translate/docs/advanced/labels
             for more information.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    source_language_code = proto.Field(
+    source_language_code: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    target_language_code = proto.Field(
+    target_language_code: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    document_input_config = proto.Field(
+    document_input_config: "DocumentInputConfig" = proto.Field(
         proto.MESSAGE,
         number=4,
         message="DocumentInputConfig",
     )
-    document_output_config = proto.Field(
+    document_output_config: "DocumentOutputConfig" = proto.Field(
         proto.MESSAGE,
         number=5,
         message="DocumentOutputConfig",
     )
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=6,
     )
-    glossary_config = proto.Field(
+    glossary_config: "TranslateTextGlossaryConfig" = proto.Field(
         proto.MESSAGE,
         number=7,
         message="TranslateTextGlossaryConfig",
     )
-    labels = proto.MapField(
+    labels: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=8,
     )
 
 
 class DocumentTranslation(proto.Message):
     r"""A translated document message.
 
     Attributes:
-        byte_stream_outputs (Sequence[bytes]):
+        byte_stream_outputs (MutableSequence[bytes]):
             The array of translated documents. It is
             expected to be size 1 for now. We may produce
             multiple translated documents in the future for
             other type of file formats.
         mime_type (str):
             The translated document's mime type.
         detected_language_code (str):
@@ -950,23 +952,23 @@
             for the input document, this field will have the
             language code automatically detected. If the
             source language was passed, auto-detection of
             the language does not occur and this field is
             empty.
     """
 
-    byte_stream_outputs = proto.RepeatedField(
+    byte_stream_outputs: MutableSequence[bytes] = proto.RepeatedField(
         proto.BYTES,
         number=1,
     )
-    mime_type = proto.Field(
+    mime_type: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    detected_language_code = proto.Field(
+    detected_language_code: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class TranslateDocumentResponse(proto.Message):
     r"""A translated document response message.
@@ -988,29 +990,29 @@
             ``projects/{project-id}/locations/{location-id}/models/general/nmt``
             then ``model`` here would be normalized to
             ``projects/{project-number}/locations/{location-id}/models/general/nmt``.
         glossary_config (google.cloud.translate_v3.types.TranslateTextGlossaryConfig):
             The ``glossary_config`` used for this translation.
     """
 
-    document_translation = proto.Field(
+    document_translation: "DocumentTranslation" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="DocumentTranslation",
     )
-    glossary_document_translation = proto.Field(
+    glossary_document_translation: "DocumentTranslation" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="DocumentTranslation",
     )
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    glossary_config = proto.Field(
+    glossary_config: "TranslateTextGlossaryConfig" = proto.Field(
         proto.MESSAGE,
         number=4,
         message="TranslateTextGlossaryConfig",
     )
 
 
 class BatchTranslateTextRequest(proto.Message):
@@ -1028,94 +1030,94 @@
             translation.
 
             Only AutoML Translation models or glossaries within the same
             region (have the same location-id) can be used, otherwise an
             INVALID_ARGUMENT (400) error is returned.
         source_language_code (str):
             Required. Source language code.
-        target_language_codes (Sequence[str]):
+        target_language_codes (MutableSequence[str]):
             Required. Specify up to 10 language codes
             here.
-        models (Mapping[str, str]):
+        models (MutableMapping[str, str]):
             Optional. The models to use for translation. Map's key is
             target language code. Map's value is model name. Value can
             be a built-in general model, or an AutoML Translation model.
 
             The value format depends on model type:
 
             -  AutoML Translation models:
                ``projects/{project-number-or-id}/locations/{location-id}/models/{model-id}``
 
             -  General (built-in) models:
                ``projects/{project-number-or-id}/locations/{location-id}/models/general/nmt``,
 
             If the map is empty or a specific model is not requested for
             a language pair, then default google model (nmt) is used.
-        input_configs (Sequence[google.cloud.translate_v3.types.InputConfig]):
+        input_configs (MutableSequence[google.cloud.translate_v3.types.InputConfig]):
             Required. Input configurations.
             The total number of files matched should be <=
             100. The total content size should be <= 100M
             Unicode codepoints. The files must use UTF-8
             encoding.
         output_config (google.cloud.translate_v3.types.OutputConfig):
             Required. Output configuration.
             If 2 input configs match to the same file (that
             is, same input path), we don't generate output
             for duplicate inputs.
-        glossaries (Mapping[str, google.cloud.translate_v3.types.TranslateTextGlossaryConfig]):
+        glossaries (MutableMapping[str, google.cloud.translate_v3.types.TranslateTextGlossaryConfig]):
             Optional. Glossaries to be applied for
             translation. It's keyed by target language code.
-        labels (Mapping[str, str]):
+        labels (MutableMapping[str, str]):
             Optional. The labels with user-defined
             metadata for the request.
             Label keys and values can be no longer than 63
             characters (Unicode codepoints), can only
             contain lowercase letters, numeric characters,
             underscores and dashes. International characters
             are allowed. Label values are optional. Label
             keys must start with a letter.
             See
             https://cloud.google.com/translate/docs/advanced/labels
             for more information.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    source_language_code = proto.Field(
+    source_language_code: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    target_language_codes = proto.RepeatedField(
+    target_language_codes: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=3,
     )
-    models = proto.MapField(
+    models: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=4,
     )
-    input_configs = proto.RepeatedField(
+    input_configs: MutableSequence["InputConfig"] = proto.RepeatedField(
         proto.MESSAGE,
         number=5,
         message="InputConfig",
     )
-    output_config = proto.Field(
+    output_config: "OutputConfig" = proto.Field(
         proto.MESSAGE,
         number=6,
         message="OutputConfig",
     )
-    glossaries = proto.MapField(
+    glossaries: MutableMapping[str, "TranslateTextGlossaryConfig"] = proto.MapField(
         proto.STRING,
         proto.MESSAGE,
         number=7,
         message="TranslateTextGlossaryConfig",
     )
-    labels = proto.MapField(
+    labels: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=9,
     )
 
 
 class BatchTranslateMetadata(proto.Message):
@@ -1145,32 +1147,32 @@
         STATE_UNSPECIFIED = 0
         RUNNING = 1
         SUCCEEDED = 2
         FAILED = 3
         CANCELLING = 4
         CANCELLED = 5
 
-    state = proto.Field(
+    state: State = proto.Field(
         proto.ENUM,
         number=1,
         enum=State,
     )
-    translated_characters = proto.Field(
+    translated_characters: int = proto.Field(
         proto.INT64,
         number=2,
     )
-    failed_characters = proto.Field(
+    failed_characters: int = proto.Field(
         proto.INT64,
         number=3,
     )
-    total_characters = proto.Field(
+    total_characters: int = proto.Field(
         proto.INT64,
         number=4,
     )
-    submit_time = proto.Field(
+    submit_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=5,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class BatchTranslateResponse(proto.Message):
@@ -1193,32 +1195,32 @@
             Time when the operation was submitted.
         end_time (google.protobuf.timestamp_pb2.Timestamp):
             The time when the operation is finished and
             [google.longrunning.Operation.done][google.longrunning.Operation.done]
             is set to true.
     """
 
-    total_characters = proto.Field(
+    total_characters: int = proto.Field(
         proto.INT64,
         number=1,
     )
-    translated_characters = proto.Field(
+    translated_characters: int = proto.Field(
         proto.INT64,
         number=2,
     )
-    failed_characters = proto.Field(
+    failed_characters: int = proto.Field(
         proto.INT64,
         number=3,
     )
-    submit_time = proto.Field(
+    submit_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=4,
         message=timestamp_pb2.Timestamp,
     )
-    end_time = proto.Field(
+    end_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=5,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class GlossaryInputConfig(proto.Message):
@@ -1252,15 +1254,15 @@
                glossary terms in multiple languages. See documentation
                for more information -
                `glossaries <https://cloud.google.com/translate/docs/advanced/glossary>`__.
 
             This field is a member of `oneof`_ ``source``.
     """
 
-    gcs_source = proto.Field(
+    gcs_source: "GcsSource" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="source",
         message="GcsSource",
     )
 
 
@@ -1311,70 +1313,70 @@
                 GlossaryTerm.language_code.
             target_language_code (str):
                 Required. The BCP-47 language code for translation output,
                 for example, "zh-CN". Expected to be an exact match for
                 GlossaryTerm.language_code.
         """
 
-        source_language_code = proto.Field(
+        source_language_code: str = proto.Field(
             proto.STRING,
             number=1,
         )
-        target_language_code = proto.Field(
+        target_language_code: str = proto.Field(
             proto.STRING,
             number=2,
         )
 
     class LanguageCodesSet(proto.Message):
         r"""Used with equivalent term set glossaries.
 
         Attributes:
-            language_codes (Sequence[str]):
+            language_codes (MutableSequence[str]):
                 The BCP-47 language code(s) for terms defined in the
                 glossary. All entries are unique. The list contains at least
                 two entries. Expected to be an exact match for
                 GlossaryTerm.language_code.
         """
 
-        language_codes = proto.RepeatedField(
+        language_codes: MutableSequence[str] = proto.RepeatedField(
             proto.STRING,
             number=1,
         )
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    language_pair = proto.Field(
+    language_pair: LanguageCodePair = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="languages",
         message=LanguageCodePair,
     )
-    language_codes_set = proto.Field(
+    language_codes_set: LanguageCodesSet = proto.Field(
         proto.MESSAGE,
         number=4,
         oneof="languages",
         message=LanguageCodesSet,
     )
-    input_config = proto.Field(
+    input_config: "GlossaryInputConfig" = proto.Field(
         proto.MESSAGE,
         number=5,
         message="GlossaryInputConfig",
     )
-    entry_count = proto.Field(
+    entry_count: int = proto.Field(
         proto.INT32,
         number=6,
     )
-    submit_time = proto.Field(
+    submit_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=7,
         message=timestamp_pb2.Timestamp,
     )
-    end_time = proto.Field(
+    end_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=8,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class CreateGlossaryRequest(proto.Message):
@@ -1383,19 +1385,19 @@
     Attributes:
         parent (str):
             Required. The project name.
         glossary (google.cloud.translate_v3.types.Glossary):
             Required. The glossary to create.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    glossary = proto.Field(
+    glossary: "Glossary" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="Glossary",
     )
 
 
 class GetGlossaryRequest(proto.Message):
@@ -1403,29 +1405,29 @@
 
     Attributes:
         name (str):
             Required. The name of the glossary to
             retrieve.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class DeleteGlossaryRequest(proto.Message):
     r"""Request message for DeleteGlossary.
 
     Attributes:
         name (str):
             Required. The name of the glossary to delete.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ListGlossariesRequest(proto.Message):
     r"""Request message for ListGlossaries.
@@ -1468,55 +1470,55 @@
             the target language code "zh-CN", but all
             equivalent term set glossaries which contain
             "en-US" and "zh-CN" in their language set will
             be picked. If missing, no filtering is
             performed.
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
 
 
 class ListGlossariesResponse(proto.Message):
     r"""Response message for ListGlossaries.
 
     Attributes:
-        glossaries (Sequence[google.cloud.translate_v3.types.Glossary]):
+        glossaries (MutableSequence[google.cloud.translate_v3.types.Glossary]):
             The list of glossaries for a project.
         next_page_token (str):
             A token to retrieve a page of results. Pass this value in
             the [ListGlossariesRequest.page_token] field in the
             subsequent call to ``ListGlossaries`` method to retrieve the
             next page of results.
     """
 
     @property
     def raw_page(self):
         return self
 
-    glossaries = proto.RepeatedField(
+    glossaries: MutableSequence["Glossary"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="Glossary",
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class CreateGlossaryMetadata(proto.Message):
     r"""Stored in the
@@ -1542,24 +1544,24 @@
         STATE_UNSPECIFIED = 0
         RUNNING = 1
         SUCCEEDED = 2
         FAILED = 3
         CANCELLING = 4
         CANCELLED = 5
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    state = proto.Field(
+    state: State = proto.Field(
         proto.ENUM,
         number=2,
         enum=State,
     )
-    submit_time = proto.Field(
+    submit_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=3,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class DeleteGlossaryMetadata(proto.Message):
@@ -1586,24 +1588,24 @@
         STATE_UNSPECIFIED = 0
         RUNNING = 1
         SUCCEEDED = 2
         FAILED = 3
         CANCELLING = 4
         CANCELLED = 5
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    state = proto.Field(
+    state: State = proto.Field(
         proto.ENUM,
         number=2,
         enum=State,
     )
-    submit_time = proto.Field(
+    submit_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=3,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class DeleteGlossaryResponse(proto.Message):
@@ -1619,24 +1621,24 @@
             the server.
         end_time (google.protobuf.timestamp_pb2.Timestamp):
             The time when the glossary deletion is finished and
             [google.longrunning.Operation.done][google.longrunning.Operation.done]
             is set to true.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    submit_time = proto.Field(
+    submit_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=2,
         message=timestamp_pb2.Timestamp,
     )
-    end_time = proto.Field(
+    end_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=3,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class BatchTranslateDocumentRequest(proto.Message):
@@ -1657,30 +1659,30 @@
             INVALID_ARGUMENT (400) error is returned.
         source_language_code (str):
             Required. The BCP-47 language code of the
             input document if known, for example, "en-US" or
             "sr-Latn". Supported language codes are listed
             in Language Support
             (https://cloud.google.com/translate/docs/languages).
-        target_language_codes (Sequence[str]):
+        target_language_codes (MutableSequence[str]):
             Required. The BCP-47 language code to use for
             translation of the input document. Specify up to
             10 language codes here.
-        input_configs (Sequence[google.cloud.translate_v3.types.BatchDocumentInputConfig]):
+        input_configs (MutableSequence[google.cloud.translate_v3.types.BatchDocumentInputConfig]):
             Required. Input configurations.
             The total number of files matched should be <=
             100. The total content size to translate should
             be <= 100M Unicode codepoints. The files must
             use UTF-8 encoding.
         output_config (google.cloud.translate_v3.types.BatchDocumentOutputConfig):
             Required. Output configuration.
             If 2 input configs match to the same file (that
             is, same input path), we don't generate output
             for duplicate inputs.
-        models (Mapping[str, str]):
+        models (MutableMapping[str, str]):
             Optional. The models to use for translation. Map's key is
             target language code. Map's value is the model name. Value
             can be a built-in general model, or an AutoML Translation
             model.
 
             The value format depends on model type:
 
@@ -1688,65 +1690,65 @@
                ``projects/{project-number-or-id}/locations/{location-id}/models/{model-id}``
 
             -  General (built-in) models:
                ``projects/{project-number-or-id}/locations/{location-id}/models/general/nmt``,
 
             If the map is empty or a specific model is not requested for
             a language pair, then default google model (nmt) is used.
-        glossaries (Mapping[str, google.cloud.translate_v3.types.TranslateTextGlossaryConfig]):
+        glossaries (MutableMapping[str, google.cloud.translate_v3.types.TranslateTextGlossaryConfig]):
             Optional. Glossaries to be applied. It's
             keyed by target language code.
-        format_conversions (Mapping[str, str]):
+        format_conversions (MutableMapping[str, str]):
             Optional. File format conversion map to be applied to all
             input files. Map's key is the original mime_type. Map's
             value is the target mime_type of translated documents.
 
             Supported file format conversion includes:
 
             -  ``application/pdf`` to
                ``application/vnd.openxmlformats-officedocument.wordprocessingml.document``
 
             If nothing specified, output files will be in the same
             format as the original file.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    source_language_code = proto.Field(
+    source_language_code: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    target_language_codes = proto.RepeatedField(
+    target_language_codes: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=3,
     )
-    input_configs = proto.RepeatedField(
+    input_configs: MutableSequence["BatchDocumentInputConfig"] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message="BatchDocumentInputConfig",
     )
-    output_config = proto.Field(
+    output_config: "BatchDocumentOutputConfig" = proto.Field(
         proto.MESSAGE,
         number=5,
         message="BatchDocumentOutputConfig",
     )
-    models = proto.MapField(
+    models: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=6,
     )
-    glossaries = proto.MapField(
+    glossaries: MutableMapping[str, "TranslateTextGlossaryConfig"] = proto.MapField(
         proto.STRING,
         proto.MESSAGE,
         number=7,
         message="TranslateTextGlossaryConfig",
     )
-    format_conversions = proto.MapField(
+    format_conversions: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=8,
     )
 
 
 class BatchDocumentInputConfig(proto.Message):
@@ -1776,15 +1778,15 @@
             ``.xlsx`` is 100MB. The max file size to support for
             ``.pdf`` is 1GB and the max page limit is 1000 pages. The
             max file size to support for all input documents is 1GB.
 
             This field is a member of `oneof`_ ``source``.
     """
 
-    gcs_source = proto.Field(
+    gcs_source: "GcsSource" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="source",
         message="GcsSource",
     )
 
 
@@ -1847,15 +1849,15 @@
             ``glossary_error_output``:
             gs://translation_test/a_b_c*\ [trg]_glossary_translation.txt
             The error output is a txt file containing error details.
 
             This field is a member of `oneof`_ ``destination``.
     """
 
-    gcs_destination = proto.Field(
+    gcs_destination: "GcsDestination" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="destination",
         message="GcsDestination",
     )
 
 
@@ -1898,52 +1900,52 @@
             Time when the operation was submitted.
         end_time (google.protobuf.timestamp_pb2.Timestamp):
             The time when the operation is finished and
             [google.longrunning.Operation.done][google.longrunning.Operation.done]
             is set to true.
     """
 
-    total_pages = proto.Field(
+    total_pages: int = proto.Field(
         proto.INT64,
         number=1,
     )
-    translated_pages = proto.Field(
+    translated_pages: int = proto.Field(
         proto.INT64,
         number=2,
     )
-    failed_pages = proto.Field(
+    failed_pages: int = proto.Field(
         proto.INT64,
         number=3,
     )
-    total_billable_pages = proto.Field(
+    total_billable_pages: int = proto.Field(
         proto.INT64,
         number=4,
     )
-    total_characters = proto.Field(
+    total_characters: int = proto.Field(
         proto.INT64,
         number=5,
     )
-    translated_characters = proto.Field(
+    translated_characters: int = proto.Field(
         proto.INT64,
         number=6,
     )
-    failed_characters = proto.Field(
+    failed_characters: int = proto.Field(
         proto.INT64,
         number=7,
     )
-    total_billable_characters = proto.Field(
+    total_billable_characters: int = proto.Field(
         proto.INT64,
         number=8,
     )
-    submit_time = proto.Field(
+    submit_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=9,
         message=timestamp_pb2.Timestamp,
     )
-    end_time = proto.Field(
+    end_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=10,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class BatchTranslateDocumentMetadata(proto.Message):
@@ -1991,52 +1993,52 @@
         STATE_UNSPECIFIED = 0
         RUNNING = 1
         SUCCEEDED = 2
         FAILED = 3
         CANCELLING = 4
         CANCELLED = 5
 
-    state = proto.Field(
+    state: State = proto.Field(
         proto.ENUM,
         number=1,
         enum=State,
     )
-    total_pages = proto.Field(
+    total_pages: int = proto.Field(
         proto.INT64,
         number=2,
     )
-    translated_pages = proto.Field(
+    translated_pages: int = proto.Field(
         proto.INT64,
         number=3,
     )
-    failed_pages = proto.Field(
+    failed_pages: int = proto.Field(
         proto.INT64,
         number=4,
     )
-    total_billable_pages = proto.Field(
+    total_billable_pages: int = proto.Field(
         proto.INT64,
         number=5,
     )
-    total_characters = proto.Field(
+    total_characters: int = proto.Field(
         proto.INT64,
         number=6,
     )
-    translated_characters = proto.Field(
+    translated_characters: int = proto.Field(
         proto.INT64,
         number=7,
     )
-    failed_characters = proto.Field(
+    failed_characters: int = proto.Field(
         proto.INT64,
         number=8,
     )
-    total_billable_characters = proto.Field(
+    total_billable_characters: int = proto.Field(
         proto.INT64,
         number=9,
     )
-    submit_time = proto.Field(
+    submit_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=10,
         message=timestamp_pb2.Timestamp,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/__init__.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.translate import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from .services.translation_service import TranslationServiceClient
 from .services.translation_service import TranslationServiceAsyncClient
 
 from .types.translation_service import BatchDocumentInputConfig
 from .types.translation_service import BatchDocumentOutputConfig
 from .types.translation_service import BatchTranslateDocumentMetadata
```

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/gapic_metadata.json` & `google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/services/__init__.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/services/translation_service/__init__.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/services/translation_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/services/translation_service/async_client.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/services/translation_service/async_client.py`

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
+from google.cloud.translate_v3beta1 import gapic_version as package_version
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
@@ -158,17 +169,17 @@
         type(TranslationServiceClient).get_transport_class,
         type(TranslationServiceClient),
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, TranslationServiceTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the translation service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -204,18 +215,18 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def translate_text(
         self,
-        request: Union[translation_service.TranslateTextRequest, dict] = None,
+        request: Optional[Union[translation_service.TranslateTextRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> translation_service.TranslateTextResponse:
         r"""Translates input text and returns translated text.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -241,15 +252,15 @@
                 # Make the request
                 response = await client.translate_text(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.translate_v3beta1.types.TranslateTextRequest, dict]):
+            request (Optional[Union[google.cloud.translate_v3beta1.types.TranslateTextRequest, dict]]):
                 The request object. The request message for synchronous
                 translation.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
@@ -284,21 +295,23 @@
         )
 
         # Done; return the response.
         return response
 
     async def detect_language(
         self,
-        request: Union[translation_service.DetectLanguageRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.DetectLanguageRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        model: str = None,
-        mime_type: str = None,
+        parent: Optional[str] = None,
+        model: Optional[str] = None,
+        mime_type: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> translation_service.DetectLanguageResponse:
         r"""Detects the language of text within a request.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -323,15 +336,15 @@
                 # Make the request
                 response = await client.detect_language(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.translate_v3beta1.types.DetectLanguageRequest, dict]):
+            request (Optional[Union[google.cloud.translate_v3beta1.types.DetectLanguageRequest, dict]]):
                 The request object. The request message for language
                 detection.
             parent (:class:`str`):
                 Required. Project or location to make a call. Must refer
                 to a caller's project.
 
                 Format:
@@ -429,21 +442,23 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_supported_languages(
         self,
-        request: Union[translation_service.GetSupportedLanguagesRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.GetSupportedLanguagesRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        display_language_code: str = None,
-        model: str = None,
+        parent: Optional[str] = None,
+        display_language_code: Optional[str] = None,
+        model: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> translation_service.SupportedLanguages:
         r"""Returns a list of supported languages for
         translation.
 
         .. code-block:: python
 
@@ -468,15 +483,15 @@
                 # Make the request
                 response = await client.get_supported_languages(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.translate_v3beta1.types.GetSupportedLanguagesRequest, dict]):
+            request (Optional[Union[google.cloud.translate_v3beta1.types.GetSupportedLanguagesRequest, dict]]):
                 The request object. The request message for discovering
                 supported languages.
             parent (:class:`str`):
                 Required. Project or location to make a call. Must refer
                 to a caller's project.
 
                 Format: ``projects/{project-number-or-id}`` or
@@ -589,18 +604,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def translate_document(
         self,
-        request: Union[translation_service.TranslateDocumentRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.TranslateDocumentRequest, dict]
+        ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> translation_service.TranslateDocumentResponse:
         r"""Translates documents in synchronous mode.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -629,15 +646,15 @@
                 # Make the request
                 response = await client.translate_document(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.translate_v3beta1.types.TranslateDocumentRequest, dict]):
+            request (Optional[Union[google.cloud.translate_v3beta1.types.TranslateDocumentRequest, dict]]):
                 The request object. A document translation request.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
@@ -673,18 +690,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def batch_translate_text(
         self,
-        request: Union[translation_service.BatchTranslateTextRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.BatchTranslateTextRequest, dict]
+        ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Translates a large volume of text in asynchronous
         batch mode. This function provides real-time output as
         the inputs are being processed. If caller cancels a
         request, the partial results (for an input file, it's
         all or nothing) may still be available on the specified
@@ -724,21 +743,21 @@
                 )
 
                 # Make the request
                 operation = client.batch_translate_text(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.translate_v3beta1.types.BatchTranslateTextRequest, dict]):
+            request (Optional[Union[google.cloud.translate_v3beta1.types.BatchTranslateTextRequest, dict]]):
                 The request object. The batch translation request.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
@@ -786,23 +805,27 @@
         )
 
         # Done; return the response.
         return response
 
     async def batch_translate_document(
         self,
-        request: Union[translation_service.BatchTranslateDocumentRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.BatchTranslateDocumentRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        source_language_code: str = None,
-        target_language_codes: Sequence[str] = None,
-        input_configs: Sequence[translation_service.BatchDocumentInputConfig] = None,
-        output_config: translation_service.BatchDocumentOutputConfig = None,
+        parent: Optional[str] = None,
+        source_language_code: Optional[str] = None,
+        target_language_codes: Optional[MutableSequence[str]] = None,
+        input_configs: Optional[
+            MutableSequence[translation_service.BatchDocumentInputConfig]
+        ] = None,
+        output_config: Optional[translation_service.BatchDocumentOutputConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Translates a large volume of documents in
         asynchronous batch mode. This function provides
         real-time output as the inputs are being processed. If
         caller cancels a request, the partial results (for an
         input file, it's all or nothing) may still be available
@@ -842,21 +865,21 @@
                 )
 
                 # Make the request
                 operation = client.batch_translate_document(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.translate_v3beta1.types.BatchTranslateDocumentRequest, dict]):
+            request (Optional[Union[google.cloud.translate_v3beta1.types.BatchTranslateDocumentRequest, dict]]):
                 The request object. The BatchTranslateDocument request.
             parent (:class:`str`):
                 Required. Location to make a regional call.
 
                 Format:
                 ``projects/{project-number-or-id}/locations/{location-id}``.
 
@@ -877,24 +900,24 @@
                 language codes are listed in Language
                 Support
                 (https://cloud.google.com/translate/docs/languages).
 
                 This corresponds to the ``source_language_code`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            target_language_codes (:class:`Sequence[str]`):
+            target_language_codes (:class:`MutableSequence[str]`):
                 Required. The BCP-47 language code to
                 use for translation of the input
                 document. Specify up to 10 language
                 codes here.
 
                 This corresponds to the ``target_language_codes`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            input_configs (:class:`Sequence[google.cloud.translate_v3beta1.types.BatchDocumentInputConfig]`):
+            input_configs (:class:`MutableSequence[google.cloud.translate_v3beta1.types.BatchDocumentInputConfig]`):
                 Required. Input configurations.
                 The total number of files matched should
                 be <= 100. The total content size to
                 translate should be <= 100M Unicode
                 codepoints. The files must use UTF-8
                 encoding.
 
@@ -991,20 +1014,22 @@
         )
 
         # Done; return the response.
         return response
 
     async def create_glossary(
         self,
-        request: Union[translation_service.CreateGlossaryRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.CreateGlossaryRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        glossary: translation_service.Glossary = None,
+        parent: Optional[str] = None,
+        glossary: Optional[translation_service.Glossary] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Creates a glossary and returns the long-running operation.
         Returns NOT_FOUND, if the project doesn't exist.
 
         .. code-block:: python
 
@@ -1031,21 +1056,21 @@
                 )
 
                 # Make the request
                 operation = client.create_glossary(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.translate_v3beta1.types.CreateGlossaryRequest, dict]):
+            request (Optional[Union[google.cloud.translate_v3beta1.types.CreateGlossaryRequest, dict]]):
                 The request object. Request message for CreateGlossary.
             parent (:class:`str`):
                 Required. The project name.
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             glossary (:class:`google.cloud.translate_v3beta1.types.Glossary`):
@@ -1118,20 +1143,22 @@
         )
 
         # Done; return the response.
         return response
 
     async def list_glossaries(
         self,
-        request: Union[translation_service.ListGlossariesRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.ListGlossariesRequest, dict]
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
     ) -> pagers.ListGlossariesAsyncPager:
         r"""Lists glossaries in a project. Returns NOT_FOUND, if the project
         doesn't exist.
 
         .. code-block:: python
 
@@ -1157,15 +1184,15 @@
                 page_result = client.list_glossaries(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.translate_v3beta1.types.ListGlossariesRequest, dict]):
+            request (Optional[Union[google.cloud.translate_v3beta1.types.ListGlossariesRequest, dict]]):
                 The request object. Request message for ListGlossaries.
             parent (:class:`str`):
                 Required. The name of the project
                 from which to list all of the
                 glossaries.
 
                 This corresponds to the ``parent`` field
@@ -1280,19 +1307,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_glossary(
         self,
-        request: Union[translation_service.GetGlossaryRequest, dict] = None,
+        request: Optional[Union[translation_service.GetGlossaryRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> translation_service.Glossary:
         r"""Gets a glossary. Returns NOT_FOUND, if the glossary doesn't
         exist.
 
         .. code-block:: python
 
@@ -1317,15 +1344,15 @@
                 # Make the request
                 response = await client.get_glossary(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.translate_v3beta1.types.GetGlossaryRequest, dict]):
+            request (Optional[Union[google.cloud.translate_v3beta1.types.GetGlossaryRequest, dict]]):
                 The request object. Request message for GetGlossary.
             name (:class:`str`):
                 Required. The name of the glossary to
                 retrieve.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1392,19 +1419,21 @@
         )
 
         # Done; return the response.
         return response
 
     async def delete_glossary(
         self,
-        request: Union[translation_service.DeleteGlossaryRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.DeleteGlossaryRequest, dict]
+        ] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Deletes a glossary, or cancels glossary construction if the
         glossary isn't created yet. Returns NOT_FOUND, if the glossary
         doesn't exist.
 
         .. code-block:: python
@@ -1428,21 +1457,21 @@
                 )
 
                 # Make the request
                 operation = client.delete_glossary(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.translate_v3beta1.types.DeleteGlossaryRequest, dict]):
+            request (Optional[Union[google.cloud.translate_v3beta1.types.DeleteGlossaryRequest, dict]]):
                 The request object. Request message for DeleteGlossary.
             name (:class:`str`):
                 Required. The name of the glossary to
                 delete.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1525,18 +1554,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-translate",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("TranslationServiceAsyncClient",)
```

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/services/translation_service/client.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/services/translation_service/client.py`

 * *Files 9% similar despite different names*

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
+from google.cloud.translate_v3beta1 import gapic_version as package_version
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport import mtls  # type: ignore
@@ -56,15 +68,15 @@
         OrderedDict()
     )  # type: Dict[str, Type[TranslationServiceTransport]]
     _transport_registry["grpc"] = TranslationServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = TranslationServiceGrpcAsyncIOTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[TranslationServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -331,30 +343,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, TranslationServiceTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, TranslationServiceTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the translation service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, TranslationServiceTransport]): The
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
@@ -376,14 +388,15 @@
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
@@ -428,18 +441,18 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def translate_text(
         self,
-        request: Union[translation_service.TranslateTextRequest, dict] = None,
+        request: Optional[Union[translation_service.TranslateTextRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> translation_service.TranslateTextResponse:
         r"""Translates input text and returns translated text.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -509,21 +522,23 @@
         )
 
         # Done; return the response.
         return response
 
     def detect_language(
         self,
-        request: Union[translation_service.DetectLanguageRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.DetectLanguageRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        model: str = None,
-        mime_type: str = None,
+        parent: Optional[str] = None,
+        model: Optional[str] = None,
+        mime_type: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> translation_service.DetectLanguageResponse:
         r"""Detects the language of text within a request.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -654,21 +669,23 @@
         )
 
         # Done; return the response.
         return response
 
     def get_supported_languages(
         self,
-        request: Union[translation_service.GetSupportedLanguagesRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.GetSupportedLanguagesRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        display_language_code: str = None,
-        model: str = None,
+        parent: Optional[str] = None,
+        display_language_code: Optional[str] = None,
+        model: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> translation_service.SupportedLanguages:
         r"""Returns a list of supported languages for
         translation.
 
         .. code-block:: python
 
@@ -804,18 +821,20 @@
         )
 
         # Done; return the response.
         return response
 
     def translate_document(
         self,
-        request: Union[translation_service.TranslateDocumentRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.TranslateDocumentRequest, dict]
+        ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> translation_service.TranslateDocumentResponse:
         r"""Translates documents in synchronous mode.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -889,18 +908,20 @@
         )
 
         # Done; return the response.
         return response
 
     def batch_translate_text(
         self,
-        request: Union[translation_service.BatchTranslateTextRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.BatchTranslateTextRequest, dict]
+        ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Translates a large volume of text in asynchronous
         batch mode. This function provides real-time output as
         the inputs are being processed. If caller cancels a
         request, the partial results (for an input file, it's
         all or nothing) may still be available on the specified
@@ -1003,23 +1024,27 @@
         )
 
         # Done; return the response.
         return response
 
     def batch_translate_document(
         self,
-        request: Union[translation_service.BatchTranslateDocumentRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.BatchTranslateDocumentRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        source_language_code: str = None,
-        target_language_codes: Sequence[str] = None,
-        input_configs: Sequence[translation_service.BatchDocumentInputConfig] = None,
-        output_config: translation_service.BatchDocumentOutputConfig = None,
+        parent: Optional[str] = None,
+        source_language_code: Optional[str] = None,
+        target_language_codes: Optional[MutableSequence[str]] = None,
+        input_configs: Optional[
+            MutableSequence[translation_service.BatchDocumentInputConfig]
+        ] = None,
+        output_config: Optional[translation_service.BatchDocumentOutputConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Translates a large volume of documents in
         asynchronous batch mode. This function provides
         real-time output as the inputs are being processed. If
         caller cancels a request, the partial results (for an
         input file, it's all or nothing) may still be available
@@ -1094,24 +1119,24 @@
                 language codes are listed in Language
                 Support
                 (https://cloud.google.com/translate/docs/languages).
 
                 This corresponds to the ``source_language_code`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            target_language_codes (Sequence[str]):
+            target_language_codes (MutableSequence[str]):
                 Required. The BCP-47 language code to
                 use for translation of the input
                 document. Specify up to 10 language
                 codes here.
 
                 This corresponds to the ``target_language_codes`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            input_configs (Sequence[google.cloud.translate_v3beta1.types.BatchDocumentInputConfig]):
+            input_configs (MutableSequence[google.cloud.translate_v3beta1.types.BatchDocumentInputConfig]):
                 Required. Input configurations.
                 The total number of files matched should
                 be <= 100. The total content size to
                 translate should be <= 100M Unicode
                 codepoints. The files must use UTF-8
                 encoding.
 
@@ -1208,20 +1233,22 @@
         )
 
         # Done; return the response.
         return response
 
     def create_glossary(
         self,
-        request: Union[translation_service.CreateGlossaryRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.CreateGlossaryRequest, dict]
+        ] = None,
         *,
-        parent: str = None,
-        glossary: translation_service.Glossary = None,
+        parent: Optional[str] = None,
+        glossary: Optional[translation_service.Glossary] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Creates a glossary and returns the long-running operation.
         Returns NOT_FOUND, if the project doesn't exist.
 
         .. code-block:: python
 
@@ -1335,20 +1362,22 @@
         )
 
         # Done; return the response.
         return response
 
     def list_glossaries(
         self,
-        request: Union[translation_service.ListGlossariesRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.ListGlossariesRequest, dict]
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
     ) -> pagers.ListGlossariesPager:
         r"""Lists glossaries in a project. Returns NOT_FOUND, if the project
         doesn't exist.
 
         .. code-block:: python
 
@@ -1487,19 +1516,19 @@
         )
 
         # Done; return the response.
         return response
 
     def get_glossary(
         self,
-        request: Union[translation_service.GetGlossaryRequest, dict] = None,
+        request: Optional[Union[translation_service.GetGlossaryRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> translation_service.Glossary:
         r"""Gets a glossary. Returns NOT_FOUND, if the glossary doesn't
         exist.
 
         .. code-block:: python
 
@@ -1589,19 +1618,21 @@
         )
 
         # Done; return the response.
         return response
 
     def delete_glossary(
         self,
-        request: Union[translation_service.DeleteGlossaryRequest, dict] = None,
+        request: Optional[
+            Union[translation_service.DeleteGlossaryRequest, dict]
+        ] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Deletes a glossary, or cancels glossary construction if the
         glossary isn't created yet. Returns NOT_FOUND, if the glossary
         doesn't exist.
 
         .. code-block:: python
@@ -1719,18 +1750,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-translate",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("TranslationServiceClient",)
```

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/services/translation_service/pagers.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/services/translation_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/services/translation_service/transports/__init__.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/services/translation_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/services/translation_service/transports/base.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3/services/translation_service/transports/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,36 +11,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import abc
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Union
-import pkg_resources
+
+from google.cloud.translate_v3 import gapic_version as package_version
 
 import google.auth  # type: ignore
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core import operations_v1
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-from google.cloud.translate_v3beta1.types import translation_service
+from google.cloud.translate_v3.types import translation_service
 from google.longrunning import operations_pb2  # type: ignore
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-translate",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class TranslationServiceTransport(abc.ABC):
     """Abstract transport class for TranslationService."""
 
     AUTH_SCOPES = (
         "https://www.googleapis.com/auth/cloud-platform",
@@ -49,15 +45,15 @@
 
     DEFAULT_HOST: str = "translate.googleapis.com"
 
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

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/services/translation_service/transports/grpc.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/services/translation_service/transports/grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,22 +45,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "translate.googleapis.com",
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
 
@@ -180,16 +180,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "translate.googleapis.com",
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

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/services/translation_service/transports/grpc_asyncio.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/services/translation_service/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "translate.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -90,23 +90,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "translate.googleapis.com",
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

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/types/__init__.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/google/cloud/translate_v3beta1/types/translation_service.py` & `google-cloud-translate-3.9.0/google/cloud/translate_v3beta1/types/translation_service.py`

 * *Files 6% similar despite different names*

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
 
 from google.protobuf import timestamp_pb2  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.cloud.translation.v3beta1",
@@ -72,29 +74,29 @@
             Use this format: projects/\ */locations/*/glossaries/\*
         ignore_case (bool):
             Optional. Indicates match is
             case-insensitive. Default value is false if
             missing.
     """
 
-    glossary = proto.Field(
+    glossary: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    ignore_case = proto.Field(
+    ignore_case: bool = proto.Field(
         proto.BOOL,
         number=2,
     )
 
 
 class TranslateTextRequest(proto.Message):
     r"""The request message for synchronous translation.
 
     Attributes:
-        contents (Sequence[str]):
+        contents (MutableSequence[str]):
             Required. The content of the input in string
             format. We recommend the total content be less
             than 30k codepoints. The max length of this
             field is 1024.
             Use BatchTranslateText for larger text.
         mime_type (str):
             Optional. The format of the source text, for
@@ -146,86 +148,86 @@
 
             If not provided, the default Google model (NMT) will be used
         glossary_config (google.cloud.translate_v3beta1.types.TranslateTextGlossaryConfig):
             Optional. Glossary to be applied. The glossary must be
             within the same region (have the same location-id) as the
             model, otherwise an INVALID_ARGUMENT (400) error is
             returned.
-        labels (Mapping[str, str]):
+        labels (MutableMapping[str, str]):
             Optional. The labels with user-defined
             metadata for the request.
             Label keys and values can be no longer than 63
             characters (Unicode codepoints), can only
             contain lowercase letters, numeric characters,
             underscores and dashes. International characters
             are allowed. Label values are optional. Label
             keys must start with a letter.
             See
             https://cloud.google.com/translate/docs/labels
             for more information.
     """
 
-    contents = proto.RepeatedField(
+    contents: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=1,
     )
-    mime_type = proto.Field(
+    mime_type: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    source_language_code = proto.Field(
+    source_language_code: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    target_language_code = proto.Field(
+    target_language_code: str = proto.Field(
         proto.STRING,
         number=5,
     )
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=8,
     )
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=6,
     )
-    glossary_config = proto.Field(
+    glossary_config: "TranslateTextGlossaryConfig" = proto.Field(
         proto.MESSAGE,
         number=7,
         message="TranslateTextGlossaryConfig",
     )
-    labels = proto.MapField(
+    labels: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=10,
     )
 
 
 class TranslateTextResponse(proto.Message):
     r"""
 
     Attributes:
-        translations (Sequence[google.cloud.translate_v3beta1.types.Translation]):
+        translations (MutableSequence[google.cloud.translate_v3beta1.types.Translation]):
             Text translation responses with no glossary applied. This
             field has the same length as
             [``contents``][google.cloud.translation.v3beta1.TranslateTextRequest.contents].
-        glossary_translations (Sequence[google.cloud.translate_v3beta1.types.Translation]):
+        glossary_translations (MutableSequence[google.cloud.translate_v3beta1.types.Translation]):
             Text translation responses if a glossary is provided in the
             request. This can be the same as
             [``translations``][google.cloud.translation.v3beta1.TranslateTextResponse.translations]
             if no terms apply. This field has the same length as
             [``contents``][google.cloud.translation.v3beta1.TranslateTextRequest.contents].
     """
 
-    translations = proto.RepeatedField(
+    translations: MutableSequence["Translation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="Translation",
     )
-    glossary_translations = proto.RepeatedField(
+    glossary_translations: MutableSequence["Translation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="Translation",
     )
 
 
 class Translation(proto.Message):
@@ -252,27 +254,27 @@
             request. If the source language was passed,
             auto-detection of the language does not occur
             and this field is empty.
         glossary_config (google.cloud.translate_v3beta1.types.TranslateTextGlossaryConfig):
             The ``glossary_config`` used for this translation.
     """
 
-    translated_text = proto.Field(
+    translated_text: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    detected_language_code = proto.Field(
+    detected_language_code: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    glossary_config = proto.Field(
+    glossary_config: "TranslateTextGlossaryConfig" = proto.Field(
         proto.MESSAGE,
         number=3,
         message="TranslateTextGlossaryConfig",
     )
 
 
 class DetectLanguageRequest(proto.Message):
@@ -310,46 +312,46 @@
             The content of the input stored as a string.
 
             This field is a member of `oneof`_ ``source``.
         mime_type (str):
             Optional. The format of the source text, for
             example, "text/html", "text/plain". If left
             blank, the MIME type defaults to "text/html".
-        labels (Mapping[str, str]):
+        labels (MutableMapping[str, str]):
             Optional. The labels with user-defined
             metadata for the request.
             Label keys and values can be no longer than 63
             characters (Unicode codepoints), can only
             contain lowercase letters, numeric characters,
             underscores and dashes. International characters
             are allowed. Label values are optional. Label
             keys must start with a letter.
             See
             https://cloud.google.com/translate/docs/labels
             for more information.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=5,
     )
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    content = proto.Field(
+    content: str = proto.Field(
         proto.STRING,
         number=1,
         oneof="source",
     )
-    mime_type = proto.Field(
+    mime_type: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    labels = proto.MapField(
+    labels: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=6,
     )
 
 
 class DetectedLanguage(proto.Message):
@@ -360,35 +362,35 @@
             The BCP-47 language code of source content in
             the request, detected automatically.
         confidence (float):
             The confidence of the detection result for
             this language.
     """
 
-    language_code = proto.Field(
+    language_code: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
 
 
 class DetectLanguageResponse(proto.Message):
     r"""The response message for language detection.
 
     Attributes:
-        languages (Sequence[google.cloud.translate_v3beta1.types.DetectedLanguage]):
+        languages (MutableSequence[google.cloud.translate_v3beta1.types.DetectedLanguage]):
             A list of detected languages sorted by
             detection confidence in descending order. The
             most probable language first.
     """
 
-    languages = proto.RepeatedField(
+    languages: MutableSequence["DetectedLanguage"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="DetectedLanguage",
     )
 
 
 class GetSupportedLanguagesRequest(proto.Message):
@@ -428,39 +430,39 @@
                ``projects/{project-number-or-id}/locations/{location-id}/models/general/nmt``,
 
             Returns languages supported by the specified model. If
             missing, we get supported languages of Google general NMT
             model.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    display_language_code = proto.Field(
+    display_language_code: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class SupportedLanguages(proto.Message):
     r"""The response message for discovering supported languages.
 
     Attributes:
-        languages (Sequence[google.cloud.translate_v3beta1.types.SupportedLanguage]):
+        languages (MutableSequence[google.cloud.translate_v3beta1.types.SupportedLanguage]):
             A list of supported language responses. This
             list contains an entry for each language the
             Translation API supports.
     """
 
-    languages = proto.RepeatedField(
+    languages: MutableSequence["SupportedLanguage"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="SupportedLanguage",
     )
 
 
 class SupportedLanguage(proto.Message):
@@ -480,42 +482,42 @@
             request.
         support_source (bool):
             Can be used as source language.
         support_target (bool):
             Can be used as target language.
     """
 
-    language_code = proto.Field(
+    language_code: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    display_name = proto.Field(
+    display_name: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    support_source = proto.Field(
+    support_source: bool = proto.Field(
         proto.BOOL,
         number=3,
     )
-    support_target = proto.Field(
+    support_target: bool = proto.Field(
         proto.BOOL,
         number=4,
     )
 
 
 class GcsSource(proto.Message):
     r"""The Google Cloud Storage location for the input content.
 
     Attributes:
         input_uri (str):
             Required. Source data URI. For example,
             ``gs://my_bucket/my_object``.
     """
 
-    input_uri = proto.Field(
+    input_uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class InputConfig(proto.Message):
     r"""Input configuration for BatchTranslateText request.
@@ -548,19 +550,19 @@
 
             The other supported file extensions are ``.txt`` or
             ``.html``, which is treated as a single large chunk of text.
 
             This field is a member of `oneof`_ ``source``.
     """
 
-    mime_type = proto.Field(
+    mime_type: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    gcs_source = proto.Field(
+    gcs_source: "GcsSource" = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="source",
         message="GcsSource",
     )
 
 
@@ -571,15 +573,15 @@
         output_uri_prefix (str):
             Required. There must be no files under 'output_uri_prefix'.
             'output_uri_prefix' must end with "/" and start with
             "gs://", otherwise an INVALID_ARGUMENT (400) error is
             returned.
     """
 
-    output_uri_prefix = proto.Field(
+    output_uri_prefix: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class OutputConfig(proto.Message):
     r"""Output configuration for BatchTranslateText request.
@@ -626,15 +628,15 @@
             Since index.csv will be keeping updated during the process,
             please make sure there is no custom retention policy applied
             on the output bucket that may avoid file updating.
             (https://cloud.google.com/storage/docs/bucket-lock?hl=en#retention-policy)
 
             The format of translations_file (for target language code
             'trg') is:
-            gs://translation_test/a_b_c\_'trg'_translations.[extension]
+            ``gs://translation_test/a_b_c\_'trg'_translations.[extension]``
 
             If the input file extension is tsv, the output has the
             following columns: Column 1: ID of the request provided in
             the input, if it's not provided in the input, then the input
             row number is used (0-based). Column 2: source sentence.
             Column 3: translation without applying a glossary. Empty
             string if there is an error. Column 4 (only present if a
@@ -664,15 +666,15 @@
             glossary_error_file will be generated that contains error
             details. glossary_error_file has format of
             gs://translation_test/a_b_c\_'trg'_glossary_errors.[extension]
 
             This field is a member of `oneof`_ ``destination``.
     """
 
-    gcs_destination = proto.Field(
+    gcs_destination: "GcsDestination" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="destination",
         message="GcsDestination",
     )
 
 
@@ -707,26 +709,26 @@
 
             -  application/pdf
             -  application/vnd.openxmlformats-officedocument.wordprocessingml.document
             -  application/vnd.openxmlformats-officedocument.presentationml.presentation
             -  application/vnd.openxmlformats-officedocument.spreadsheetml.sheet
     """
 
-    content = proto.Field(
+    content: bytes = proto.Field(
         proto.BYTES,
         number=1,
         oneof="source",
     )
-    gcs_source = proto.Field(
+    gcs_source: "GcsSource" = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="source",
         message="GcsSource",
     )
-    mime_type = proto.Field(
+    mime_type: str = proto.Field(
         proto.STRING,
         number=4,
     )
 
 
 class DocumentOutputConfig(proto.Message):
     r"""A document translation request output config.
@@ -794,21 +796,21 @@
 
             -  application/pdf
             -  application/vnd.openxmlformats-officedocument.wordprocessingml.document
             -  application/vnd.openxmlformats-officedocument.presentationml.presentation
             -  application/vnd.openxmlformats-officedocument.spreadsheetml.sheet
     """
 
-    gcs_destination = proto.Field(
+    gcs_destination: "GcsDestination" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="destination",
         message="GcsDestination",
     )
-    mime_type = proto.Field(
+    mime_type: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class TranslateDocumentRequest(proto.Message):
     r"""A document translation request.
@@ -867,71 +869,71 @@
             If not provided, the default Google model (NMT) will be used
             for translation.
         glossary_config (google.cloud.translate_v3beta1.types.TranslateTextGlossaryConfig):
             Optional. Glossary to be applied. The glossary must be
             within the same region (have the same location-id) as the
             model, otherwise an INVALID_ARGUMENT (400) error is
             returned.
-        labels (Mapping[str, str]):
+        labels (MutableMapping[str, str]):
             Optional. The labels with user-defined
             metadata for the request.
             Label keys and values can be no longer than 63
             characters (Unicode codepoints), can only
             contain lowercase letters, numeric characters,
             underscores and dashes. International characters
             are allowed. Label values are optional. Label
             keys must start with a letter.
             See
             https://cloud.google.com/translate/docs/advanced/labels
             for more information.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    source_language_code = proto.Field(
+    source_language_code: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    target_language_code = proto.Field(
+    target_language_code: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    document_input_config = proto.Field(
+    document_input_config: "DocumentInputConfig" = proto.Field(
         proto.MESSAGE,
         number=4,
         message="DocumentInputConfig",
     )
-    document_output_config = proto.Field(
+    document_output_config: "DocumentOutputConfig" = proto.Field(
         proto.MESSAGE,
         number=5,
         message="DocumentOutputConfig",
     )
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=6,
     )
-    glossary_config = proto.Field(
+    glossary_config: "TranslateTextGlossaryConfig" = proto.Field(
         proto.MESSAGE,
         number=7,
         message="TranslateTextGlossaryConfig",
     )
-    labels = proto.MapField(
+    labels: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=8,
     )
 
 
 class DocumentTranslation(proto.Message):
     r"""A translated document message.
 
     Attributes:
-        byte_stream_outputs (Sequence[bytes]):
+        byte_stream_outputs (MutableSequence[bytes]):
             The array of translated documents. It is
             expected to be size 1 for now. We may produce
             multiple translated documents in the future for
             other type of file formats.
         mime_type (str):
             The translated document's mime type.
         detected_language_code (str):
@@ -940,23 +942,23 @@
             for the input document, this field will have the
             language code automatically detected. If the
             source language was passed, auto-detection of
             the language does not occur and this field is
             empty.
     """
 
-    byte_stream_outputs = proto.RepeatedField(
+    byte_stream_outputs: MutableSequence[bytes] = proto.RepeatedField(
         proto.BYTES,
         number=1,
     )
-    mime_type = proto.Field(
+    mime_type: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    detected_language_code = proto.Field(
+    detected_language_code: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class TranslateDocumentResponse(proto.Message):
     r"""A translated document response message.
@@ -978,29 +980,29 @@
             ``projects/{project-id}/locations/{location-id}/models/general/nmt``
             then ``model`` here would be normalized to
             ``projects/{project-number}/locations/{location-id}/models/general/nmt``.
         glossary_config (google.cloud.translate_v3beta1.types.TranslateTextGlossaryConfig):
             The ``glossary_config`` used for this translation.
     """
 
-    document_translation = proto.Field(
+    document_translation: "DocumentTranslation" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="DocumentTranslation",
     )
-    glossary_document_translation = proto.Field(
+    glossary_document_translation: "DocumentTranslation" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="DocumentTranslation",
     )
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    glossary_config = proto.Field(
+    glossary_config: "TranslateTextGlossaryConfig" = proto.Field(
         proto.MESSAGE,
         number=4,
         message="TranslateTextGlossaryConfig",
     )
 
 
 class BatchTranslateTextRequest(proto.Message):
@@ -1018,94 +1020,94 @@
             translation.
 
             Only AutoML Translation models or glossaries within the same
             region (have the same location-id) can be used, otherwise an
             INVALID_ARGUMENT (400) error is returned.
         source_language_code (str):
             Required. Source language code.
-        target_language_codes (Sequence[str]):
+        target_language_codes (MutableSequence[str]):
             Required. Specify up to 10 language codes
             here.
-        models (Mapping[str, str]):
+        models (MutableMapping[str, str]):
             Optional. The models to use for translation. Map's key is
             target language code. Map's value is model name. Value can
             be a built-in general model, or an AutoML Translation model.
 
             The value format depends on model type:
 
             -  AutoML Translation models:
                ``projects/{project-number-or-id}/locations/{location-id}/models/{model-id}``
 
             -  General (built-in) models:
                ``projects/{project-number-or-id}/locations/{location-id}/models/general/nmt``,
 
             If the map is empty or a specific model is not requested for
             a language pair, then default google model (nmt) is used.
-        input_configs (Sequence[google.cloud.translate_v3beta1.types.InputConfig]):
+        input_configs (MutableSequence[google.cloud.translate_v3beta1.types.InputConfig]):
             Required. Input configurations.
             The total number of files matched should be <=
             100. The total content size should be <= 100M
             Unicode codepoints. The files must use UTF-8
             encoding.
         output_config (google.cloud.translate_v3beta1.types.OutputConfig):
             Required. Output configuration.
             If 2 input configs match to the same file (that
             is, same input path), we don't generate output
             for duplicate inputs.
-        glossaries (Mapping[str, google.cloud.translate_v3beta1.types.TranslateTextGlossaryConfig]):
+        glossaries (MutableMapping[str, google.cloud.translate_v3beta1.types.TranslateTextGlossaryConfig]):
             Optional. Glossaries to be applied for
             translation. It's keyed by target language code.
-        labels (Mapping[str, str]):
+        labels (MutableMapping[str, str]):
             Optional. The labels with user-defined
             metadata for the request.
             Label keys and values can be no longer than 63
             characters (Unicode codepoints), can only
             contain lowercase letters, numeric characters,
             underscores and dashes. International characters
             are allowed. Label values are optional. Label
             keys must start with a letter.
             See
             https://cloud.google.com/translate/docs/labels
             for more information.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    source_language_code = proto.Field(
+    source_language_code: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    target_language_codes = proto.RepeatedField(
+    target_language_codes: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=3,
     )
-    models = proto.MapField(
+    models: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=4,
     )
-    input_configs = proto.RepeatedField(
+    input_configs: MutableSequence["InputConfig"] = proto.RepeatedField(
         proto.MESSAGE,
         number=5,
         message="InputConfig",
     )
-    output_config = proto.Field(
+    output_config: "OutputConfig" = proto.Field(
         proto.MESSAGE,
         number=6,
         message="OutputConfig",
     )
-    glossaries = proto.MapField(
+    glossaries: MutableMapping[str, "TranslateTextGlossaryConfig"] = proto.MapField(
         proto.STRING,
         proto.MESSAGE,
         number=7,
         message="TranslateTextGlossaryConfig",
     )
-    labels = proto.MapField(
+    labels: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=9,
     )
 
 
 class BatchTranslateMetadata(proto.Message):
@@ -1135,32 +1137,32 @@
         STATE_UNSPECIFIED = 0
         RUNNING = 1
         SUCCEEDED = 2
         FAILED = 3
         CANCELLING = 4
         CANCELLED = 5
 
-    state = proto.Field(
+    state: State = proto.Field(
         proto.ENUM,
         number=1,
         enum=State,
     )
-    translated_characters = proto.Field(
+    translated_characters: int = proto.Field(
         proto.INT64,
         number=2,
     )
-    failed_characters = proto.Field(
+    failed_characters: int = proto.Field(
         proto.INT64,
         number=3,
     )
-    total_characters = proto.Field(
+    total_characters: int = proto.Field(
         proto.INT64,
         number=4,
     )
-    submit_time = proto.Field(
+    submit_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=5,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class BatchTranslateResponse(proto.Message):
@@ -1183,32 +1185,32 @@
             Time when the operation was submitted.
         end_time (google.protobuf.timestamp_pb2.Timestamp):
             The time when the operation is finished and
             [google.longrunning.Operation.done][google.longrunning.Operation.done]
             is set to true.
     """
 
-    total_characters = proto.Field(
+    total_characters: int = proto.Field(
         proto.INT64,
         number=1,
     )
-    translated_characters = proto.Field(
+    translated_characters: int = proto.Field(
         proto.INT64,
         number=2,
     )
-    failed_characters = proto.Field(
+    failed_characters: int = proto.Field(
         proto.INT64,
         number=3,
     )
-    submit_time = proto.Field(
+    submit_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=4,
         message=timestamp_pb2.Timestamp,
     )
-    end_time = proto.Field(
+    end_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=5,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class GlossaryInputConfig(proto.Message):
@@ -1243,15 +1245,15 @@
                defined for Google Translation Toolkit and documented in
                `Use a
                glossary <https://support.google.com/translatortoolkit/answer/6306379?hl=en>`__.
 
             This field is a member of `oneof`_ ``source``.
     """
 
-    gcs_source = proto.Field(
+    gcs_source: "GcsSource" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="source",
         message="GcsSource",
     )
 
 
@@ -1302,70 +1304,70 @@
                 GlossaryTerm.language_code.
             target_language_code (str):
                 Required. The BCP-47 language code for translation output,
                 for example, "zh-CN". Expected to be an exact match for
                 GlossaryTerm.language_code.
         """
 
-        source_language_code = proto.Field(
+        source_language_code: str = proto.Field(
             proto.STRING,
             number=1,
         )
-        target_language_code = proto.Field(
+        target_language_code: str = proto.Field(
             proto.STRING,
             number=2,
         )
 
     class LanguageCodesSet(proto.Message):
         r"""Used with equivalent term set glossaries.
 
         Attributes:
-            language_codes (Sequence[str]):
+            language_codes (MutableSequence[str]):
                 The BCP-47 language code(s) for terms defined in the
                 glossary. All entries are unique. The list contains at least
                 two entries. Expected to be an exact match for
                 GlossaryTerm.language_code.
         """
 
-        language_codes = proto.RepeatedField(
+        language_codes: MutableSequence[str] = proto.RepeatedField(
             proto.STRING,
             number=1,
         )
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    language_pair = proto.Field(
+    language_pair: LanguageCodePair = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="languages",
         message=LanguageCodePair,
     )
-    language_codes_set = proto.Field(
+    language_codes_set: LanguageCodesSet = proto.Field(
         proto.MESSAGE,
         number=4,
         oneof="languages",
         message=LanguageCodesSet,
     )
-    input_config = proto.Field(
+    input_config: "GlossaryInputConfig" = proto.Field(
         proto.MESSAGE,
         number=5,
         message="GlossaryInputConfig",
     )
-    entry_count = proto.Field(
+    entry_count: int = proto.Field(
         proto.INT32,
         number=6,
     )
-    submit_time = proto.Field(
+    submit_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=7,
         message=timestamp_pb2.Timestamp,
     )
-    end_time = proto.Field(
+    end_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=8,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class CreateGlossaryRequest(proto.Message):
@@ -1374,19 +1376,19 @@
     Attributes:
         parent (str):
             Required. The project name.
         glossary (google.cloud.translate_v3beta1.types.Glossary):
             Required. The glossary to create.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    glossary = proto.Field(
+    glossary: "Glossary" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="Glossary",
     )
 
 
 class GetGlossaryRequest(proto.Message):
@@ -1394,29 +1396,29 @@
 
     Attributes:
         name (str):
             Required. The name of the glossary to
             retrieve.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class DeleteGlossaryRequest(proto.Message):
     r"""Request message for DeleteGlossary.
 
     Attributes:
         name (str):
             Required. The name of the glossary to delete.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ListGlossariesRequest(proto.Message):
     r"""Request message for ListGlossaries.
@@ -1459,55 +1461,55 @@
             the target language code "zh-CN", but all
             equivalent term set glossaries which contain
             "en-US" and "zh-CN" in their language set will
             be picked. If missing, no filtering is
             performed.
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
 
 
 class ListGlossariesResponse(proto.Message):
     r"""Response message for ListGlossaries.
 
     Attributes:
-        glossaries (Sequence[google.cloud.translate_v3beta1.types.Glossary]):
+        glossaries (MutableSequence[google.cloud.translate_v3beta1.types.Glossary]):
             The list of glossaries for a project.
         next_page_token (str):
             A token to retrieve a page of results. Pass this value in
             the [ListGlossariesRequest.page_token] field in the
             subsequent call to ``ListGlossaries`` method to retrieve the
             next page of results.
     """
 
     @property
     def raw_page(self):
         return self
 
-    glossaries = proto.RepeatedField(
+    glossaries: MutableSequence["Glossary"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="Glossary",
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class CreateGlossaryMetadata(proto.Message):
     r"""Stored in the
@@ -1533,24 +1535,24 @@
         STATE_UNSPECIFIED = 0
         RUNNING = 1
         SUCCEEDED = 2
         FAILED = 3
         CANCELLING = 4
         CANCELLED = 5
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    state = proto.Field(
+    state: State = proto.Field(
         proto.ENUM,
         number=2,
         enum=State,
     )
-    submit_time = proto.Field(
+    submit_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=3,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class DeleteGlossaryMetadata(proto.Message):
@@ -1577,24 +1579,24 @@
         STATE_UNSPECIFIED = 0
         RUNNING = 1
         SUCCEEDED = 2
         FAILED = 3
         CANCELLING = 4
         CANCELLED = 5
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    state = proto.Field(
+    state: State = proto.Field(
         proto.ENUM,
         number=2,
         enum=State,
     )
-    submit_time = proto.Field(
+    submit_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=3,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class DeleteGlossaryResponse(proto.Message):
@@ -1610,24 +1612,24 @@
             the server.
         end_time (google.protobuf.timestamp_pb2.Timestamp):
             The time when the glossary deletion is finished and
             [google.longrunning.Operation.done][google.longrunning.Operation.done]
             is set to true.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    submit_time = proto.Field(
+    submit_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=2,
         message=timestamp_pb2.Timestamp,
     )
-    end_time = proto.Field(
+    end_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=3,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class BatchTranslateDocumentRequest(proto.Message):
@@ -1648,30 +1650,30 @@
             INVALID_ARGUMENT (400) error is returned.
         source_language_code (str):
             Required. The BCP-47 language code of the
             input document if known, for example, "en-US" or
             "sr-Latn". Supported language codes are listed
             in Language Support
             (https://cloud.google.com/translate/docs/languages).
-        target_language_codes (Sequence[str]):
+        target_language_codes (MutableSequence[str]):
             Required. The BCP-47 language code to use for
             translation of the input document. Specify up to
             10 language codes here.
-        input_configs (Sequence[google.cloud.translate_v3beta1.types.BatchDocumentInputConfig]):
+        input_configs (MutableSequence[google.cloud.translate_v3beta1.types.BatchDocumentInputConfig]):
             Required. Input configurations.
             The total number of files matched should be <=
             100. The total content size to translate should
             be <= 100M Unicode codepoints. The files must
             use UTF-8 encoding.
         output_config (google.cloud.translate_v3beta1.types.BatchDocumentOutputConfig):
             Required. Output configuration.
             If 2 input configs match to the same file (that
             is, same input path), we don't generate output
             for duplicate inputs.
-        models (Mapping[str, str]):
+        models (MutableMapping[str, str]):
             Optional. The models to use for translation. Map's key is
             target language code. Map's value is the model name. Value
             can be a built-in general model, or an AutoML Translation
             model.
 
             The value format depends on model type:
 
@@ -1679,65 +1681,65 @@
                ``projects/{project-number-or-id}/locations/{location-id}/models/{model-id}``
 
             -  General (built-in) models:
                ``projects/{project-number-or-id}/locations/{location-id}/models/general/nmt``,
 
             If the map is empty or a specific model is not requested for
             a language pair, then default google model (nmt) is used.
-        glossaries (Mapping[str, google.cloud.translate_v3beta1.types.TranslateTextGlossaryConfig]):
+        glossaries (MutableMapping[str, google.cloud.translate_v3beta1.types.TranslateTextGlossaryConfig]):
             Optional. Glossaries to be applied. It's
             keyed by target language code.
-        format_conversions (Mapping[str, str]):
+        format_conversions (MutableMapping[str, str]):
             Optional. File format conversion map to be applied to all
             input files. Map's key is the original mime_type. Map's
             value is the target mime_type of translated documents.
 
             Supported file format conversion includes:
 
             -  ``application/pdf`` to
                ``application/vnd.openxmlformats-officedocument.wordprocessingml.document``
 
             If nothing specified, output files will be in the same
             format as the original file.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    source_language_code = proto.Field(
+    source_language_code: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    target_language_codes = proto.RepeatedField(
+    target_language_codes: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=3,
     )
-    input_configs = proto.RepeatedField(
+    input_configs: MutableSequence["BatchDocumentInputConfig"] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message="BatchDocumentInputConfig",
     )
-    output_config = proto.Field(
+    output_config: "BatchDocumentOutputConfig" = proto.Field(
         proto.MESSAGE,
         number=5,
         message="BatchDocumentOutputConfig",
     )
-    models = proto.MapField(
+    models: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=6,
     )
-    glossaries = proto.MapField(
+    glossaries: MutableMapping[str, "TranslateTextGlossaryConfig"] = proto.MapField(
         proto.STRING,
         proto.MESSAGE,
         number=7,
         message="TranslateTextGlossaryConfig",
     )
-    format_conversions = proto.MapField(
+    format_conversions: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=8,
     )
 
 
 class BatchDocumentInputConfig(proto.Message):
@@ -1767,15 +1769,15 @@
             ``.xlsx`` is 100MB. The max file size to support for
             ``.pdf`` is 1GB and the max page limit is 1000 pages. The
             max file size to support for all input documents is 1GB.
 
             This field is a member of `oneof`_ ``source``.
     """
 
-    gcs_source = proto.Field(
+    gcs_source: "GcsSource" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="source",
         message="GcsSource",
     )
 
 
@@ -1838,15 +1840,15 @@
             ``glossary_error_output``:
             gs://translation_test/a_b_c*\ [trg]_glossary_translation.txt
             The error output is a txt file containing error details.
 
             This field is a member of `oneof`_ ``destination``.
     """
 
-    gcs_destination = proto.Field(
+    gcs_destination: "GcsDestination" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="destination",
         message="GcsDestination",
     )
 
 
@@ -1889,52 +1891,52 @@
             Time when the operation was submitted.
         end_time (google.protobuf.timestamp_pb2.Timestamp):
             The time when the operation is finished and
             [google.longrunning.Operation.done][google.longrunning.Operation.done]
             is set to true.
     """
 
-    total_pages = proto.Field(
+    total_pages: int = proto.Field(
         proto.INT64,
         number=1,
     )
-    translated_pages = proto.Field(
+    translated_pages: int = proto.Field(
         proto.INT64,
         number=2,
     )
-    failed_pages = proto.Field(
+    failed_pages: int = proto.Field(
         proto.INT64,
         number=3,
     )
-    total_billable_pages = proto.Field(
+    total_billable_pages: int = proto.Field(
         proto.INT64,
         number=4,
     )
-    total_characters = proto.Field(
+    total_characters: int = proto.Field(
         proto.INT64,
         number=5,
     )
-    translated_characters = proto.Field(
+    translated_characters: int = proto.Field(
         proto.INT64,
         number=6,
     )
-    failed_characters = proto.Field(
+    failed_characters: int = proto.Field(
         proto.INT64,
         number=7,
     )
-    total_billable_characters = proto.Field(
+    total_billable_characters: int = proto.Field(
         proto.INT64,
         number=8,
     )
-    submit_time = proto.Field(
+    submit_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=9,
         message=timestamp_pb2.Timestamp,
     )
-    end_time = proto.Field(
+    end_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=10,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class BatchTranslateDocumentMetadata(proto.Message):
@@ -1982,52 +1984,52 @@
         STATE_UNSPECIFIED = 0
         RUNNING = 1
         SUCCEEDED = 2
         FAILED = 3
         CANCELLING = 4
         CANCELLED = 5
 
-    state = proto.Field(
+    state: State = proto.Field(
         proto.ENUM,
         number=1,
         enum=State,
     )
-    total_pages = proto.Field(
+    total_pages: int = proto.Field(
         proto.INT64,
         number=2,
     )
-    translated_pages = proto.Field(
+    translated_pages: int = proto.Field(
         proto.INT64,
         number=3,
     )
-    failed_pages = proto.Field(
+    failed_pages: int = proto.Field(
         proto.INT64,
         number=4,
     )
-    total_billable_pages = proto.Field(
+    total_billable_pages: int = proto.Field(
         proto.INT64,
         number=5,
     )
-    total_characters = proto.Field(
+    total_characters: int = proto.Field(
         proto.INT64,
         number=6,
     )
-    translated_characters = proto.Field(
+    translated_characters: int = proto.Field(
         proto.INT64,
         number=7,
     )
-    failed_characters = proto.Field(
+    failed_characters: int = proto.Field(
         proto.INT64,
         number=8,
     )
-    total_billable_characters = proto.Field(
+    total_billable_characters: int = proto.Field(
         proto.INT64,
         number=9,
     )
-    submit_time = proto.Field(
+    submit_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=10,
         message=timestamp_pb2.Timestamp,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-translate-3.8.4/google_cloud_translate.egg-info/PKG-INFO` & `google-cloud-translate-3.9.0/google_cloud_translate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: google-cloud-translate
-Version: 3.8.4
-Summary: Google Cloud Translation API client library
+Version: 3.9.0
+Summary: Google Cloud Translate API client library
 Home-page: https://github.com/googleapis/python-translate
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `google-cloud-translate-3.8.4/google_cloud_translate.egg-info/SOURCES.txt` & `google-cloud-translate-3.9.0/google_cloud_translate.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,34 +2,37 @@
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 google/__init__.py
 google/cloud/__init__.py
 google/cloud/translate/__init__.py
+google/cloud/translate/gapic_version.py
 google/cloud/translate/py.typed
 google/cloud/translate_v2/__init__.py
 google/cloud/translate_v2/_http.py
 google/cloud/translate_v2/client.py
 google/cloud/translate_v3/__init__.py
 google/cloud/translate_v3/gapic_metadata.json
+google/cloud/translate_v3/gapic_version.py
 google/cloud/translate_v3/py.typed
 google/cloud/translate_v3/services/__init__.py
 google/cloud/translate_v3/services/translation_service/__init__.py
 google/cloud/translate_v3/services/translation_service/async_client.py
 google/cloud/translate_v3/services/translation_service/client.py
 google/cloud/translate_v3/services/translation_service/pagers.py
 google/cloud/translate_v3/services/translation_service/transports/__init__.py
 google/cloud/translate_v3/services/translation_service/transports/base.py
 google/cloud/translate_v3/services/translation_service/transports/grpc.py
 google/cloud/translate_v3/services/translation_service/transports/grpc_asyncio.py
 google/cloud/translate_v3/types/__init__.py
 google/cloud/translate_v3/types/translation_service.py
 google/cloud/translate_v3beta1/__init__.py
 google/cloud/translate_v3beta1/gapic_metadata.json
+google/cloud/translate_v3beta1/gapic_version.py
 google/cloud/translate_v3beta1/py.typed
 google/cloud/translate_v3beta1/services/__init__.py
 google/cloud/translate_v3beta1/services/translation_service/__init__.py
 google/cloud/translate_v3beta1/services/translation_service/async_client.py
 google/cloud/translate_v3beta1/services/translation_service/client.py
 google/cloud/translate_v3beta1/services/translation_service/pagers.py
 google/cloud/translate_v3beta1/services/translation_service/transports/__init__.py
@@ -41,16 +44,14 @@
 google_cloud_translate.egg-info/PKG-INFO
 google_cloud_translate.egg-info/SOURCES.txt
 google_cloud_translate.egg-info/dependency_links.txt
 google_cloud_translate.egg-info/namespace_packages.txt
 google_cloud_translate.egg-info/not-zip-safe
 google_cloud_translate.egg-info/requires.txt
 google_cloud_translate.egg-info/top_level.txt
-scripts/fixup_translate_v3_keywords.py
-scripts/fixup_translate_v3beta1_keywords.py
 tests/__init__.py
 tests/system.py
 tests/system/test_vpcsc.py
 tests/unit/__init__.py
 tests/unit/gapic/__init__.py
 tests/unit/gapic/translate_v3/__init__.py
 tests/unit/gapic/translate_v3/test_translation_service.py
```

### Comparing `google-cloud-translate-3.8.4/setup.py` & `google-cloud-translate-3.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-# Copyright 2018 Google LLC
+# -*- coding: utf-8 -*-
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
-
+#
 import io
 import os
 
-import setuptools
+import setuptools  # type: ignore
 
-
-# Package metadata.
+package_root = os.path.abspath(os.path.dirname(__file__))
 
 name = "google-cloud-translate"
-description = "Google Cloud Translation API client library"
-version = "3.8.4"
-# Should be one of:
-# 'Development Status :: 3 - Alpha'
-# 'Development Status :: 4 - Beta'
-# 'Development Status :: 5 - Production/Stable'
-release_status = "Development Status :: 5 - Production/Stable"
+
+
+description = "Google Cloud Translate API client library"
+
+version = {}
+with open(os.path.join(package_root, "google/cloud/translate/gapic_version.py")) as fp:
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
     "google-cloud-core >= 1.3.0, <3.0.0dev",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-extras = {}
-
-
-# Setup boilerplate below this line.
+url = "https://github.com/googleapis/python-translate"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
-# Only include packages under the 'google' namespace. Do not include tests,
-# benchmarks, etc.
 packages = [
     package
     for package in setuptools.PEP420PackageFinder.find()
     if package.startswith("google")
 ]
 
-# Determine which namespaces are needed.
 namespaces = ["google"]
 if "google.cloud" in packages:
     namespaces.append("google.cloud")
 
-
 setuptools.setup(
     name=name,
     version=version,
     description=description,
     long_description=readme,
     author="Google LLC",
     author_email="googleapis-packages@google.com",
     license="Apache 2.0",
-    url="https://github.com/googleapis/python-translate",
+    url=url,
     classifiers=[
         release_status,
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
@@ -79,18 +79,13 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
         "Topic :: Internet",
     ],
     platforms="Posix; MacOS X; Windows",
     packages=packages,
-    scripts=[
-        "scripts/fixup_translate_v3_keywords.py",
-        "scripts/fixup_translate_v3beta1_keywords.py",
-    ],
+    python_requires=">=3.7",
     namespace_packages=namespaces,
     install_requires=dependencies,
-    extras_require=extras,
-    python_requires=">=3.7",
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `google-cloud-translate-3.8.4/tests/__init__.py` & `google-cloud-translate-3.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/tests/system/test_vpcsc.py` & `google-cloud-translate-3.9.0/tests/system/test_vpcsc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/tests/system.py` & `google-cloud-translate-3.9.0/tests/system.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/tests/unit/__init__.py` & `google-cloud-translate-3.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/tests/unit/gapic/__init__.py` & `google-cloud-translate-3.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/tests/unit/gapic/translate_v3/__init__.py` & `google-cloud-translate-3.9.0/tests/unit/gapic/translate_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/tests/unit/gapic/translate_v3/test_translation_service.py` & `google-cloud-translate-3.9.0/tests/unit/gapic/translate_v3/test_translation_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/tests/unit/gapic/translate_v3beta1/__init__.py` & `google-cloud-translate-3.9.0/tests/unit/gapic/translate_v3beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/tests/unit/gapic/translate_v3beta1/test_translation_service.py` & `google-cloud-translate-3.9.0/tests/unit/gapic/translate_v3beta1/test_translation_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/tests/unit/v2/test__http.py` & `google-cloud-translate-3.9.0/tests/unit/v2/test__http.py`

 * *Files identical despite different names*

### Comparing `google-cloud-translate-3.8.4/tests/unit/v2/test_client.py` & `google-cloud-translate-3.9.0/tests/unit/v2/test_client.py`

 * *Files identical despite different names*

