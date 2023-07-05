# Comparing `tmp/google-cloud-public-ca-0.3.2.tar.gz` & `tmp/google-cloud-public-ca-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-public-ca-0.3.2.tar", last modified: Mon Mar 27 15:44:26 2023, max compression
+gzip compressed data, was "google-cloud-public-ca-0.3.3.tar", last modified: Wed Jul  5 15:54:49 2023, max compression
```

## Comparing `google-cloud-public-ca-0.3.2.tar` & `google-cloud-public-ca-0.3.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:26.529914 google-cloud-public-ca-0.3.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4801 2023-03-27 15:44:26.529914 google-cloud-public-ca-0.3.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3883 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:26.521914 google-cloud-public-ca-0.3.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:26.521914 google-cloud-public-ca-0.3.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:26.521914 google-cloud-public-ca-0.3.2/google/cloud/security/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:26.525914 google-cloud-public-ca-0.3.2/google/cloud/security/publicca/
--rw-rw-r--   0 root         (0)     1003     1409 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/google/cloud/security/publicca/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/google/cloud/security/publicca/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       83 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/google/cloud/security/publicca/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:26.525914 google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/
--rw-rw-r--   0 root         (0)     1003     1173 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1200 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       83 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:26.525914 google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:26.525914 google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/
--rw-rw-r--   0 root         (0)     1003      845 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    15841 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    24811 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:26.529914 google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/
--rw-rw-r--   0 root         (0)     1003     1693 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6151 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12210 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12443 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    13407 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:26.529914 google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003      775 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     1913 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/types/resources.py
--rw-rw-r--   0 root         (0)     1003     2130 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:26.529914 google-cloud-public-ca-0.3.2/google_cloud_public_ca.egg-info/
--rw-r--r--   0 root         (0)     1003     4801 2023-03-27 15:44:26.000000 google-cloud-public-ca-0.3.2/google_cloud_public_ca.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1974 2023-03-27 15:44:26.000000 google-cloud-public-ca-0.3.2/google_cloud_public_ca.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:44:26.000000 google-cloud-public-ca-0.3.2/google_cloud_public_ca.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       42 2023-03-27 15:44:26.000000 google-cloud-public-ca-0.3.2/google_cloud_public_ca.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:44:26.000000 google-cloud-public-ca-0.3.2/google_cloud_public_ca.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 15:44:26.000000 google-cloud-public-ca-0.3.2/google_cloud_public_ca.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:44:26.000000 google-cloud-public-ca-0.3.2/google_cloud_public_ca.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:44:26.529914 google-cloud-public-ca-0.3.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2977 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:26.529914 google-cloud-public-ca-0.3.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:26.529914 google-cloud-public-ca-0.3.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:26.529914 google-cloud-public-ca-0.3.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:26.529914 google-cloud-public-ca-0.3.2/tests/unit/gapic/publicca_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/tests/unit/gapic/publicca_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    78657 2023-03-27 15:41:57.000000 google-cloud-public-ca-0.3.2/tests/unit/gapic/publicca_v1beta1/test_public_certificate_authority_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:49.327576 google-cloud-public-ca-0.3.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4759 2023-07-05 15:54:49.327576 google-cloud-public-ca-0.3.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3847 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:49.323576 google-cloud-public-ca-0.3.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:49.323576 google-cloud-public-ca-0.3.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:49.323576 google-cloud-public-ca-0.3.3/google/cloud/security/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:49.323576 google-cloud-public-ca-0.3.3/google/cloud/security/publicca/
+-rw-rw-r--   0 root         (0)     1003     1409 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/google/cloud/security/publicca/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/google/cloud/security/publicca/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       83 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/google/cloud/security/publicca/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:49.323576 google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     1173 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1200 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       83 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:49.323576 google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:49.323576 google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/
+-rw-rw-r--   0 root         (0)     1003      845 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15891 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    24811 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:49.327576 google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1693 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6151 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12210 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12443 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    13407 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:49.327576 google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003      775 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1913 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/types/resources.py
+-rw-rw-r--   0 root         (0)     1003     2130 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:49.327576 google-cloud-public-ca-0.3.3/google_cloud_public_ca.egg-info/
+-rw-r--r--   0 root         (0)     1003     4759 2023-07-05 15:54:49.000000 google-cloud-public-ca-0.3.3/google_cloud_public_ca.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1974 2023-07-05 15:54:49.000000 google-cloud-public-ca-0.3.3/google_cloud_public_ca.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:49.000000 google-cloud-public-ca-0.3.3/google_cloud_public_ca.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       42 2023-07-05 15:54:49.000000 google-cloud-public-ca-0.3.3/google_cloud_public_ca.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:49.000000 google-cloud-public-ca-0.3.3/google_cloud_public_ca.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:54:49.000000 google-cloud-public-ca-0.3.3/google_cloud_public_ca.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:54:49.000000 google-cloud-public-ca-0.3.3/google_cloud_public_ca.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:54:49.327576 google-cloud-public-ca-0.3.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2971 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:49.327576 google-cloud-public-ca-0.3.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:49.327576 google-cloud-public-ca-0.3.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:49.327576 google-cloud-public-ca-0.3.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:49.327576 google-cloud-public-ca-0.3.3/tests/unit/gapic/publicca_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/tests/unit/gapic/publicca_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    78657 2023-07-05 15:46:59.000000 google-cloud-public-ca-0.3.3/tests/unit/gapic/publicca_v1beta1/test_public_certificate_authority_service.py
```

### Comparing `google-cloud-public-ca-0.3.2/LICENSE` & `google-cloud-public-ca-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-public-ca-0.3.2/MANIFEST.in` & `google-cloud-public-ca-0.3.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-public-ca-0.3.2/PKG-INFO` & `google-cloud-public-ca-0.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-public-ca
-Version: 0.3.2
+Version: 0.3.3
 Summary: Google Cloud Public Ca API client library
-Home-page: https://github.com/googleapis/python-security-public-ca
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for Public Certificate Authority API
-==================================================
+Python Client for Public Certificate Authority
+==============================================
 
 |preview| |pypi| |versions|
 
-`Public Certificate Authority API`_: simplifies the deployment and management of public CAs without managing infrastructure.
+`Public Certificate Authority`_: simplifies the deployment and management of public CAs without managing infrastructure.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-public-ca.svg
    :target: https://pypi.org/project/google-cloud-public-ca/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-public-ca.svg
    :target: https://pypi.org/project/google-cloud-public-ca/
-.. _Public Certificate Authority API: https://cloud.google.com/certificate-manager/docs/public-ca
+.. _Public Certificate Authority: https://cloud.google.com/certificate-manager/docs/public-ca
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/publicca/latest
 .. _Product Documentation:  https://cloud.google.com/certificate-manager/docs/public-ca
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Public Certificate Authority API.`_
+3. `Enable the Public Certificate Authority.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Public Certificate Authority API.:  https://cloud.google.com/certificate-manager/docs/public-ca
+.. _Enable the Public Certificate Authority.:  https://cloud.google.com/certificate-manager/docs/public-ca
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-public-ca
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Public Certificate Authority API
+-  Read the `Client Library Documentation`_ for Public Certificate Authority
    to see other available methods on the client.
--  Read the `Public Certificate Authority API Product documentation`_ to learn
+-  Read the `Public Certificate Authority Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Public Certificate Authority API Product documentation:  https://cloud.google.com/certificate-manager/docs/public-ca
+.. _Public Certificate Authority Product documentation:  https://cloud.google.com/certificate-manager/docs/public-ca
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-public-ca-0.3.2/README.rst` & `google-cloud-public-ca-0.3.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Public Certificate Authority API
-==================================================
+Python Client for Public Certificate Authority
+==============================================
 
 |preview| |pypi| |versions|
 
-`Public Certificate Authority API`_: simplifies the deployment and management of public CAs without managing infrastructure.
+`Public Certificate Authority`_: simplifies the deployment and management of public CAs without managing infrastructure.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-public-ca.svg
    :target: https://pypi.org/project/google-cloud-public-ca/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-public-ca.svg
    :target: https://pypi.org/project/google-cloud-public-ca/
-.. _Public Certificate Authority API: https://cloud.google.com/certificate-manager/docs/public-ca
+.. _Public Certificate Authority: https://cloud.google.com/certificate-manager/docs/public-ca
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/publicca/latest
 .. _Product Documentation:  https://cloud.google.com/certificate-manager/docs/public-ca
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Public Certificate Authority API.`_
+3. `Enable the Public Certificate Authority.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Public Certificate Authority API.:  https://cloud.google.com/certificate-manager/docs/public-ca
+.. _Enable the Public Certificate Authority.:  https://cloud.google.com/certificate-manager/docs/public-ca
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-public-ca
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Public Certificate Authority API
+-  Read the `Client Library Documentation`_ for Public Certificate Authority
    to see other available methods on the client.
--  Read the `Public Certificate Authority API Product documentation`_ to learn
+-  Read the `Public Certificate Authority Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Public Certificate Authority API Product documentation:  https://cloud.google.com/certificate-manager/docs/public-ca
+.. _Public Certificate Authority Product documentation:  https://cloud.google.com/certificate-manager/docs/public-ca
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-public-ca-0.3.2/google/cloud/security/publicca/__init__.py` & `google-cloud-public-ca-0.3.3/google/cloud/security/publicca/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-public-ca-0.3.2/google/cloud/security/publicca/gapic_version.py` & `google-cloud-public-ca-0.3.3/google/cloud/security/publicca/gapic_version.py`

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
-__version__ = "0.3.2"  # {x-release-please-version}
+__version__ = "0.3.3"  # {x-release-please-version}
```

### Comparing `google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/__init__.py` & `google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/gapic_metadata.json` & `google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/gapic_version.py` & `google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/gapic_version.py`

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
-__version__ = "0.3.2"  # {x-release-please-version}
+__version__ = "0.3.3"  # {x-release-please-version}
```

### Comparing `google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/services/__init__.py` & `google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/__init__.py` & `google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/async_client.py` & `google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,15 +356,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "PublicCertificateAuthorityServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/client.py` & `google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/__init__.py` & `google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/base.py` & `google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/grpc.py` & `google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/grpc_asyncio.py` & `google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/rest.py` & `google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/services/public_certificate_authority_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/types/__init__.py` & `google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/types/resources.py` & `google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/types/resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-public-ca-0.3.2/google/cloud/security/publicca_v1beta1/types/service.py` & `google-cloud-public-ca-0.3.3/google/cloud/security/publicca_v1beta1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-public-ca-0.3.2/google_cloud_public_ca.egg-info/PKG-INFO` & `google-cloud-public-ca-0.3.3/google_cloud_public_ca.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-public-ca
-Version: 0.3.2
+Version: 0.3.3
 Summary: Google Cloud Public Ca API client library
-Home-page: https://github.com/googleapis/python-security-public-ca
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for Public Certificate Authority API
-==================================================
+Python Client for Public Certificate Authority
+==============================================
 
 |preview| |pypi| |versions|
 
-`Public Certificate Authority API`_: simplifies the deployment and management of public CAs without managing infrastructure.
+`Public Certificate Authority`_: simplifies the deployment and management of public CAs without managing infrastructure.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-public-ca.svg
    :target: https://pypi.org/project/google-cloud-public-ca/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-public-ca.svg
    :target: https://pypi.org/project/google-cloud-public-ca/
-.. _Public Certificate Authority API: https://cloud.google.com/certificate-manager/docs/public-ca
+.. _Public Certificate Authority: https://cloud.google.com/certificate-manager/docs/public-ca
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/publicca/latest
 .. _Product Documentation:  https://cloud.google.com/certificate-manager/docs/public-ca
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Public Certificate Authority API.`_
+3. `Enable the Public Certificate Authority.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Public Certificate Authority API.:  https://cloud.google.com/certificate-manager/docs/public-ca
+.. _Enable the Public Certificate Authority.:  https://cloud.google.com/certificate-manager/docs/public-ca
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-public-ca
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Public Certificate Authority API
+-  Read the `Client Library Documentation`_ for Public Certificate Authority
    to see other available methods on the client.
--  Read the `Public Certificate Authority API Product documentation`_ to learn
+-  Read the `Public Certificate Authority Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Public Certificate Authority API Product documentation:  https://cloud.google.com/certificate-manager/docs/public-ca
+.. _Public Certificate Authority Product documentation:  https://cloud.google.com/certificate-manager/docs/public-ca
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-public-ca-0.3.2/google_cloud_public_ca.egg-info/SOURCES.txt` & `google-cloud-public-ca-0.3.3/google_cloud_public_ca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-public-ca-0.3.2/setup.py` & `google-cloud-public-ca-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-security-public-ca"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-public-ca-0.3.2/tests/__init__.py` & `google-cloud-public-ca-0.3.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-public-ca-0.3.2/tests/unit/__init__.py` & `google-cloud-public-ca-0.3.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-public-ca-0.3.2/tests/unit/gapic/__init__.py` & `google-cloud-public-ca-0.3.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-public-ca-0.3.2/tests/unit/gapic/publicca_v1beta1/__init__.py` & `google-cloud-public-ca-0.3.3/tests/unit/gapic/publicca_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-public-ca-0.3.2/tests/unit/gapic/publicca_v1beta1/test_public_certificate_authority_service.py` & `google-cloud-public-ca-0.3.3/tests/unit/gapic/publicca_v1beta1/test_public_certificate_authority_service.py`

 * *Files identical despite different names*

