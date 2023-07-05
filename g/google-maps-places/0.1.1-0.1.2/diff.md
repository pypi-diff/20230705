# Comparing `tmp/google-maps-places-0.1.1.tar.gz` & `tmp/google-maps-places-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-maps-places-0.1.1.tar", last modified: Mon Jun  5 14:00:18 2023, max compression
+gzip compressed data, was "google-maps-places-0.1.2.tar", last modified: Wed Jul  5 15:57:13 2023, max compression
```

## Comparing `google-maps-places-0.1.1.tar` & `google-maps-places-0.1.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:18.048024 google-maps-places-0.1.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4594 2023-06-05 14:00:18.048024 google-maps-places-0.1.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3690 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:18.040023 google-maps-places-0.1.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:18.040023 google-maps-places-0.1.1/google/maps/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:18.044023 google-maps-places-0.1.1/google/maps/places/
--rw-rw-r--   0 root         (0)     1003     1276 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/google/maps/places/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/google/maps/places/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       79 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/google/maps/places/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:18.044023 google-maps-places-0.1.1/google/maps/places_v1/
--rw-rw-r--   0 root         (0)     1003     1109 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/google/maps/places_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      968 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/google/maps/places_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/google/maps/places_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       79 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/google/maps/places_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:18.044023 google-maps-places-0.1.1/google/maps/places_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/google/maps/places_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:18.044023 google-maps-places-0.1.1/google/maps/places_v1/services/places/
--rw-rw-r--   0 root         (0)     1003      737 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/google/maps/places_v1/services/places/__init__.py
--rw-rw-r--   0 root         (0)     1003    11592 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/google/maps/places_v1/services/places/async_client.py
--rw-rw-r--   0 root         (0)     1003    20296 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/google/maps/places_v1/services/places/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:18.044023 google-maps-places-0.1.1/google/maps/places_v1/services/places/transports/
--rw-rw-r--   0 root         (0)     1003     1288 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/google/maps/places_v1/services/places/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     5971 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/google/maps/places_v1/services/places/transports/base.py
--rw-rw-r--   0 root         (0)     1003    11651 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/google/maps/places_v1/services/places/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    11848 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/google/maps/places_v1/services/places/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12045 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/google/maps/places_v1/services/places/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:18.044023 google-maps-places-0.1.1/google/maps/places_v1/types/
--rw-rw-r--   0 root         (0)     1003      873 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/google/maps/places_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     1616 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/google/maps/places_v1/types/geometry.py
--rw-rw-r--   0 root         (0)     1003    29965 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/google/maps/places_v1/types/place.py
--rw-rw-r--   0 root         (0)     1003    11880 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/google/maps/places_v1/types/places_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:18.048024 google-maps-places-0.1.1/google_maps_places.egg-info/
--rw-r--r--   0 root         (0)     1003     4594 2023-06-05 14:00:17.000000 google-maps-places-0.1.1/google_maps_places.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1387 2023-06-05 14:00:18.000000 google-maps-places-0.1.1/google_maps_places.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-05 14:00:17.000000 google-maps-places-0.1.1/google_maps_places.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       19 2023-06-05 14:00:17.000000 google-maps-places-0.1.1/google_maps_places.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-05 14:00:17.000000 google-maps-places-0.1.1/google_maps_places.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      348 2023-06-05 14:00:17.000000 google-maps-places-0.1.1/google_maps_places.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-05 14:00:17.000000 google-maps-places-0.1.1/google_maps_places.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-06-05 14:00:18.048024 google-maps-places-0.1.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2962 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:18.048024 google-maps-places-0.1.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:18.048024 google-maps-places-0.1.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:18.048024 google-maps-places-0.1.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:18.048024 google-maps-places-0.1.1/tests/unit/gapic/places_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/tests/unit/gapic/places_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    60694 2023-06-05 13:56:51.000000 google-maps-places-0.1.1/tests/unit/gapic/places_v1/test_places.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:13.754322 google-maps-places-0.1.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4594 2023-07-05 15:57:13.750320 google-maps-places-0.1.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3690 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:13.746318 google-maps-places-0.1.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:13.746318 google-maps-places-0.1.2/google/maps/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:13.746318 google-maps-places-0.1.2/google/maps/places/
+-rw-rw-r--   0 root         (0)     1003     1276 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/google/maps/places/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/google/maps/places/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       79 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/google/maps/places/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:13.746318 google-maps-places-0.1.2/google/maps/places_v1/
+-rw-rw-r--   0 root         (0)     1003     1109 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/google/maps/places_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      968 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/google/maps/places_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/google/maps/places_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       79 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/google/maps/places_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:13.746318 google-maps-places-0.1.2/google/maps/places_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/google/maps/places_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:13.750320 google-maps-places-0.1.2/google/maps/places_v1/services/places/
+-rw-rw-r--   0 root         (0)     1003      737 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/google/maps/places_v1/services/places/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11615 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/google/maps/places_v1/services/places/async_client.py
+-rw-rw-r--   0 root         (0)     1003    20296 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/google/maps/places_v1/services/places/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:13.750320 google-maps-places-0.1.2/google/maps/places_v1/services/places/transports/
+-rw-rw-r--   0 root         (0)     1003     1288 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/google/maps/places_v1/services/places/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5971 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/google/maps/places_v1/services/places/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    11651 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/google/maps/places_v1/services/places/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    11848 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/google/maps/places_v1/services/places/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12045 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/google/maps/places_v1/services/places/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:13.750320 google-maps-places-0.1.2/google/maps/places_v1/types/
+-rw-rw-r--   0 root         (0)     1003      873 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/google/maps/places_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1616 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/google/maps/places_v1/types/geometry.py
+-rw-rw-r--   0 root         (0)     1003    29965 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/google/maps/places_v1/types/place.py
+-rw-rw-r--   0 root         (0)     1003    11880 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/google/maps/places_v1/types/places_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:13.750320 google-maps-places-0.1.2/google_maps_places.egg-info/
+-rw-r--r--   0 root         (0)     1003     4594 2023-07-05 15:57:13.000000 google-maps-places-0.1.2/google_maps_places.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1387 2023-07-05 15:57:13.000000 google-maps-places-0.1.2/google_maps_places.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:57:13.000000 google-maps-places-0.1.2/google_maps_places.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       19 2023-07-05 15:57:13.000000 google-maps-places-0.1.2/google_maps_places.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:57:13.000000 google-maps-places-0.1.2/google_maps_places.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      348 2023-07-05 15:57:13.000000 google-maps-places-0.1.2/google_maps_places.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:57:13.000000 google-maps-places-0.1.2/google_maps_places.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:57:13.754322 google-maps-places-0.1.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2962 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:13.750320 google-maps-places-0.1.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:13.750320 google-maps-places-0.1.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:13.750320 google-maps-places-0.1.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:13.750320 google-maps-places-0.1.2/tests/unit/gapic/places_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/tests/unit/gapic/places_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    60694 2023-07-05 15:46:59.000000 google-maps-places-0.1.2/tests/unit/gapic/places_v1/test_places.py
```

### Comparing `google-maps-places-0.1.1/LICENSE` & `google-maps-places-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/MANIFEST.in` & `google-maps-places-0.1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/PKG-INFO` & `google-maps-places-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-places
-Version: 0.1.1
+Version: 0.1.2
 Summary: Google Maps Places API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-places-0.1.1/README.rst` & `google-maps-places-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/google/maps/places/__init__.py` & `google-maps-places-0.1.2/google/maps/places/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/google/maps/places/gapic_version.py` & `google-maps-places-0.1.2/google/maps/places/gapic_version.py`

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
-__version__ = "0.1.1"  # {x-release-please-version}
+__version__ = "0.1.2"  # {x-release-please-version}
```

### Comparing `google-maps-places-0.1.1/google/maps/places_v1/__init__.py` & `google-maps-places-0.1.2/google/maps/places_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/google/maps/places_v1/gapic_metadata.json` & `google-maps-places-0.1.2/google/maps/places_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/google/maps/places_v1/gapic_version.py` & `google-maps-places-0.1.2/google/maps/places_v1/gapic_version.py`

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
-__version__ = "0.1.1"  # {x-release-please-version}
+__version__ = "0.1.2"  # {x-release-please-version}
```

### Comparing `google-maps-places-0.1.1/google/maps/places_v1/services/__init__.py` & `google-maps-places-0.1.2/google/maps/places_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/google/maps/places_v1/services/places/__init__.py` & `google-maps-places-0.1.2/google/maps/places_v1/services/places/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/google/maps/places_v1/services/places/async_client.py` & `google-maps-places-0.1.2/google/maps/places_v1/services/places/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,15 +269,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "PlacesAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-maps-places-0.1.1/google/maps/places_v1/services/places/client.py` & `google-maps-places-0.1.2/google/maps/places_v1/services/places/client.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/google/maps/places_v1/services/places/transports/__init__.py` & `google-maps-places-0.1.2/google/maps/places_v1/services/places/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/google/maps/places_v1/services/places/transports/base.py` & `google-maps-places-0.1.2/google/maps/places_v1/services/places/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/google/maps/places_v1/services/places/transports/grpc.py` & `google-maps-places-0.1.2/google/maps/places_v1/services/places/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/google/maps/places_v1/services/places/transports/grpc_asyncio.py` & `google-maps-places-0.1.2/google/maps/places_v1/services/places/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/google/maps/places_v1/services/places/transports/rest.py` & `google-maps-places-0.1.2/google/maps/places_v1/services/places/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/google/maps/places_v1/types/__init__.py` & `google-maps-places-0.1.2/google/maps/places_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/google/maps/places_v1/types/geometry.py` & `google-maps-places-0.1.2/google/maps/places_v1/types/geometry.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/google/maps/places_v1/types/place.py` & `google-maps-places-0.1.2/google/maps/places_v1/types/place.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/google/maps/places_v1/types/places_service.py` & `google-maps-places-0.1.2/google/maps/places_v1/types/places_service.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/google_maps_places.egg-info/PKG-INFO` & `google-maps-places-0.1.2/google_maps_places.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-places
-Version: 0.1.1
+Version: 0.1.2
 Summary: Google Maps Places API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-places-0.1.1/google_maps_places.egg-info/SOURCES.txt` & `google-maps-places-0.1.2/google_maps_places.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/setup.py` & `google-maps-places-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/tests/__init__.py` & `google-maps-places-0.1.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/tests/unit/__init__.py` & `google-maps-places-0.1.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/tests/unit/gapic/__init__.py` & `google-maps-places-0.1.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/tests/unit/gapic/places_v1/__init__.py` & `google-maps-places-0.1.2/tests/unit/gapic/places_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.1/tests/unit/gapic/places_v1/test_places.py` & `google-maps-places-0.1.2/tests/unit/gapic/places_v1/test_places.py`

 * *Files identical despite different names*

