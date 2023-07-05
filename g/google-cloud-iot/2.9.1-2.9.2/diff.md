# Comparing `tmp/google-cloud-iot-2.9.1.tar.gz` & `tmp/google-cloud-iot-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-iot-2.9.1.tar", last modified: Mon Mar 27 14:51:45 2023, max compression
+gzip compressed data, was "google-cloud-iot-2.9.2.tar", last modified: Wed Jul  5 15:45:28 2023, max compression
```

## Comparing `google-cloud-iot-2.9.1.tar` & `google-cloud-iot-2.9.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:51:45.810878 google-cloud-iot-2.9.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4951 2023-03-27 14:51:45.810878 google-cloud-iot-2.9.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4047 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:51:45.802880 google-cloud-iot-2.9.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:51:45.802880 google-cloud-iot-2.9.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:51:45.802880 google-cloud-iot-2.9.1/google/cloud/iot/
--rw-rw-r--   0 root         (0)     1003     3524 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/google/cloud/iot/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/google/cloud/iot/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/google/cloud/iot/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:51:45.802880 google-cloud-iot-2.9.1/google/cloud/iot_v1/
--rw-rw-r--   0 root         (0)     1003     3386 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/google/cloud/iot_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8102 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/google/cloud/iot_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/google/cloud/iot_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/google/cloud/iot_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:51:45.802880 google-cloud-iot-2.9.1/google/cloud/iot_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/google/cloud/iot_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:51:45.806879 google-cloud-iot-2.9.1/google/cloud/iot_v1/services/device_manager/
--rw-rw-r--   0 root         (0)     1003      765 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/google/cloud/iot_v1/services/device_manager/__init__.py
--rw-rw-r--   0 root         (0)     1003   107123 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/google/cloud/iot_v1/services/device_manager/async_client.py
--rw-rw-r--   0 root         (0)     1003   115726 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/google/cloud/iot_v1/services/device_manager/client.py
--rw-rw-r--   0 root         (0)     1003    10884 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/google/cloud/iot_v1/services/device_manager/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:51:45.806879 google-cloud-iot-2.9.1/google/cloud/iot_v1/services/device_manager/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/google/cloud/iot_v1/services/device_manager/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    18984 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/google/cloud/iot_v1/services/device_manager/transports/base.py
--rw-rw-r--   0 root         (0)     1003    34477 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/google/cloud/iot_v1/services/device_manager/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    35141 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/google/cloud/iot_v1/services/device_manager/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   114380 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/google/cloud/iot_v1/services/device_manager/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:51:45.806879 google-cloud-iot-2.9.1/google/cloud/iot_v1/types/
--rw-rw-r--   0 root         (0)     1003     3122 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/google/cloud/iot_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    22525 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/google/cloud/iot_v1/types/device_manager.py
--rw-rw-r--   0 root         (0)     1003    30618 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/google/cloud/iot_v1/types/resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:51:45.806879 google-cloud-iot-2.9.1/google_cloud_iot.egg-info/
--rw-r--r--   0 root         (0)     1003     4951 2023-03-27 14:51:45.000000 google-cloud-iot-2.9.1/google_cloud_iot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1484 2023-03-27 14:51:45.000000 google-cloud-iot-2.9.1/google_cloud_iot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:51:45.000000 google-cloud-iot-2.9.1/google_cloud_iot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:51:45.000000 google-cloud-iot-2.9.1/google_cloud_iot.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:51:45.000000 google-cloud-iot-2.9.1/google_cloud_iot.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 14:51:45.000000 google-cloud-iot-2.9.1/google_cloud_iot.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:51:45.000000 google-cloud-iot-2.9.1/google_cloud_iot.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 14:51:45.810878 google-cloud-iot-2.9.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2952 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:51:45.806879 google-cloud-iot-2.9.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:51:45.802880 google-cloud-iot-2.9.1/tests/system/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:51:45.802880 google-cloud-iot-2.9.1/tests/system/gapic/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:51:45.806879 google-cloud-iot-2.9.1/tests/system/gapic/v1/
--rw-rw-r--   0 root         (0)     1003      975 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/tests/system/gapic/v1/test_system_device_manager_v1.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:51:45.810878 google-cloud-iot-2.9.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:51:45.810878 google-cloud-iot-2.9.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:51:45.810878 google-cloud-iot-2.9.1/tests/unit/gapic/iot_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/tests/unit/gapic/iot_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   445486 2023-03-27 14:49:13.000000 google-cloud-iot-2.9.1/tests/unit/gapic/iot_v1/test_device_manager.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:28.168684 google-cloud-iot-2.9.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4951 2023-07-05 15:45:28.168684 google-cloud-iot-2.9.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4047 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:28.156683 google-cloud-iot-2.9.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:28.156683 google-cloud-iot-2.9.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:28.160683 google-cloud-iot-2.9.2/google/cloud/iot/
+-rw-rw-r--   0 root         (0)     1003     3524 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/google/cloud/iot/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/google/cloud/iot/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/google/cloud/iot/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:28.160683 google-cloud-iot-2.9.2/google/cloud/iot_v1/
+-rw-rw-r--   0 root         (0)     1003     3386 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/google/cloud/iot_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8102 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/google/cloud/iot_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/google/cloud/iot_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/google/cloud/iot_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:28.160683 google-cloud-iot-2.9.2/google/cloud/iot_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/google/cloud/iot_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:28.160683 google-cloud-iot-2.9.2/google/cloud/iot_v1/services/device_manager/
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/google/cloud/iot_v1/services/device_manager/__init__.py
+-rw-rw-r--   0 root         (0)     1003   107153 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/google/cloud/iot_v1/services/device_manager/async_client.py
+-rw-rw-r--   0 root         (0)     1003   115726 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/google/cloud/iot_v1/services/device_manager/client.py
+-rw-rw-r--   0 root         (0)     1003    10884 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/google/cloud/iot_v1/services/device_manager/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:28.160683 google-cloud-iot-2.9.2/google/cloud/iot_v1/services/device_manager/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/google/cloud/iot_v1/services/device_manager/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18984 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/google/cloud/iot_v1/services/device_manager/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    34477 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/google/cloud/iot_v1/services/device_manager/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    35141 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/google/cloud/iot_v1/services/device_manager/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   114380 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/google/cloud/iot_v1/services/device_manager/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:28.164683 google-cloud-iot-2.9.2/google/cloud/iot_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3122 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/google/cloud/iot_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22525 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/google/cloud/iot_v1/types/device_manager.py
+-rw-rw-r--   0 root         (0)     1003    30618 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/google/cloud/iot_v1/types/resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:28.164683 google-cloud-iot-2.9.2/google_cloud_iot.egg-info/
+-rw-r--r--   0 root         (0)     1003     4951 2023-07-05 15:45:28.000000 google-cloud-iot-2.9.2/google_cloud_iot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1484 2023-07-05 15:45:28.000000 google-cloud-iot-2.9.2/google_cloud_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:45:28.000000 google-cloud-iot-2.9.2/google_cloud_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:45:28.000000 google-cloud-iot-2.9.2/google_cloud_iot.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:45:28.000000 google-cloud-iot-2.9.2/google_cloud_iot.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:45:28.000000 google-cloud-iot-2.9.2/google_cloud_iot.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:45:28.000000 google-cloud-iot-2.9.2/google_cloud_iot.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:45:28.168684 google-cloud-iot-2.9.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2952 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:28.164683 google-cloud-iot-2.9.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:28.156683 google-cloud-iot-2.9.2/tests/system/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:28.156683 google-cloud-iot-2.9.2/tests/system/gapic/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:28.164683 google-cloud-iot-2.9.2/tests/system/gapic/v1/
+-rw-rw-r--   0 root         (0)     1003      975 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/tests/system/gapic/v1/test_system_device_manager_v1.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:28.164683 google-cloud-iot-2.9.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:28.164683 google-cloud-iot-2.9.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:28.164683 google-cloud-iot-2.9.2/tests/unit/gapic/iot_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/tests/unit/gapic/iot_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   445884 2023-07-05 15:42:31.000000 google-cloud-iot-2.9.2/tests/unit/gapic/iot_v1/test_device_manager.py
```

### Comparing `google-cloud-iot-2.9.1/LICENSE` & `google-cloud-iot-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/MANIFEST.in` & `google-cloud-iot-2.9.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/PKG-INFO` & `google-cloud-iot-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-iot
-Version: 2.9.1
+Version: 2.9.2
 Summary: Google Cloud Iot API client library
 Home-page: https://github.com/googleapis/python-iot
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-iot-2.9.1/README.rst` & `google-cloud-iot-2.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/google/cloud/iot/__init__.py` & `google-cloud-iot-2.9.2/google/cloud/iot/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/google/cloud/iot/gapic_version.py` & `google-cloud-iot-2.9.2/google/cloud/iot/gapic_version.py`

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
-__version__ = "2.9.1"  # {x-release-please-version}
+__version__ = "2.9.2"  # {x-release-please-version}
```

### Comparing `google-cloud-iot-2.9.1/google/cloud/iot_v1/__init__.py` & `google-cloud-iot-2.9.2/google/cloud/iot_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/google/cloud/iot_v1/gapic_metadata.json` & `google-cloud-iot-2.9.2/google/cloud/iot_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/google/cloud/iot_v1/gapic_version.py` & `google-cloud-iot-2.9.2/google/cloud/iot_v1/gapic_version.py`

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
-__version__ = "2.9.1"  # {x-release-please-version}
+__version__ = "2.9.2"  # {x-release-please-version}
```

### Comparing `google-cloud-iot-2.9.1/google/cloud/iot_v1/services/__init__.py` & `google-cloud-iot-2.9.2/google/cloud/iot_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/google/cloud/iot_v1/services/device_manager/__init__.py` & `google-cloud-iot-2.9.2/google/cloud/iot_v1/services/device_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/google/cloud/iot_v1/services/device_manager/async_client.py` & `google-cloud-iot-2.9.2/google/cloud/iot_v1/services/device_manager/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2567,15 +2567,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "DeviceManagerAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-iot-2.9.1/google/cloud/iot_v1/services/device_manager/client.py` & `google-cloud-iot-2.9.2/google/cloud/iot_v1/services/device_manager/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/google/cloud/iot_v1/services/device_manager/pagers.py` & `google-cloud-iot-2.9.2/google/cloud/iot_v1/services/device_manager/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/google/cloud/iot_v1/services/device_manager/transports/__init__.py` & `google-cloud-iot-2.9.2/google/cloud/iot_v1/services/device_manager/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/google/cloud/iot_v1/services/device_manager/transports/base.py` & `google-cloud-iot-2.9.2/google/cloud/iot_v1/services/device_manager/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/google/cloud/iot_v1/services/device_manager/transports/grpc.py` & `google-cloud-iot-2.9.2/google/cloud/iot_v1/services/device_manager/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/google/cloud/iot_v1/services/device_manager/transports/grpc_asyncio.py` & `google-cloud-iot-2.9.2/google/cloud/iot_v1/services/device_manager/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/google/cloud/iot_v1/services/device_manager/transports/rest.py` & `google-cloud-iot-2.9.2/google/cloud/iot_v1/services/device_manager/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/google/cloud/iot_v1/types/__init__.py` & `google-cloud-iot-2.9.2/google/cloud/iot_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/google/cloud/iot_v1/types/device_manager.py` & `google-cloud-iot-2.9.2/google/cloud/iot_v1/types/device_manager.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/google/cloud/iot_v1/types/resources.py` & `google-cloud-iot-2.9.2/google/cloud/iot_v1/types/resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/google_cloud_iot.egg-info/PKG-INFO` & `google-cloud-iot-2.9.2/google_cloud_iot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-iot
-Version: 2.9.1
+Version: 2.9.2
 Summary: Google Cloud Iot API client library
 Home-page: https://github.com/googleapis/python-iot
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-iot-2.9.1/google_cloud_iot.egg-info/SOURCES.txt` & `google-cloud-iot-2.9.2/google_cloud_iot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/setup.py` & `google-cloud-iot-2.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/tests/__init__.py` & `google-cloud-iot-2.9.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/tests/system/gapic/v1/test_system_device_manager_v1.py` & `google-cloud-iot-2.9.2/tests/system/gapic/v1/test_system_device_manager_v1.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/tests/unit/__init__.py` & `google-cloud-iot-2.9.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/tests/unit/gapic/__init__.py` & `google-cloud-iot-2.9.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/tests/unit/gapic/iot_v1/__init__.py` & `google-cloud-iot-2.9.2/tests/unit/gapic/iot_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iot-2.9.1/tests/unit/gapic/iot_v1/test_device_manager.py` & `google-cloud-iot-2.9.2/tests/unit/gapic/iot_v1/test_device_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -2164,17 +2164,19 @@
                     resources.DeviceRegistry(),
                     resources.DeviceRegistry(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_device_registries(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3556,17 +3558,19 @@
                     resources.Device(),
                     resources.Device(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_devices(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

