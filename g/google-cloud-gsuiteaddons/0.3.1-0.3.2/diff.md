# Comparing `tmp/google-cloud-gsuiteaddons-0.3.1.tar.gz` & `tmp/google-cloud-gsuiteaddons-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-gsuiteaddons-0.3.1.tar", last modified: Mon Mar 27 16:06:11 2023, max compression
+gzip compressed data, was "google-cloud-gsuiteaddons-0.3.2.tar", last modified: Wed Jul  5 15:08:00 2023, max compression
```

## Comparing `google-cloud-gsuiteaddons-0.3.1.tar` & `google-cloud-gsuiteaddons-0.3.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:11.921116 google-cloud-gsuiteaddons-0.3.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4810 2023-03-27 16:06:11.921116 google-cloud-gsuiteaddons-0.3.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3892 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:11.913115 google-cloud-gsuiteaddons-0.3.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:11.913115 google-cloud-gsuiteaddons-0.3.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:11.913115 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons/
--rw-rw-r--   0 root         (0)     1003     1807 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:11.913115 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/
--rw-rw-r--   0 root         (0)     1003     1651 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4123 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:11.913115 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:11.917116 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/
--rw-rw-r--   0 root         (0)     1003      761 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/__init__.py
--rw-rw-r--   0 root         (0)     1003    48815 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/async_client.py
--rw-rw-r--   0 root         (0)     1003    60099 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/client.py
--rw-rw-r--   0 root         (0)     1003     5876 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:11.917116 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9638 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22748 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    23220 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    52175 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:11.917116 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/types/
--rw-rw-r--   0 root         (0)     1003     1387 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    12852 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/types/gsuiteaddons.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:11.921116 google-cloud-gsuiteaddons-0.3.1/google_cloud_gsuiteaddons.egg-info/
--rw-r--r--   0 root         (0)     1003     4810 2023-03-27 16:06:11.000000 google-cloud-gsuiteaddons-0.3.1/google_cloud_gsuiteaddons.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1650 2023-03-27 16:06:11.000000 google-cloud-gsuiteaddons-0.3.1/google_cloud_gsuiteaddons.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:06:11.000000 google-cloud-gsuiteaddons-0.3.1/google_cloud_gsuiteaddons.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 16:06:11.000000 google-cloud-gsuiteaddons-0.3.1/google_cloud_gsuiteaddons.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:06:11.000000 google-cloud-gsuiteaddons-0.3.1/google_cloud_gsuiteaddons.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      356 2023-03-27 16:06:11.000000 google-cloud-gsuiteaddons-0.3.1/google_cloud_gsuiteaddons.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 16:06:11.000000 google-cloud-gsuiteaddons-0.3.1/google_cloud_gsuiteaddons.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 16:06:11.921116 google-cloud-gsuiteaddons-0.3.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3049 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:11.921116 google-cloud-gsuiteaddons-0.3.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:11.921116 google-cloud-gsuiteaddons-0.3.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:11.921116 google-cloud-gsuiteaddons-0.3.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:06:11.921116 google-cloud-gsuiteaddons-0.3.1/tests/unit/gapic/gsuiteaddons_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/tests/unit/gapic/gsuiteaddons_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   242203 2023-03-27 16:03:18.000000 google-cloud-gsuiteaddons-0.3.1/tests/unit/gapic/gsuiteaddons_v1/test_g_suite_add_ons.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:08:00.142829 google-cloud-gsuiteaddons-0.3.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4810 2023-07-05 15:08:00.146830 google-cloud-gsuiteaddons-0.3.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3892 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:08:00.134826 google-cloud-gsuiteaddons-0.3.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:08:00.134826 google-cloud-gsuiteaddons-0.3.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:08:00.138827 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons/
+-rw-rw-r--   0 root         (0)     1003     1807 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:08:00.138827 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/
+-rw-rw-r--   0 root         (0)     1003     1651 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4123 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:08:00.138827 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:08:00.138827 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/
+-rw-rw-r--   0 root         (0)     1003      761 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/__init__.py
+-rw-rw-r--   0 root         (0)     1003    48844 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/async_client.py
+-rw-rw-r--   0 root         (0)     1003    60099 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/client.py
+-rw-rw-r--   0 root         (0)     1003     5876 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:08:00.142829 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9638 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22748 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    23220 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    52175 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:08:00.142829 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1387 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12852 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/types/gsuiteaddons.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:08:00.142829 google-cloud-gsuiteaddons-0.3.2/google_cloud_gsuiteaddons.egg-info/
+-rw-r--r--   0 root         (0)     1003     4810 2023-07-05 15:08:00.000000 google-cloud-gsuiteaddons-0.3.2/google_cloud_gsuiteaddons.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1650 2023-07-05 15:08:00.000000 google-cloud-gsuiteaddons-0.3.2/google_cloud_gsuiteaddons.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:08:00.000000 google-cloud-gsuiteaddons-0.3.2/google_cloud_gsuiteaddons.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:08:00.000000 google-cloud-gsuiteaddons-0.3.2/google_cloud_gsuiteaddons.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:08:00.000000 google-cloud-gsuiteaddons-0.3.2/google_cloud_gsuiteaddons.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      356 2023-07-05 15:08:00.000000 google-cloud-gsuiteaddons-0.3.2/google_cloud_gsuiteaddons.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:08:00.000000 google-cloud-gsuiteaddons-0.3.2/google_cloud_gsuiteaddons.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:08:00.146830 google-cloud-gsuiteaddons-0.3.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3049 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:08:00.142829 google-cloud-gsuiteaddons-0.3.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:08:00.142829 google-cloud-gsuiteaddons-0.3.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:08:00.142829 google-cloud-gsuiteaddons-0.3.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:08:00.142829 google-cloud-gsuiteaddons-0.3.2/tests/unit/gapic/gsuiteaddons_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/tests/unit/gapic/gsuiteaddons_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   242203 2023-07-05 15:05:15.000000 google-cloud-gsuiteaddons-0.3.2/tests/unit/gapic/gsuiteaddons_v1/test_g_suite_add_ons.py
```

### Comparing `google-cloud-gsuiteaddons-0.3.1/LICENSE` & `google-cloud-gsuiteaddons-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/MANIFEST.in` & `google-cloud-gsuiteaddons-0.3.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/PKG-INFO` & `google-cloud-gsuiteaddons-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-gsuiteaddons
-Version: 0.3.1
+Version: 0.3.2
 Summary: Google Cloud Gsuiteaddons API client library
 Home-page: https://github.com/googleapis/python-gsuiteaddons
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-gsuiteaddons-0.3.1/README.rst` & `google-cloud-gsuiteaddons-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons/__init__.py` & `google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons/gapic_version.py` & `google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons/gapic_version.py`

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
-__version__ = "0.3.1"  # {x-release-please-version}
+__version__ = "0.3.2"  # {x-release-please-version}
```

### Comparing `google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/__init__.py` & `google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/gapic_metadata.json` & `google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/gapic_version.py` & `google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/gapic_version.py`

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
-__version__ = "0.3.1"  # {x-release-please-version}
+__version__ = "0.3.2"  # {x-release-please-version}
```

### Comparing `google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/__init__.py` & `google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/__init__.py` & `google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/async_client.py` & `google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1181,15 +1181,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "GSuiteAddOnsAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/client.py` & `google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/pagers.py` & `google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/__init__.py` & `google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/base.py` & `google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/grpc.py` & `google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/grpc_asyncio.py` & `google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/rest.py` & `google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/services/g_suite_add_ons/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/types/__init__.py` & `google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/google/cloud/gsuiteaddons_v1/types/gsuiteaddons.py` & `google-cloud-gsuiteaddons-0.3.2/google/cloud/gsuiteaddons_v1/types/gsuiteaddons.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/google_cloud_gsuiteaddons.egg-info/PKG-INFO` & `google-cloud-gsuiteaddons-0.3.2/google_cloud_gsuiteaddons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-gsuiteaddons
-Version: 0.3.1
+Version: 0.3.2
 Summary: Google Cloud Gsuiteaddons API client library
 Home-page: https://github.com/googleapis/python-gsuiteaddons
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-gsuiteaddons-0.3.1/google_cloud_gsuiteaddons.egg-info/SOURCES.txt` & `google-cloud-gsuiteaddons-0.3.2/google_cloud_gsuiteaddons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/setup.py` & `google-cloud-gsuiteaddons-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/tests/__init__.py` & `google-cloud-gsuiteaddons-0.3.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/tests/unit/__init__.py` & `google-cloud-gsuiteaddons-0.3.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/tests/unit/gapic/__init__.py` & `google-cloud-gsuiteaddons-0.3.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/tests/unit/gapic/gsuiteaddons_v1/__init__.py` & `google-cloud-gsuiteaddons-0.3.2/tests/unit/gapic/gsuiteaddons_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gsuiteaddons-0.3.1/tests/unit/gapic/gsuiteaddons_v1/test_g_suite_add_ons.py` & `google-cloud-gsuiteaddons-0.3.2/tests/unit/gapic/gsuiteaddons_v1/test_g_suite_add_ons.py`

 * *Files identical despite different names*

