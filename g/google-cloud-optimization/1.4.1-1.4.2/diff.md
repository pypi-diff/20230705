# Comparing `tmp/google-cloud-optimization-1.4.1.tar.gz` & `tmp/google-cloud-optimization-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-optimization-1.4.1.tar", last modified: Mon Mar 27 15:49:20 2023, max compression
+gzip compressed data, was "google-cloud-optimization-1.4.2.tar", last modified: Wed Jul  5 15:23:11 2023, max compression
```

## Comparing `google-cloud-optimization-1.4.1.tar` & `google-cloud-optimization-1.4.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:20.441312 google-cloud-optimization-1.4.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4761 2023-03-27 15:49:20.441312 google-cloud-optimization-1.4.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3830 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:20.433313 google-cloud-optimization-1.4.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:20.433313 google-cloud-optimization-1.4.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:20.433313 google-cloud-optimization-1.4.1/google/cloud/optimization/
--rw-rw-r--   0 root         (0)     1003     3857 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/google/cloud/optimization/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/google/cloud/optimization/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/google/cloud/optimization/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:20.433313 google-cloud-optimization-1.4.1/google/cloud/optimization_v1/
--rw-rw-r--   0 root         (0)     1003     2973 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/google/cloud/optimization_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1423 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/google/cloud/optimization_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/google/cloud/optimization_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/google/cloud/optimization_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:20.433313 google-cloud-optimization-1.4.1/google/cloud/optimization_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/google/cloud/optimization_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:20.437312 google-cloud-optimization-1.4.1/google/cloud/optimization_v1/services/fleet_routing/
--rw-rw-r--   0 root         (0)     1003      761 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/google/cloud/optimization_v1/services/fleet_routing/__init__.py
--rw-rw-r--   0 root         (0)     1003    21896 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/google/cloud/optimization_v1/services/fleet_routing/async_client.py
--rw-rw-r--   0 root         (0)     1003    30019 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/google/cloud/optimization_v1/services/fleet_routing/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:20.437312 google-cloud-optimization-1.4.1/google/cloud/optimization_v1/services/fleet_routing/transports/
--rw-rw-r--   0 root         (0)     1003     1390 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/google/cloud/optimization_v1/services/fleet_routing/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7770 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/google/cloud/optimization_v1/services/fleet_routing/transports/base.py
--rw-rw-r--   0 root         (0)     1003    16741 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/google/cloud/optimization_v1/services/fleet_routing/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17034 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/google/cloud/optimization_v1/services/fleet_routing/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    24773 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/google/cloud/optimization_v1/services/fleet_routing/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:20.437312 google-cloud-optimization-1.4.1/google/cloud/optimization_v1/types/
--rw-rw-r--   0 root         (0)     1003     1969 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/google/cloud/optimization_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     5614 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/google/cloud/optimization_v1/types/async_model.py
--rw-rw-r--   0 root         (0)     1003   189252 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/google/cloud/optimization_v1/types/fleet_routing.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:20.437312 google-cloud-optimization-1.4.1/google_cloud_optimization.egg-info/
--rw-r--r--   0 root         (0)     1003     4761 2023-03-27 15:49:20.000000 google-cloud-optimization-1.4.1/google_cloud_optimization.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1619 2023-03-27 15:49:20.000000 google-cloud-optimization-1.4.1/google_cloud_optimization.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:49:20.000000 google-cloud-optimization-1.4.1/google_cloud_optimization.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:49:20.000000 google-cloud-optimization-1.4.1/google_cloud_optimization.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:49:20.000000 google-cloud-optimization-1.4.1/google_cloud_optimization.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 15:49:20.000000 google-cloud-optimization-1.4.1/google_cloud_optimization.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:49:20.000000 google-cloud-optimization-1.4.1/google_cloud_optimization.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:49:20.441312 google-cloud-optimization-1.4.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2947 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:20.437312 google-cloud-optimization-1.4.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:20.437312 google-cloud-optimization-1.4.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:20.441312 google-cloud-optimization-1.4.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:49:20.441312 google-cloud-optimization-1.4.1/tests/unit/gapic/optimization_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/tests/unit/gapic/optimization_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    88610 2023-03-27 15:47:23.000000 google-cloud-optimization-1.4.1/tests/unit/gapic/optimization_v1/test_fleet_routing.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:11.459028 google-cloud-optimization-1.4.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4761 2023-07-05 15:23:11.459028 google-cloud-optimization-1.4.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3830 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:11.447019 google-cloud-optimization-1.4.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:11.447019 google-cloud-optimization-1.4.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:11.451022 google-cloud-optimization-1.4.2/google/cloud/optimization/
+-rw-rw-r--   0 root         (0)     1003     3857 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/google/cloud/optimization/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/google/cloud/optimization/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/google/cloud/optimization/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:11.451022 google-cloud-optimization-1.4.2/google/cloud/optimization_v1/
+-rw-rw-r--   0 root         (0)     1003     2973 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/google/cloud/optimization_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1423 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/google/cloud/optimization_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/google/cloud/optimization_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/google/cloud/optimization_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:11.451022 google-cloud-optimization-1.4.2/google/cloud/optimization_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/google/cloud/optimization_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:11.451022 google-cloud-optimization-1.4.2/google/cloud/optimization_v1/services/fleet_routing/
+-rw-rw-r--   0 root         (0)     1003      761 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/google/cloud/optimization_v1/services/fleet_routing/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21925 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/google/cloud/optimization_v1/services/fleet_routing/async_client.py
+-rw-rw-r--   0 root         (0)     1003    30019 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/google/cloud/optimization_v1/services/fleet_routing/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:11.455025 google-cloud-optimization-1.4.2/google/cloud/optimization_v1/services/fleet_routing/transports/
+-rw-rw-r--   0 root         (0)     1003     1390 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/google/cloud/optimization_v1/services/fleet_routing/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7770 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/google/cloud/optimization_v1/services/fleet_routing/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    16741 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/google/cloud/optimization_v1/services/fleet_routing/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17034 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/google/cloud/optimization_v1/services/fleet_routing/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    24773 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/google/cloud/optimization_v1/services/fleet_routing/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:11.455025 google-cloud-optimization-1.4.2/google/cloud/optimization_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1969 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/google/cloud/optimization_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5614 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/google/cloud/optimization_v1/types/async_model.py
+-rw-rw-r--   0 root         (0)     1003   189252 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/google/cloud/optimization_v1/types/fleet_routing.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:11.455025 google-cloud-optimization-1.4.2/google_cloud_optimization.egg-info/
+-rw-r--r--   0 root         (0)     1003     4761 2023-07-05 15:23:11.000000 google-cloud-optimization-1.4.2/google_cloud_optimization.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1619 2023-07-05 15:23:11.000000 google-cloud-optimization-1.4.2/google_cloud_optimization.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:23:11.000000 google-cloud-optimization-1.4.2/google_cloud_optimization.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:23:11.000000 google-cloud-optimization-1.4.2/google_cloud_optimization.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:23:11.000000 google-cloud-optimization-1.4.2/google_cloud_optimization.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:23:11.000000 google-cloud-optimization-1.4.2/google_cloud_optimization.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:23:11.000000 google-cloud-optimization-1.4.2/google_cloud_optimization.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:23:11.459028 google-cloud-optimization-1.4.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2947 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:11.455025 google-cloud-optimization-1.4.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:11.455025 google-cloud-optimization-1.4.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:11.455025 google-cloud-optimization-1.4.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:23:11.455025 google-cloud-optimization-1.4.2/tests/unit/gapic/optimization_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/tests/unit/gapic/optimization_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    88610 2023-07-05 15:21:18.000000 google-cloud-optimization-1.4.2/tests/unit/gapic/optimization_v1/test_fleet_routing.py
```

### Comparing `google-cloud-optimization-1.4.1/LICENSE` & `google-cloud-optimization-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-optimization-1.4.1/MANIFEST.in` & `google-cloud-optimization-1.4.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-optimization-1.4.1/PKG-INFO` & `google-cloud-optimization-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-optimization
-Version: 1.4.1
+Version: 1.4.2
 Summary: Google Cloud Optimization API client library
 Home-page: https://github.com/googleapis/python-optimization
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-optimization-1.4.1/README.rst` & `google-cloud-optimization-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-optimization-1.4.1/google/cloud/optimization/__init__.py` & `google-cloud-optimization-1.4.2/google/cloud/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-optimization-1.4.1/google/cloud/optimization/gapic_version.py` & `google-cloud-optimization-1.4.2/google/cloud/optimization_v1/services/__init__.py`

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

### Comparing `google-cloud-optimization-1.4.1/google/cloud/optimization_v1/__init__.py` & `google-cloud-optimization-1.4.2/google/cloud/optimization_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-optimization-1.4.1/google/cloud/optimization_v1/gapic_metadata.json` & `google-cloud-optimization-1.4.2/google/cloud/optimization_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-optimization-1.4.1/google/cloud/optimization_v1/gapic_version.py` & `google-cloud-optimization-1.4.2/tests/__init__.py`

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

### Comparing `google-cloud-optimization-1.4.1/google/cloud/optimization_v1/services/__init__.py` & `google-cloud-optimization-1.4.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-optimization-1.4.1/google/cloud/optimization_v1/services/fleet_routing/__init__.py` & `google-cloud-optimization-1.4.2/google/cloud/optimization_v1/services/fleet_routing/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-optimization-1.4.1/google/cloud/optimization_v1/services/fleet_routing/async_client.py` & `google-cloud-optimization-1.4.2/google/cloud/optimization_v1/services/fleet_routing/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -515,15 +515,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "FleetRoutingAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-optimization-1.4.1/google/cloud/optimization_v1/services/fleet_routing/client.py` & `google-cloud-optimization-1.4.2/google/cloud/optimization_v1/services/fleet_routing/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-optimization-1.4.1/google/cloud/optimization_v1/services/fleet_routing/transports/__init__.py` & `google-cloud-optimization-1.4.2/google/cloud/optimization_v1/services/fleet_routing/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-optimization-1.4.1/google/cloud/optimization_v1/services/fleet_routing/transports/base.py` & `google-cloud-optimization-1.4.2/google/cloud/optimization_v1/services/fleet_routing/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-optimization-1.4.1/google/cloud/optimization_v1/services/fleet_routing/transports/grpc.py` & `google-cloud-optimization-1.4.2/google/cloud/optimization_v1/services/fleet_routing/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-optimization-1.4.1/google/cloud/optimization_v1/services/fleet_routing/transports/grpc_asyncio.py` & `google-cloud-optimization-1.4.2/google/cloud/optimization_v1/services/fleet_routing/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-optimization-1.4.1/google/cloud/optimization_v1/services/fleet_routing/transports/rest.py` & `google-cloud-optimization-1.4.2/google/cloud/optimization_v1/services/fleet_routing/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-optimization-1.4.1/google/cloud/optimization_v1/types/__init__.py` & `google-cloud-optimization-1.4.2/google/cloud/optimization_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-optimization-1.4.1/google/cloud/optimization_v1/types/async_model.py` & `google-cloud-optimization-1.4.2/google/cloud/optimization_v1/types/async_model.py`

 * *Files identical despite different names*

### Comparing `google-cloud-optimization-1.4.1/google/cloud/optimization_v1/types/fleet_routing.py` & `google-cloud-optimization-1.4.2/google/cloud/optimization_v1/types/fleet_routing.py`

 * *Files identical despite different names*

### Comparing `google-cloud-optimization-1.4.1/google_cloud_optimization.egg-info/PKG-INFO` & `google-cloud-optimization-1.4.2/google_cloud_optimization.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-optimization
-Version: 1.4.1
+Version: 1.4.2
 Summary: Google Cloud Optimization API client library
 Home-page: https://github.com/googleapis/python-optimization
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-optimization-1.4.1/google_cloud_optimization.egg-info/SOURCES.txt` & `google-cloud-optimization-1.4.2/google_cloud_optimization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-optimization-1.4.1/setup.py` & `google-cloud-optimization-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-optimization-1.4.1/tests/__init__.py` & `google-cloud-optimization-1.4.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-optimization-1.4.1/tests/unit/__init__.py` & `google-cloud-optimization-1.4.2/tests/unit/gapic/optimization_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-optimization-1.4.1/tests/unit/gapic/optimization_v1/test_fleet_routing.py` & `google-cloud-optimization-1.4.2/tests/unit/gapic/optimization_v1/test_fleet_routing.py`

 * *Files identical despite different names*

