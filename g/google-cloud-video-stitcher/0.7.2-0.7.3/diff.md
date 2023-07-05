# Comparing `tmp/google-cloud-video-stitcher-0.7.2.tar.gz` & `tmp/google-cloud-video-stitcher-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-video-stitcher-0.7.2.tar", last modified: Wed May 31 20:39:32 2023, max compression
+gzip compressed data, was "google-cloud-video-stitcher-0.7.3.tar", last modified: Wed Jul  5 15:26:52 2023, max compression
```

## Comparing `google-cloud-video-stitcher-0.7.2.tar` & `google-cloud-video-stitcher-0.7.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:39:32.391920 google-cloud-video-stitcher-0.7.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4771 2023-05-31 20:39:32.391920 google-cloud-video-stitcher-0.7.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3847 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:39:32.383920 google-cloud-video-stitcher-0.7.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:39:32.383920 google-cloud-video-stitcher-0.7.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:39:32.383920 google-cloud-video-stitcher-0.7.2/google/cloud/video/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:39:32.383920 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher/
--rw-rw-r--   0 root         (0)     1003     4591 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       88 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:39:32.387920 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/
--rw-rw-r--   0 root         (0)     1003     4140 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     6599 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       88 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:39:32.387920 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:39:32.387920 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/video_stitcher_service/
--rw-rw-r--   0 root         (0)     1003      793 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/video_stitcher_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   134907 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/video_stitcher_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   152083 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/video_stitcher_service/client.py
--rw-rw-r--   0 root         (0)     1003    32467 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/video_stitcher_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:39:32.387920 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/
--rw-rw-r--   0 root         (0)     1003     1255 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    18084 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    43836 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    44712 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   110180 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:39:32.391920 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/types/
--rw-rw-r--   0 root         (0)     1003     3774 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     4835 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/types/ad_tag_details.py
--rw-rw-r--   0 root         (0)     1003     4222 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/types/cdn_keys.py
--rw-rw-r--   0 root         (0)     1003     6930 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/types/companions.py
--rw-rw-r--   0 root         (0)     1003     5153 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/types/events.py
--rw-rw-r--   0 root         (0)     1003     7320 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/types/live_configs.py
--rw-rw-r--   0 root         (0)     1003    13278 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/types/sessions.py
--rw-rw-r--   0 root         (0)     1003     2314 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/types/slates.py
--rw-rw-r--   0 root         (0)     1003     3049 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/types/stitch_details.py
--rw-rw-r--   0 root         (0)     1003    26456 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/types/video_stitcher_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:39:32.391920 google-cloud-video-stitcher-0.7.2/google_cloud_video_stitcher.egg-info/
--rw-r--r--   0 root         (0)     1003     4771 2023-05-31 20:39:32.000000 google-cloud-video-stitcher-0.7.2/google_cloud_video_stitcher.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2180 2023-05-31 20:39:32.000000 google-cloud-video-stitcher-0.7.2/google_cloud_video_stitcher.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-31 20:39:32.000000 google-cloud-video-stitcher-0.7.2/google_cloud_video_stitcher.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       39 2023-05-31 20:39:32.000000 google-cloud-video-stitcher-0.7.2/google_cloud_video_stitcher.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-31 20:39:32.000000 google-cloud-video-stitcher-0.7.2/google_cloud_video_stitcher.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-05-31 20:39:32.000000 google-cloud-video-stitcher-0.7.2/google_cloud_video_stitcher.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-05-31 20:39:32.000000 google-cloud-video-stitcher-0.7.2/google_cloud_video_stitcher.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-05-31 20:39:32.391920 google-cloud-video-stitcher-0.7.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2977 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:39:32.391920 google-cloud-video-stitcher-0.7.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:39:32.391920 google-cloud-video-stitcher-0.7.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:39:32.391920 google-cloud-video-stitcher-0.7.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:39:32.391920 google-cloud-video-stitcher-0.7.2/tests/unit/gapic/stitcher_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/tests/unit/gapic/stitcher_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   336343 2023-05-31 20:36:55.000000 google-cloud-video-stitcher-0.7.2/tests/unit/gapic/stitcher_v1/test_video_stitcher_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:52.096557 google-cloud-video-stitcher-0.7.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4771 2023-07-05 15:26:52.096557 google-cloud-video-stitcher-0.7.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3847 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:52.088553 google-cloud-video-stitcher-0.7.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:52.088553 google-cloud-video-stitcher-0.7.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:52.088553 google-cloud-video-stitcher-0.7.3/google/cloud/video/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:52.088553 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher/
+-rw-rw-r--   0 root         (0)     1003     4591 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       88 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:52.088553 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/
+-rw-rw-r--   0 root         (0)     1003     4140 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6599 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       88 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:52.088553 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:52.092555 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/video_stitcher_service/
+-rw-rw-r--   0 root         (0)     1003      793 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/video_stitcher_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   134944 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/video_stitcher_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   152083 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/video_stitcher_service/client.py
+-rw-rw-r--   0 root         (0)     1003    32467 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/video_stitcher_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:52.092555 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1255 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18084 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    43836 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    44712 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   110180 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:52.092555 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3774 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4835 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/types/ad_tag_details.py
+-rw-rw-r--   0 root         (0)     1003     4222 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/types/cdn_keys.py
+-rw-rw-r--   0 root         (0)     1003     6930 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/types/companions.py
+-rw-rw-r--   0 root         (0)     1003     5153 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/types/events.py
+-rw-rw-r--   0 root         (0)     1003     7320 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/types/live_configs.py
+-rw-rw-r--   0 root         (0)     1003    13278 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/types/sessions.py
+-rw-rw-r--   0 root         (0)     1003     2314 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/types/slates.py
+-rw-rw-r--   0 root         (0)     1003     3049 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/types/stitch_details.py
+-rw-rw-r--   0 root         (0)     1003    26456 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/types/video_stitcher_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:52.096557 google-cloud-video-stitcher-0.7.3/google_cloud_video_stitcher.egg-info/
+-rw-r--r--   0 root         (0)     1003     4771 2023-07-05 15:26:52.000000 google-cloud-video-stitcher-0.7.3/google_cloud_video_stitcher.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2180 2023-07-05 15:26:52.000000 google-cloud-video-stitcher-0.7.3/google_cloud_video_stitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:26:52.000000 google-cloud-video-stitcher-0.7.3/google_cloud_video_stitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       39 2023-07-05 15:26:52.000000 google-cloud-video-stitcher-0.7.3/google_cloud_video_stitcher.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:26:52.000000 google-cloud-video-stitcher-0.7.3/google_cloud_video_stitcher.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:26:52.000000 google-cloud-video-stitcher-0.7.3/google_cloud_video_stitcher.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:26:52.000000 google-cloud-video-stitcher-0.7.3/google_cloud_video_stitcher.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:26:52.096557 google-cloud-video-stitcher-0.7.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2977 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:52.096557 google-cloud-video-stitcher-0.7.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:52.096557 google-cloud-video-stitcher-0.7.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:52.096557 google-cloud-video-stitcher-0.7.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:52.096557 google-cloud-video-stitcher-0.7.3/tests/unit/gapic/stitcher_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/tests/unit/gapic/stitcher_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   337454 2023-07-05 15:24:15.000000 google-cloud-video-stitcher-0.7.3/tests/unit/gapic/stitcher_v1/test_video_stitcher_service.py
```

### Comparing `google-cloud-video-stitcher-0.7.2/LICENSE` & `google-cloud-video-stitcher-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/MANIFEST.in` & `google-cloud-video-stitcher-0.7.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/PKG-INFO` & `google-cloud-video-stitcher-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-video-stitcher
-Version: 0.7.2
+Version: 0.7.3
 Summary: Google Cloud Video Stitcher API client library
 Home-page: https://github.com/googleapis/python-video-stitcher
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-video-stitcher-0.7.2/README.rst` & `google-cloud-video-stitcher-0.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher/__init__.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher/gapic_version.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.7.2"  # {x-release-please-version}
```

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/__init__.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/gapic_metadata.json` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/gapic_version.py` & `google-cloud-video-stitcher-0.7.3/tests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.7.2"  # {x-release-please-version}
```

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/__init__.py` & `google-cloud-video-stitcher-0.7.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/video_stitcher_service/__init__.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/video_stitcher_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/video_stitcher_service/async_client.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/video_stitcher_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3359,15 +3359,15 @@
         await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "VideoStitcherServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/video_stitcher_service/client.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/video_stitcher_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/video_stitcher_service/pagers.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/video_stitcher_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/__init__.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/base.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc_asyncio.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/rest.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/types/__init__.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/types/ad_tag_details.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/types/ad_tag_details.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/types/cdn_keys.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/types/cdn_keys.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/types/companions.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/types/companions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/types/events.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/types/events.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/types/live_configs.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/types/live_configs.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/types/sessions.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/types/sessions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/types/slates.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/types/slates.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/types/stitch_details.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/types/stitch_details.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google/cloud/video/stitcher_v1/types/video_stitcher_service.py` & `google-cloud-video-stitcher-0.7.3/google/cloud/video/stitcher_v1/types/video_stitcher_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/google_cloud_video_stitcher.egg-info/PKG-INFO` & `google-cloud-video-stitcher-0.7.3/google_cloud_video_stitcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-video-stitcher
-Version: 0.7.2
+Version: 0.7.3
 Summary: Google Cloud Video Stitcher API client library
 Home-page: https://github.com/googleapis/python-video-stitcher
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-video-stitcher-0.7.2/google_cloud_video_stitcher.egg-info/SOURCES.txt` & `google-cloud-video-stitcher-0.7.3/google_cloud_video_stitcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/setup.py` & `google-cloud-video-stitcher-0.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/tests/__init__.py` & `google-cloud-video-stitcher-0.7.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/tests/unit/__init__.py` & `google-cloud-video-stitcher-0.7.3/tests/unit/gapic/stitcher_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.2/tests/unit/gapic/stitcher_v1/test_video_stitcher_service.py` & `google-cloud-video-stitcher-0.7.3/tests/unit/gapic/stitcher_v1/test_video_stitcher_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1398,17 +1398,19 @@
                     cdn_keys.CdnKey(),
                     cdn_keys.CdnKey(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_cdn_keys(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1429,15 +1431,14 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_cdn_key), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = cdn_keys.CdnKey(
             name="name_value",
             hostname="hostname_value",
-            google_cdn_key=cdn_keys.GoogleCdnKey(private_key=b"private_key_blob"),
         )
         response = client.get_cdn_key(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == video_stitcher_service.GetCdnKeyRequest()
@@ -3073,17 +3074,19 @@
                     stitch_details.VodStitchDetail(),
                     stitch_details.VodStitchDetail(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_vod_stitch_details(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3763,17 +3766,19 @@
                     ad_tag_details.VodAdTagDetail(),
                     ad_tag_details.VodAdTagDetail(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_vod_ad_tag_details(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4453,17 +4458,19 @@
                     ad_tag_details.LiveAdTagDetail(),
                     ad_tag_details.LiveAdTagDetail(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_live_ad_tag_details(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5372,17 +5379,19 @@
                     slates.Slate(),
                     slates.Slate(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_slates(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -7282,17 +7291,19 @@
                     live_configs.LiveConfig(),
                     live_configs.LiveConfig(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_live_configs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

