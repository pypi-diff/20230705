# Comparing `tmp/google-cloud-ids-1.5.1.tar.gz` & `tmp/google-cloud-ids-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-ids-1.5.1.tar", last modified: Fri Apr 21 13:52:32 2023, max compression
+gzip compressed data, was "google-cloud-ids-1.5.2.tar", last modified: Wed Jul  5 15:53:34 2023, max compression
```

## Comparing `google-cloud-ids-1.5.1.tar` & `google-cloud-ids-1.5.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.929609 google-cloud-ids-1.5.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4817 2023-04-21 13:52:32.929609 google-cloud-ids-1.5.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3904 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.921610 google-cloud-ids-1.5.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.921610 google-cloud-ids-1.5.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.925610 google-cloud-ids-1.5.1/google/cloud/ids/
--rw-rw-r--   0 root         (0)     1003     1292 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.925610 google-cloud-ids-1.5.1/google/cloud/ids_v1/
--rw-rw-r--   0 root         (0)     1003     1193 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2068 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.925610 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.925610 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/
--rw-rw-r--   0 root         (0)     1003      725 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/__init__.py
--rw-rw-r--   0 root         (0)     1003    28490 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/async_client.py
--rw-rw-r--   0 root         (0)     1003    37521 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/client.py
--rw-rw-r--   0 root         (0)     1003     5614 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.925610 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/
--rw-rw-r--   0 root         (0)     1003     1246 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8104 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15455 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15775 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    28432 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.925610 google-cloud-ids-1.5.1/google/cloud/ids_v1/types/
--rw-rw-r--   0 root         (0)     1003      986 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    12472 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/types/ids.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.929609 google-cloud-ids-1.5.1/google_cloud_ids.egg-info/
--rw-r--r--   0 root         (0)     1003     4817 2023-04-21 13:52:32.000000 google-cloud-ids-1.5.1/google_cloud_ids.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1269 2023-04-21 13:52:32.000000 google-cloud-ids-1.5.1/google_cloud_ids.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-21 13:52:32.000000 google-cloud-ids-1.5.1/google_cloud_ids.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-04-21 13:52:32.000000 google-cloud-ids-1.5.1/google_cloud_ids.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-21 13:52:32.000000 google-cloud-ids-1.5.1/google_cloud_ids.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-04-21 13:52:32.000000 google-cloud-ids-1.5.1/google_cloud_ids.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-21 13:52:32.000000 google-cloud-ids-1.5.1/google_cloud_ids.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-04-21 13:52:32.929609 google-cloud-ids-1.5.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2914 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.929609 google-cloud-ids-1.5.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.929609 google-cloud-ids-1.5.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.929609 google-cloud-ids-1.5.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.929609 google-cloud-ids-1.5.1/tests/unit/gapic/ids_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/tests/unit/gapic/ids_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   135027 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/tests/unit/gapic/ids_v1/test_ids.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:34.185076 google-cloud-ids-1.5.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4817 2023-07-05 15:53:34.185076 google-cloud-ids-1.5.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3904 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:34.177076 google-cloud-ids-1.5.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:34.177076 google-cloud-ids-1.5.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:34.181076 google-cloud-ids-1.5.2/google/cloud/ids/
+-rw-rw-r--   0 root         (0)     1003     1292 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/google/cloud/ids/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/google/cloud/ids/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/google/cloud/ids/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:34.181076 google-cloud-ids-1.5.2/google/cloud/ids_v1/
+-rw-rw-r--   0 root         (0)     1003     1193 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/google/cloud/ids_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2068 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/google/cloud/ids_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/google/cloud/ids_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/google/cloud/ids_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:34.181076 google-cloud-ids-1.5.2/google/cloud/ids_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/google/cloud/ids_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:34.181076 google-cloud-ids-1.5.2/google/cloud/ids_v1/services/ids/
+-rw-rw-r--   0 root         (0)     1003      725 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/google/cloud/ids_v1/services/ids/__init__.py
+-rw-rw-r--   0 root         (0)     1003    28510 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/google/cloud/ids_v1/services/ids/async_client.py
+-rw-rw-r--   0 root         (0)     1003    37521 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/google/cloud/ids_v1/services/ids/client.py
+-rw-rw-r--   0 root         (0)     1003     5614 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/google/cloud/ids_v1/services/ids/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:34.185076 google-cloud-ids-1.5.2/google/cloud/ids_v1/services/ids/transports/
+-rw-rw-r--   0 root         (0)     1003     1246 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/google/cloud/ids_v1/services/ids/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8104 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/google/cloud/ids_v1/services/ids/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15455 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/google/cloud/ids_v1/services/ids/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15775 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/google/cloud/ids_v1/services/ids/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    28432 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/google/cloud/ids_v1/services/ids/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:34.185076 google-cloud-ids-1.5.2/google/cloud/ids_v1/types/
+-rw-rw-r--   0 root         (0)     1003      986 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/google/cloud/ids_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12472 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/google/cloud/ids_v1/types/ids.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:34.185076 google-cloud-ids-1.5.2/google_cloud_ids.egg-info/
+-rw-r--r--   0 root         (0)     1003     4817 2023-07-05 15:53:34.000000 google-cloud-ids-1.5.2/google_cloud_ids.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1269 2023-07-05 15:53:34.000000 google-cloud-ids-1.5.2/google_cloud_ids.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:34.000000 google-cloud-ids-1.5.2/google_cloud_ids.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:53:34.000000 google-cloud-ids-1.5.2/google_cloud_ids.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:34.000000 google-cloud-ids-1.5.2/google_cloud_ids.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:53:34.000000 google-cloud-ids-1.5.2/google_cloud_ids.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:53:34.000000 google-cloud-ids-1.5.2/google_cloud_ids.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:53:34.185076 google-cloud-ids-1.5.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2914 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:34.185076 google-cloud-ids-1.5.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:34.185076 google-cloud-ids-1.5.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:34.185076 google-cloud-ids-1.5.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:34.185076 google-cloud-ids-1.5.2/tests/unit/gapic/ids_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/tests/unit/gapic/ids_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   135226 2023-07-05 15:46:59.000000 google-cloud-ids-1.5.2/tests/unit/gapic/ids_v1/test_ids.py
```

### Comparing `google-cloud-ids-1.5.1/LICENSE` & `google-cloud-ids-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/MANIFEST.in` & `google-cloud-ids-1.5.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/PKG-INFO` & `google-cloud-ids-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-ids
-Version: 1.5.1
+Version: 1.5.2
 Summary: Google Cloud Ids API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-ids-1.5.1/README.rst` & `google-cloud-ids-1.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/google/cloud/ids/__init__.py` & `google-cloud-ids-1.5.2/google/cloud/ids/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/google/cloud/ids/gapic_version.py` & `google-cloud-ids-1.5.2/google/cloud/ids/gapic_version.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.5.1"  # {x-release-please-version}
+__version__ = "1.5.2"  # {x-release-please-version}
```

### Comparing `google-cloud-ids-1.5.1/google/cloud/ids_v1/__init__.py` & `google-cloud-ids-1.5.2/google/cloud/ids_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/google/cloud/ids_v1/gapic_metadata.json` & `google-cloud-ids-1.5.2/google/cloud/ids_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/google/cloud/ids_v1/gapic_version.py` & `google-cloud-ids-1.5.2/google/cloud/ids_v1/gapic_version.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.5.1"  # {x-release-please-version}
+__version__ = "1.5.2"  # {x-release-please-version}
```

### Comparing `google-cloud-ids-1.5.1/google/cloud/ids_v1/services/__init__.py` & `google-cloud-ids-1.5.2/google/cloud/ids_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/__init__.py` & `google-cloud-ids-1.5.2/google/cloud/ids_v1/services/ids/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/async_client.py` & `google-cloud-ids-1.5.2/google/cloud/ids_v1/services/ids/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -703,15 +703,15 @@
             empty_pb2.Empty,
             metadata_type=ids.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "IDSAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/client.py` & `google-cloud-ids-1.5.2/google/cloud/ids_v1/services/ids/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/pagers.py` & `google-cloud-ids-1.5.2/google/cloud/ids_v1/services/ids/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/__init__.py` & `google-cloud-ids-1.5.2/google/cloud/ids_v1/services/ids/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/base.py` & `google-cloud-ids-1.5.2/google/cloud/ids_v1/services/ids/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/grpc.py` & `google-cloud-ids-1.5.2/google/cloud/ids_v1/services/ids/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/grpc_asyncio.py` & `google-cloud-ids-1.5.2/google/cloud/ids_v1/services/ids/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/rest.py` & `google-cloud-ids-1.5.2/google/cloud/ids_v1/services/ids/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/google/cloud/ids_v1/types/__init__.py` & `google-cloud-ids-1.5.2/google/cloud/ids_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/google/cloud/ids_v1/types/ids.py` & `google-cloud-ids-1.5.2/google/cloud/ids_v1/types/ids.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/google_cloud_ids.egg-info/PKG-INFO` & `google-cloud-ids-1.5.2/google_cloud_ids.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-ids
-Version: 1.5.1
+Version: 1.5.2
 Summary: Google Cloud Ids API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-ids-1.5.1/google_cloud_ids.egg-info/SOURCES.txt` & `google-cloud-ids-1.5.2/google_cloud_ids.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/setup.py` & `google-cloud-ids-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/tests/__init__.py` & `google-cloud-ids-1.5.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/tests/unit/__init__.py` & `google-cloud-ids-1.5.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/tests/unit/gapic/__init__.py` & `google-cloud-ids-1.5.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/tests/unit/gapic/ids_v1/__init__.py` & `google-cloud-ids-1.5.2/tests/unit/gapic/ids_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.1/tests/unit/gapic/ids_v1/test_ids.py` & `google-cloud-ids-1.5.2/tests/unit/gapic/ids_v1/test_ids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1063,17 +1063,19 @@
                     ids.Endpoint(),
                     ids.Endpoint(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_endpoints(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

