# Comparing `tmp/google-cloud-datacatalog-lineage-0.2.2.tar.gz` & `tmp/google-cloud-datacatalog-lineage-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-datacatalog-lineage-0.2.2.tar", last modified: Mon Mar 27 14:58:32 2023, max compression
+gzip compressed data, was "google-cloud-datacatalog-lineage-0.2.3.tar", last modified: Wed Jul  5 15:51:54 2023, max compression
```

## Comparing `google-cloud-datacatalog-lineage-0.2.2.tar` & `google-cloud-datacatalog-lineage-0.2.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:32.715566 google-cloud-datacatalog-lineage-0.2.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4866 2023-03-27 14:58:32.715566 google-cloud-datacatalog-lineage-0.2.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3934 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:32.707566 google-cloud-datacatalog-lineage-0.2.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:32.707566 google-cloud-datacatalog-lineage-0.2.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:32.707566 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:32.711566 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage/
--rw-rw-r--   0 root         (0)     1003     2539 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:32.711566 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/
--rw-rw-r--   0 root         (0)     1003     2379 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     6514 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:32.711566 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:32.711566 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/lineage/
--rw-rw-r--   0 root         (0)     1003      741 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/lineage/__init__.py
--rw-rw-r--   0 root         (0)     1003    89426 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/lineage/async_client.py
--rw-rw-r--   0 root         (0)     1003   102203 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/lineage/client.py
--rw-rw-r--   0 root         (0)     1003    26060 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/lineage/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:32.711566 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/lineage/transports/
--rw-rw-r--   0 root         (0)     1003     1302 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/lineage/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    13470 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/lineage/transports/base.py
--rw-rw-r--   0 root         (0)     1003    33602 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/lineage/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    34234 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/lineage/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   103876 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/lineage/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:32.715566 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/types/
--rw-rw-r--   0 root         (0)     1003     2136 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    36413 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/types/lineage.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:32.715566 google-cloud-datacatalog-lineage-0.2.2/google_cloud_datacatalog_lineage.egg-info/
--rw-r--r--   0 root         (0)     1003     4866 2023-03-27 14:58:32.000000 google-cloud-datacatalog-lineage-0.2.2/google_cloud_datacatalog_lineage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1727 2023-03-27 14:58:32.000000 google-cloud-datacatalog-lineage-0.2.2/google_cloud_datacatalog_lineage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:58:32.000000 google-cloud-datacatalog-lineage-0.2.2/google_cloud_datacatalog_lineage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       45 2023-03-27 14:58:32.000000 google-cloud-datacatalog-lineage-0.2.2/google_cloud_datacatalog_lineage.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:58:32.000000 google-cloud-datacatalog-lineage-0.2.2/google_cloud_datacatalog_lineage.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 14:58:32.000000 google-cloud-datacatalog-lineage-0.2.2/google_cloud_datacatalog_lineage.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:58:32.000000 google-cloud-datacatalog-lineage-0.2.2/google_cloud_datacatalog_lineage.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-03-27 14:58:32.715566 google-cloud-datacatalog-lineage-0.2.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2996 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:32.715566 google-cloud-datacatalog-lineage-0.2.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:32.715566 google-cloud-datacatalog-lineage-0.2.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:32.715566 google-cloud-datacatalog-lineage-0.2.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:32.715566 google-cloud-datacatalog-lineage-0.2.2/tests/unit/gapic/lineage_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/tests/unit/gapic/lineage_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   408024 2023-03-27 14:55:35.000000 google-cloud-datacatalog-lineage-0.2.2/tests/unit/gapic/lineage_v1/test_lineage.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:54.160817 google-cloud-datacatalog-lineage-0.2.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4866 2023-07-05 15:51:54.160817 google-cloud-datacatalog-lineage-0.2.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3934 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:54.152817 google-cloud-datacatalog-lineage-0.2.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:54.152817 google-cloud-datacatalog-lineage-0.2.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:54.152817 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:54.156818 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage/
+-rw-rw-r--   0 root         (0)     1003     2539 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:54.156818 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/
+-rw-rw-r--   0 root         (0)     1003     2379 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6514 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:54.156818 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:54.156818 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/lineage/
+-rw-rw-r--   0 root         (0)     1003      741 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/lineage/__init__.py
+-rw-rw-r--   0 root         (0)     1003    89450 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/lineage/async_client.py
+-rw-rw-r--   0 root         (0)     1003   102203 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/lineage/client.py
+-rw-rw-r--   0 root         (0)     1003    26060 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/lineage/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:54.156818 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/lineage/transports/
+-rw-rw-r--   0 root         (0)     1003     1302 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/lineage/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13470 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/lineage/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    33602 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/lineage/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    34234 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/lineage/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   103864 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/lineage/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:54.160817 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2136 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    36413 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/types/lineage.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:54.160817 google-cloud-datacatalog-lineage-0.2.3/google_cloud_datacatalog_lineage.egg-info/
+-rw-r--r--   0 root         (0)     1003     4866 2023-07-05 15:51:54.000000 google-cloud-datacatalog-lineage-0.2.3/google_cloud_datacatalog_lineage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1727 2023-07-05 15:51:54.000000 google-cloud-datacatalog-lineage-0.2.3/google_cloud_datacatalog_lineage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:51:54.000000 google-cloud-datacatalog-lineage-0.2.3/google_cloud_datacatalog_lineage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       45 2023-07-05 15:51:54.000000 google-cloud-datacatalog-lineage-0.2.3/google_cloud_datacatalog_lineage.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:51:54.000000 google-cloud-datacatalog-lineage-0.2.3/google_cloud_datacatalog_lineage.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:51:54.000000 google-cloud-datacatalog-lineage-0.2.3/google_cloud_datacatalog_lineage.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:51:54.000000 google-cloud-datacatalog-lineage-0.2.3/google_cloud_datacatalog_lineage.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:51:54.160817 google-cloud-datacatalog-lineage-0.2.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2996 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:54.160817 google-cloud-datacatalog-lineage-0.2.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:54.160817 google-cloud-datacatalog-lineage-0.2.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:54.160817 google-cloud-datacatalog-lineage-0.2.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:54.160817 google-cloud-datacatalog-lineage-0.2.3/tests/unit/gapic/lineage_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/tests/unit/gapic/lineage_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   409019 2023-07-05 15:46:58.000000 google-cloud-datacatalog-lineage-0.2.3/tests/unit/gapic/lineage_v1/test_lineage.py
```

### Comparing `google-cloud-datacatalog-lineage-0.2.2/LICENSE` & `google-cloud-datacatalog-lineage-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/MANIFEST.in` & `google-cloud-datacatalog-lineage-0.2.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/PKG-INFO` & `google-cloud-datacatalog-lineage-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-datacatalog-lineage
-Version: 0.2.2
+Version: 0.2.3
 Summary: Google Cloud Datacatalog Lineage API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-datacatalog-lineage-0.2.2/README.rst` & `google-cloud-datacatalog-lineage-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage/__init__.py` & `google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage/gapic_version.py` & `google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage/gapic_version.py`

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
-__version__ = "0.2.2"  # {x-release-please-version}
+__version__ = "0.2.3"  # {x-release-please-version}
```

### Comparing `google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/__init__.py` & `google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/gapic_metadata.json` & `google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/gapic_version.py` & `google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/gapic_version.py`

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
-__version__ = "0.2.2"  # {x-release-please-version}
+__version__ = "0.2.3"  # {x-release-please-version}
```

### Comparing `google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/__init__.py` & `google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/lineage/__init__.py` & `google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/lineage/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/lineage/async_client.py` & `google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/lineage/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2222,15 +2222,15 @@
         await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "LineageAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/lineage/client.py` & `google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/lineage/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/lineage/pagers.py` & `google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/lineage/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/lineage/transports/__init__.py` & `google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/lineage/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/lineage/transports/base.py` & `google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/lineage/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/lineage/transports/grpc.py` & `google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/lineage/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/lineage/transports/grpc_asyncio.py` & `google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/lineage/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/services/lineage/transports/rest.py` & `google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/services/lineage/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -2421,15 +2421,15 @@
 
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

### Comparing `google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/types/__init__.py` & `google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/google/cloud/datacatalog/lineage_v1/types/lineage.py` & `google-cloud-datacatalog-lineage-0.2.3/google/cloud/datacatalog/lineage_v1/types/lineage.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/google_cloud_datacatalog_lineage.egg-info/PKG-INFO` & `google-cloud-datacatalog-lineage-0.2.3/google_cloud_datacatalog_lineage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-datacatalog-lineage
-Version: 0.2.2
+Version: 0.2.3
 Summary: Google Cloud Datacatalog Lineage API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-datacatalog-lineage-0.2.2/google_cloud_datacatalog_lineage.egg-info/SOURCES.txt` & `google-cloud-datacatalog-lineage-0.2.3/google_cloud_datacatalog_lineage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/setup.py` & `google-cloud-datacatalog-lineage-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/tests/__init__.py` & `google-cloud-datacatalog-lineage-0.2.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/tests/unit/__init__.py` & `google-cloud-datacatalog-lineage-0.2.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/tests/unit/gapic/__init__.py` & `google-cloud-datacatalog-lineage-0.2.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/tests/unit/gapic/lineage_v1/__init__.py` & `google-cloud-datacatalog-lineage-0.2.3/tests/unit/gapic/lineage_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-lineage-0.2.2/tests/unit/gapic/lineage_v1/test_lineage.py` & `google-cloud-datacatalog-lineage-0.2.3/tests/unit/gapic/lineage_v1/test_lineage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1796,17 +1796,19 @@
                     lineage.Process(),
                     lineage.Process(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_processes(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3170,17 +3172,19 @@
                     lineage.Run(),
                     lineage.Run(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_runs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4340,17 +4344,19 @@
                     lineage.LineageEvent(),
                     lineage.LineageEvent(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_lineage_events(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4912,17 +4918,19 @@
                     lineage.Link(),
                     lineage.Link(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.search_links(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5269,17 +5277,19 @@
                     lineage.ProcessLinks(),
                     lineage.ProcessLinks(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.batch_search_link_processes(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

