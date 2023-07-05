# Comparing `tmp/google-cloud-phishing-protection-1.9.0.tar.gz` & `tmp/google-cloud-phishing-protection-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-phishing-protection-1.9.0.tar", last modified: Fri Feb 24 01:13:14 2023, max compression
+gzip compressed data, was "google-cloud-phishing-protection-1.9.1.tar", last modified: Wed Jul  5 15:54:32 2023, max compression
```

## Comparing `google-cloud-phishing-protection-1.9.0.tar` & `google-cloud-phishing-protection-1.9.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:13:14.705029 google-cloud-phishing-protection-1.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5065 2023-02-24 01:13:14.705029 google-cloud-phishing-protection-1.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4114 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:13:14.697025 google-cloud-phishing-protection-1.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:13:14.697025 google-cloud-phishing-protection-1.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:13:14.701027 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection/
--rw-rw-r--   0 root         (0)     1003     1346 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:13:14.701027 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/
--rw-rw-r--   0 root         (0)     1003     1141 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1132 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:13:14.701027 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/proto/
--rw-rw-r--   0 root         (0)     1003     2939 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/proto/phishingprotection.proto
--rw-rw-r--   0 root         (0)     1003       93 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:13:14.701027 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:13:14.701027 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/
--rw-rw-r--   0 root         (0)     1003      841 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    15017 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/async_client.py
--rw-rw-r--   0 root         (0)     1003    23434 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:13:14.701027 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/
--rw-rw-r--   0 root         (0)     1003     1679 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6187 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12460 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12683 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12824 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:13:14.701027 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003      752 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     1558 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/types/phishingprotection.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:13:14.705029 google-cloud-phishing-protection-1.9.0/google_cloud_phishing_protection.egg-info/
--rw-r--r--   0 root         (0)     1003     5065 2023-02-24 01:13:14.000000 google-cloud-phishing-protection-1.9.0/google_cloud_phishing_protection.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2106 2023-02-24 01:13:14.000000 google-cloud-phishing-protection-1.9.0/google_cloud_phishing_protection.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-02-24 01:13:14.000000 google-cloud-phishing-protection-1.9.0/google_cloud_phishing_protection.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-02-24 01:13:14.000000 google-cloud-phishing-protection-1.9.0/google_cloud_phishing_protection.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-02-24 01:13:14.000000 google-cloud-phishing-protection-1.9.0/google_cloud_phishing_protection.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-02-24 01:13:14.000000 google-cloud-phishing-protection-1.9.0/google_cloud_phishing_protection.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-02-24 01:13:14.000000 google-cloud-phishing-protection-1.9.0/google_cloud_phishing_protection.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-02-24 01:13:14.705029 google-cloud-phishing-protection-1.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2973 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:13:14.705029 google-cloud-phishing-protection-1.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:13:14.705029 google-cloud-phishing-protection-1.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:13:14.705029 google-cloud-phishing-protection-1.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:13:14.705029 google-cloud-phishing-protection-1.9.0/tests/unit/gapic/phishingprotection_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/tests/unit/gapic/phishingprotection_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    75744 2023-02-24 01:10:52.000000 google-cloud-phishing-protection-1.9.0/tests/unit/gapic/phishingprotection_v1beta1/test_phishing_protection_service_v1_beta1.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:32.843984 google-cloud-phishing-protection-1.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5023 2023-07-05 15:54:32.843984 google-cloud-phishing-protection-1.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4078 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:32.835985 google-cloud-phishing-protection-1.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:32.835985 google-cloud-phishing-protection-1.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:32.839985 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection/
+-rw-rw-r--   0 root         (0)     1003     1346 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:32.839985 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     1141 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1132 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:32.839985 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/proto/
+-rw-rw-r--   0 root         (0)     1003     2939 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/proto/phishingprotection.proto
+-rw-rw-r--   0 root         (0)     1003       93 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:32.839985 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:32.839985 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/
+-rw-rw-r--   0 root         (0)     1003      841 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15066 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/async_client.py
+-rw-rw-r--   0 root         (0)     1003    23434 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:32.839985 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/
+-rw-rw-r--   0 root         (0)     1003     1679 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6187 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12460 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12683 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12829 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:32.843984 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003      752 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1594 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/types/phishingprotection.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:32.843984 google-cloud-phishing-protection-1.9.1/google_cloud_phishing_protection.egg-info/
+-rw-r--r--   0 root         (0)     1003     5023 2023-07-05 15:54:32.000000 google-cloud-phishing-protection-1.9.1/google_cloud_phishing_protection.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2106 2023-07-05 15:54:32.000000 google-cloud-phishing-protection-1.9.1/google_cloud_phishing_protection.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:32.000000 google-cloud-phishing-protection-1.9.1/google_cloud_phishing_protection.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:54:32.000000 google-cloud-phishing-protection-1.9.1/google_cloud_phishing_protection.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:32.000000 google-cloud-phishing-protection-1.9.1/google_cloud_phishing_protection.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:54:32.000000 google-cloud-phishing-protection-1.9.1/google_cloud_phishing_protection.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:54:32.000000 google-cloud-phishing-protection-1.9.1/google_cloud_phishing_protection.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:54:32.843984 google-cloud-phishing-protection-1.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2967 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:32.843984 google-cloud-phishing-protection-1.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:32.843984 google-cloud-phishing-protection-1.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:32.843984 google-cloud-phishing-protection-1.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:32.843984 google-cloud-phishing-protection-1.9.1/tests/unit/gapic/phishingprotection_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/tests/unit/gapic/phishingprotection_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    75744 2023-07-05 15:46:59.000000 google-cloud-phishing-protection-1.9.1/tests/unit/gapic/phishingprotection_v1beta1/test_phishing_protection_service_v1_beta1.py
```

### Comparing `google-cloud-phishing-protection-1.9.0/LICENSE` & `google-cloud-phishing-protection-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-phishing-protection-1.9.0/MANIFEST.in` & `google-cloud-phishing-protection-1.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-phishing-protection-1.9.0/PKG-INFO` & `google-cloud-phishing-protection-1.9.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-phishing-protection
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Phishing Protection API client library
-Home-page: https://github.com/googleapis/python-phishingprotection
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
 
-Python Client for Phishing Protection API
-=========================================
+Python Client for Phishing Protection
+=====================================
 
 |preview| |pypi| |versions|
 
-`Phishing Protection API`_: helps prevent users from accessing phishing sites by identifying various signals associated with malicious content, including the use of your brand assets, classifying malicious content that uses your brand and reporting the unsafe URLs to Google Safe Browsing. Once a site is propagated to Safe Browsing, users will see warnings across more than 4 billion devices.
+`Phishing Protection`_: helps prevent users from accessing phishing sites by identifying various signals associated with malicious content, including the use of your brand assets, classifying malicious content that uses your brand and reporting the unsafe URLs to Google Safe Browsing. Once a site is propagated to Safe Browsing, users will see warnings across more than 4 billion devices.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-phishing-protection.svg
    :target: https://pypi.org/project/google-cloud-phishing-protection/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-phishing-protection.svg
    :target: https://pypi.org/project/google-cloud-phishing-protection/
-.. _Phishing Protection API: https://cloud.google.com/phishing-protection/docs/
+.. _Phishing Protection: https://cloud.google.com/phishing-protection/docs/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/phishingprotection/latest
 .. _Product Documentation:  https://cloud.google.com/phishing-protection/docs/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Phishing Protection API.`_
+3. `Enable the Phishing Protection.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Phishing Protection API.:  https://cloud.google.com/phishing-protection/docs/
+.. _Enable the Phishing Protection.:  https://cloud.google.com/phishing-protection/docs/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-phishing-protection
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Phishing Protection API
+-  Read the `Client Library Documentation`_ for Phishing Protection
    to see other available methods on the client.
--  Read the `Phishing Protection API Product documentation`_ to learn
+-  Read the `Phishing Protection Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Phishing Protection API Product documentation:  https://cloud.google.com/phishing-protection/docs/
+.. _Phishing Protection Product documentation:  https://cloud.google.com/phishing-protection/docs/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-phishing-protection-1.9.0/README.rst` & `google-cloud-phishing-protection-1.9.1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Phishing Protection API
-=========================================
+Python Client for Phishing Protection
+=====================================
 
 |preview| |pypi| |versions|
 
-`Phishing Protection API`_: helps prevent users from accessing phishing sites by identifying various signals associated with malicious content, including the use of your brand assets, classifying malicious content that uses your brand and reporting the unsafe URLs to Google Safe Browsing. Once a site is propagated to Safe Browsing, users will see warnings across more than 4 billion devices.
+`Phishing Protection`_: helps prevent users from accessing phishing sites by identifying various signals associated with malicious content, including the use of your brand assets, classifying malicious content that uses your brand and reporting the unsafe URLs to Google Safe Browsing. Once a site is propagated to Safe Browsing, users will see warnings across more than 4 billion devices.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-phishing-protection.svg
    :target: https://pypi.org/project/google-cloud-phishing-protection/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-phishing-protection.svg
    :target: https://pypi.org/project/google-cloud-phishing-protection/
-.. _Phishing Protection API: https://cloud.google.com/phishing-protection/docs/
+.. _Phishing Protection: https://cloud.google.com/phishing-protection/docs/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/phishingprotection/latest
 .. _Product Documentation:  https://cloud.google.com/phishing-protection/docs/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Phishing Protection API.`_
+3. `Enable the Phishing Protection.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Phishing Protection API.:  https://cloud.google.com/phishing-protection/docs/
+.. _Enable the Phishing Protection.:  https://cloud.google.com/phishing-protection/docs/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-phishing-protection
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Phishing Protection API
+-  Read the `Client Library Documentation`_ for Phishing Protection
    to see other available methods on the client.
--  Read the `Phishing Protection API Product documentation`_ to learn
+-  Read the `Phishing Protection Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Phishing Protection API Product documentation:  https://cloud.google.com/phishing-protection/docs/
+.. _Phishing Protection Product documentation:  https://cloud.google.com/phishing-protection/docs/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection/__init__.py` & `google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection/gapic_version.py` & `google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection/gapic_version.py`

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
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/__init__.py` & `google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/gapic_metadata.json` & `google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/gapic_version.py` & `google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/gapic_version.py`

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
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/proto/phishingprotection.proto` & `google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/proto/phishingprotection.proto`

 * *Files identical despite different names*

### Comparing `google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/services/__init__.py` & `google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/__init__.py` & `google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/async_client.py` & `google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,15 +343,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "PhishingProtectionServiceV1Beta1AsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/client.py` & `google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/__init__.py` & `google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/base.py` & `google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/grpc.py` & `google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/grpc_asyncio.py` & `google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/rest.py` & `google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/services/phishing_protection_service_v1_beta1/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import dataclasses
 import json  # type: ignore
 import re
-from typing import Callable, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
 import warnings
 
 from google.api_core import gapic_v1, path_template, rest_helpers, rest_streaming
 from google.api_core import exceptions as core_exceptions
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
@@ -201,15 +201,15 @@
         )
         self._prep_wrapped_messages(client_info)
 
     class _ReportPhishing(PhishingProtectionServiceV1Beta1RestStub):
         def __hash__(self):
             return hash("ReportPhishing")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
```

### Comparing `google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/types/__init__.py` & `google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-phishing-protection-1.9.0/google/cloud/phishingprotection_v1beta1/types/phishingprotection.py` & `google-cloud-phishing-protection-1.9.1/google/cloud/phishingprotection_v1beta1/types/phishingprotection.py`

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
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.phishingprotection.v1beta1",
     manifest={
```

### Comparing `google-cloud-phishing-protection-1.9.0/google_cloud_phishing_protection.egg-info/PKG-INFO` & `google-cloud-phishing-protection-1.9.1/google_cloud_phishing_protection.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-phishing-protection
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Phishing Protection API client library
-Home-page: https://github.com/googleapis/python-phishingprotection
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
 
-Python Client for Phishing Protection API
-=========================================
+Python Client for Phishing Protection
+=====================================
 
 |preview| |pypi| |versions|
 
-`Phishing Protection API`_: helps prevent users from accessing phishing sites by identifying various signals associated with malicious content, including the use of your brand assets, classifying malicious content that uses your brand and reporting the unsafe URLs to Google Safe Browsing. Once a site is propagated to Safe Browsing, users will see warnings across more than 4 billion devices.
+`Phishing Protection`_: helps prevent users from accessing phishing sites by identifying various signals associated with malicious content, including the use of your brand assets, classifying malicious content that uses your brand and reporting the unsafe URLs to Google Safe Browsing. Once a site is propagated to Safe Browsing, users will see warnings across more than 4 billion devices.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-phishing-protection.svg
    :target: https://pypi.org/project/google-cloud-phishing-protection/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-phishing-protection.svg
    :target: https://pypi.org/project/google-cloud-phishing-protection/
-.. _Phishing Protection API: https://cloud.google.com/phishing-protection/docs/
+.. _Phishing Protection: https://cloud.google.com/phishing-protection/docs/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/phishingprotection/latest
 .. _Product Documentation:  https://cloud.google.com/phishing-protection/docs/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Phishing Protection API.`_
+3. `Enable the Phishing Protection.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Phishing Protection API.:  https://cloud.google.com/phishing-protection/docs/
+.. _Enable the Phishing Protection.:  https://cloud.google.com/phishing-protection/docs/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-phishing-protection
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Phishing Protection API
+-  Read the `Client Library Documentation`_ for Phishing Protection
    to see other available methods on the client.
--  Read the `Phishing Protection API Product documentation`_ to learn
+-  Read the `Phishing Protection Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Phishing Protection API Product documentation:  https://cloud.google.com/phishing-protection/docs/
+.. _Phishing Protection Product documentation:  https://cloud.google.com/phishing-protection/docs/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-phishing-protection-1.9.0/google_cloud_phishing_protection.egg-info/SOURCES.txt` & `google-cloud-phishing-protection-1.9.1/google_cloud_phishing_protection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-phishing-protection-1.9.0/setup.py` & `google-cloud-phishing-protection-1.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-phishingprotection"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-phishing-protection-1.9.0/tests/__init__.py` & `google-cloud-phishing-protection-1.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-phishing-protection-1.9.0/tests/unit/__init__.py` & `google-cloud-phishing-protection-1.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-phishing-protection-1.9.0/tests/unit/gapic/__init__.py` & `google-cloud-phishing-protection-1.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-phishing-protection-1.9.0/tests/unit/gapic/phishingprotection_v1beta1/__init__.py` & `google-cloud-phishing-protection-1.9.1/tests/unit/gapic/phishingprotection_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-phishing-protection-1.9.0/tests/unit/gapic/phishingprotection_v1beta1/test_phishing_protection_service_v1_beta1.py` & `google-cloud-phishing-protection-1.9.1/tests/unit/gapic/phishingprotection_v1beta1/test_phishing_protection_service_v1_beta1.py`

 * *Files identical despite different names*

