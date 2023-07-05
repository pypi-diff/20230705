# Comparing `tmp/google-cloud-policy-troubleshooter-1.8.1.tar.gz` & `tmp/google-cloud-policy-troubleshooter-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-policy-troubleshooter-1.8.1.tar", last modified: Mon Mar 27 14:54:57 2023, max compression
+gzip compressed data, was "google-cloud-policy-troubleshooter-1.8.2.tar", last modified: Wed Jul  5 15:54:36 2023, max compression
```

## Comparing `google-cloud-policy-troubleshooter-1.8.1.tar` & `google-cloud-policy-troubleshooter-1.8.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:57.463718 google-cloud-policy-troubleshooter-1.8.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5271 2023-03-27 14:54:57.463718 google-cloud-policy-troubleshooter-1.8.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4313 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:57.455716 google-cloud-policy-troubleshooter-1.8.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:57.455716 google-cloud-policy-troubleshooter-1.8.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:57.459717 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter/
--rw-rw-r--   0 root         (0)     1003     1506 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:57.459717 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/
--rw-rw-r--   0 root         (0)     1003     1281 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1083 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:57.459717 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:57.459717 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/services/iam_checker/
--rw-rw-r--   0 root         (0)     1003      753 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/services/iam_checker/__init__.py
--rw-rw-r--   0 root         (0)     1003    12280 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/services/iam_checker/async_client.py
--rw-rw-r--   0 root         (0)     1003    20942 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/services/iam_checker/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:57.459717 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/
--rw-rw-r--   0 root         (0)     1003     1344 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6117 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12044 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12254 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12240 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:57.463718 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/types/
--rw-rw-r--   0 root         (0)     1003     1015 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3071 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/types/checker.py
--rw-rw-r--   0 root         (0)     1003    14093 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/types/explanations.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:57.463718 google-cloud-policy-troubleshooter-1.8.1/google_cloud_policy_troubleshooter.egg-info/
--rw-r--r--   0 root         (0)     1003     5271 2023-03-27 14:54:57.000000 google-cloud-policy-troubleshooter-1.8.1/google_cloud_policy_troubleshooter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1827 2023-03-27 14:54:57.000000 google-cloud-policy-troubleshooter-1.8.1/google_cloud_policy_troubleshooter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:54:57.000000 google-cloud-policy-troubleshooter-1.8.1/google_cloud_policy_troubleshooter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:54:57.000000 google-cloud-policy-troubleshooter-1.8.1/google_cloud_policy_troubleshooter.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:54:57.000000 google-cloud-policy-troubleshooter-1.8.1/google_cloud_policy_troubleshooter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 14:54:57.000000 google-cloud-policy-troubleshooter-1.8.1/google_cloud_policy_troubleshooter.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:54:57.000000 google-cloud-policy-troubleshooter-1.8.1/google_cloud_policy_troubleshooter.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 14:54:57.463718 google-cloud-policy-troubleshooter-1.8.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3029 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:57.463718 google-cloud-policy-troubleshooter-1.8.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:57.463718 google-cloud-policy-troubleshooter-1.8.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:57.463718 google-cloud-policy-troubleshooter-1.8.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:57.463718 google-cloud-policy-troubleshooter-1.8.1/tests/unit/gapic/policytroubleshooter_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/tests/unit/gapic/policytroubleshooter_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    59589 2023-03-27 14:52:19.000000 google-cloud-policy-troubleshooter-1.8.1/tests/unit/gapic/policytroubleshooter_v1/test_iam_checker.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.663893 google-cloud-policy-troubleshooter-1.8.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5226 2023-07-05 15:54:36.663893 google-cloud-policy-troubleshooter-1.8.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4277 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.655893 google-cloud-policy-troubleshooter-1.8.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.655893 google-cloud-policy-troubleshooter-1.8.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.659893 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter/
+-rw-rw-r--   0 root         (0)     1003     1506 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.659893 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/
+-rw-rw-r--   0 root         (0)     1003     1281 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1083 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.659893 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.659893 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/
+-rw-rw-r--   0 root         (0)     1003      753 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12307 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/async_client.py
+-rw-rw-r--   0 root         (0)     1003    20942 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.659893 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/
+-rw-rw-r--   0 root         (0)     1003     1344 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6117 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12044 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12254 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12240 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.663893 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1015 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3071 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/types/checker.py
+-rw-rw-r--   0 root         (0)     1003    14093 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/types/explanations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.663893 google-cloud-policy-troubleshooter-1.8.2/google_cloud_policy_troubleshooter.egg-info/
+-rw-r--r--   0 root         (0)     1003     5226 2023-07-05 15:54:36.000000 google-cloud-policy-troubleshooter-1.8.2/google_cloud_policy_troubleshooter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1827 2023-07-05 15:54:36.000000 google-cloud-policy-troubleshooter-1.8.2/google_cloud_policy_troubleshooter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:36.000000 google-cloud-policy-troubleshooter-1.8.2/google_cloud_policy_troubleshooter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:54:36.000000 google-cloud-policy-troubleshooter-1.8.2/google_cloud_policy_troubleshooter.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:36.000000 google-cloud-policy-troubleshooter-1.8.2/google_cloud_policy_troubleshooter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:54:36.000000 google-cloud-policy-troubleshooter-1.8.2/google_cloud_policy_troubleshooter.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:54:36.000000 google-cloud-policy-troubleshooter-1.8.2/google_cloud_policy_troubleshooter.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:54:36.663893 google-cloud-policy-troubleshooter-1.8.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3020 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.663893 google-cloud-policy-troubleshooter-1.8.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.663893 google-cloud-policy-troubleshooter-1.8.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.663893 google-cloud-policy-troubleshooter-1.8.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.663893 google-cloud-policy-troubleshooter-1.8.2/tests/unit/gapic/policytroubleshooter_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/tests/unit/gapic/policytroubleshooter_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    59589 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/tests/unit/gapic/policytroubleshooter_v1/test_iam_checker.py
```

### Comparing `google-cloud-policy-troubleshooter-1.8.1/LICENSE` & `google-cloud-policy-troubleshooter-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.1/MANIFEST.in` & `google-cloud-policy-troubleshooter-1.8.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.1/PKG-INFO` & `google-cloud-policy-troubleshooter-1.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-policy-troubleshooter
-Version: 1.8.1
+Version: 1.8.2
 Summary: Google Cloud Policy Troubleshooter API client library
-Home-page: https://github.com/googleapis/python-policy-troubleshooter
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
 
-Python Client for IAM Policy Troubleshooter API API
-===================================================
+Python Client for IAM Policy Troubleshooter API
+===============================================
 
 |stable| |pypi| |versions|
 
-`IAM Policy Troubleshooter API API`_: makes it easier to understand why a user has access to a resource or doesn't have permission to call an API. Given an email, resource, and permission, Policy Troubleshooter examines all Identity and Access Management (IAM) policies that apply to the resource. It then reveals whether the member's roles include the permission on that resource and, if so, which policies bind the member to those roles.
+`IAM Policy Troubleshooter API`_: makes it easier to understand why a user has access to a resource or doesn't have permission to call an API. Given an email, resource, and permission, Policy Troubleshooter examines all Identity and Access Management (IAM) policies that apply to the resource. It then reveals whether the member's roles include the permission on that resource and, if so, which policies bind the member to those roles.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-policy-troubleshooter.svg
    :target: https://pypi.org/project/google-cloud-policy-troubleshooter/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-policy-troubleshooter.svg
    :target: https://pypi.org/project/google-cloud-policy-troubleshooter/
-.. _IAM Policy Troubleshooter API API: https://cloud.google.com/iam/docs/troubleshooting-access#rest-api/
+.. _IAM Policy Troubleshooter API: https://cloud.google.com/iam/docs/troubleshooting-access#rest-api/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/policytroubleshooter/latest
 .. _Product Documentation:  https://cloud.google.com/iam/docs/troubleshooting-access#rest-api/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the IAM Policy Troubleshooter API API.`_
+3. `Enable the IAM Policy Troubleshooter API.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the IAM Policy Troubleshooter API API.:  https://cloud.google.com/iam/docs/troubleshooting-access#rest-api/
+.. _Enable the IAM Policy Troubleshooter API.:  https://cloud.google.com/iam/docs/troubleshooting-access#rest-api/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-policy-troubleshooter
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for IAM Policy Troubleshooter API API
+-  Read the `Client Library Documentation`_ for IAM Policy Troubleshooter API
    to see other available methods on the client.
--  Read the `IAM Policy Troubleshooter API API Product documentation`_ to learn
+-  Read the `IAM Policy Troubleshooter API Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _IAM Policy Troubleshooter API API Product documentation:  https://cloud.google.com/iam/docs/troubleshooting-access#rest-api/
+.. _IAM Policy Troubleshooter API Product documentation:  https://cloud.google.com/iam/docs/troubleshooting-access#rest-api/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-policy-troubleshooter-1.8.1/README.rst` & `google-cloud-policy-troubleshooter-1.8.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for IAM Policy Troubleshooter API API
-===================================================
+Python Client for IAM Policy Troubleshooter API
+===============================================
 
 |stable| |pypi| |versions|
 
-`IAM Policy Troubleshooter API API`_: makes it easier to understand why a user has access to a resource or doesn't have permission to call an API. Given an email, resource, and permission, Policy Troubleshooter examines all Identity and Access Management (IAM) policies that apply to the resource. It then reveals whether the member's roles include the permission on that resource and, if so, which policies bind the member to those roles.
+`IAM Policy Troubleshooter API`_: makes it easier to understand why a user has access to a resource or doesn't have permission to call an API. Given an email, resource, and permission, Policy Troubleshooter examines all Identity and Access Management (IAM) policies that apply to the resource. It then reveals whether the member's roles include the permission on that resource and, if so, which policies bind the member to those roles.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-policy-troubleshooter.svg
    :target: https://pypi.org/project/google-cloud-policy-troubleshooter/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-policy-troubleshooter.svg
    :target: https://pypi.org/project/google-cloud-policy-troubleshooter/
-.. _IAM Policy Troubleshooter API API: https://cloud.google.com/iam/docs/troubleshooting-access#rest-api/
+.. _IAM Policy Troubleshooter API: https://cloud.google.com/iam/docs/troubleshooting-access#rest-api/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/policytroubleshooter/latest
 .. _Product Documentation:  https://cloud.google.com/iam/docs/troubleshooting-access#rest-api/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the IAM Policy Troubleshooter API API.`_
+3. `Enable the IAM Policy Troubleshooter API.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the IAM Policy Troubleshooter API API.:  https://cloud.google.com/iam/docs/troubleshooting-access#rest-api/
+.. _Enable the IAM Policy Troubleshooter API.:  https://cloud.google.com/iam/docs/troubleshooting-access#rest-api/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-policy-troubleshooter
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for IAM Policy Troubleshooter API API
+-  Read the `Client Library Documentation`_ for IAM Policy Troubleshooter API
    to see other available methods on the client.
--  Read the `IAM Policy Troubleshooter API API Product documentation`_ to learn
+-  Read the `IAM Policy Troubleshooter API Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _IAM Policy Troubleshooter API API Product documentation:  https://cloud.google.com/iam/docs/troubleshooting-access#rest-api/
+.. _IAM Policy Troubleshooter API Product documentation:  https://cloud.google.com/iam/docs/troubleshooting-access#rest-api/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter/__init__.py` & `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter/gapic_version.py` & `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter/gapic_version.py`

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
-__version__ = "1.8.1"  # {x-release-please-version}
+__version__ = "1.8.2"  # {x-release-please-version}
```

### Comparing `google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/__init__.py` & `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/gapic_metadata.json` & `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/gapic_version.py` & `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/gapic_version.py`

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
-__version__ = "1.8.1"  # {x-release-please-version}
+__version__ = "1.8.2"  # {x-release-please-version}
```

### Comparing `google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/services/__init__.py` & `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/services/iam_checker/__init__.py` & `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/services/iam_checker/async_client.py` & `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,15 +279,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "IamCheckerAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/services/iam_checker/client.py` & `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/__init__.py` & `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/base.py` & `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/grpc.py` & `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/grpc_asyncio.py` & `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/rest.py` & `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/types/__init__.py` & `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/types/checker.py` & `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/types/checker.py`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.1/google/cloud/policytroubleshooter_v1/types/explanations.py` & `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/types/explanations.py`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.1/google_cloud_policy_troubleshooter.egg-info/PKG-INFO` & `google-cloud-policy-troubleshooter-1.8.2/google_cloud_policy_troubleshooter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-policy-troubleshooter
-Version: 1.8.1
+Version: 1.8.2
 Summary: Google Cloud Policy Troubleshooter API client library
-Home-page: https://github.com/googleapis/python-policy-troubleshooter
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
 
-Python Client for IAM Policy Troubleshooter API API
-===================================================
+Python Client for IAM Policy Troubleshooter API
+===============================================
 
 |stable| |pypi| |versions|
 
-`IAM Policy Troubleshooter API API`_: makes it easier to understand why a user has access to a resource or doesn't have permission to call an API. Given an email, resource, and permission, Policy Troubleshooter examines all Identity and Access Management (IAM) policies that apply to the resource. It then reveals whether the member's roles include the permission on that resource and, if so, which policies bind the member to those roles.
+`IAM Policy Troubleshooter API`_: makes it easier to understand why a user has access to a resource or doesn't have permission to call an API. Given an email, resource, and permission, Policy Troubleshooter examines all Identity and Access Management (IAM) policies that apply to the resource. It then reveals whether the member's roles include the permission on that resource and, if so, which policies bind the member to those roles.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-policy-troubleshooter.svg
    :target: https://pypi.org/project/google-cloud-policy-troubleshooter/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-policy-troubleshooter.svg
    :target: https://pypi.org/project/google-cloud-policy-troubleshooter/
-.. _IAM Policy Troubleshooter API API: https://cloud.google.com/iam/docs/troubleshooting-access#rest-api/
+.. _IAM Policy Troubleshooter API: https://cloud.google.com/iam/docs/troubleshooting-access#rest-api/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/policytroubleshooter/latest
 .. _Product Documentation:  https://cloud.google.com/iam/docs/troubleshooting-access#rest-api/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the IAM Policy Troubleshooter API API.`_
+3. `Enable the IAM Policy Troubleshooter API.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the IAM Policy Troubleshooter API API.:  https://cloud.google.com/iam/docs/troubleshooting-access#rest-api/
+.. _Enable the IAM Policy Troubleshooter API.:  https://cloud.google.com/iam/docs/troubleshooting-access#rest-api/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-policy-troubleshooter
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for IAM Policy Troubleshooter API API
+-  Read the `Client Library Documentation`_ for IAM Policy Troubleshooter API
    to see other available methods on the client.
--  Read the `IAM Policy Troubleshooter API API Product documentation`_ to learn
+-  Read the `IAM Policy Troubleshooter API Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _IAM Policy Troubleshooter API API Product documentation:  https://cloud.google.com/iam/docs/troubleshooting-access#rest-api/
+.. _IAM Policy Troubleshooter API Product documentation:  https://cloud.google.com/iam/docs/troubleshooting-access#rest-api/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-policy-troubleshooter-1.8.1/google_cloud_policy_troubleshooter.egg-info/SOURCES.txt` & `google-cloud-policy-troubleshooter-1.8.2/google_cloud_policy_troubleshooter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.1/setup.py` & `google-cloud-policy-troubleshooter-1.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
-url = "https://github.com/googleapis/python-policy-troubleshooter"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-policy-troubleshooter-1.8.1/tests/__init__.py` & `google-cloud-policy-troubleshooter-1.8.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.1/tests/unit/__init__.py` & `google-cloud-policy-troubleshooter-1.8.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.1/tests/unit/gapic/__init__.py` & `google-cloud-policy-troubleshooter-1.8.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.1/tests/unit/gapic/policytroubleshooter_v1/__init__.py` & `google-cloud-policy-troubleshooter-1.8.2/tests/unit/gapic/policytroubleshooter_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.1/tests/unit/gapic/policytroubleshooter_v1/test_iam_checker.py` & `google-cloud-policy-troubleshooter-1.8.2/tests/unit/gapic/policytroubleshooter_v1/test_iam_checker.py`

 * *Files identical despite different names*

