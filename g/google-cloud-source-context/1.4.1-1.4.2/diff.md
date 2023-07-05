# Comparing `tmp/google-cloud-source-context-1.4.1.tar.gz` & `tmp/google-cloud-source-context-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-source-context-1.4.1.tar", last modified: Mon Jan 23 15:42:26 2023, max compression
+gzip compressed data, was "google-cloud-source-context-1.4.2.tar", last modified: Wed Jul  5 15:56:00 2023, max compression
```

## Comparing `google-cloud-source-context-1.4.1.tar` & `google-cloud-source-context-1.4.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:26.063948 google-cloud-source-context-1.4.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-23 15:38:59.000000 google-cloud-source-context-1.4.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-23 15:38:59.000000 google-cloud-source-context-1.4.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4490 2023-01-23 15:42:26.063948 google-cloud-source-context-1.4.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3553 2023-01-23 15:38:59.000000 google-cloud-source-context-1.4.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:26.059949 google-cloud-source-context-1.4.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:26.059949 google-cloud-source-context-1.4.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:26.059949 google-cloud-source-context-1.4.1/google/cloud/source_context/
--rw-rw-r--   0 root         (0)     1003     1271 2023-01-23 15:38:59.000000 google-cloud-source-context-1.4.1/google/cloud/source_context/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-23 15:38:59.000000 google-cloud-source-context-1.4.1/google/cloud/source_context/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       88 2023-01-23 15:38:59.000000 google-cloud-source-context-1.4.1/google/cloud/source_context/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:26.063948 google-cloud-source-context-1.4.1/google/cloud/source_context_v1/
--rw-rw-r--   0 root         (0)     1003     1241 2023-01-23 15:38:59.000000 google-cloud-source-context-1.4.1/google/cloud/source_context_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      244 2023-01-23 15:38:59.000000 google-cloud-source-context-1.4.1/google/cloud/source_context_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-23 15:38:59.000000 google-cloud-source-context-1.4.1/google/cloud/source_context_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       88 2023-01-23 15:38:59.000000 google-cloud-source-context-1.4.1/google/cloud/source_context_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:26.063948 google-cloud-source-context-1.4.1/google/cloud/source_context_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:38:59.000000 google-cloud-source-context-1.4.1/google/cloud/source_context_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:26.063948 google-cloud-source-context-1.4.1/google/cloud/source_context_v1/types/
--rw-rw-r--   0 root         (0)     1003     1117 2023-01-23 15:38:59.000000 google-cloud-source-context-1.4.1/google/cloud/source_context_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    11557 2023-01-23 15:38:59.000000 google-cloud-source-context-1.4.1/google/cloud/source_context_v1/types/source_context.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:26.063948 google-cloud-source-context-1.4.1/google_cloud_source_context.egg-info/
--rw-r--r--   0 root         (0)     1003     4490 2023-01-23 15:42:26.000000 google-cloud-source-context-1.4.1/google_cloud_source_context.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1051 2023-01-23 15:42:26.000000 google-cloud-source-context-1.4.1/google_cloud_source_context.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-23 15:42:26.000000 google-cloud-source-context-1.4.1/google_cloud_source_context.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-23 15:42:26.000000 google-cloud-source-context-1.4.1/google_cloud_source_context.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-23 15:42:26.000000 google-cloud-source-context-1.4.1/google_cloud_source_context.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-01-23 15:42:26.000000 google-cloud-source-context-1.4.1/google_cloud_source_context.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-23 15:42:26.000000 google-cloud-source-context-1.4.1/google_cloud_source_context.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-01-23 15:42:26.063948 google-cloud-source-context-1.4.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3008 2023-01-23 15:38:59.000000 google-cloud-source-context-1.4.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:26.063948 google-cloud-source-context-1.4.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:38:59.000000 google-cloud-source-context-1.4.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:26.063948 google-cloud-source-context-1.4.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:38:59.000000 google-cloud-source-context-1.4.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:26.063948 google-cloud-source-context-1.4.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:38:59.000000 google-cloud-source-context-1.4.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:42:26.063948 google-cloud-source-context-1.4.1/tests/unit/gapic/source_context_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:38:59.000000 google-cloud-source-context-1.4.1/tests/unit/gapic/source_context_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      818 2023-01-23 15:38:59.000000 google-cloud-source-context-1.4.1/tests/unit/gapic/source_context_v1/test_source_context_v1.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:00.777451 google-cloud-source-context-1.4.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-source-context-1.4.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-source-context-1.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4452 2023-07-05 15:56:00.777451 google-cloud-source-context-1.4.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3517 2023-07-05 15:46:59.000000 google-cloud-source-context-1.4.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:00.769451 google-cloud-source-context-1.4.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:00.769451 google-cloud-source-context-1.4.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:00.773451 google-cloud-source-context-1.4.2/google/cloud/source_context/
+-rw-rw-r--   0 root         (0)     1003     1271 2023-07-05 15:46:59.000000 google-cloud-source-context-1.4.2/google/cloud/source_context/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-source-context-1.4.2/google/cloud/source_context/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       88 2023-07-05 15:46:59.000000 google-cloud-source-context-1.4.2/google/cloud/source_context/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:00.773451 google-cloud-source-context-1.4.2/google/cloud/source_context_v1/
+-rw-rw-r--   0 root         (0)     1003     1244 2023-07-05 15:46:59.000000 google-cloud-source-context-1.4.2/google/cloud/source_context_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      244 2023-07-05 15:46:59.000000 google-cloud-source-context-1.4.2/google/cloud/source_context_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-source-context-1.4.2/google/cloud/source_context_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       88 2023-07-05 15:46:59.000000 google-cloud-source-context-1.4.2/google/cloud/source_context_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:00.773451 google-cloud-source-context-1.4.2/google/cloud/source_context_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-source-context-1.4.2/google/cloud/source_context_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:00.773451 google-cloud-source-context-1.4.2/google/cloud/source_context_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1117 2023-07-05 15:46:59.000000 google-cloud-source-context-1.4.2/google/cloud/source_context_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11593 2023-07-05 15:46:59.000000 google-cloud-source-context-1.4.2/google/cloud/source_context_v1/types/source_context.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:00.777451 google-cloud-source-context-1.4.2/google_cloud_source_context.egg-info/
+-rw-r--r--   0 root         (0)     1003     4452 2023-07-05 15:56:00.000000 google-cloud-source-context-1.4.2/google_cloud_source_context.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1051 2023-07-05 15:56:00.000000 google-cloud-source-context-1.4.2/google_cloud_source_context.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:56:00.000000 google-cloud-source-context-1.4.2/google_cloud_source_context.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:56:00.000000 google-cloud-source-context-1.4.2/google_cloud_source_context.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:56:00.000000 google-cloud-source-context-1.4.2/google_cloud_source_context.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:56:00.000000 google-cloud-source-context-1.4.2/google_cloud_source_context.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:56:00.000000 google-cloud-source-context-1.4.2/google_cloud_source_context.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:56:00.777451 google-cloud-source-context-1.4.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2953 2023-07-05 15:46:59.000000 google-cloud-source-context-1.4.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:00.777451 google-cloud-source-context-1.4.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-source-context-1.4.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:00.777451 google-cloud-source-context-1.4.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-source-context-1.4.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:00.777451 google-cloud-source-context-1.4.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-source-context-1.4.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:00.777451 google-cloud-source-context-1.4.2/tests/unit/gapic/source_context_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-source-context-1.4.2/tests/unit/gapic/source_context_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      818 2023-07-05 15:46:59.000000 google-cloud-source-context-1.4.2/tests/unit/gapic/source_context_v1/test_source_context_v1.py
```

### Comparing `google-cloud-source-context-1.4.1/LICENSE` & `google-cloud-source-context-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-source-context-1.4.1/MANIFEST.in` & `google-cloud-source-context-1.4.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-source-context-1.4.1/PKG-INFO` & `google-cloud-source-context-1.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-source-context
-Version: 1.4.1
+Version: 1.4.2
 Summary: Google Cloud Source Context API client library
-Home-page: https://github.com/googleapis/python-source-context
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
 
-Python Client for Source Context API
-====================================
+Python Client for Source Context
+================================
 
 |stable| |pypi| |versions|
 
-`Source Context API`_: 
+`Source Context`_: 
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-source-context.svg
    :target: https://pypi.org/project/google-cloud-source-context/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-source-context.svg
    :target: https://pypi.org/project/google-cloud-source-context/
-.. _Source Context API: https://cloud.google.com
+.. _Source Context: https://cloud.google.com
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/source/latest
 .. _Product Documentation:  https://cloud.google.com
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Source Context API.`_
+3. `Enable the Source Context.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Source Context API.:  https://cloud.google.com
+.. _Enable the Source Context.:  https://cloud.google.com
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-source-context
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Source Context API
+-  Read the `Client Library Documentation`_ for Source Context
    to see other available methods on the client.
--  Read the `Source Context API Product documentation`_ to learn
+-  Read the `Source Context Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Source Context API Product documentation:  https://cloud.google.com
+.. _Source Context Product documentation:  https://cloud.google.com
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-source-context-1.4.1/README.rst` & `google-cloud-source-context-1.4.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Source Context API
-====================================
+Python Client for Source Context
+================================
 
 |stable| |pypi| |versions|
 
-`Source Context API`_: 
+`Source Context`_: 
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-source-context.svg
    :target: https://pypi.org/project/google-cloud-source-context/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-source-context.svg
    :target: https://pypi.org/project/google-cloud-source-context/
-.. _Source Context API: https://cloud.google.com
+.. _Source Context: https://cloud.google.com
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/source/latest
 .. _Product Documentation:  https://cloud.google.com
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Source Context API.`_
+3. `Enable the Source Context.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Source Context API.:  https://cloud.google.com
+.. _Enable the Source Context.:  https://cloud.google.com
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-source-context
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Source Context API
+-  Read the `Client Library Documentation`_ for Source Context
    to see other available methods on the client.
--  Read the `Source Context API Product documentation`_ to learn
+-  Read the `Source Context Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Source Context API Product documentation:  https://cloud.google.com
+.. _Source Context Product documentation:  https://cloud.google.com
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-source-context-1.4.1/google/cloud/source_context/__init__.py` & `google-cloud-source-context-1.4.2/google/cloud/source_context/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-source-context-1.4.1/google/cloud/source_context/gapic_version.py` & `google-cloud-source-context-1.4.2/google/cloud/source_context_v1/services/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.4.1"  # {x-release-please-version}
```

### Comparing `google-cloud-source-context-1.4.1/google/cloud/source_context_v1/__init__.py` & `google-cloud-source-context-1.4.2/google/cloud/source_context_v1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.source_context import gapic_version as package_version
+from google.cloud.source_context_v1 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
 from .types.source_context import (
     AliasContext,
     CloudRepoSourceContext,
```

### Comparing `google-cloud-source-context-1.4.1/google/cloud/source_context_v1/gapic_version.py` & `google-cloud-source-context-1.4.2/tests/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.4.1"  # {x-release-please-version}
```

### Comparing `google-cloud-source-context-1.4.1/google/cloud/source_context_v1/services/__init__.py` & `google-cloud-source-context-1.4.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-source-context-1.4.1/google/cloud/source_context_v1/types/__init__.py` & `google-cloud-source-context-1.4.2/google/cloud/source_context_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-source-context-1.4.1/google/cloud/source_context_v1/types/source_context.py` & `google-cloud-source-context-1.4.2/google/cloud/source_context_v1/types/source_context.py`

 * *Files 1% similar despite different names*

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
     package="google.devtools.source.v1",
     manifest={
```

### Comparing `google-cloud-source-context-1.4.1/google_cloud_source_context.egg-info/PKG-INFO` & `google-cloud-source-context-1.4.2/google_cloud_source_context.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-source-context
-Version: 1.4.1
+Version: 1.4.2
 Summary: Google Cloud Source Context API client library
-Home-page: https://github.com/googleapis/python-source-context
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
 
-Python Client for Source Context API
-====================================
+Python Client for Source Context
+================================
 
 |stable| |pypi| |versions|
 
-`Source Context API`_: 
+`Source Context`_: 
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-source-context.svg
    :target: https://pypi.org/project/google-cloud-source-context/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-source-context.svg
    :target: https://pypi.org/project/google-cloud-source-context/
-.. _Source Context API: https://cloud.google.com
+.. _Source Context: https://cloud.google.com
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/source/latest
 .. _Product Documentation:  https://cloud.google.com
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Source Context API.`_
+3. `Enable the Source Context.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Source Context API.:  https://cloud.google.com
+.. _Enable the Source Context.:  https://cloud.google.com
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-source-context
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Source Context API
+-  Read the `Client Library Documentation`_ for Source Context
    to see other available methods on the client.
--  Read the `Source Context API Product documentation`_ to learn
+-  Read the `Source Context Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Source Context API Product documentation:  https://cloud.google.com
+.. _Source Context Product documentation:  https://cloud.google.com
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-source-context-1.4.1/google_cloud_source_context.egg-info/SOURCES.txt` & `google-cloud-source-context-1.4.2/google_cloud_source_context.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-source-context-1.4.1/setup.py` & `google-cloud-source-context-1.4.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,31 +39,29 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-source-context"
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

### Comparing `google-cloud-source-context-1.4.1/tests/__init__.py` & `google-cloud-source-context-1.4.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-source-context-1.4.1/tests/unit/__init__.py` & `google-cloud-source-context-1.4.2/tests/unit/gapic/source_context_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-source-context-1.4.1/tests/unit/gapic/source_context_v1/test_source_context_v1.py` & `google-cloud-source-context-1.4.2/tests/unit/gapic/source_context_v1/test_source_context_v1.py`

 * *Files identical despite different names*

