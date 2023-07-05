# Comparing `tmp/google-cloud-filestore-1.6.0.tar.gz` & `tmp/google-cloud-filestore-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-filestore-1.6.0.tar", last modified: Mon Mar 27 15:44:34 2023, max compression
+gzip compressed data, was "google-cloud-filestore-1.6.1.tar", last modified: Wed Jul  5 15:23:23 2023, max compression
```

## Comparing `google-cloud-filestore-1.6.0.tar` & `google-cloud-filestore-1.6.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:34.596133 google-cloud-filestore-1.6.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4635 2023-03-27 15:44:34.596133 google-cloud-filestore-1.6.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3713 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:34.588129 google-cloud-filestore-1.6.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:34.588129 google-cloud-filestore-1.6.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:34.592131 google-cloud-filestore-1.6.0/google/cloud/filestore/
--rw-rw-r--   0 root         (0)     1003     2350 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/google/cloud/filestore/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/google/cloud/filestore/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       83 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/google/cloud/filestore/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:34.592131 google-cloud-filestore-1.6.0/google/cloud/filestore_v1/
--rw-rw-r--   0 root         (0)     1003     2208 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/google/cloud/filestore_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     6514 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/google/cloud/filestore_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/google/cloud/filestore_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       83 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/google/cloud/filestore_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:34.592131 google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:34.592131 google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/cloud_filestore_manager/
--rw-rw-r--   0 root         (0)     1003      797 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/cloud_filestore_manager/__init__.py
--rw-rw-r--   0 root         (0)     1003    91566 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/cloud_filestore_manager/async_client.py
--rw-rw-r--   0 root         (0)     1003   102946 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/cloud_filestore_manager/client.py
--rw-rw-r--   0 root         (0)     1003    16146 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/cloud_filestore_manager/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:34.596133 google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/
--rw-rw-r--   0 root         (0)     1003     1519 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14646 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/base.py
--rw-rw-r--   0 root         (0)     1003    31330 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    32034 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    93909 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:34.596133 google-cloud-filestore-1.6.0/google/cloud/filestore_v1/types/
--rw-rw-r--   0 root         (0)     1003     1890 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/google/cloud/filestore_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    39664 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/google/cloud/filestore_v1/types/cloud_filestore_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:34.596133 google-cloud-filestore-1.6.0/google_cloud_filestore.egg-info/
--rw-r--r--   0 root         (0)     1003     4635 2023-03-27 15:44:34.000000 google-cloud-filestore-1.6.0/google_cloud_filestore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1657 2023-03-27 15:44:34.000000 google-cloud-filestore-1.6.0/google_cloud_filestore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:44:34.000000 google-cloud-filestore-1.6.0/google_cloud_filestore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:44:34.000000 google-cloud-filestore-1.6.0/google_cloud_filestore.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:44:34.000000 google-cloud-filestore-1.6.0/google_cloud_filestore.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 15:44:34.000000 google-cloud-filestore-1.6.0/google_cloud_filestore.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:44:34.000000 google-cloud-filestore-1.6.0/google_cloud_filestore.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:44:34.596133 google-cloud-filestore-1.6.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3029 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:34.596133 google-cloud-filestore-1.6.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:34.596133 google-cloud-filestore-1.6.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:34.596133 google-cloud-filestore-1.6.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:44:34.596133 google-cloud-filestore-1.6.0/tests/unit/gapic/filestore_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/tests/unit/gapic/filestore_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   395376 2023-03-27 15:42:03.000000 google-cloud-filestore-1.6.0/tests/unit/gapic/filestore_v1/test_cloud_filestore_manager.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:23.132641 google-cloud-filestore-1.6.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4635 2023-07-05 15:23:23.132641 google-cloud-filestore-1.6.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3713 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:23.124639 google-cloud-filestore-1.6.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:23.124639 google-cloud-filestore-1.6.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:23.128640 google-cloud-filestore-1.6.1/google/cloud/filestore/
+-rw-rw-r--   0 root         (0)     1003     2350 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/google/cloud/filestore/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/google/cloud/filestore/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       83 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/google/cloud/filestore/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:23.128640 google-cloud-filestore-1.6.1/google/cloud/filestore_v1/
+-rw-rw-r--   0 root         (0)     1003     2208 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/google/cloud/filestore_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6514 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/google/cloud/filestore_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/google/cloud/filestore_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       83 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/google/cloud/filestore_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:23.128640 google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:23.128640 google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/cloud_filestore_manager/
+-rw-rw-r--   0 root         (0)     1003      797 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/cloud_filestore_manager/__init__.py
+-rw-rw-r--   0 root         (0)     1003    91513 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/cloud_filestore_manager/async_client.py
+-rw-rw-r--   0 root         (0)     1003   102855 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/cloud_filestore_manager/client.py
+-rw-rw-r--   0 root         (0)     1003    16146 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/cloud_filestore_manager/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:23.128640 google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/
+-rw-rw-r--   0 root         (0)     1003     1519 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14646 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    31330 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    32034 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    93909 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:23.128640 google-cloud-filestore-1.6.1/google/cloud/filestore_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1890 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/google/cloud/filestore_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    39664 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/google/cloud/filestore_v1/types/cloud_filestore_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:23.132641 google-cloud-filestore-1.6.1/google_cloud_filestore.egg-info/
+-rw-r--r--   0 root         (0)     1003     4635 2023-07-05 15:23:23.000000 google-cloud-filestore-1.6.1/google_cloud_filestore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1657 2023-07-05 15:23:23.000000 google-cloud-filestore-1.6.1/google_cloud_filestore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:23:23.000000 google-cloud-filestore-1.6.1/google_cloud_filestore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:23:23.000000 google-cloud-filestore-1.6.1/google_cloud_filestore.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:23:23.000000 google-cloud-filestore-1.6.1/google_cloud_filestore.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:23:23.000000 google-cloud-filestore-1.6.1/google_cloud_filestore.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:23:23.000000 google-cloud-filestore-1.6.1/google_cloud_filestore.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:23:23.132641 google-cloud-filestore-1.6.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3029 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:23.132641 google-cloud-filestore-1.6.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:23.132641 google-cloud-filestore-1.6.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:23.132641 google-cloud-filestore-1.6.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:23.132641 google-cloud-filestore-1.6.1/tests/unit/gapic/filestore_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/tests/unit/gapic/filestore_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   395922 2023-07-05 15:21:04.000000 google-cloud-filestore-1.6.1/tests/unit/gapic/filestore_v1/test_cloud_filestore_manager.py
```

### Comparing `google-cloud-filestore-1.6.0/LICENSE` & `google-cloud-filestore-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/MANIFEST.in` & `google-cloud-filestore-1.6.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/PKG-INFO` & `google-cloud-filestore-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-filestore
-Version: 1.6.0
+Version: 1.6.1
 Summary: Google Cloud Filestore API client library
 Home-page: https://github.com/googleapis/python-filestore
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-filestore-1.6.0/README.rst` & `google-cloud-filestore-1.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/google/cloud/filestore/__init__.py` & `google-cloud-filestore-1.6.1/google/cloud/filestore/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/google/cloud/filestore/gapic_version.py` & `google-cloud-filestore-1.6.1/google/cloud/filestore/gapic_version.py`

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
-__version__ = "1.6.0"  # {x-release-please-version}
+__version__ = "1.6.1"  # {x-release-please-version}
```

### Comparing `google-cloud-filestore-1.6.0/google/cloud/filestore_v1/__init__.py` & `google-cloud-filestore-1.6.1/google/cloud/filestore_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/google/cloud/filestore_v1/gapic_metadata.json` & `google-cloud-filestore-1.6.1/google/cloud/filestore_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/google/cloud/filestore_v1/gapic_version.py` & `google-cloud-filestore-1.6.1/google/cloud/filestore_v1/gapic_version.py`

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
-__version__ = "1.6.0"  # {x-release-please-version}
+__version__ = "1.6.1"  # {x-release-please-version}
```

### Comparing `google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/__init__.py` & `google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/cloud_filestore_manager/__init__.py` & `google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/cloud_filestore_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/cloud_filestore_manager/async_client.py` & `google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/cloud_filestore_manager/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,17 +40,15 @@
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
-from google.cloud.common.types import (
-    operation_metadata as operation_metadata_pb2,
-)  # type: ignore
+from google.cloud.common.types import operation_metadata
 from google.protobuf import empty_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.protobuf import wrappers_pb2  # type: ignore
 
 from google.cloud.filestore_v1.services.cloud_filestore_manager import pagers
 from google.cloud.filestore_v1.types import cloud_filestore_service
@@ -632,15 +630,15 @@
         )
 
         # Wrap the response in an operation future.
         response = operation_async.from_gapic(
             response,
             self._client._transport.operations_client,
             cloud_filestore_service.Instance,
-            metadata_type=operation_metadata_pb2.OperationMetadata,
+            metadata_type=operation_metadata.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
     async def update_instance(
         self,
@@ -765,15 +763,15 @@
         )
 
         # Wrap the response in an operation future.
         response = operation_async.from_gapic(
             response,
             self._client._transport.operations_client,
             cloud_filestore_service.Instance,
-            metadata_type=operation_metadata_pb2.OperationMetadata,
+            metadata_type=operation_metadata.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
     async def restore_instance(
         self,
@@ -869,15 +867,15 @@
         )
 
         # Wrap the response in an operation future.
         response = operation_async.from_gapic(
             response,
             self._client._transport.operations_client,
             cloud_filestore_service.Instance,
-            metadata_type=operation_metadata_pb2.OperationMetadata,
+            metadata_type=operation_metadata.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
     async def delete_instance(
         self,
@@ -995,15 +993,15 @@
         )
 
         # Wrap the response in an operation future.
         response = operation_async.from_gapic(
             response,
             self._client._transport.operations_client,
             empty_pb2.Empty,
-            metadata_type=operation_metadata_pb2.OperationMetadata,
+            metadata_type=operation_metadata.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
     async def list_snapshots(
         self,
@@ -1359,15 +1357,15 @@
         )
 
         # Wrap the response in an operation future.
         response = operation_async.from_gapic(
             response,
             self._client._transport.operations_client,
             cloud_filestore_service.Snapshot,
-            metadata_type=operation_metadata_pb2.OperationMetadata,
+            metadata_type=operation_metadata.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
     async def delete_snapshot(
         self,
@@ -1485,15 +1483,15 @@
         )
 
         # Wrap the response in an operation future.
         response = operation_async.from_gapic(
             response,
             self._client._transport.operations_client,
             empty_pb2.Empty,
-            metadata_type=operation_metadata_pb2.OperationMetadata,
+            metadata_type=operation_metadata.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
     async def update_snapshot(
         self,
@@ -1615,15 +1613,15 @@
         )
 
         # Wrap the response in an operation future.
         response = operation_async.from_gapic(
             response,
             self._client._transport.operations_client,
             cloud_filestore_service.Snapshot,
-            metadata_type=operation_metadata_pb2.OperationMetadata,
+            metadata_type=operation_metadata.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
     async def list_backups(
         self,
@@ -2001,15 +1999,15 @@
         )
 
         # Wrap the response in an operation future.
         response = operation_async.from_gapic(
             response,
             self._client._transport.operations_client,
             cloud_filestore_service.Backup,
-            metadata_type=operation_metadata_pb2.OperationMetadata,
+            metadata_type=operation_metadata.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
     async def delete_backup(
         self,
@@ -2126,15 +2124,15 @@
         )
 
         # Wrap the response in an operation future.
         response = operation_async.from_gapic(
             response,
             self._client._transport.operations_client,
             empty_pb2.Empty,
-            metadata_type=operation_metadata_pb2.OperationMetadata,
+            metadata_type=operation_metadata.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
     async def update_backup(
         self,
@@ -2257,21 +2255,21 @@
         )
 
         # Wrap the response in an operation future.
         response = operation_async.from_gapic(
             response,
             self._client._transport.operations_client,
             cloud_filestore_service.Backup,
-            metadata_type=operation_metadata_pb2.OperationMetadata,
+            metadata_type=operation_metadata.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "CloudFilestoreManagerAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/cloud_filestore_manager/client.py` & `google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/cloud_filestore_manager/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,17 +44,15 @@
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
-from google.cloud.common.types import (
-    operation_metadata as operation_metadata_pb2,
-)  # type: ignore
+from google.cloud.common.types import operation_metadata
 from google.protobuf import empty_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.protobuf import wrappers_pb2  # type: ignore
 
 from google.cloud.filestore_v1.services.cloud_filestore_manager import pagers
 from google.cloud.filestore_v1.types import cloud_filestore_service
@@ -882,15 +880,15 @@
         )
 
         # Wrap the response in an operation future.
         response = operation.from_gapic(
             response,
             self._transport.operations_client,
             cloud_filestore_service.Instance,
-            metadata_type=operation_metadata_pb2.OperationMetadata,
+            metadata_type=operation_metadata.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
     def update_instance(
         self,
@@ -1015,15 +1013,15 @@
         )
 
         # Wrap the response in an operation future.
         response = operation.from_gapic(
             response,
             self._transport.operations_client,
             cloud_filestore_service.Instance,
-            metadata_type=operation_metadata_pb2.OperationMetadata,
+            metadata_type=operation_metadata.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
     def restore_instance(
         self,
@@ -1120,15 +1118,15 @@
         )
 
         # Wrap the response in an operation future.
         response = operation.from_gapic(
             response,
             self._transport.operations_client,
             cloud_filestore_service.Instance,
-            metadata_type=operation_metadata_pb2.OperationMetadata,
+            metadata_type=operation_metadata.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
     def delete_instance(
         self,
@@ -1246,15 +1244,15 @@
         )
 
         # Wrap the response in an operation future.
         response = operation.from_gapic(
             response,
             self._transport.operations_client,
             empty_pb2.Empty,
-            metadata_type=operation_metadata_pb2.OperationMetadata,
+            metadata_type=operation_metadata.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
     def list_snapshots(
         self,
@@ -1610,15 +1608,15 @@
         )
 
         # Wrap the response in an operation future.
         response = operation.from_gapic(
             response,
             self._transport.operations_client,
             cloud_filestore_service.Snapshot,
-            metadata_type=operation_metadata_pb2.OperationMetadata,
+            metadata_type=operation_metadata.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
     def delete_snapshot(
         self,
@@ -1736,15 +1734,15 @@
         )
 
         # Wrap the response in an operation future.
         response = operation.from_gapic(
             response,
             self._transport.operations_client,
             empty_pb2.Empty,
-            metadata_type=operation_metadata_pb2.OperationMetadata,
+            metadata_type=operation_metadata.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
     def update_snapshot(
         self,
@@ -1866,15 +1864,15 @@
         )
 
         # Wrap the response in an operation future.
         response = operation.from_gapic(
             response,
             self._transport.operations_client,
             cloud_filestore_service.Snapshot,
-            metadata_type=operation_metadata_pb2.OperationMetadata,
+            metadata_type=operation_metadata.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
     def list_backups(
         self,
@@ -2234,15 +2232,15 @@
         )
 
         # Wrap the response in an operation future.
         response = operation.from_gapic(
             response,
             self._transport.operations_client,
             cloud_filestore_service.Backup,
-            metadata_type=operation_metadata_pb2.OperationMetadata,
+            metadata_type=operation_metadata.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
     def delete_backup(
         self,
@@ -2359,15 +2357,15 @@
         )
 
         # Wrap the response in an operation future.
         response = operation.from_gapic(
             response,
             self._transport.operations_client,
             empty_pb2.Empty,
-            metadata_type=operation_metadata_pb2.OperationMetadata,
+            metadata_type=operation_metadata.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
     def update_backup(
         self,
@@ -2490,15 +2488,15 @@
         )
 
         # Wrap the response in an operation future.
         response = operation.from_gapic(
             response,
             self._transport.operations_client,
             cloud_filestore_service.Backup,
-            metadata_type=operation_metadata_pb2.OperationMetadata,
+            metadata_type=operation_metadata.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
     def __enter__(self) -> "CloudFilestoreManagerClient":
         return self
```

### Comparing `google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/cloud_filestore_manager/pagers.py` & `google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/cloud_filestore_manager/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/__init__.py` & `google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/base.py` & `google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/grpc.py` & `google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/grpc_asyncio.py` & `google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/rest.py` & `google-cloud-filestore-1.6.1/google/cloud/filestore_v1/services/cloud_filestore_manager/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/google/cloud/filestore_v1/types/__init__.py` & `google-cloud-filestore-1.6.1/google/cloud/filestore_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/google/cloud/filestore_v1/types/cloud_filestore_service.py` & `google-cloud-filestore-1.6.1/google/cloud/filestore_v1/types/cloud_filestore_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/google_cloud_filestore.egg-info/PKG-INFO` & `google-cloud-filestore-1.6.1/google_cloud_filestore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-filestore
-Version: 1.6.0
+Version: 1.6.1
 Summary: Google Cloud Filestore API client library
 Home-page: https://github.com/googleapis/python-filestore
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-filestore-1.6.0/google_cloud_filestore.egg-info/SOURCES.txt` & `google-cloud-filestore-1.6.1/google_cloud_filestore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/setup.py` & `google-cloud-filestore-1.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/tests/__init__.py` & `google-cloud-filestore-1.6.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/tests/unit/__init__.py` & `google-cloud-filestore-1.6.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/tests/unit/gapic/__init__.py` & `google-cloud-filestore-1.6.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/tests/unit/gapic/filestore_v1/__init__.py` & `google-cloud-filestore-1.6.1/tests/unit/gapic/filestore_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-filestore-1.6.0/tests/unit/gapic/filestore_v1/test_cloud_filestore_manager.py` & `google-cloud-filestore-1.6.1/tests/unit/gapic/filestore_v1/test_cloud_filestore_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,17 +37,15 @@
 )
 from google.api_core import client_options
 from google.api_core import exceptions as core_exceptions
 from google.api_core import operation_async  # type: ignore
 import google.auth
 from google.auth import credentials as ga_credentials
 from google.auth.exceptions import MutualTLSChannelError
-from google.cloud.common.types import (
-    operation_metadata as operation_metadata_pb2,
-)  # type: ignore
+from google.cloud.common.types import operation_metadata
 from google.longrunning import operations_pb2
 from google.oauth2 import service_account
 from google.protobuf import empty_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import json_format
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.protobuf import wrappers_pb2  # type: ignore
@@ -1178,17 +1176,19 @@
                     cloud_filestore_service.Instance(),
                     cloud_filestore_service.Instance(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_instances(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2724,17 +2724,19 @@
                     cloud_filestore_service.Snapshot(),
                     cloud_filestore_service.Snapshot(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_snapshots(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4105,17 +4107,19 @@
                     cloud_filestore_service.Backup(),
                     cloud_filestore_service.Backup(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_backups(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

