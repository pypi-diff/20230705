# Comparing `tmp/google-cloud-iam-logging-1.2.0.tar.gz` & `tmp/google-cloud-iam-logging-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-iam-logging-1.2.0.tar", last modified: Tue Jan 10 18:33:26 2023, max compression
+gzip compressed data, was "google-cloud-iam-logging-1.2.1.tar", last modified: Wed Jul  5 15:53:26 2023, max compression
```

## Comparing `google-cloud-iam-logging-1.2.0.tar` & `google-cloud-iam-logging-1.2.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:33:26.929973 google-cloud-iam-logging-1.2.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-10 18:29:57.000000 google-cloud-iam-logging-1.2.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-10 18:29:57.000000 google-cloud-iam-logging-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4595 2023-01-10 18:33:26.929973 google-cloud-iam-logging-1.2.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3667 2023-01-10 18:29:57.000000 google-cloud-iam-logging-1.2.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:33:26.925973 google-cloud-iam-logging-1.2.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:33:26.925973 google-cloud-iam-logging-1.2.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:33:26.925973 google-cloud-iam-logging-1.2.0/google/cloud/iam_logging/
--rw-rw-r--   0 root         (0)     1003      808 2023-01-10 18:29:57.000000 google-cloud-iam-logging-1.2.0/google/cloud/iam_logging/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-10 18:29:57.000000 google-cloud-iam-logging-1.2.0/google/cloud/iam_logging/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       85 2023-01-10 18:29:57.000000 google-cloud-iam-logging-1.2.0/google/cloud/iam_logging/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:33:26.929973 google-cloud-iam-logging-1.2.0/google/cloud/iam_logging_v1/
--rw-rw-r--   0 root         (0)     1003      781 2023-01-10 18:29:57.000000 google-cloud-iam-logging-1.2.0/google/cloud/iam_logging_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      237 2023-01-10 18:29:57.000000 google-cloud-iam-logging-1.2.0/google/cloud/iam_logging_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       85 2023-01-10 18:29:57.000000 google-cloud-iam-logging-1.2.0/google/cloud/iam_logging_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:33:26.929973 google-cloud-iam-logging-1.2.0/google/cloud/iam_logging_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 18:29:57.000000 google-cloud-iam-logging-1.2.0/google/cloud/iam_logging_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:33:26.929973 google-cloud-iam-logging-1.2.0/google/cloud/iam_logging_v1/types/
--rw-rw-r--   0 root         (0)     1003      660 2023-01-10 18:29:57.000000 google-cloud-iam-logging-1.2.0/google/cloud/iam_logging_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     1416 2023-01-10 18:29:57.000000 google-cloud-iam-logging-1.2.0/google/cloud/iam_logging_v1/types/audit_data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:33:26.929973 google-cloud-iam-logging-1.2.0/google_cloud_iam_logging.egg-info/
--rw-r--r--   0 root         (0)     1003     4595 2023-01-10 18:33:26.000000 google-cloud-iam-logging-1.2.0/google_cloud_iam_logging.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003      939 2023-01-10 18:33:26.000000 google-cloud-iam-logging-1.2.0/google_cloud_iam_logging.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-10 18:33:26.000000 google-cloud-iam-logging-1.2.0/google_cloud_iam_logging.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-10 18:33:26.000000 google-cloud-iam-logging-1.2.0/google_cloud_iam_logging.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-10 18:33:26.000000 google-cloud-iam-logging-1.2.0/google_cloud_iam_logging.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-01-10 18:33:26.000000 google-cloud-iam-logging-1.2.0/google_cloud_iam_logging.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-10 18:33:26.000000 google-cloud-iam-logging-1.2.0/google_cloud_iam_logging.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-01-10 18:33:26.929973 google-cloud-iam-logging-1.2.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3044 2023-01-10 18:29:57.000000 google-cloud-iam-logging-1.2.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:33:26.929973 google-cloud-iam-logging-1.2.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 18:29:57.000000 google-cloud-iam-logging-1.2.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:33:26.929973 google-cloud-iam-logging-1.2.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 18:29:57.000000 google-cloud-iam-logging-1.2.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:33:26.929973 google-cloud-iam-logging-1.2.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 18:29:57.000000 google-cloud-iam-logging-1.2.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:33:26.929973 google-cloud-iam-logging-1.2.0/tests/unit/gapic/iam_logging_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 18:29:57.000000 google-cloud-iam-logging-1.2.0/tests/unit/gapic/iam_logging_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      804 2023-01-10 18:29:57.000000 google-cloud-iam-logging-1.2.0/tests/unit/gapic/iam_logging_v1/test_iam_logging.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:26.717164 google-cloud-iam-logging-1.2.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-iam-logging-1.2.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-iam-logging-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4560 2023-07-05 15:53:26.717164 google-cloud-iam-logging-1.2.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3631 2023-07-05 15:46:59.000000 google-cloud-iam-logging-1.2.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:26.713164 google-cloud-iam-logging-1.2.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:26.713164 google-cloud-iam-logging-1.2.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:26.713164 google-cloud-iam-logging-1.2.1/google/cloud/iam_logging/
+-rw-rw-r--   0 root         (0)     1003      808 2023-07-05 15:46:59.000000 google-cloud-iam-logging-1.2.1/google/cloud/iam_logging/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-iam-logging-1.2.1/google/cloud/iam_logging/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       85 2023-07-05 15:46:59.000000 google-cloud-iam-logging-1.2.1/google/cloud/iam_logging/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:26.717164 google-cloud-iam-logging-1.2.1/google/cloud/iam_logging_v1/
+-rw-rw-r--   0 root         (0)     1003      784 2023-07-05 15:46:59.000000 google-cloud-iam-logging-1.2.1/google/cloud/iam_logging_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      237 2023-07-05 15:46:59.000000 google-cloud-iam-logging-1.2.1/google/cloud/iam_logging_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-iam-logging-1.2.1/google/cloud/iam_logging_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       85 2023-07-05 15:46:59.000000 google-cloud-iam-logging-1.2.1/google/cloud/iam_logging_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:26.717164 google-cloud-iam-logging-1.2.1/google/cloud/iam_logging_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-iam-logging-1.2.1/google/cloud/iam_logging_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:26.717164 google-cloud-iam-logging-1.2.1/google/cloud/iam_logging_v1/types/
+-rw-rw-r--   0 root         (0)     1003      660 2023-07-05 15:46:59.000000 google-cloud-iam-logging-1.2.1/google/cloud/iam_logging_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1452 2023-07-05 15:46:59.000000 google-cloud-iam-logging-1.2.1/google/cloud/iam_logging_v1/types/audit_data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:26.717164 google-cloud-iam-logging-1.2.1/google_cloud_iam_logging.egg-info/
+-rw-r--r--   0 root         (0)     1003     4560 2023-07-05 15:53:26.000000 google-cloud-iam-logging-1.2.1/google_cloud_iam_logging.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003      984 2023-07-05 15:53:26.000000 google-cloud-iam-logging-1.2.1/google_cloud_iam_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:26.000000 google-cloud-iam-logging-1.2.1/google_cloud_iam_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:53:26.000000 google-cloud-iam-logging-1.2.1/google_cloud_iam_logging.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:26.000000 google-cloud-iam-logging-1.2.1/google_cloud_iam_logging.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:53:26.000000 google-cloud-iam-logging-1.2.1/google_cloud_iam_logging.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:53:26.000000 google-cloud-iam-logging-1.2.1/google_cloud_iam_logging.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:53:26.717164 google-cloud-iam-logging-1.2.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2991 2023-07-05 15:46:59.000000 google-cloud-iam-logging-1.2.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:26.717164 google-cloud-iam-logging-1.2.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-iam-logging-1.2.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:26.717164 google-cloud-iam-logging-1.2.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-iam-logging-1.2.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:26.717164 google-cloud-iam-logging-1.2.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-iam-logging-1.2.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:26.717164 google-cloud-iam-logging-1.2.1/tests/unit/gapic/iam_logging_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-iam-logging-1.2.1/tests/unit/gapic/iam_logging_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      804 2023-07-05 15:46:59.000000 google-cloud-iam-logging-1.2.1/tests/unit/gapic/iam_logging_v1/test_iam_logging.py
```

### Comparing `google-cloud-iam-logging-1.2.0/LICENSE` & `google-cloud-iam-logging-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-logging-1.2.0/MANIFEST.in` & `google-cloud-iam-logging-1.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-logging-1.2.0/PKG-INFO` & `google-cloud-iam-logging-1.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-iam-logging
-Version: 1.2.0
+Version: 1.2.1
 Summary: Google Cloud Iam Logging API client library
-Home-page: https://github.com/googleapis/python-iam-logging
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
 
-Python Client for IAM Logging Protos API
-========================================
+Python Client for IAM Logging Protos
+====================================
 
 |stable| |pypi| |versions|
 
-`IAM Logging Protos API`_: 
+`IAM Logging Protos`_: 
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-iam-logging.svg
    :target: https://pypi.org/project/google-cloud-iam-logging/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-iam-logging.svg
    :target: https://pypi.org/project/google-cloud-iam-logging/
-.. _IAM Logging Protos API: https://cloud.google.com/iam/docs/audit-logging
+.. _IAM Logging Protos: https://cloud.google.com/iam/docs/audit-logging
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/iamlogging/latest
 .. _Product Documentation:  https://cloud.google.com/iam/docs/audit-logging
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the IAM Logging Protos API.`_
+3. `Enable the IAM Logging Protos.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the IAM Logging Protos API.:  https://cloud.google.com/iam/docs/audit-logging
+.. _Enable the IAM Logging Protos.:  https://cloud.google.com/iam/docs/audit-logging
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-iam-logging
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for IAM Logging Protos API
+-  Read the `Client Library Documentation`_ for IAM Logging Protos
    to see other available methods on the client.
--  Read the `IAM Logging Protos API Product documentation`_ to learn
+-  Read the `IAM Logging Protos Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _IAM Logging Protos API Product documentation:  https://cloud.google.com/iam/docs/audit-logging
+.. _IAM Logging Protos Product documentation:  https://cloud.google.com/iam/docs/audit-logging
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-iam-logging-1.2.0/README.rst` & `google-cloud-iam-logging-1.2.1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for IAM Logging Protos API
-========================================
+Python Client for IAM Logging Protos
+====================================
 
 |stable| |pypi| |versions|
 
-`IAM Logging Protos API`_: 
+`IAM Logging Protos`_: 
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-iam-logging.svg
    :target: https://pypi.org/project/google-cloud-iam-logging/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-iam-logging.svg
    :target: https://pypi.org/project/google-cloud-iam-logging/
-.. _IAM Logging Protos API: https://cloud.google.com/iam/docs/audit-logging
+.. _IAM Logging Protos: https://cloud.google.com/iam/docs/audit-logging
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/iamlogging/latest
 .. _Product Documentation:  https://cloud.google.com/iam/docs/audit-logging
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the IAM Logging Protos API.`_
+3. `Enable the IAM Logging Protos.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the IAM Logging Protos API.:  https://cloud.google.com/iam/docs/audit-logging
+.. _Enable the IAM Logging Protos.:  https://cloud.google.com/iam/docs/audit-logging
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-iam-logging
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for IAM Logging Protos API
+-  Read the `Client Library Documentation`_ for IAM Logging Protos
    to see other available methods on the client.
--  Read the `IAM Logging Protos API Product documentation`_ to learn
+-  Read the `IAM Logging Protos Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _IAM Logging Protos API Product documentation:  https://cloud.google.com/iam/docs/audit-logging
+.. _IAM Logging Protos Product documentation:  https://cloud.google.com/iam/docs/audit-logging
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-iam-logging-1.2.0/google/cloud/iam_logging/__init__.py` & `google-cloud-iam-logging-1.2.1/google/cloud/iam_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-logging-1.2.0/google/cloud/iam_logging/gapic_version.py` & `google-cloud-iam-logging-1.2.1/google/cloud/iam_logging/gapic_version.py`

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
-__version__ = "1.2.0"  # {x-release-please-version}
+__version__ = "1.2.1"  # {x-release-please-version}
```

### Comparing `google-cloud-iam-logging-1.2.0/google/cloud/iam_logging_v1/__init__.py` & `google-cloud-iam-logging-1.2.1/google/cloud/iam_logging_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.iam_logging import gapic_version as package_version
+from google.cloud.iam_logging_v1 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
 from .types.audit_data import AuditData
 
 __all__ = ("AuditData",)
```

### Comparing `google-cloud-iam-logging-1.2.0/google/cloud/iam_logging_v1/services/__init__.py` & `google-cloud-iam-logging-1.2.1/google/cloud/iam_logging_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-logging-1.2.0/google/cloud/iam_logging_v1/types/__init__.py` & `google-cloud-iam-logging-1.2.1/google/cloud/iam_logging_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-logging-1.2.0/google/cloud/iam_logging_v1/types/audit_data.py` & `google-cloud-iam-logging-1.2.1/google/cloud/iam_logging_v1/types/audit_data.py`

 * *Files 7% similar despite different names*

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
 
 from google.iam.v1 import policy_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.iam.v1.logging",
```

### Comparing `google-cloud-iam-logging-1.2.0/google_cloud_iam_logging.egg-info/PKG-INFO` & `google-cloud-iam-logging-1.2.1/google_cloud_iam_logging.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-iam-logging
-Version: 1.2.0
+Version: 1.2.1
 Summary: Google Cloud Iam Logging API client library
-Home-page: https://github.com/googleapis/python-iam-logging
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
 
-Python Client for IAM Logging Protos API
-========================================
+Python Client for IAM Logging Protos
+====================================
 
 |stable| |pypi| |versions|
 
-`IAM Logging Protos API`_: 
+`IAM Logging Protos`_: 
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-iam-logging.svg
    :target: https://pypi.org/project/google-cloud-iam-logging/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-iam-logging.svg
    :target: https://pypi.org/project/google-cloud-iam-logging/
-.. _IAM Logging Protos API: https://cloud.google.com/iam/docs/audit-logging
+.. _IAM Logging Protos: https://cloud.google.com/iam/docs/audit-logging
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/iamlogging/latest
 .. _Product Documentation:  https://cloud.google.com/iam/docs/audit-logging
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the IAM Logging Protos API.`_
+3. `Enable the IAM Logging Protos.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the IAM Logging Protos API.:  https://cloud.google.com/iam/docs/audit-logging
+.. _Enable the IAM Logging Protos.:  https://cloud.google.com/iam/docs/audit-logging
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-iam-logging
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for IAM Logging Protos API
+-  Read the `Client Library Documentation`_ for IAM Logging Protos
    to see other available methods on the client.
--  Read the `IAM Logging Protos API Product documentation`_ to learn
+-  Read the `IAM Logging Protos Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _IAM Logging Protos API Product documentation:  https://cloud.google.com/iam/docs/audit-logging
+.. _IAM Logging Protos Product documentation:  https://cloud.google.com/iam/docs/audit-logging
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-iam-logging-1.2.0/google_cloud_iam_logging.egg-info/SOURCES.txt` & `google-cloud-iam-logging-1.2.1/google_cloud_iam_logging.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.cfg
 setup.py
 google/cloud/iam_logging/__init__.py
 google/cloud/iam_logging/gapic_version.py
 google/cloud/iam_logging/py.typed
 google/cloud/iam_logging_v1/__init__.py
 google/cloud/iam_logging_v1/gapic_metadata.json
+google/cloud/iam_logging_v1/gapic_version.py
 google/cloud/iam_logging_v1/py.typed
 google/cloud/iam_logging_v1/services/__init__.py
 google/cloud/iam_logging_v1/types/__init__.py
 google/cloud/iam_logging_v1/types/audit_data.py
 google_cloud_iam_logging.egg-info/PKG-INFO
 google_cloud_iam_logging.egg-info/SOURCES.txt
 google_cloud_iam_logging.egg-info/dependency_links.txt
```

### Comparing `google-cloud-iam-logging-1.2.0/setup.py` & `google-cloud-iam-logging-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,33 +38,31 @@
     release_status = "Development Status :: 5 - Production/Stable"
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
-    "grpc-google-iam-v1 >= 0.12.4, < 1.0.0dev",
+    "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
-url = "https://github.com/googleapis/python-iam-logging"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 packages = [
     package
     for package in setuptools.PEP420PackageFinder.find()
     if package.startswith("google")
 ]
 
-namespaces = ["google"]
-if "google.cloud" in packages:
-    namespaces.append("google.cloud")
+namespaces = ["google", "google.cloud"]
 
 setuptools.setup(
     name=name,
     version=version,
     description=description,
     long_description=readme,
     author="Google LLC",
```

### Comparing `google-cloud-iam-logging-1.2.0/tests/__init__.py` & `google-cloud-iam-logging-1.2.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-logging-1.2.0/tests/unit/__init__.py` & `google-cloud-iam-logging-1.2.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-logging-1.2.0/tests/unit/gapic/__init__.py` & `google-cloud-iam-logging-1.2.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-logging-1.2.0/tests/unit/gapic/iam_logging_v1/__init__.py` & `google-cloud-iam-logging-1.2.1/tests/unit/gapic/iam_logging_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-logging-1.2.0/tests/unit/gapic/iam_logging_v1/test_iam_logging.py` & `google-cloud-iam-logging-1.2.1/tests/unit/gapic/iam_logging_v1/test_iam_logging.py`

 * *Files identical despite different names*

