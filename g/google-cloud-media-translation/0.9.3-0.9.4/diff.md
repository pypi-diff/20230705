# Comparing `tmp/google-cloud-media-translation-0.9.3.tar.gz` & `tmp/google-cloud-media-translation-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-media-translation-0.9.3.tar", last modified: Tue Oct  4 00:37:51 2022, max compression
+gzip compressed data, was "google-cloud-media-translation-0.9.4.tar", last modified: Mon Oct 10 16:15:08 2022, max compression
```

## Comparing `google-cloud-media-translation-0.9.3.tar` & `google-cloud-media-translation-0.9.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:37:51.168574 google-cloud-media-translation-0.9.3/
--rw-rw-r--   0 root         (0)     1003    11358 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4495 2022-10-04 00:37:51.168574 google-cloud-media-translation-0.9.3/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3753 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:37:51.160570 google-cloud-media-translation-0.9.3/docs/
--rw-rw-r--   0 root         (0)     1003    12530 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/docs/conf.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:37:51.156567 google-cloud-media-translation-0.9.3/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:37:51.156567 google-cloud-media-translation-0.9.3/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:37:51.160570 google-cloud-media-translation-0.9.3/google/cloud/mediatranslation/
--rw-rw-r--   0 root         (0)     1003     1410 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/google/cloud/mediatranslation/__init__.py
--rw-rw-r--   0 root         (0)     1003       91 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/google/cloud/mediatranslation/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:37:51.160570 google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/
--rw-rw-r--   0 root         (0)     1003     1226 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003      893 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       91 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:37:51.160570 google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:37:51.160570 google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/
--rw-rw-r--   0 root         (0)     1003      809 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    14162 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    21970 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:37:51.164572 google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/transports/
--rw-rw-r--   0 root         (0)     1003     1291 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6333 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12047 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12275 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:37:51.164572 google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1008 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    10702 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/types/media_translation.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:37:51.164572 google-cloud-media-translation-0.9.3/google_cloud_media_translation.egg-info/
--rw-r--r--   0 root         (0)     1003     4495 2022-10-04 00:37:51.000000 google-cloud-media-translation-0.9.3/google_cloud_media_translation.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2184 2022-10-04 00:37:51.000000 google-cloud-media-translation-0.9.3/google_cloud_media_translation.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-04 00:37:51.000000 google-cloud-media-translation-0.9.3/google_cloud_media_translation.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-10-04 00:37:51.000000 google-cloud-media-translation-0.9.3/google_cloud_media_translation.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-04 00:37:51.000000 google-cloud-media-translation-0.9.3/google_cloud_media_translation.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      160 2022-10-04 00:37:51.000000 google-cloud-media-translation-0.9.3/google_cloud_media_translation.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003       42 2022-10-04 00:37:51.000000 google-cloud-media-translation-0.9.3/google_cloud_media_translation.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:37:51.156567 google-cloud-media-translation-0.9.3/samples/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:37:51.164572 google-cloud-media-translation-0.9.3/samples/generated_samples/
--rw-rw-r--   0 root         (0)     1003     2758 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/samples/generated_samples/mediatranslation_v1beta1_generated_speech_translation_service_streaming_translate_speech_async.py
--rw-rw-r--   0 root         (0)     1003     2733 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/samples/generated_samples/mediatranslation_v1beta1_generated_speech_translation_service_streaming_translate_speech_sync.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:37:51.168574 google-cloud-media-translation-0.9.3/samples/snippets/
--rw-rw-r--   0 root         (0)     1003     9920 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/samples/snippets/noxfile.py
--rw-rw-r--   0 root         (0)     1003     2649 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/samples/snippets/translate_from_file.py
--rw-rw-r--   0 root         (0)     1003      914 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/samples/snippets/translate_from_file_test.py
--rw-rw-r--   0 root         (0)     1003     5474 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/samples/snippets/translate_from_mic.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:37:51.168574 google-cloud-media-translation-0.9.3/scripts/
--rw-rw-r--   0 root         (0)     1003     6001 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/scripts/fixup_keywords.py
--rw-rw-r--   0 root         (0)     1003     6007 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/scripts/fixup_mediatranslation_v1beta1_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-10-04 00:37:51.168574 google-cloud-media-translation-0.9.3/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2087 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:37:51.168574 google-cloud-media-translation-0.9.3/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:37:51.168574 google-cloud-media-translation-0.9.3/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:37:51.168574 google-cloud-media-translation-0.9.3/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:37:51.168574 google-cloud-media-translation-0.9.3/tests/unit/gapic/mediatranslation_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/tests/unit/gapic/mediatranslation_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    54928 2022-10-04 00:34:14.000000 google-cloud-media-translation-0.9.3/tests/unit/gapic/mediatranslation_v1beta1/test_speech_translation_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:08.986892 google-cloud-media-translation-0.9.4/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4495 2022-10-10 16:15:08.986892 google-cloud-media-translation-0.9.4/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3753 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:08.978895 google-cloud-media-translation-0.9.4/docs/
+-rw-rw-r--   0 root         (0)     1003    12530 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/docs/conf.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:08.978895 google-cloud-media-translation-0.9.4/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:08.978895 google-cloud-media-translation-0.9.4/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:08.978895 google-cloud-media-translation-0.9.4/google/cloud/mediatranslation/
+-rw-rw-r--   0 root         (0)     1003     1410 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/google/cloud/mediatranslation/__init__.py
+-rw-rw-r--   0 root         (0)     1003       91 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/google/cloud/mediatranslation/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:08.982894 google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     1226 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      893 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       91 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:08.982894 google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:08.982894 google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/
+-rw-rw-r--   0 root         (0)     1003      809 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14162 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    21970 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:08.982894 google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1291 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6333 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12047 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12275 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:08.982894 google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1008 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10702 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/types/media_translation.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:08.982894 google-cloud-media-translation-0.9.4/google_cloud_media_translation.egg-info/
+-rw-r--r--   0 root         (0)     1003     4495 2022-10-10 16:15:08.000000 google-cloud-media-translation-0.9.4/google_cloud_media_translation.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2184 2022-10-10 16:15:08.000000 google-cloud-media-translation-0.9.4/google_cloud_media_translation.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:15:08.000000 google-cloud-media-translation-0.9.4/google_cloud_media_translation.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-10-10 16:15:08.000000 google-cloud-media-translation-0.9.4/google_cloud_media_translation.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:15:08.000000 google-cloud-media-translation-0.9.4/google_cloud_media_translation.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      232 2022-10-10 16:15:08.000000 google-cloud-media-translation-0.9.4/google_cloud_media_translation.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003       42 2022-10-10 16:15:08.000000 google-cloud-media-translation-0.9.4/google_cloud_media_translation.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:08.978895 google-cloud-media-translation-0.9.4/samples/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:08.982894 google-cloud-media-translation-0.9.4/samples/generated_samples/
+-rw-rw-r--   0 root         (0)     1003     2758 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/samples/generated_samples/mediatranslation_v1beta1_generated_speech_translation_service_streaming_translate_speech_async.py
+-rw-rw-r--   0 root         (0)     1003     2733 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/samples/generated_samples/mediatranslation_v1beta1_generated_speech_translation_service_streaming_translate_speech_sync.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:08.986892 google-cloud-media-translation-0.9.4/samples/snippets/
+-rw-rw-r--   0 root         (0)     1003     9920 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/samples/snippets/noxfile.py
+-rw-rw-r--   0 root         (0)     1003     2649 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/samples/snippets/translate_from_file.py
+-rw-rw-r--   0 root         (0)     1003      914 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/samples/snippets/translate_from_file_test.py
+-rw-rw-r--   0 root         (0)     1003     5474 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/samples/snippets/translate_from_mic.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:08.986892 google-cloud-media-translation-0.9.4/scripts/
+-rw-rw-r--   0 root         (0)     1003     6001 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/scripts/fixup_keywords.py
+-rw-rw-r--   0 root         (0)     1003     6007 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/scripts/fixup_mediatranslation_v1beta1_keywords.py
+-rw-rw-r--   0 root         (0)     1003       67 2022-10-10 16:15:08.986892 google-cloud-media-translation-0.9.4/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2156 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:08.986892 google-cloud-media-translation-0.9.4/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:08.986892 google-cloud-media-translation-0.9.4/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:08.986892 google-cloud-media-translation-0.9.4/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:08.986892 google-cloud-media-translation-0.9.4/tests/unit/gapic/mediatranslation_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/tests/unit/gapic/mediatranslation_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    54928 2022-10-10 16:11:53.000000 google-cloud-media-translation-0.9.4/tests/unit/gapic/mediatranslation_v1beta1/test_speech_translation_service.py
```

### Comparing `google-cloud-media-translation-0.9.3/LICENSE` & `google-cloud-media-translation-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/MANIFEST.in` & `google-cloud-media-translation-0.9.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/PKG-INFO` & `google-cloud-media-translation-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-media-translation
-Version: 0.9.3
+Version: 0.9.4
 Home-page: https://github.com/googleapis/python-media-translation
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `google-cloud-media-translation-0.9.3/README.rst` & `google-cloud-media-translation-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/docs/conf.py` & `google-cloud-media-translation-0.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/google/cloud/mediatranslation/__init__.py` & `google-cloud-media-translation-0.9.4/google/cloud/mediatranslation/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/__init__.py` & `google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/gapic_metadata.json` & `google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/services/__init__.py` & `google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/__init__.py` & `google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/async_client.py` & `google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/client.py` & `google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/transports/__init__.py` & `google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/transports/base.py` & `google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/transports/grpc.py` & `google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/transports/grpc_asyncio.py` & `google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/services/speech_translation_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/types/__init__.py` & `google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/google/cloud/mediatranslation_v1beta1/types/media_translation.py` & `google-cloud-media-translation-0.9.4/google/cloud/mediatranslation_v1beta1/types/media_translation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/google_cloud_media_translation.egg-info/PKG-INFO` & `google-cloud-media-translation-0.9.4/google_cloud_media_translation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-media-translation
-Version: 0.9.3
+Version: 0.9.4
 Home-page: https://github.com/googleapis/python-media-translation
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `google-cloud-media-translation-0.9.3/google_cloud_media_translation.egg-info/SOURCES.txt` & `google-cloud-media-translation-0.9.4/google_cloud_media_translation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/samples/generated_samples/mediatranslation_v1beta1_generated_speech_translation_service_streaming_translate_speech_async.py` & `google-cloud-media-translation-0.9.4/samples/generated_samples/mediatranslation_v1beta1_generated_speech_translation_service_streaming_translate_speech_async.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/samples/generated_samples/mediatranslation_v1beta1_generated_speech_translation_service_streaming_translate_speech_sync.py` & `google-cloud-media-translation-0.9.4/samples/generated_samples/mediatranslation_v1beta1_generated_speech_translation_service_streaming_translate_speech_sync.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/samples/snippets/noxfile.py` & `google-cloud-media-translation-0.9.4/samples/snippets/noxfile.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/samples/snippets/translate_from_file.py` & `google-cloud-media-translation-0.9.4/samples/snippets/translate_from_file.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/samples/snippets/translate_from_file_test.py` & `google-cloud-media-translation-0.9.4/samples/snippets/translate_from_file_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/samples/snippets/translate_from_mic.py` & `google-cloud-media-translation-0.9.4/samples/snippets/translate_from_mic.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/scripts/fixup_keywords.py` & `google-cloud-media-translation-0.9.4/scripts/fixup_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/scripts/fixup_mediatranslation_v1beta1_keywords.py` & `google-cloud-media-translation-0.9.4/scripts/fixup_mediatranslation_v1beta1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/setup.py` & `google-cloud-media-translation-0.9.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # limitations under the License.
 #
 import io
 import os
 
 import setuptools  # type: ignore
 
-version = "0.9.3"
+version = "0.9.4"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
@@ -38,15 +38,15 @@
     packages=setuptools.PEP420PackageFinder.find(),
     namespace_packages=("google", "google.cloud"),
     platforms="Posix; MacOS X; Windows",
     include_package_data=True,
     install_requires=(
         "google-api-core[grpc] >= 1.32.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
         "proto-plus >= 1.22.0, <2.0.0dev",
-        "protobuf >= 3.20.2, <5.0.0dev",
+        "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     ),
     python_requires=">=3.7",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.7",
```

### Comparing `google-cloud-media-translation-0.9.3/tests/__init__.py` & `google-cloud-media-translation-0.9.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/tests/unit/__init__.py` & `google-cloud-media-translation-0.9.4/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/tests/unit/gapic/__init__.py` & `google-cloud-media-translation-0.9.4/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/tests/unit/gapic/mediatranslation_v1beta1/__init__.py` & `google-cloud-media-translation-0.9.4/tests/unit/gapic/mediatranslation_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-media-translation-0.9.3/tests/unit/gapic/mediatranslation_v1beta1/test_speech_translation_service.py` & `google-cloud-media-translation-0.9.4/tests/unit/gapic/mediatranslation_v1beta1/test_speech_translation_service.py`

 * *Files identical despite different names*

