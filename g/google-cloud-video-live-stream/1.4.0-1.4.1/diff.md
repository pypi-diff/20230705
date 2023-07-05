# Comparing `tmp/google-cloud-video-live-stream-1.4.0.tar.gz` & `tmp/google-cloud-video-live-stream-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-video-live-stream-1.4.0.tar", last modified: Mon Mar 27 15:50:01 2023, max compression
+gzip compressed data, was "google-cloud-video-live-stream-1.4.1.tar", last modified: Wed Jul  5 15:26:48 2023, max compression
```

## Comparing `google-cloud-video-live-stream-1.4.0.tar` & `google-cloud-video-live-stream-1.4.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:50:01.676483 google-cloud-video-live-stream-1.4.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4761 2023-03-27 15:50:01.676483 google-cloud-video-live-stream-1.4.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3815 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:50:01.668483 google-cloud-video-live-stream-1.4.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:50:01.668483 google-cloud-video-live-stream-1.4.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:50:01.668483 google-cloud-video-live-stream-1.4.0/google/cloud/video/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:50:01.668483 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream/
--rw-rw-r--   0 root         (0)     1003     3136 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:50:01.672483 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/
--rw-rw-r--   0 root         (0)     1003     2909 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     6345 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:50:01.672483 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:50:01.672483 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/livestream_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/livestream_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   104474 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/livestream_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   115215 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/livestream_service/client.py
--rw-rw-r--   0 root         (0)     1003    15587 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/livestream_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:50:01.672483 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/livestream_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/livestream_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    15984 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/livestream_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    34267 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/livestream_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    34939 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/livestream_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   110301 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/livestream_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:50:01.672483 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/types/
--rw-rw-r--   0 root         (0)     1003     2592 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    30278 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/types/outputs.py
--rw-rw-r--   0 root         (0)     1003    34991 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/types/resources.py
--rw-rw-r--   0 root         (0)     1003    31085 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:50:01.676483 google-cloud-video-live-stream-1.4.0/google_cloud_video_live_stream.egg-info/
--rw-r--r--   0 root         (0)     1003     4761 2023-03-27 15:50:01.000000 google-cloud-video-live-stream-1.4.0/google_cloud_video_live_stream.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1907 2023-03-27 15:50:01.000000 google-cloud-video-live-stream-1.4.0/google_cloud_video_live_stream.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:50:01.000000 google-cloud-video-live-stream-1.4.0/google_cloud_video_live_stream.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       39 2023-03-27 15:50:01.000000 google-cloud-video-live-stream-1.4.0/google_cloud_video_live_stream.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:50:01.000000 google-cloud-video-live-stream-1.4.0/google_cloud_video_live_stream.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 15:50:01.000000 google-cloud-video-live-stream-1.4.0/google_cloud_video_live_stream.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:50:01.000000 google-cloud-video-live-stream-1.4.0/google_cloud_video_live_stream.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:50:01.676483 google-cloud-video-live-stream-1.4.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2989 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:50:01.676483 google-cloud-video-live-stream-1.4.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:50:01.676483 google-cloud-video-live-stream-1.4.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:50:01.676483 google-cloud-video-live-stream-1.4.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:50:01.676483 google-cloud-video-live-stream-1.4.0/tests/unit/gapic/live_stream_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/tests/unit/gapic/live_stream_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   447174 2023-03-27 15:47:30.000000 google-cloud-video-live-stream-1.4.0/tests/unit/gapic/live_stream_v1/test_livestream_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:48.818067 google-cloud-video-live-stream-1.4.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4761 2023-07-05 15:26:48.818067 google-cloud-video-live-stream-1.4.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3815 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:48.810064 google-cloud-video-live-stream-1.4.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:48.810064 google-cloud-video-live-stream-1.4.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:48.810064 google-cloud-video-live-stream-1.4.1/google/cloud/video/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:48.810064 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream/
+-rw-rw-r--   0 root         (0)     1003     3136 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:48.810064 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/
+-rw-rw-r--   0 root         (0)     1003     2909 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6345 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:48.810064 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:48.814065 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/livestream_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/livestream_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   104508 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/livestream_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   115215 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/livestream_service/client.py
+-rw-rw-r--   0 root         (0)     1003    15587 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/livestream_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:48.814065 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/livestream_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/livestream_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15984 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/livestream_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    34267 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/livestream_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    34939 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/livestream_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   110289 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/livestream_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:48.814065 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2592 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    30278 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/types/outputs.py
+-rw-rw-r--   0 root         (0)     1003    34991 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/types/resources.py
+-rw-rw-r--   0 root         (0)     1003    31085 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:48.818067 google-cloud-video-live-stream-1.4.1/google_cloud_video_live_stream.egg-info/
+-rw-r--r--   0 root         (0)     1003     4761 2023-07-05 15:26:48.000000 google-cloud-video-live-stream-1.4.1/google_cloud_video_live_stream.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1907 2023-07-05 15:26:48.000000 google-cloud-video-live-stream-1.4.1/google_cloud_video_live_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:26:48.000000 google-cloud-video-live-stream-1.4.1/google_cloud_video_live_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       39 2023-07-05 15:26:48.000000 google-cloud-video-live-stream-1.4.1/google_cloud_video_live_stream.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:26:48.000000 google-cloud-video-live-stream-1.4.1/google_cloud_video_live_stream.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:26:48.000000 google-cloud-video-live-stream-1.4.1/google_cloud_video_live_stream.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:26:48.000000 google-cloud-video-live-stream-1.4.1/google_cloud_video_live_stream.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:26:48.818067 google-cloud-video-live-stream-1.4.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2989 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:48.818067 google-cloud-video-live-stream-1.4.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:48.818067 google-cloud-video-live-stream-1.4.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:48.818067 google-cloud-video-live-stream-1.4.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:26:48.818067 google-cloud-video-live-stream-1.4.1/tests/unit/gapic/live_stream_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/tests/unit/gapic/live_stream_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   447423 2023-07-05 15:23:46.000000 google-cloud-video-live-stream-1.4.1/tests/unit/gapic/live_stream_v1/test_livestream_service.py
```

### Comparing `google-cloud-video-live-stream-1.4.0/LICENSE` & `google-cloud-video-live-stream-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/MANIFEST.in` & `google-cloud-video-live-stream-1.4.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/PKG-INFO` & `google-cloud-video-live-stream-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-video-live-stream
-Version: 1.4.0
+Version: 1.4.1
 Summary: Google Cloud Video Live Stream API client library
 Home-page: https://github.com/googleapis/python-video-live-stream
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-video-live-stream-1.4.0/README.rst` & `google-cloud-video-live-stream-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream/__init__.py` & `google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream/gapic_version.py` & `google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream/gapic_version.py`

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
-__version__ = "1.4.0"  # {x-release-please-version}
+__version__ = "1.4.1"  # {x-release-please-version}
```

### Comparing `google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/__init__.py` & `google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/gapic_metadata.json` & `google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/gapic_version.py` & `google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/gapic_version.py`

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
-__version__ = "1.4.0"  # {x-release-please-version}
+__version__ = "1.4.1"  # {x-release-please-version}
```

### Comparing `google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/__init__.py` & `google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/livestream_service/__init__.py` & `google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/livestream_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/livestream_service/async_client.py` & `google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/livestream_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2563,15 +2563,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "LivestreamServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/livestream_service/client.py` & `google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/livestream_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/livestream_service/pagers.py` & `google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/livestream_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/livestream_service/transports/__init__.py` & `google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/livestream_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/livestream_service/transports/base.py` & `google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/livestream_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/livestream_service/transports/grpc.py` & `google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/livestream_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/livestream_service/transports/grpc_asyncio.py` & `google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/livestream_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/services/livestream_service/transports/rest.py` & `google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/services/livestream_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -2581,15 +2581,15 @@
 
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

### Comparing `google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/types/__init__.py` & `google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/types/outputs.py` & `google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/types/outputs.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/types/resources.py` & `google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/types/resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/google/cloud/video/live_stream_v1/types/service.py` & `google-cloud-video-live-stream-1.4.1/google/cloud/video/live_stream_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/google_cloud_video_live_stream.egg-info/PKG-INFO` & `google-cloud-video-live-stream-1.4.1/google_cloud_video_live_stream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-video-live-stream
-Version: 1.4.0
+Version: 1.4.1
 Summary: Google Cloud Video Live Stream API client library
 Home-page: https://github.com/googleapis/python-video-live-stream
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-video-live-stream-1.4.0/google_cloud_video_live_stream.egg-info/SOURCES.txt` & `google-cloud-video-live-stream-1.4.1/google_cloud_video_live_stream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/setup.py` & `google-cloud-video-live-stream-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/tests/__init__.py` & `google-cloud-video-live-stream-1.4.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/tests/unit/__init__.py` & `google-cloud-video-live-stream-1.4.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/tests/unit/gapic/__init__.py` & `google-cloud-video-live-stream-1.4.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/tests/unit/gapic/live_stream_v1/__init__.py` & `google-cloud-video-live-stream-1.4.1/tests/unit/gapic/live_stream_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-live-stream-1.4.0/tests/unit/gapic/live_stream_v1/test_livestream_service.py` & `google-cloud-video-live-stream-1.4.1/tests/unit/gapic/live_stream_v1/test_livestream_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1408,17 +1408,19 @@
                     resources.Channel(),
                     resources.Channel(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_channels(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3228,17 +3230,19 @@
                     resources.Input(),
                     resources.Input(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_inputs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3962,15 +3966,14 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_event), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = resources.Event(
             name="name_value",
             execute_now=True,
             state=resources.Event.State.SCHEDULED,
-            input_switch=resources.Event.InputSwitchTask(input_key="input_key_value"),
         )
         response = client.create_event(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.CreateEventRequest()
@@ -4611,17 +4614,19 @@
                     resources.Event(),
                     resources.Event(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_events(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4643,15 +4648,14 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_event), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = resources.Event(
             name="name_value",
             execute_now=True,
             state=resources.Event.State.SCHEDULED,
-            input_switch=resources.Event.InputSwitchTask(input_key="input_key_value"),
         )
         response = client.get_event(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.GetEventRequest()
@@ -9261,15 +9265,14 @@
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = resources.Event(
             name="name_value",
             execute_now=True,
             state=resources.Event.State.SCHEDULED,
-            input_switch=resources.Event.InputSwitchTask(input_key="input_key_value"),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = resources.Event.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -9939,15 +9942,14 @@
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = resources.Event(
             name="name_value",
             execute_now=True,
             state=resources.Event.State.SCHEDULED,
-            input_switch=resources.Event.InputSwitchTask(input_key="input_key_value"),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = resources.Event.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

