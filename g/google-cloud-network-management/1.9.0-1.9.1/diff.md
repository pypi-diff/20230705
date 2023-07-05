# Comparing `tmp/google-cloud-network-management-1.9.0.tar.gz` & `tmp/google-cloud-network-management-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-network-management-1.9.0.tar", last modified: Thu Jun 29 16:29:49 2023, max compression
+gzip compressed data, was "google-cloud-network-management-1.9.1.tar", last modified: Wed Jul  5 15:54:13 2023, max compression
```

## Comparing `google-cloud-network-management-1.9.0.tar` & `google-cloud-network-management-1.9.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.819268 google-cloud-network-management-1.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4691 2023-06-29 16:29:49.819268 google-cloud-network-management-1.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3748 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.811269 google-cloud-network-management-1.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.811269 google-cloud-network-management-1.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.815269 google-cloud-network-management-1.9.0/google/cloud/network_management/
--rw-rw-r--   0 root         (0)     1003     2621 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       92 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.815269 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/
--rw-rw-r--   0 root         (0)     1003     2370 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3205 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       92 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.815269 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.815269 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    41915 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    51661 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/client.py
--rw-rw-r--   0 root         (0)     1003     6105 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.819268 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/
--rw-rw-r--   0 root         (0)     1003     1478 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8803 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    21371 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    21772 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    42143 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.819268 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/types/
--rw-rw-r--   0 root         (0)     1003     2042 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    13540 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/types/connectivity_test.py
--rw-rw-r--   0 root         (0)     1003     8907 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/types/reachability.py
--rw-rw-r--   0 root         (0)     1003    51873 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/types/trace.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.819268 google-cloud-network-management-1.9.0/google_cloud_network_management.egg-info/
--rw-r--r--   0 root         (0)     1003     4691 2023-06-29 16:29:49.000000 google-cloud-network-management-1.9.0/google_cloud_network_management.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1980 2023-06-29 16:29:49.000000 google-cloud-network-management-1.9.0/google_cloud_network_management.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-29 16:29:49.000000 google-cloud-network-management-1.9.0/google_cloud_network_management.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-06-29 16:29:49.000000 google-cloud-network-management-1.9.0/google_cloud_network_management.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-29 16:29:49.000000 google-cloud-network-management-1.9.0/google_cloud_network_management.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-06-29 16:29:49.000000 google-cloud-network-management-1.9.0/google_cloud_network_management.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-29 16:29:49.000000 google-cloud-network-management-1.9.0/google_cloud_network_management.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-06-29 16:29:49.823268 google-cloud-network-management-1.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2965 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.819268 google-cloud-network-management-1.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.819268 google-cloud-network-management-1.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.819268 google-cloud-network-management-1.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.819268 google-cloud-network-management-1.9.0/tests/unit/gapic/network_management_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/tests/unit/gapic/network_management_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   217053 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/tests/unit/gapic/network_management_v1/test_reachability_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:13.796407 google-cloud-network-management-1.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4691 2023-07-05 15:54:13.796407 google-cloud-network-management-1.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3748 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:13.788407 google-cloud-network-management-1.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:13.788407 google-cloud-network-management-1.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:13.788407 google-cloud-network-management-1.9.1/google/cloud/network_management/
+-rw-rw-r--   0 root         (0)     1003     2621 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/google/cloud/network_management/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/google/cloud/network_management/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       92 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/google/cloud/network_management/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:13.788407 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/
+-rw-rw-r--   0 root         (0)     1003     2370 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3205 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       92 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:13.788407 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:13.792407 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/reachability_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/reachability_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    41951 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/reachability_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    51661 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/reachability_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6105 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/reachability_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:13.792407 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/reachability_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1478 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/reachability_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8803 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/reachability_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    21371 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/reachability_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    21772 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/reachability_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    42143 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/reachability_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:13.792407 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2042 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13540 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/types/connectivity_test.py
+-rw-rw-r--   0 root         (0)     1003     8907 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/types/reachability.py
+-rw-rw-r--   0 root         (0)     1003    51873 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/google/cloud/network_management_v1/types/trace.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:13.792407 google-cloud-network-management-1.9.1/google_cloud_network_management.egg-info/
+-rw-r--r--   0 root         (0)     1003     4691 2023-07-05 15:54:13.000000 google-cloud-network-management-1.9.1/google_cloud_network_management.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1980 2023-07-05 15:54:13.000000 google-cloud-network-management-1.9.1/google_cloud_network_management.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:13.000000 google-cloud-network-management-1.9.1/google_cloud_network_management.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:54:13.000000 google-cloud-network-management-1.9.1/google_cloud_network_management.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:13.000000 google-cloud-network-management-1.9.1/google_cloud_network_management.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:54:13.000000 google-cloud-network-management-1.9.1/google_cloud_network_management.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:54:13.000000 google-cloud-network-management-1.9.1/google_cloud_network_management.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:54:13.796407 google-cloud-network-management-1.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2965 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:13.792407 google-cloud-network-management-1.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:13.792407 google-cloud-network-management-1.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:13.792407 google-cloud-network-management-1.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:13.792407 google-cloud-network-management-1.9.1/tests/unit/gapic/network_management_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/tests/unit/gapic/network_management_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   217252 2023-07-05 15:46:59.000000 google-cloud-network-management-1.9.1/tests/unit/gapic/network_management_v1/test_reachability_service.py
```

### Comparing `google-cloud-network-management-1.9.0/LICENSE` & `google-cloud-network-management-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/MANIFEST.in` & `google-cloud-network-management-1.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/PKG-INFO` & `google-cloud-network-management-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-network-management
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Network Management API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-network-management-1.9.0/README.rst` & `google-cloud-network-management-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/google/cloud/network_management/__init__.py` & `google-cloud-network-management-1.9.1/google/cloud/network_management/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/google/cloud/network_management/gapic_version.py` & `google-cloud-network-management-1.9.1/google/cloud/network_management/gapic_version.py`

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

### Comparing `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/__init__.py` & `google-cloud-network-management-1.9.1/google/cloud/network_management_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/gapic_metadata.json` & `google-cloud-network-management-1.9.1/google/cloud/network_management_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/gapic_version.py` & `google-cloud-network-management-1.9.1/google/cloud/network_management_v1/gapic_version.py`

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

### Comparing `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/__init__.py` & `google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/__init__.py` & `google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/reachability_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/async_client.py` & `google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/reachability_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -993,15 +993,15 @@
             empty_pb2.Empty,
             metadata_type=reachability.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ReachabilityServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/client.py` & `google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/reachability_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/pagers.py` & `google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/reachability_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/__init__.py` & `google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/reachability_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/base.py` & `google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/reachability_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/grpc.py` & `google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/reachability_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/grpc_asyncio.py` & `google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/reachability_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/rest.py` & `google-cloud-network-management-1.9.1/google/cloud/network_management_v1/services/reachability_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/types/__init__.py` & `google-cloud-network-management-1.9.1/google/cloud/network_management_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/types/connectivity_test.py` & `google-cloud-network-management-1.9.1/google/cloud/network_management_v1/types/connectivity_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/types/reachability.py` & `google-cloud-network-management-1.9.1/google/cloud/network_management_v1/types/reachability.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/types/trace.py` & `google-cloud-network-management-1.9.1/google/cloud/network_management_v1/types/trace.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/google_cloud_network_management.egg-info/PKG-INFO` & `google-cloud-network-management-1.9.1/google_cloud_network_management.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-network-management
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Network Management API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-network-management-1.9.0/google_cloud_network_management.egg-info/SOURCES.txt` & `google-cloud-network-management-1.9.1/google_cloud_network_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/setup.py` & `google-cloud-network-management-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/tests/__init__.py` & `google-cloud-network-management-1.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/tests/unit/__init__.py` & `google-cloud-network-management-1.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/tests/unit/gapic/__init__.py` & `google-cloud-network-management-1.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/tests/unit/gapic/network_management_v1/__init__.py` & `google-cloud-network-management-1.9.1/tests/unit/gapic/network_management_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.9.0/tests/unit/gapic/network_management_v1/test_reachability_service.py` & `google-cloud-network-management-1.9.1/tests/unit/gapic/network_management_v1/test_reachability_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1202,17 +1202,19 @@
                     connectivity_test.ConnectivityTest(),
                     connectivity_test.ConnectivityTest(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_connectivity_tests(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

