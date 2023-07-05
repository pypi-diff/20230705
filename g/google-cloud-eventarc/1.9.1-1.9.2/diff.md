# Comparing `tmp/google-cloud-eventarc-1.9.1.tar.gz` & `tmp/google-cloud-eventarc-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-eventarc-1.9.1.tar", last modified: Mon Mar 27 16:02:57 2023, max compression
+gzip compressed data, was "google-cloud-eventarc-1.9.2.tar", last modified: Wed Jul  5 15:53:09 2023, max compression
```

## Comparing `google-cloud-eventarc-1.9.1.tar` & `google-cloud-eventarc-1.9.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:02:57.430601 google-cloud-eventarc-1.9.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4704 2023-03-27 16:02:57.430601 google-cloud-eventarc-1.9.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3785 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:02:57.422600 google-cloud-eventarc-1.9.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:02:57.422600 google-cloud-eventarc-1.9.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:02:57.422600 google-cloud-eventarc-1.9.1/google/cloud/eventarc/
--rw-rw-r--   0 root         (0)     1003     3114 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:02:57.422600 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/
--rw-rw-r--   0 root         (0)     1003     2858 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     7528 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:02:57.422600 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:02:57.426601 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/eventarc/
--rw-rw-r--   0 root         (0)     1003      745 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/eventarc/__init__.py
--rw-rw-r--   0 root         (0)     1003   123854 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/eventarc/async_client.py
--rw-rw-r--   0 root         (0)     1003   140195 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/eventarc/client.py
--rw-rw-r--   0 root         (0)     1003    20862 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/eventarc/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:02:57.426601 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/eventarc/transports/
--rw-rw-r--   0 root         (0)     1003     1316 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/eventarc/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    16559 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/eventarc/transports/base.py
--rw-rw-r--   0 root         (0)     1003    40629 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/eventarc/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    41356 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/eventarc/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   135930 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/eventarc/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:02:57.426601 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/types/
--rw-rw-r--   0 root         (0)     1003     2591 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     5641 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/types/channel.py
--rw-rw-r--   0 root         (0)     1003     2927 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/types/channel_connection.py
--rw-rw-r--   0 root         (0)     1003     4479 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/types/discovery.py
--rw-rw-r--   0 root         (0)     1003    23161 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/types/eventarc.py
--rw-rw-r--   0 root         (0)     1003     2202 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/types/google_channel_config.py
--rw-rw-r--   0 root         (0)     1003    13664 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/types/trigger.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:02:57.426601 google-cloud-eventarc-1.9.1/google_cloud_eventarc.egg-info/
--rw-r--r--   0 root         (0)     1003     4704 2023-03-27 16:02:57.000000 google-cloud-eventarc-1.9.1/google_cloud_eventarc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1701 2023-03-27 16:02:57.000000 google-cloud-eventarc-1.9.1/google_cloud_eventarc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:02:57.000000 google-cloud-eventarc-1.9.1/google_cloud_eventarc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 16:02:57.000000 google-cloud-eventarc-1.9.1/google_cloud_eventarc.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:02:57.000000 google-cloud-eventarc-1.9.1/google_cloud_eventarc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 16:02:57.000000 google-cloud-eventarc-1.9.1/google_cloud_eventarc.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 16:02:57.000000 google-cloud-eventarc-1.9.1/google_cloud_eventarc.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 16:02:57.430601 google-cloud-eventarc-1.9.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2972 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:02:57.430601 google-cloud-eventarc-1.9.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:02:57.430601 google-cloud-eventarc-1.9.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:02:57.430601 google-cloud-eventarc-1.9.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:02:57.430601 google-cloud-eventarc-1.9.1/tests/unit/gapic/eventarc_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/tests/unit/gapic/eventarc_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   513164 2023-03-27 16:01:03.000000 google-cloud-eventarc-1.9.1/tests/unit/gapic/eventarc_v1/test_eventarc.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:09.369316 google-cloud-eventarc-1.9.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-eventarc-1.9.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-eventarc-1.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4672 2023-07-05 15:53:09.369316 google-cloud-eventarc-1.9.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3749 2023-07-05 15:46:58.000000 google-cloud-eventarc-1.9.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:09.361316 google-cloud-eventarc-1.9.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:09.361316 google-cloud-eventarc-1.9.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:09.361316 google-cloud-eventarc-1.9.2/google/cloud/eventarc/
+-rw-rw-r--   0 root         (0)     1003     3114 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:09.361316 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/
+-rw-rw-r--   0 root         (0)     1003     2858 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7528 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:09.361316 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:09.365316 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/eventarc/
+-rw-rw-r--   0 root         (0)     1003      745 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/eventarc/__init__.py
+-rw-rw-r--   0 root         (0)     1003   123879 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/eventarc/async_client.py
+-rw-rw-r--   0 root         (0)     1003   140195 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/eventarc/client.py
+-rw-rw-r--   0 root         (0)     1003    20862 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/eventarc/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:09.365316 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/eventarc/transports/
+-rw-rw-r--   0 root         (0)     1003     1316 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/eventarc/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16559 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/eventarc/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    40629 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/eventarc/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    41356 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/eventarc/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   135894 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/eventarc/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:09.365316 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2591 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5641 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/types/channel.py
+-rw-rw-r--   0 root         (0)     1003     2927 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/types/channel_connection.py
+-rw-rw-r--   0 root         (0)     1003     4479 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/types/discovery.py
+-rw-rw-r--   0 root         (0)     1003    23161 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/types/eventarc.py
+-rw-rw-r--   0 root         (0)     1003     2202 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/types/google_channel_config.py
+-rw-rw-r--   0 root         (0)     1003    13664 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/types/trigger.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:09.369316 google-cloud-eventarc-1.9.2/google_cloud_eventarc.egg-info/
+-rw-r--r--   0 root         (0)     1003     4672 2023-07-05 15:53:09.000000 google-cloud-eventarc-1.9.2/google_cloud_eventarc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1701 2023-07-05 15:53:09.000000 google-cloud-eventarc-1.9.2/google_cloud_eventarc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:09.000000 google-cloud-eventarc-1.9.2/google_cloud_eventarc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:53:09.000000 google-cloud-eventarc-1.9.2/google_cloud_eventarc.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:09.000000 google-cloud-eventarc-1.9.2/google_cloud_eventarc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:53:09.000000 google-cloud-eventarc-1.9.2/google_cloud_eventarc.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:53:09.000000 google-cloud-eventarc-1.9.2/google_cloud_eventarc.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:53:09.369316 google-cloud-eventarc-1.9.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2976 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:09.369316 google-cloud-eventarc-1.9.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:09.369316 google-cloud-eventarc-1.9.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:09.369316 google-cloud-eventarc-1.9.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:09.369316 google-cloud-eventarc-1.9.2/tests/unit/gapic/eventarc_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/tests/unit/gapic/eventarc_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   513960 2023-07-05 15:46:59.000000 google-cloud-eventarc-1.9.2/tests/unit/gapic/eventarc_v1/test_eventarc.py
```

### Comparing `google-cloud-eventarc-1.9.1/LICENSE` & `google-cloud-eventarc-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/MANIFEST.in` & `google-cloud-eventarc-1.9.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/PKG-INFO` & `google-cloud-eventarc-1.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-eventarc
-Version: 1.9.1
+Version: 1.9.2
 Summary: Google Cloud Eventarc API client library
-Home-page: https://github.com/googleapis/python-eventarc
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
 
-Python Client for Eventarc API
-==============================
+Python Client for Eventarc
+==========================
 
 |stable| |pypi| |versions|
 
-`Eventarc API`_: lets you asynchronously deliver events from Google services, SaaS, and your own apps using loosely coupled services that react to state changes. Eventarc requires no infrastructure management, you can optimize productivity and costs while building a modern, event-driven solution.
+`Eventarc`_: lets you asynchronously deliver events from Google services, SaaS, and your own apps using loosely coupled services that react to state changes. Eventarc requires no infrastructure management, you can optimize productivity and costs while building a modern, event-driven solution.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-eventarc.svg
    :target: https://pypi.org/project/google-cloud-eventarc/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-eventarc.svg
    :target: https://pypi.org/project/google-cloud-eventarc/
-.. _Eventarc API: https://cloud.google.com/eventarc/
+.. _Eventarc: https://cloud.google.com/eventarc/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/eventarc/latest
 .. _Product Documentation:  https://cloud.google.com/eventarc/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Eventarc API.`_
+3. `Enable the Eventarc.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Eventarc API.:  https://cloud.google.com/eventarc/
+.. _Enable the Eventarc.:  https://cloud.google.com/eventarc/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-eventarc
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Eventarc API
+-  Read the `Client Library Documentation`_ for Eventarc
    to see other available methods on the client.
--  Read the `Eventarc API Product documentation`_ to learn
+-  Read the `Eventarc Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Eventarc API Product documentation:  https://cloud.google.com/eventarc/
+.. _Eventarc Product documentation:  https://cloud.google.com/eventarc/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-eventarc-1.9.1/README.rst` & `google-cloud-eventarc-1.9.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Eventarc API
-==============================
+Python Client for Eventarc
+==========================
 
 |stable| |pypi| |versions|
 
-`Eventarc API`_: lets you asynchronously deliver events from Google services, SaaS, and your own apps using loosely coupled services that react to state changes. Eventarc requires no infrastructure management, you can optimize productivity and costs while building a modern, event-driven solution.
+`Eventarc`_: lets you asynchronously deliver events from Google services, SaaS, and your own apps using loosely coupled services that react to state changes. Eventarc requires no infrastructure management, you can optimize productivity and costs while building a modern, event-driven solution.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-eventarc.svg
    :target: https://pypi.org/project/google-cloud-eventarc/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-eventarc.svg
    :target: https://pypi.org/project/google-cloud-eventarc/
-.. _Eventarc API: https://cloud.google.com/eventarc/
+.. _Eventarc: https://cloud.google.com/eventarc/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/eventarc/latest
 .. _Product Documentation:  https://cloud.google.com/eventarc/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Eventarc API.`_
+3. `Enable the Eventarc.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Eventarc API.:  https://cloud.google.com/eventarc/
+.. _Enable the Eventarc.:  https://cloud.google.com/eventarc/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-eventarc
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Eventarc API
+-  Read the `Client Library Documentation`_ for Eventarc
    to see other available methods on the client.
--  Read the `Eventarc API Product documentation`_ to learn
+-  Read the `Eventarc Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Eventarc API Product documentation:  https://cloud.google.com/eventarc/
+.. _Eventarc Product documentation:  https://cloud.google.com/eventarc/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc/__init__.py` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc/gapic_version.py` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc/gapic_version.py`

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
-__version__ = "1.9.1"  # {x-release-please-version}
+__version__ = "1.9.2"  # {x-release-please-version}
```

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/__init__.py` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/gapic_metadata.json` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/gapic_version.py` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/gapic_version.py`

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
-__version__ = "1.9.1"  # {x-release-please-version}
+__version__ = "1.9.2"  # {x-release-please-version}
```

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/__init__.py` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/eventarc/__init__.py` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/eventarc/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/eventarc/async_client.py` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/eventarc/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3061,15 +3061,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "EventarcAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/eventarc/client.py` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/eventarc/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/eventarc/pagers.py` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/eventarc/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/eventarc/transports/__init__.py` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/eventarc/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/eventarc/transports/base.py` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/eventarc/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/eventarc/transports/grpc.py` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/eventarc/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/eventarc/transports/grpc_asyncio.py` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/eventarc/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/services/eventarc/transports/rest.py` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/services/eventarc/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -3086,15 +3086,15 @@
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
@@ -3168,15 +3168,15 @@
 
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
@@ -3237,15 +3237,15 @@
 
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

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/types/__init__.py` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/types/channel.py` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/types/channel.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/types/channel_connection.py` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/types/channel_connection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/types/discovery.py` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/types/discovery.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/types/eventarc.py` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/types/eventarc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/types/google_channel_config.py` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/types/google_channel_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/google/cloud/eventarc_v1/types/trigger.py` & `google-cloud-eventarc-1.9.2/google/cloud/eventarc_v1/types/trigger.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/google_cloud_eventarc.egg-info/PKG-INFO` & `google-cloud-eventarc-1.9.2/google_cloud_eventarc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-eventarc
-Version: 1.9.1
+Version: 1.9.2
 Summary: Google Cloud Eventarc API client library
-Home-page: https://github.com/googleapis/python-eventarc
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
 
-Python Client for Eventarc API
-==============================
+Python Client for Eventarc
+==========================
 
 |stable| |pypi| |versions|
 
-`Eventarc API`_: lets you asynchronously deliver events from Google services, SaaS, and your own apps using loosely coupled services that react to state changes. Eventarc requires no infrastructure management, you can optimize productivity and costs while building a modern, event-driven solution.
+`Eventarc`_: lets you asynchronously deliver events from Google services, SaaS, and your own apps using loosely coupled services that react to state changes. Eventarc requires no infrastructure management, you can optimize productivity and costs while building a modern, event-driven solution.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-eventarc.svg
    :target: https://pypi.org/project/google-cloud-eventarc/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-eventarc.svg
    :target: https://pypi.org/project/google-cloud-eventarc/
-.. _Eventarc API: https://cloud.google.com/eventarc/
+.. _Eventarc: https://cloud.google.com/eventarc/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/eventarc/latest
 .. _Product Documentation:  https://cloud.google.com/eventarc/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Eventarc API.`_
+3. `Enable the Eventarc.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Eventarc API.:  https://cloud.google.com/eventarc/
+.. _Enable the Eventarc.:  https://cloud.google.com/eventarc/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-eventarc
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Eventarc API
+-  Read the `Client Library Documentation`_ for Eventarc
    to see other available methods on the client.
--  Read the `Eventarc API Product documentation`_ to learn
+-  Read the `Eventarc Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Eventarc API Product documentation:  https://cloud.google.com/eventarc/
+.. _Eventarc Product documentation:  https://cloud.google.com/eventarc/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-eventarc-1.9.1/google_cloud_eventarc.egg-info/SOURCES.txt` & `google-cloud-eventarc-1.9.2/google_cloud_eventarc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/setup.py` & `google-cloud-eventarc-1.9.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
-url = "https://github.com/googleapis/python-eventarc"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-eventarc-1.9.1/tests/__init__.py` & `google-cloud-eventarc-1.9.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/tests/unit/__init__.py` & `google-cloud-eventarc-1.9.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/tests/unit/gapic/__init__.py` & `google-cloud-eventarc-1.9.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/tests/unit/gapic/eventarc_v1/__init__.py` & `google-cloud-eventarc-1.9.2/tests/unit/gapic/eventarc_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-eventarc-1.9.1/tests/unit/gapic/eventarc_v1/test_eventarc.py` & `google-cloud-eventarc-1.9.2/tests/unit/gapic/eventarc_v1/test_eventarc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1350,17 +1350,19 @@
                     trigger.Trigger(),
                     trigger.Trigger(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_triggers(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2751,17 +2753,19 @@
                     channel.Channel(),
                     channel.Channel(),
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
@@ -4115,17 +4119,19 @@
                     discovery.Provider(),
                     discovery.Provider(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_providers(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4821,17 +4827,19 @@
                     channel_connection.ChannelConnection(),
                     channel_connection.ChannelConnection(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_channel_connections(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

