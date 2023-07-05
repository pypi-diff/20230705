# Comparing `tmp/google-cloud-monitoring-metrics-scopes-1.4.2.tar.gz` & `tmp/google-cloud-monitoring-metrics-scopes-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-monitoring-metrics-scopes-1.4.2.tar", last modified: Mon Mar 27 14:58:54 2023, max compression
+gzip compressed data, was "google-cloud-monitoring-metrics-scopes-1.4.3.tar", last modified: Wed Jul  5 15:54:05 2023, max compression
```

## Comparing `google-cloud-monitoring-metrics-scopes-1.4.2.tar` & `google-cloud-monitoring-metrics-scopes-1.4.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:54.089772 google-cloud-monitoring-metrics-scopes-1.4.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4739 2023-03-27 14:58:54.089772 google-cloud-monitoring-metrics-scopes-1.4.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3769 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:54.081772 google-cloud-monitoring-metrics-scopes-1.4.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:54.081772 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:54.081772 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope/
--rw-rw-r--   0 root         (0)     1003     1726 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       99 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:54.085772 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/
--rw-rw-r--   0 root         (0)     1003     1482 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1727 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       99 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:54.085772 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:54.085772 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/
--rw-rw-r--   0 root         (0)     1003      765 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/__init__.py
--rw-rw-r--   0 root         (0)     1003    28906 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/async_client.py
--rw-rw-r--   0 root         (0)     1003    38850 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:54.085772 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/transports/
--rw-rw-r--   0 root         (0)     1003     1184 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8077 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/transports/base.py
--rw-rw-r--   0 root         (0)     1003    16749 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17096 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:54.085772 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/types/
--rw-rw-r--   0 root         (0)     1003     1197 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3676 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/types/metrics_scope.py
--rw-rw-r--   0 root         (0)     1003     5917 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/types/metrics_scopes.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:54.085772 google-cloud-monitoring-metrics-scopes-1.4.2/google_cloud_monitoring_metrics_scopes.egg-info/
--rw-r--r--   0 root         (0)     1003     4739 2023-03-27 14:58:54.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google_cloud_monitoring_metrics_scopes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1890 2023-03-27 14:58:54.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google_cloud_monitoring_metrics_scopes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:58:54.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google_cloud_monitoring_metrics_scopes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:58:54.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google_cloud_monitoring_metrics_scopes.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:58:54.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google_cloud_monitoring_metrics_scopes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 14:58:54.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google_cloud_monitoring_metrics_scopes.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:58:54.000000 google-cloud-monitoring-metrics-scopes-1.4.2/google_cloud_monitoring_metrics_scopes.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 14:58:54.089772 google-cloud-monitoring-metrics-scopes-1.4.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2998 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:54.089772 google-cloud-monitoring-metrics-scopes-1.4.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:54.089772 google-cloud-monitoring-metrics-scopes-1.4.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:54.089772 google-cloud-monitoring-metrics-scopes-1.4.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:54.089772 google-cloud-monitoring-metrics-scopes-1.4.2/tests/unit/gapic/monitoring_metrics_scope_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/tests/unit/gapic/monitoring_metrics_scope_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    83589 2023-03-27 14:56:17.000000 google-cloud-monitoring-metrics-scopes-1.4.2/tests/unit/gapic/monitoring_metrics_scope_v1/test_metrics_scopes.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:05.292576 google-cloud-monitoring-metrics-scopes-1.4.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4690 2023-07-05 15:54:05.292576 google-cloud-monitoring-metrics-scopes-1.4.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3733 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:05.288576 google-cloud-monitoring-metrics-scopes-1.4.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:05.288576 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:05.288576 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope/
+-rw-rw-r--   0 root         (0)     1003     1726 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       99 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:05.292576 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/
+-rw-rw-r--   0 root         (0)     1003     1482 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1727 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       99 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:05.292576 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:05.292576 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/__init__.py
+-rw-rw-r--   0 root         (0)     1003    28936 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/async_client.py
+-rw-rw-r--   0 root         (0)     1003    38850 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:05.292576 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/transports/
+-rw-rw-r--   0 root         (0)     1003     1184 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8077 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    16749 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17096 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:05.292576 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1197 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3676 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/types/metrics_scope.py
+-rw-rw-r--   0 root         (0)     1003     5917 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/types/metrics_scopes.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:05.292576 google-cloud-monitoring-metrics-scopes-1.4.3/google_cloud_monitoring_metrics_scopes.egg-info/
+-rw-r--r--   0 root         (0)     1003     4690 2023-07-05 15:54:05.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google_cloud_monitoring_metrics_scopes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1890 2023-07-05 15:54:05.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google_cloud_monitoring_metrics_scopes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:05.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google_cloud_monitoring_metrics_scopes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:54:05.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google_cloud_monitoring_metrics_scopes.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:05.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google_cloud_monitoring_metrics_scopes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:54:05.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google_cloud_monitoring_metrics_scopes.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:54:05.000000 google-cloud-monitoring-metrics-scopes-1.4.3/google_cloud_monitoring_metrics_scopes.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:54:05.296576 google-cloud-monitoring-metrics-scopes-1.4.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2985 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:05.292576 google-cloud-monitoring-metrics-scopes-1.4.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:05.292576 google-cloud-monitoring-metrics-scopes-1.4.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:05.292576 google-cloud-monitoring-metrics-scopes-1.4.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:05.292576 google-cloud-monitoring-metrics-scopes-1.4.3/tests/unit/gapic/monitoring_metrics_scope_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/tests/unit/gapic/monitoring_metrics_scope_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    83589 2023-07-05 15:46:59.000000 google-cloud-monitoring-metrics-scopes-1.4.3/tests/unit/gapic/monitoring_metrics_scope_v1/test_metrics_scopes.py
```

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/LICENSE` & `google-cloud-monitoring-metrics-scopes-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/MANIFEST.in` & `google-cloud-monitoring-metrics-scopes-1.4.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/PKG-INFO` & `google-cloud-monitoring-metrics-scopes-1.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-monitoring-metrics-scopes
-Version: 1.4.2
+Version: 1.4.3
 Summary: Google Cloud Monitoring Metrics Scopes API client library
-Home-page: https://github.com/googleapis/python-monitoring-metrics-scopes
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
 
-Python Client for Metrics Scopes API
-====================================
+Python Client for Metrics Scopes
+================================
 
 |stable| |pypi| |versions|
 
-`Metrics Scopes API`_: Manages your Cloud Monitoring data and configurations.
+`Metrics Scopes`_: Manages your Cloud Monitoring data and configurations.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-monitoring-metrics-scopes.svg
    :target: https://pypi.org/project/google-cloud-monitoring-metrics-scopes/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-monitoring-metrics-scopes.svg
    :target: https://pypi.org/project/google-cloud-monitoring-metrics-scopes/
-.. _Metrics Scopes API: https://cloud.google.com/monitoring/docs
+.. _Metrics Scopes: https://cloud.google.com/monitoring/docs
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/google-cloud-monitoring-metrics-scopes/latest
 .. _Product Documentation:  https://cloud.google.com/monitoring/docs
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Metrics Scopes API.`_
+3. `Enable the Metrics Scopes.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Metrics Scopes API.:  https://cloud.google.com/monitoring/docs
+.. _Enable the Metrics Scopes.:  https://cloud.google.com/monitoring/docs
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-monitoring-metrics-scopes
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Metrics Scopes API
+-  Read the `Client Library Documentation`_ for Metrics Scopes
    to see other available methods on the client.
--  Read the `Metrics Scopes API Product documentation`_ to learn
+-  Read the `Metrics Scopes Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Metrics Scopes API Product documentation:  https://cloud.google.com/monitoring/docs
+.. _Metrics Scopes Product documentation:  https://cloud.google.com/monitoring/docs
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/README.rst` & `google-cloud-monitoring-metrics-scopes-1.4.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Metrics Scopes API
-====================================
+Python Client for Metrics Scopes
+================================
 
 |stable| |pypi| |versions|
 
-`Metrics Scopes API`_: Manages your Cloud Monitoring data and configurations.
+`Metrics Scopes`_: Manages your Cloud Monitoring data and configurations.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-monitoring-metrics-scopes.svg
    :target: https://pypi.org/project/google-cloud-monitoring-metrics-scopes/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-monitoring-metrics-scopes.svg
    :target: https://pypi.org/project/google-cloud-monitoring-metrics-scopes/
-.. _Metrics Scopes API: https://cloud.google.com/monitoring/docs
+.. _Metrics Scopes: https://cloud.google.com/monitoring/docs
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/google-cloud-monitoring-metrics-scopes/latest
 .. _Product Documentation:  https://cloud.google.com/monitoring/docs
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Metrics Scopes API.`_
+3. `Enable the Metrics Scopes.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Metrics Scopes API.:  https://cloud.google.com/monitoring/docs
+.. _Enable the Metrics Scopes.:  https://cloud.google.com/monitoring/docs
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-monitoring-metrics-scopes
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Metrics Scopes API
+-  Read the `Client Library Documentation`_ for Metrics Scopes
    to see other available methods on the client.
--  Read the `Metrics Scopes API Product documentation`_ to learn
+-  Read the `Metrics Scopes Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Metrics Scopes API Product documentation:  https://cloud.google.com/monitoring/docs
+.. _Metrics Scopes Product documentation:  https://cloud.google.com/monitoring/docs
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope/__init__.py` & `google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope/gapic_version.py` & `google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.4.2"  # {x-release-please-version}
+__version__ = "1.4.3"  # {x-release-please-version}
```

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/__init__.py` & `google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/gapic_metadata.json` & `google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/gapic_version.py` & `google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.4.2"  # {x-release-please-version}
+__version__ = "1.4.3"  # {x-release-please-version}
```

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/services/__init__.py` & `google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/__init__.py` & `google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/async_client.py` & `google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -673,15 +673,15 @@
             empty_pb2.Empty,
             metadata_type=metrics_scopes.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "MetricsScopesAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/client.py` & `google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/transports/__init__.py` & `google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/transports/base.py` & `google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/transports/grpc.py` & `google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/transports/grpc_asyncio.py` & `google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/services/metrics_scopes/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/types/__init__.py` & `google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/types/metrics_scope.py` & `google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/types/metrics_scope.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/google/cloud/monitoring_metrics_scope_v1/types/metrics_scopes.py` & `google-cloud-monitoring-metrics-scopes-1.4.3/google/cloud/monitoring_metrics_scope_v1/types/metrics_scopes.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/google_cloud_monitoring_metrics_scopes.egg-info/PKG-INFO` & `google-cloud-monitoring-metrics-scopes-1.4.3/google_cloud_monitoring_metrics_scopes.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-monitoring-metrics-scopes
-Version: 1.4.2
+Version: 1.4.3
 Summary: Google Cloud Monitoring Metrics Scopes API client library
-Home-page: https://github.com/googleapis/python-monitoring-metrics-scopes
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
 
-Python Client for Metrics Scopes API
-====================================
+Python Client for Metrics Scopes
+================================
 
 |stable| |pypi| |versions|
 
-`Metrics Scopes API`_: Manages your Cloud Monitoring data and configurations.
+`Metrics Scopes`_: Manages your Cloud Monitoring data and configurations.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-monitoring-metrics-scopes.svg
    :target: https://pypi.org/project/google-cloud-monitoring-metrics-scopes/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-monitoring-metrics-scopes.svg
    :target: https://pypi.org/project/google-cloud-monitoring-metrics-scopes/
-.. _Metrics Scopes API: https://cloud.google.com/monitoring/docs
+.. _Metrics Scopes: https://cloud.google.com/monitoring/docs
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/google-cloud-monitoring-metrics-scopes/latest
 .. _Product Documentation:  https://cloud.google.com/monitoring/docs
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Metrics Scopes API.`_
+3. `Enable the Metrics Scopes.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Metrics Scopes API.:  https://cloud.google.com/monitoring/docs
+.. _Enable the Metrics Scopes.:  https://cloud.google.com/monitoring/docs
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-monitoring-metrics-scopes
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Metrics Scopes API
+-  Read the `Client Library Documentation`_ for Metrics Scopes
    to see other available methods on the client.
--  Read the `Metrics Scopes API Product documentation`_ to learn
+-  Read the `Metrics Scopes Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Metrics Scopes API Product documentation:  https://cloud.google.com/monitoring/docs
+.. _Metrics Scopes Product documentation:  https://cloud.google.com/monitoring/docs
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/google_cloud_monitoring_metrics_scopes.egg-info/SOURCES.txt` & `google-cloud-monitoring-metrics-scopes-1.4.3/google_cloud_monitoring_metrics_scopes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/setup.py` & `google-cloud-monitoring-metrics-scopes-1.4.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-monitoring-metrics-scopes"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/tests/__init__.py` & `google-cloud-monitoring-metrics-scopes-1.4.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/tests/unit/__init__.py` & `google-cloud-monitoring-metrics-scopes-1.4.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/tests/unit/gapic/__init__.py` & `google-cloud-monitoring-metrics-scopes-1.4.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/tests/unit/gapic/monitoring_metrics_scope_v1/__init__.py` & `google-cloud-monitoring-metrics-scopes-1.4.3/tests/unit/gapic/monitoring_metrics_scope_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-metrics-scopes-1.4.2/tests/unit/gapic/monitoring_metrics_scope_v1/test_metrics_scopes.py` & `google-cloud-monitoring-metrics-scopes-1.4.3/tests/unit/gapic/monitoring_metrics_scope_v1/test_metrics_scopes.py`

 * *Files identical despite different names*

