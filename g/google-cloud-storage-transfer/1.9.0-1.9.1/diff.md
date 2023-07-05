# Comparing `tmp/google-cloud-storage-transfer-1.9.0.tar.gz` & `tmp/google-cloud-storage-transfer-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-storage-transfer-1.9.0.tar", last modified: Wed Jun 28 22:20:48 2023, max compression
+gzip compressed data, was "google-cloud-storage-transfer-1.9.1.tar", last modified: Wed Jul  5 15:33:13 2023, max compression
```

## Comparing `google-cloud-storage-transfer-1.9.0.tar` & `google-cloud-storage-transfer-1.9.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-28 22:20:48.953781 google-cloud-storage-transfer-1.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4761 2023-06-28 22:20:48.953781 google-cloud-storage-transfer-1.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3818 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-28 22:20:48.945781 google-cloud-storage-transfer-1.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-28 22:20:48.945781 google-cloud-storage-transfer-1.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-28 22:20:48.949781 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer/
--rw-rw-r--   0 root         (0)     1003     3231 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-28 22:20:48.949781 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/
--rw-rw-r--   0 root         (0)     1003     3035 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     6180 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-28 22:20:48.949781 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-28 22:20:48.949781 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/storage_transfer_service/
--rw-rw-r--   0 root         (0)     1003      801 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/storage_transfer_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    69442 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/storage_transfer_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    80424 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/storage_transfer_service/client.py
--rw-rw-r--   0 root         (0)     1003    10982 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/storage_transfer_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-28 22:20:48.949781 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/
--rw-rw-r--   0 root         (0)     1003     1533 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12943 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    31284 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    31949 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    88847 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-28 22:20:48.953781 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/types/
--rw-rw-r--   0 root         (0)     1003     2699 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    14227 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/types/transfer.py
--rw-rw-r--   0 root         (0)     1003    81425 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/types/transfer_types.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-28 22:20:48.953781 google-cloud-storage-transfer-1.9.0/google_cloud_storage_transfer.egg-info/
--rw-r--r--   0 root         (0)     1003     4761 2023-06-28 22:20:48.000000 google-cloud-storage-transfer-1.9.0/google_cloud_storage_transfer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1905 2023-06-28 22:20:48.000000 google-cloud-storage-transfer-1.9.0/google_cloud_storage_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-28 22:20:48.000000 google-cloud-storage-transfer-1.9.0/google_cloud_storage_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-06-28 22:20:48.000000 google-cloud-storage-transfer-1.9.0/google_cloud_storage_transfer.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-28 22:20:48.000000 google-cloud-storage-transfer-1.9.0/google_cloud_storage_transfer.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-06-28 22:20:48.000000 google-cloud-storage-transfer-1.9.0/google_cloud_storage_transfer.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-28 22:20:48.000000 google-cloud-storage-transfer-1.9.0/google_cloud_storage_transfer.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-06-28 22:20:48.953781 google-cloud-storage-transfer-1.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2963 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-28 22:20:48.953781 google-cloud-storage-transfer-1.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-28 22:20:48.953781 google-cloud-storage-transfer-1.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-28 22:20:48.953781 google-cloud-storage-transfer-1.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-28 22:20:48.953781 google-cloud-storage-transfer-1.9.0/tests/unit/gapic/storage_transfer_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/tests/unit/gapic/storage_transfer_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   321810 2023-06-28 22:18:08.000000 google-cloud-storage-transfer-1.9.0/tests/unit/gapic/storage_transfer_v1/test_storage_transfer_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:33:13.689967 google-cloud-storage-transfer-1.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4761 2023-07-05 15:33:13.689967 google-cloud-storage-transfer-1.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3818 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:33:13.681971 google-cloud-storage-transfer-1.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:33:13.681971 google-cloud-storage-transfer-1.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:33:13.681971 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer/
+-rw-rw-r--   0 root         (0)     1003     3231 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:33:13.681971 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/
+-rw-rw-r--   0 root         (0)     1003     3035 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6180 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:33:13.685969 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:33:13.685969 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/storage_transfer_service/
+-rw-rw-r--   0 root         (0)     1003      801 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/storage_transfer_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    69481 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/storage_transfer_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    80424 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/storage_transfer_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10982 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/storage_transfer_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:33:13.685969 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1533 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12943 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    31284 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    31949 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    88835 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:33:13.685969 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2699 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14227 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/types/transfer.py
+-rw-rw-r--   0 root         (0)     1003    81425 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/types/transfer_types.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:33:13.685969 google-cloud-storage-transfer-1.9.1/google_cloud_storage_transfer.egg-info/
+-rw-r--r--   0 root         (0)     1003     4761 2023-07-05 15:33:13.000000 google-cloud-storage-transfer-1.9.1/google_cloud_storage_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1905 2023-07-05 15:33:13.000000 google-cloud-storage-transfer-1.9.1/google_cloud_storage_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:33:13.000000 google-cloud-storage-transfer-1.9.1/google_cloud_storage_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:33:13.000000 google-cloud-storage-transfer-1.9.1/google_cloud_storage_transfer.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:33:13.000000 google-cloud-storage-transfer-1.9.1/google_cloud_storage_transfer.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:33:13.000000 google-cloud-storage-transfer-1.9.1/google_cloud_storage_transfer.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:33:13.000000 google-cloud-storage-transfer-1.9.1/google_cloud_storage_transfer.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:33:13.689967 google-cloud-storage-transfer-1.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2963 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:33:13.685969 google-cloud-storage-transfer-1.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:33:13.685969 google-cloud-storage-transfer-1.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:33:13.689967 google-cloud-storage-transfer-1.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:33:13.689967 google-cloud-storage-transfer-1.9.1/tests/unit/gapic/storage_transfer_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/tests/unit/gapic/storage_transfer_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   322208 2023-07-05 15:30:43.000000 google-cloud-storage-transfer-1.9.1/tests/unit/gapic/storage_transfer_v1/test_storage_transfer_service.py
```

### Comparing `google-cloud-storage-transfer-1.9.0/LICENSE` & `google-cloud-storage-transfer-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/MANIFEST.in` & `google-cloud-storage-transfer-1.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/PKG-INFO` & `google-cloud-storage-transfer-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-storage-transfer
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Storage Transfer API client library
 Home-page: https://github.com/googleapis/python-storage-transfer
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-storage-transfer-1.9.0/README.rst` & `google-cloud-storage-transfer-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer/__init__.py` & `google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer/gapic_version.py` & `google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer/gapic_version.py`

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

### Comparing `google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/__init__.py` & `google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/gapic_metadata.json` & `google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/gapic_version.py` & `google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/gapic_version.py`

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

### Comparing `google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/__init__.py` & `google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/storage_transfer_service/__init__.py` & `google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/storage_transfer_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/storage_transfer_service/async_client.py` & `google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/storage_transfer_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1695,15 +1695,15 @@
         await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "StorageTransferServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/storage_transfer_service/client.py` & `google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/storage_transfer_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/storage_transfer_service/pagers.py` & `google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/storage_transfer_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/__init__.py` & `google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/base.py` & `google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/grpc.py` & `google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/grpc_asyncio.py` & `google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/rest.py` & `google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/services/storage_transfer_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -2090,15 +2090,15 @@
 
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

### Comparing `google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/types/__init__.py` & `google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/types/transfer.py` & `google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/types/transfer.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/google/cloud/storage_transfer_v1/types/transfer_types.py` & `google-cloud-storage-transfer-1.9.1/google/cloud/storage_transfer_v1/types/transfer_types.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/google_cloud_storage_transfer.egg-info/PKG-INFO` & `google-cloud-storage-transfer-1.9.1/google_cloud_storage_transfer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-storage-transfer
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Storage Transfer API client library
 Home-page: https://github.com/googleapis/python-storage-transfer
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-storage-transfer-1.9.0/google_cloud_storage_transfer.egg-info/SOURCES.txt` & `google-cloud-storage-transfer-1.9.1/google_cloud_storage_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/setup.py` & `google-cloud-storage-transfer-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/tests/__init__.py` & `google-cloud-storage-transfer-1.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/tests/unit/__init__.py` & `google-cloud-storage-transfer-1.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/tests/unit/gapic/__init__.py` & `google-cloud-storage-transfer-1.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/tests/unit/gapic/storage_transfer_v1/__init__.py` & `google-cloud-storage-transfer-1.9.1/tests/unit/gapic/storage_transfer_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-transfer-1.9.0/tests/unit/gapic/storage_transfer_v1/test_storage_transfer_service.py` & `google-cloud-storage-transfer-1.9.1/tests/unit/gapic/storage_transfer_v1/test_storage_transfer_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1660,17 +1660,19 @@
                     transfer_types.TransferJob(),
                     transfer_types.TransferJob(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_transfer_jobs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3453,17 +3455,19 @@
                     transfer_types.AgentPool(),
                     transfer_types.AgentPool(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_agent_pools(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

