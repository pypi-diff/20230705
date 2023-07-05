# Comparing `tmp/google-cloud-vmwareengine-1.1.0.tar.gz` & `tmp/google-cloud-vmwareengine-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-vmwareengine-1.1.0.tar", last modified: Mon Jun 12 18:45:51 2023, max compression
+gzip compressed data, was "google-cloud-vmwareengine-1.1.1.tar", last modified: Wed Jul  5 15:56:32 2023, max compression
```

## Comparing `google-cloud-vmwareengine-1.1.0.tar` & `google-cloud-vmwareengine-1.1.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.330111 google-cloud-vmwareengine-1.1.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4615 2023-06-12 18:45:51.330111 google-cloud-vmwareengine-1.1.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3684 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.318116 google-cloud-vmwareengine-1.1.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.318116 google-cloud-vmwareengine-1.1.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.322115 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine/
--rw-rw-r--   0 root         (0)     1003     4873 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.322115 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/
--rw-rw-r--   0 root         (0)     1003     4691 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    16363 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.322115 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.322115 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/
--rw-rw-r--   0 root         (0)     1003      761 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/__init__.py
--rw-rw-r--   0 root         (0)     1003   254602 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/async_client.py
--rw-rw-r--   0 root         (0)     1003   268896 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/client.py
--rw-rw-r--   0 root         (0)     1003    47957 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.326113 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    33470 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/base.py
--rw-rw-r--   0 root         (0)     1003    71402 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    72836 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   249912 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.326113 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/types/
--rw-rw-r--   0 root         (0)     1003     4423 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    83908 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/types/vmwareengine.py
--rw-rw-r--   0 root         (0)     1003    48277 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/types/vmwareengine_resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.326113 google-cloud-vmwareengine-1.1.0/google_cloud_vmwareengine.egg-info/
--rw-r--r--   0 root         (0)     1003     4615 2023-06-12 18:45:51.000000 google-cloud-vmwareengine-1.1.0/google_cloud_vmwareengine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1681 2023-06-12 18:45:51.000000 google-cloud-vmwareengine-1.1.0/google_cloud_vmwareengine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-12 18:45:51.000000 google-cloud-vmwareengine-1.1.0/google_cloud_vmwareengine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-06-12 18:45:51.000000 google-cloud-vmwareengine-1.1.0/google_cloud_vmwareengine.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-12 18:45:51.000000 google-cloud-vmwareengine-1.1.0/google_cloud_vmwareengine.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-06-12 18:45:51.000000 google-cloud-vmwareengine-1.1.0/google_cloud_vmwareengine.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-12 18:45:51.000000 google-cloud-vmwareengine-1.1.0/google_cloud_vmwareengine.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-06-12 18:45:51.330111 google-cloud-vmwareengine-1.1.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2994 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.326113 google-cloud-vmwareengine-1.1.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.326113 google-cloud-vmwareengine-1.1.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.326113 google-cloud-vmwareengine-1.1.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.330111 google-cloud-vmwareengine-1.1.0/tests/unit/gapic/vmwareengine_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/tests/unit/gapic/vmwareengine_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   986497 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/tests/unit/gapic/vmwareengine_v1/test_vmware_engine.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:32.948356 google-cloud-vmwareengine-1.1.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4615 2023-07-05 15:56:32.948356 google-cloud-vmwareengine-1.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3684 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:32.940357 google-cloud-vmwareengine-1.1.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:32.940357 google-cloud-vmwareengine-1.1.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:32.940357 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine/
+-rw-rw-r--   0 root         (0)     1003     4873 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:32.944356 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/
+-rw-rw-r--   0 root         (0)     1003     4691 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16363 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:32.944356 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:32.944356 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/vmware_engine/
+-rw-rw-r--   0 root         (0)     1003      761 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/vmware_engine/__init__.py
+-rw-rw-r--   0 root         (0)     1003   254631 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/vmware_engine/async_client.py
+-rw-rw-r--   0 root         (0)     1003   268896 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/vmware_engine/client.py
+-rw-rw-r--   0 root         (0)     1003    47957 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/vmware_engine/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:32.944356 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    33470 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    71402 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    72836 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   249888 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:32.944356 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/types/
+-rw-rw-r--   0 root         (0)     1003     4423 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    83908 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/types/vmwareengine.py
+-rw-rw-r--   0 root         (0)     1003    48277 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/types/vmwareengine_resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:32.948356 google-cloud-vmwareengine-1.1.1/google_cloud_vmwareengine.egg-info/
+-rw-r--r--   0 root         (0)     1003     4615 2023-07-05 15:56:32.000000 google-cloud-vmwareengine-1.1.1/google_cloud_vmwareengine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1681 2023-07-05 15:56:32.000000 google-cloud-vmwareengine-1.1.1/google_cloud_vmwareengine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:56:32.000000 google-cloud-vmwareengine-1.1.1/google_cloud_vmwareengine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:56:32.000000 google-cloud-vmwareengine-1.1.1/google_cloud_vmwareengine.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:56:32.000000 google-cloud-vmwareengine-1.1.1/google_cloud_vmwareengine.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:56:32.000000 google-cloud-vmwareengine-1.1.1/google_cloud_vmwareengine.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:56:32.000000 google-cloud-vmwareengine-1.1.1/google_cloud_vmwareengine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:56:32.948356 google-cloud-vmwareengine-1.1.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2994 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:32.948356 google-cloud-vmwareengine-1.1.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:32.948356 google-cloud-vmwareengine-1.1.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:32.948356 google-cloud-vmwareengine-1.1.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:32.948356 google-cloud-vmwareengine-1.1.1/tests/unit/gapic/vmwareengine_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/tests/unit/gapic/vmwareengine_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   988288 2023-07-05 15:46:59.000000 google-cloud-vmwareengine-1.1.1/tests/unit/gapic/vmwareengine_v1/test_vmware_engine.py
```

### Comparing `google-cloud-vmwareengine-1.1.0/LICENSE` & `google-cloud-vmwareengine-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/MANIFEST.in` & `google-cloud-vmwareengine-1.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/PKG-INFO` & `google-cloud-vmwareengine-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-vmwareengine
-Version: 1.1.0
+Version: 1.1.1
 Summary: Google Cloud Vmwareengine API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-vmwareengine-1.1.0/README.rst` & `google-cloud-vmwareengine-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine/__init__.py` & `google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine/gapic_version.py` & `google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.1.0"  # {x-release-please-version}
+__version__ = "1.1.1"  # {x-release-please-version}
```

### Comparing `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/__init__.py` & `google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/gapic_metadata.json` & `google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/gapic_version.py` & `google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.1.0"  # {x-release-please-version}
+__version__ = "1.1.1"  # {x-release-please-version}
```

### Comparing `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/__init__.py` & `google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/__init__.py` & `google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/vmware_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/async_client.py` & `google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/vmware_engine/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -6027,15 +6027,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "VmwareEngineAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/client.py` & `google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/vmware_engine/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/pagers.py` & `google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/vmware_engine/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/__init__.py` & `google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/base.py` & `google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/grpc.py` & `google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/grpc_asyncio.py` & `google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/rest.py` & `google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -5930,15 +5930,15 @@
                 },
             ]
 
             request, metadata = self._interceptor.pre_set_iam_policy(request, metadata)
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
@@ -6012,15 +6012,15 @@
 
             request, metadata = self._interceptor.pre_test_iam_permissions(
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

### Comparing `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/types/__init__.py` & `google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/types/vmwareengine.py` & `google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/types/vmwareengine.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/types/vmwareengine_resources.py` & `google-cloud-vmwareengine-1.1.1/google/cloud/vmwareengine_v1/types/vmwareengine_resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/google_cloud_vmwareengine.egg-info/PKG-INFO` & `google-cloud-vmwareengine-1.1.1/google_cloud_vmwareengine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-vmwareengine
-Version: 1.1.0
+Version: 1.1.1
 Summary: Google Cloud Vmwareengine API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-vmwareengine-1.1.0/google_cloud_vmwareengine.egg-info/SOURCES.txt` & `google-cloud-vmwareengine-1.1.1/google_cloud_vmwareengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/setup.py` & `google-cloud-vmwareengine-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/tests/__init__.py` & `google-cloud-vmwareengine-1.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/tests/unit/__init__.py` & `google-cloud-vmwareengine-1.1.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/tests/unit/gapic/__init__.py` & `google-cloud-vmwareengine-1.1.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/tests/unit/gapic/vmwareengine_v1/__init__.py` & `google-cloud-vmwareengine-1.1.1/tests/unit/gapic/vmwareengine_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.1.0/tests/unit/gapic/vmwareengine_v1/test_vmware_engine.py` & `google-cloud-vmwareengine-1.1.1/tests/unit/gapic/vmwareengine_v1/test_vmware_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1142,17 +1142,19 @@
                     vmwareengine_resources.PrivateCloud(),
                     vmwareengine_resources.PrivateCloud(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_private_clouds(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2819,17 +2821,19 @@
                     vmwareengine_resources.Cluster(),
                     vmwareengine_resources.Cluster(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_clusters(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4195,17 +4199,19 @@
                     vmwareengine_resources.Subnet(),
                     vmwareengine_resources.Subnet(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_subnets(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5103,17 +5109,19 @@
                     vmwareengine_resources.NodeType(),
                     vmwareengine_resources.NodeType(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_node_types(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -7066,17 +7074,19 @@
                     vmwareengine_resources.HcxActivationKey(),
                     vmwareengine_resources.HcxActivationKey(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_hcx_activation_keys(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -8046,17 +8056,19 @@
                     vmwareengine_resources.NetworkPolicy(),
                     vmwareengine_resources.NetworkPolicy(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_network_policies(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -10286,17 +10298,19 @@
                     vmwareengine_resources.VmwareEngineNetwork(),
                     vmwareengine_resources.VmwareEngineNetwork(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_vmware_engine_networks(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -11317,17 +11331,19 @@
                     vmwareengine_resources.PrivateConnection(),
                     vmwareengine_resources.PrivateConnection(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_private_connections(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -12262,17 +12278,19 @@
                     vmwareengine_resources.PeeringRoute(),
                     vmwareengine_resources.PeeringRoute(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_private_connection_peering_routes(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

