# Comparing `tmp/google-cloud-storageinsights-0.1.0.tar.gz` & `tmp/google-cloud-storageinsights-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-storageinsights-0.1.0.tar", last modified: Wed Apr 19 15:28:52 2023, max compression
+gzip compressed data, was "google-cloud-storageinsights-0.1.1.tar", last modified: Wed Jul  5 15:56:05 2023, max compression
```

## Comparing `google-cloud-storageinsights-0.1.0.tar` & `google-cloud-storageinsights-0.1.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 15:28:52.145805 google-cloud-storageinsights-0.1.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4763 2023-04-19 15:28:52.145805 google-cloud-storageinsights-0.1.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3839 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 15:28:52.133806 google-cloud-storageinsights-0.1.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 15:28:52.137806 google-cloud-storageinsights-0.1.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 15:28:52.137806 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights/
--rw-rw-r--   0 root         (0)     1003     2094 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 15:28:52.137806 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/
--rw-rw-r--   0 root         (0)     1003     1928 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3421 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 15:28:52.137806 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 15:28:52.141805 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/storage_insights/
--rw-rw-r--   0 root         (0)     1003      773 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/storage_insights/__init__.py
--rw-rw-r--   0 root         (0)     1003    54100 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/storage_insights/async_client.py
--rw-rw-r--   0 root         (0)     1003    63688 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/storage_insights/client.py
--rw-rw-r--   0 root         (0)     1003    11228 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/storage_insights/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 15:28:52.141805 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/storage_insights/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/storage_insights/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11838 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/storage_insights/transports/base.py
--rw-rw-r--   0 root         (0)     1003    24149 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/storage_insights/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    24537 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/storage_insights/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    63859 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/storage_insights/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 15:28:52.141805 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/types/
--rw-rw-r--   0 root         (0)     1003     1648 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    23487 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/types/storageinsights.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 15:28:52.141805 google-cloud-storageinsights-0.1.0/google_cloud_storageinsights.egg-info/
--rw-r--r--   0 root         (0)     1003     4763 2023-04-19 15:28:52.000000 google-cloud-storageinsights-0.1.0/google_cloud_storageinsights.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1737 2023-04-19 15:28:52.000000 google-cloud-storageinsights-0.1.0/google_cloud_storageinsights.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-19 15:28:52.000000 google-cloud-storageinsights-0.1.0/google_cloud_storageinsights.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-04-19 15:28:52.000000 google-cloud-storageinsights-0.1.0/google_cloud_storageinsights.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-19 15:28:52.000000 google-cloud-storageinsights-0.1.0/google_cloud_storageinsights.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-04-19 15:28:52.000000 google-cloud-storageinsights-0.1.0/google_cloud_storageinsights.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-19 15:28:52.000000 google-cloud-storageinsights-0.1.0/google_cloud_storageinsights.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-04-19 15:28:52.145805 google-cloud-storageinsights-0.1.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2956 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 15:28:52.145805 google-cloud-storageinsights-0.1.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 15:28:52.145805 google-cloud-storageinsights-0.1.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 15:28:52.145805 google-cloud-storageinsights-0.1.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 15:28:52.145805 google-cloud-storageinsights-0.1.0/tests/unit/gapic/storageinsights_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/tests/unit/gapic/storageinsights_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   257220 2023-04-19 15:26:06.000000 google-cloud-storageinsights-0.1.0/tests/unit/gapic/storageinsights_v1/test_storage_insights.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:05.441296 google-cloud-storageinsights-0.1.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4763 2023-07-05 15:56:05.441296 google-cloud-storageinsights-0.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3839 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:05.433297 google-cloud-storageinsights-0.1.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:05.433297 google-cloud-storageinsights-0.1.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:05.437296 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights/
+-rw-rw-r--   0 root         (0)     1003     2094 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:05.437296 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/
+-rw-rw-r--   0 root         (0)     1003     1928 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3421 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:05.437296 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:05.437296 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/storage_insights/
+-rw-rw-r--   0 root         (0)     1003      773 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/storage_insights/__init__.py
+-rw-rw-r--   0 root         (0)     1003    54132 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/storage_insights/async_client.py
+-rw-rw-r--   0 root         (0)     1003    63688 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/storage_insights/client.py
+-rw-rw-r--   0 root         (0)     1003    11228 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/storage_insights/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:05.441296 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/storage_insights/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/storage_insights/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11838 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/storage_insights/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    24149 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/storage_insights/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    24537 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/storage_insights/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    63847 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/storage_insights/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:05.441296 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1648 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    23487 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/types/storageinsights.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:05.441296 google-cloud-storageinsights-0.1.1/google_cloud_storageinsights.egg-info/
+-rw-r--r--   0 root         (0)     1003     4763 2023-07-05 15:56:05.000000 google-cloud-storageinsights-0.1.1/google_cloud_storageinsights.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1737 2023-07-05 15:56:05.000000 google-cloud-storageinsights-0.1.1/google_cloud_storageinsights.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:56:05.000000 google-cloud-storageinsights-0.1.1/google_cloud_storageinsights.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:56:05.000000 google-cloud-storageinsights-0.1.1/google_cloud_storageinsights.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:56:05.000000 google-cloud-storageinsights-0.1.1/google_cloud_storageinsights.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:56:05.000000 google-cloud-storageinsights-0.1.1/google_cloud_storageinsights.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:56:05.000000 google-cloud-storageinsights-0.1.1/google_cloud_storageinsights.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:56:05.441296 google-cloud-storageinsights-0.1.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2956 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:05.441296 google-cloud-storageinsights-0.1.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:05.441296 google-cloud-storageinsights-0.1.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:05.441296 google-cloud-storageinsights-0.1.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:05.441296 google-cloud-storageinsights-0.1.1/tests/unit/gapic/storageinsights_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/tests/unit/gapic/storageinsights_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   255902 2023-07-05 15:46:59.000000 google-cloud-storageinsights-0.1.1/tests/unit/gapic/storageinsights_v1/test_storage_insights.py
```

### Comparing `google-cloud-storageinsights-0.1.0/LICENSE` & `google-cloud-storageinsights-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/MANIFEST.in` & `google-cloud-storageinsights-0.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/PKG-INFO` & `google-cloud-storageinsights-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-storageinsights
-Version: 0.1.0
+Version: 0.1.1
 Summary: Google Cloud Storageinsights API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-storageinsights-0.1.0/README.rst` & `google-cloud-storageinsights-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/google/cloud/storageinsights/__init__.py` & `google-cloud-storageinsights-0.1.1/google/cloud/storageinsights/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/google/cloud/storageinsights/gapic_version.py` & `google-cloud-storageinsights-0.1.1/google/cloud/storageinsights/gapic_version.py`

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

### Comparing `google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/__init__.py` & `google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/gapic_metadata.json` & `google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/gapic_version.py` & `google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/gapic_version.py`

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

### Comparing `google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/__init__.py` & `google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/storage_insights/__init__.py` & `google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/storage_insights/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/storage_insights/async_client.py` & `google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/storage_insights/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1335,15 +1335,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "StorageInsightsAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/storage_insights/client.py` & `google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/storage_insights/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/storage_insights/pagers.py` & `google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/storage_insights/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/storage_insights/transports/__init__.py` & `google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/storage_insights/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/storage_insights/transports/base.py` & `google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/storage_insights/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/storage_insights/transports/grpc.py` & `google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/storage_insights/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/storage_insights/transports/grpc_asyncio.py` & `google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/storage_insights/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/services/storage_insights/transports/rest.py` & `google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/services/storage_insights/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1392,15 +1392,15 @@
 
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

### Comparing `google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/types/__init__.py` & `google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/google/cloud/storageinsights_v1/types/storageinsights.py` & `google-cloud-storageinsights-0.1.1/google/cloud/storageinsights_v1/types/storageinsights.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/google_cloud_storageinsights.egg-info/PKG-INFO` & `google-cloud-storageinsights-0.1.1/google_cloud_storageinsights.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-storageinsights
-Version: 0.1.0
+Version: 0.1.1
 Summary: Google Cloud Storageinsights API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-storageinsights-0.1.0/google_cloud_storageinsights.egg-info/SOURCES.txt` & `google-cloud-storageinsights-0.1.1/google_cloud_storageinsights.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/setup.py` & `google-cloud-storageinsights-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/tests/__init__.py` & `google-cloud-storageinsights-0.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/tests/unit/__init__.py` & `google-cloud-storageinsights-0.1.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/tests/unit/gapic/__init__.py` & `google-cloud-storageinsights-0.1.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/tests/unit/gapic/storageinsights_v1/__init__.py` & `google-cloud-storageinsights-0.1.1/tests/unit/gapic/storageinsights_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storageinsights-0.1.0/tests/unit/gapic/storageinsights_v1/test_storage_insights.py` & `google-cloud-storageinsights-0.1.1/tests/unit/gapic/storageinsights_v1/test_storage_insights.py`

 * *Files 1% similar despite different names*

```diff
@@ -1168,17 +1168,19 @@
                     storageinsights.ReportConfig(),
                     storageinsights.ReportConfig(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_report_configs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1201,20 +1203,14 @@
     with mock.patch.object(
         type(client.transport.get_report_config), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = storageinsights.ReportConfig(
             name="name_value",
             display_name="display_name_value",
-            csv_options=storageinsights.CSVOptions(
-                record_separator="record_separator_value"
-            ),
-            object_metadata_report_options=storageinsights.ObjectMetadataReportOptions(
-                metadata_fields=["metadata_fields_value"]
-            ),
         )
         response = client.get_report_config(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == storageinsights.GetReportConfigRequest()
@@ -1457,20 +1453,14 @@
     with mock.patch.object(
         type(client.transport.create_report_config), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = storageinsights.ReportConfig(
             name="name_value",
             display_name="display_name_value",
-            csv_options=storageinsights.CSVOptions(
-                record_separator="record_separator_value"
-            ),
-            object_metadata_report_options=storageinsights.ObjectMetadataReportOptions(
-                metadata_fields=["metadata_fields_value"]
-            ),
         )
         response = client.create_report_config(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == storageinsights.CreateReportConfigRequest()
@@ -1724,20 +1714,14 @@
     with mock.patch.object(
         type(client.transport.update_report_config), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = storageinsights.ReportConfig(
             name="name_value",
             display_name="display_name_value",
-            csv_options=storageinsights.CSVOptions(
-                record_separator="record_separator_value"
-            ),
-            object_metadata_report_options=storageinsights.ObjectMetadataReportOptions(
-                metadata_fields=["metadata_fields_value"]
-            ),
         )
         response = client.update_report_config(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == storageinsights.UpdateReportConfigRequest()
@@ -2640,17 +2624,19 @@
                     storageinsights.ReportDetail(),
                     storageinsights.ReportDetail(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_report_details(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3271,20 +3257,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = storageinsights.ReportConfig(
             name="name_value",
             display_name="display_name_value",
-            csv_options=storageinsights.CSVOptions(
-                record_separator="record_separator_value"
-            ),
-            object_metadata_report_options=storageinsights.ObjectMetadataReportOptions(
-                metadata_fields=["metadata_fields_value"]
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = storageinsights.ReportConfig.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -3575,20 +3555,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = storageinsights.ReportConfig(
             name="name_value",
             display_name="display_name_value",
-            csv_options=storageinsights.CSVOptions(
-                record_separator="record_separator_value"
-            ),
-            object_metadata_report_options=storageinsights.ObjectMetadataReportOptions(
-                metadata_fields=["metadata_fields_value"]
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = storageinsights.ReportConfig.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -3920,20 +3894,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = storageinsights.ReportConfig(
             name="name_value",
             display_name="display_name_value",
-            csv_options=storageinsights.CSVOptions(
-                record_separator="record_separator_value"
-            ),
-            object_metadata_report_options=storageinsights.ObjectMetadataReportOptions(
-                metadata_fields=["metadata_fields_value"]
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = storageinsights.ReportConfig.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

