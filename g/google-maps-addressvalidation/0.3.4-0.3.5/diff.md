# Comparing `tmp/google-maps-addressvalidation-0.3.4.tar.gz` & `tmp/google-maps-addressvalidation-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-maps-addressvalidation-0.3.4.tar", last modified: Mon Jun  5 14:00:08 2023, max compression
+gzip compressed data, was "google-maps-addressvalidation-0.3.5.tar", last modified: Wed Jul  5 15:57:03 2023, max compression
```

## Comparing `google-maps-addressvalidation-0.3.4.tar` & `google-maps-addressvalidation-0.3.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:08.679520 google-maps-addressvalidation-0.3.4/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4803 2023-06-05 14:00:08.679520 google-maps-addressvalidation-0.3.4/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3877 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:08.667519 google-maps-addressvalidation-0.3.4/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:08.667519 google-maps-addressvalidation-0.3.4/google/maps/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:08.671519 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation/
--rw-rw-r--   0 root         (0)     1003     1974 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:08.671519 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/
--rw-rw-r--   0 root         (0)     1003     1671 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1505 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:08.671519 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:08.671519 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/services/address_validation/
--rw-rw-r--   0 root         (0)     1003      781 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/services/address_validation/__init__.py
--rw-rw-r--   0 root         (0)     1003    15687 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/services/address_validation/async_client.py
--rw-rw-r--   0 root         (0)     1003    24571 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/services/address_validation/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:08.675519 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/services/address_validation/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/services/address_validation/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6718 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/services/address_validation/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13582 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/services/address_validation/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13812 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/services/address_validation/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    18770 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/services/address_validation/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:08.675519 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/types/
--rw-rw-r--   0 root         (0)     1003     1343 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     9245 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/types/address.py
--rw-rw-r--   0 root         (0)     1003    15189 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/types/address_validation_service.py
--rw-rw-r--   0 root         (0)     1003     4435 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/types/geocode.py
--rw-rw-r--   0 root         (0)     1003     2175 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/types/metadata_.py
--rw-rw-r--   0 root         (0)     1003    11749 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/types/usps_data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:08.675519 google-maps-addressvalidation-0.3.4/google_maps_addressvalidation.egg-info/
--rw-r--r--   0 root         (0)     1003     4803 2023-06-05 14:00:08.000000 google-maps-addressvalidation-0.3.4/google_maps_addressvalidation.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1931 2023-06-05 14:00:08.000000 google-maps-addressvalidation-0.3.4/google_maps_addressvalidation.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-05 14:00:08.000000 google-maps-addressvalidation-0.3.4/google_maps_addressvalidation.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       19 2023-06-05 14:00:08.000000 google-maps-addressvalidation-0.3.4/google_maps_addressvalidation.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-05 14:00:08.000000 google-maps-addressvalidation-0.3.4/google_maps_addressvalidation.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      348 2023-06-05 14:00:08.000000 google-maps-addressvalidation-0.3.4/google_maps_addressvalidation.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-05 14:00:08.000000 google-maps-addressvalidation-0.3.4/google_maps_addressvalidation.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-06-05 14:00:08.679520 google-maps-addressvalidation-0.3.4/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3001 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:08.675519 google-maps-addressvalidation-0.3.4/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:08.675519 google-maps-addressvalidation-0.3.4/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:08.675519 google-maps-addressvalidation-0.3.4/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:08.675519 google-maps-addressvalidation-0.3.4/tests/unit/gapic/addressvalidation_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/tests/unit/gapic/addressvalidation_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    76826 2023-06-05 13:56:51.000000 google-maps-addressvalidation-0.3.4/tests/unit/gapic/addressvalidation_v1/test_address_validation.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:03.279270 google-maps-addressvalidation-0.3.5/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4803 2023-07-05 15:57:03.279270 google-maps-addressvalidation-0.3.5/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3877 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:03.271270 google-maps-addressvalidation-0.3.5/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:03.271270 google-maps-addressvalidation-0.3.5/google/maps/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:03.271270 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation/
+-rw-rw-r--   0 root         (0)     1003     1974 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:03.275270 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/
+-rw-rw-r--   0 root         (0)     1003     1671 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1505 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:03.275270 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:03.275270 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/services/address_validation/
+-rw-rw-r--   0 root         (0)     1003      781 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/services/address_validation/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15721 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/services/address_validation/async_client.py
+-rw-rw-r--   0 root         (0)     1003    24571 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/services/address_validation/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:03.275270 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/services/address_validation/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/services/address_validation/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6718 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/services/address_validation/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13582 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/services/address_validation/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13812 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/services/address_validation/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    18770 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/services/address_validation/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:03.275270 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1343 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9245 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/types/address.py
+-rw-rw-r--   0 root         (0)     1003    15189 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/types/address_validation_service.py
+-rw-rw-r--   0 root         (0)     1003     4435 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/types/geocode.py
+-rw-rw-r--   0 root         (0)     1003     2175 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/types/metadata_.py
+-rw-rw-r--   0 root         (0)     1003    11749 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/types/usps_data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:03.279270 google-maps-addressvalidation-0.3.5/google_maps_addressvalidation.egg-info/
+-rw-r--r--   0 root         (0)     1003     4803 2023-07-05 15:57:03.000000 google-maps-addressvalidation-0.3.5/google_maps_addressvalidation.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1931 2023-07-05 15:57:03.000000 google-maps-addressvalidation-0.3.5/google_maps_addressvalidation.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:57:03.000000 google-maps-addressvalidation-0.3.5/google_maps_addressvalidation.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       19 2023-07-05 15:57:03.000000 google-maps-addressvalidation-0.3.5/google_maps_addressvalidation.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:57:03.000000 google-maps-addressvalidation-0.3.5/google_maps_addressvalidation.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      348 2023-07-05 15:57:03.000000 google-maps-addressvalidation-0.3.5/google_maps_addressvalidation.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:57:03.000000 google-maps-addressvalidation-0.3.5/google_maps_addressvalidation.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:57:03.279270 google-maps-addressvalidation-0.3.5/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3001 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:03.279270 google-maps-addressvalidation-0.3.5/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:03.279270 google-maps-addressvalidation-0.3.5/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:03.279270 google-maps-addressvalidation-0.3.5/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:03.279270 google-maps-addressvalidation-0.3.5/tests/unit/gapic/addressvalidation_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/tests/unit/gapic/addressvalidation_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    76826 2023-07-05 15:46:59.000000 google-maps-addressvalidation-0.3.5/tests/unit/gapic/addressvalidation_v1/test_address_validation.py
```

### Comparing `google-maps-addressvalidation-0.3.4/LICENSE` & `google-maps-addressvalidation-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/MANIFEST.in` & `google-maps-addressvalidation-0.3.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/PKG-INFO` & `google-maps-addressvalidation-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-addressvalidation
-Version: 0.3.4
+Version: 0.3.5
 Summary: Google Maps Addressvalidation API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-addressvalidation-0.3.4/README.rst` & `google-maps-addressvalidation-0.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/google/maps/addressvalidation/__init__.py` & `google-maps-addressvalidation-0.3.5/google/maps/addressvalidation/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/google/maps/addressvalidation/gapic_version.py` & `google-maps-addressvalidation-0.3.5/google/maps/addressvalidation/gapic_version.py`

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
-__version__ = "0.3.4"  # {x-release-please-version}
+__version__ = "0.3.5"  # {x-release-please-version}
```

### Comparing `google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/__init__.py` & `google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/gapic_metadata.json` & `google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/gapic_version.py` & `google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/gapic_version.py`

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
-__version__ = "0.3.4"  # {x-release-please-version}
+__version__ = "0.3.5"  # {x-release-please-version}
```

### Comparing `google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/services/__init__.py` & `google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/services/address_validation/__init__.py` & `google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/services/address_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/services/address_validation/async_client.py` & `google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/services/address_validation/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,15 +365,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "AddressValidationAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/services/address_validation/client.py` & `google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/services/address_validation/client.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/services/address_validation/transports/__init__.py` & `google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/services/address_validation/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/services/address_validation/transports/base.py` & `google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/services/address_validation/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/services/address_validation/transports/grpc.py` & `google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/services/address_validation/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/services/address_validation/transports/grpc_asyncio.py` & `google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/services/address_validation/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/services/address_validation/transports/rest.py` & `google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/services/address_validation/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/types/__init__.py` & `google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/types/address.py` & `google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/types/address.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/types/address_validation_service.py` & `google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/types/address_validation_service.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/types/geocode.py` & `google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/types/geocode.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/types/metadata_.py` & `google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/types/metadata_.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/google/maps/addressvalidation_v1/types/usps_data.py` & `google-maps-addressvalidation-0.3.5/google/maps/addressvalidation_v1/types/usps_data.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/google_maps_addressvalidation.egg-info/PKG-INFO` & `google-maps-addressvalidation-0.3.5/google_maps_addressvalidation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-addressvalidation
-Version: 0.3.4
+Version: 0.3.5
 Summary: Google Maps Addressvalidation API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-addressvalidation-0.3.4/google_maps_addressvalidation.egg-info/SOURCES.txt` & `google-maps-addressvalidation-0.3.5/google_maps_addressvalidation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/setup.py` & `google-maps-addressvalidation-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/tests/__init__.py` & `google-maps-addressvalidation-0.3.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/tests/unit/__init__.py` & `google-maps-addressvalidation-0.3.5/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/tests/unit/gapic/__init__.py` & `google-maps-addressvalidation-0.3.5/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/tests/unit/gapic/addressvalidation_v1/__init__.py` & `google-maps-addressvalidation-0.3.5/tests/unit/gapic/addressvalidation_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-addressvalidation-0.3.4/tests/unit/gapic/addressvalidation_v1/test_address_validation.py` & `google-maps-addressvalidation-0.3.5/tests/unit/gapic/addressvalidation_v1/test_address_validation.py`

 * *Files identical despite different names*

