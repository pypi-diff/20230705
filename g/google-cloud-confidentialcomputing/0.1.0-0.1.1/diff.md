# Comparing `tmp/google-cloud-confidentialcomputing-0.1.0.tar.gz` & `tmp/google-cloud-confidentialcomputing-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-confidentialcomputing-0.1.0.tar", last modified: Wed Apr 19 17:52:21 2023, max compression
+gzip compressed data, was "google-cloud-confidentialcomputing-0.1.1.tar", last modified: Wed Jul  5 15:51:32 2023, max compression
```

## Comparing `google-cloud-confidentialcomputing-0.1.0.tar` & `google-cloud-confidentialcomputing-0.1.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 17:52:21.894197 google-cloud-confidentialcomputing-0.1.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4822 2023-04-19 17:52:21.890196 google-cloud-confidentialcomputing-0.1.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3886 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 17:52:21.886196 google-cloud-confidentialcomputing-0.1.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 17:52:21.886196 google-cloud-confidentialcomputing-0.1.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 17:52:21.886196 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing/
--rw-rw-r--   0 root         (0)     1003     1446 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 17:52:21.886196 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/
--rw-rw-r--   0 root         (0)     1003     1269 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1480 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 17:52:21.886196 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 17:52:21.886196 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/
--rw-rw-r--   0 root         (0)     1003      797 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/__init__.py
--rw-rw-r--   0 root         (0)     1003    22580 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/async_client.py
--rw-rw-r--   0 root         (0)     1003    31103 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 17:52:21.890196 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/
--rw-rw-r--   0 root         (0)     1003     1519 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7821 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14797 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15031 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    25103 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 17:52:21.890196 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/types/
--rw-rw-r--   0 root         (0)     1003      940 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     8300 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 17:52:21.890196 google-cloud-confidentialcomputing-0.1.0/google_cloud_confidentialcomputing.egg-info/
--rw-r--r--   0 root         (0)     1003     4822 2023-04-19 17:52:21.000000 google-cloud-confidentialcomputing-0.1.0/google_cloud_confidentialcomputing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1877 2023-04-19 17:52:21.000000 google-cloud-confidentialcomputing-0.1.0/google_cloud_confidentialcomputing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-19 17:52:21.000000 google-cloud-confidentialcomputing-0.1.0/google_cloud_confidentialcomputing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-04-19 17:52:21.000000 google-cloud-confidentialcomputing-0.1.0/google_cloud_confidentialcomputing.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-19 17:52:21.000000 google-cloud-confidentialcomputing-0.1.0/google_cloud_confidentialcomputing.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-04-19 17:52:21.000000 google-cloud-confidentialcomputing-0.1.0/google_cloud_confidentialcomputing.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-19 17:52:21.000000 google-cloud-confidentialcomputing-0.1.0/google_cloud_confidentialcomputing.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-04-19 17:52:21.894197 google-cloud-confidentialcomputing-0.1.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2974 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 17:52:21.890196 google-cloud-confidentialcomputing-0.1.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 17:52:21.890196 google-cloud-confidentialcomputing-0.1.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 17:52:21.890196 google-cloud-confidentialcomputing-0.1.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 17:52:21.890196 google-cloud-confidentialcomputing-0.1.0/tests/unit/gapic/confidentialcomputing_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/tests/unit/gapic/confidentialcomputing_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   103349 2023-04-19 17:49:53.000000 google-cloud-confidentialcomputing-0.1.0/tests/unit/gapic/confidentialcomputing_v1/test_confidential_computing.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.552207 google-cloud-confidentialcomputing-0.1.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4822 2023-07-05 15:51:32.552207 google-cloud-confidentialcomputing-0.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3886 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.548206 google-cloud-confidentialcomputing-0.1.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.548206 google-cloud-confidentialcomputing-0.1.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.548206 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing/
+-rw-rw-r--   0 root         (0)     1003     1446 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.548206 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/
+-rw-rw-r--   0 root         (0)     1003     1269 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1480 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.548206 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.552207 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/
+-rw-rw-r--   0 root         (0)     1003      797 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22618 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/async_client.py
+-rw-rw-r--   0 root         (0)     1003    31103 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.552207 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/
+-rw-rw-r--   0 root         (0)     1003     1519 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7821 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14797 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15031 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    25103 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.552207 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/types/
+-rw-rw-r--   0 root         (0)     1003      940 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8300 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.552207 google-cloud-confidentialcomputing-0.1.1/google_cloud_confidentialcomputing.egg-info/
+-rw-r--r--   0 root         (0)     1003     4822 2023-07-05 15:51:32.000000 google-cloud-confidentialcomputing-0.1.1/google_cloud_confidentialcomputing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1877 2023-07-05 15:51:32.000000 google-cloud-confidentialcomputing-0.1.1/google_cloud_confidentialcomputing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:51:32.000000 google-cloud-confidentialcomputing-0.1.1/google_cloud_confidentialcomputing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:51:32.000000 google-cloud-confidentialcomputing-0.1.1/google_cloud_confidentialcomputing.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:51:32.000000 google-cloud-confidentialcomputing-0.1.1/google_cloud_confidentialcomputing.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:51:32.000000 google-cloud-confidentialcomputing-0.1.1/google_cloud_confidentialcomputing.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:51:32.000000 google-cloud-confidentialcomputing-0.1.1/google_cloud_confidentialcomputing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:51:32.556207 google-cloud-confidentialcomputing-0.1.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2974 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.552207 google-cloud-confidentialcomputing-0.1.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.552207 google-cloud-confidentialcomputing-0.1.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.552207 google-cloud-confidentialcomputing-0.1.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.552207 google-cloud-confidentialcomputing-0.1.1/tests/unit/gapic/confidentialcomputing_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/tests/unit/gapic/confidentialcomputing_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   103349 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/tests/unit/gapic/confidentialcomputing_v1/test_confidential_computing.py
```

### Comparing `google-cloud-confidentialcomputing-0.1.0/LICENSE` & `google-cloud-confidentialcomputing-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/MANIFEST.in` & `google-cloud-confidentialcomputing-0.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/PKG-INFO` & `google-cloud-confidentialcomputing-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-confidentialcomputing
-Version: 0.1.0
+Version: 0.1.1
 Summary: Google Cloud Confidentialcomputing API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-confidentialcomputing-0.1.0/README.rst` & `google-cloud-confidentialcomputing-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing/__init__.py` & `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing/gapic_version.py` & `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing/gapic_version.py`

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
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.1.1"  # {x-release-please-version}
```

### Comparing `google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/__init__.py` & `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/gapic_metadata.json` & `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/gapic_version.py` & `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/gapic_version.py`

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
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.1.1"  # {x-release-please-version}
```

### Comparing `google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/services/__init__.py` & `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/__init__.py` & `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/async_client.py` & `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -544,15 +544,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ConfidentialComputingAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/client.py` & `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/__init__.py` & `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/base.py` & `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/grpc.py` & `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/grpc_asyncio.py` & `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/rest.py` & `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/types/__init__.py` & `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/google/cloud/confidentialcomputing_v1/types/service.py` & `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/google_cloud_confidentialcomputing.egg-info/PKG-INFO` & `google-cloud-confidentialcomputing-0.1.1/google_cloud_confidentialcomputing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-confidentialcomputing
-Version: 0.1.0
+Version: 0.1.1
 Summary: Google Cloud Confidentialcomputing API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-confidentialcomputing-0.1.0/google_cloud_confidentialcomputing.egg-info/SOURCES.txt` & `google-cloud-confidentialcomputing-0.1.1/google_cloud_confidentialcomputing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/setup.py` & `google-cloud-confidentialcomputing-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/tests/__init__.py` & `google-cloud-confidentialcomputing-0.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/tests/unit/__init__.py` & `google-cloud-confidentialcomputing-0.1.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/tests/unit/gapic/__init__.py` & `google-cloud-confidentialcomputing-0.1.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/tests/unit/gapic/confidentialcomputing_v1/__init__.py` & `google-cloud-confidentialcomputing-0.1.1/tests/unit/gapic/confidentialcomputing_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.0/tests/unit/gapic/confidentialcomputing_v1/test_confidential_computing.py` & `google-cloud-confidentialcomputing-0.1.1/tests/unit/gapic/confidentialcomputing_v1/test_confidential_computing.py`

 * *Files identical despite different names*

