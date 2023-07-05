# Comparing `tmp/google-cloud-bigquery-reservation-1.9.0.tar.gz` & `tmp/google-cloud-bigquery-reservation-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-bigquery-reservation-1.9.0.tar", last modified: Wed Jan 11 16:09:05 2023, max compression
+gzip compressed data, was "google-cloud-bigquery-reservation-1.9.1.tar", last modified: Mon Jan 23 15:52:51 2023, max compression
```

## Comparing `google-cloud-bigquery-reservation-1.9.0.tar` & `google-cloud-bigquery-reservation-1.9.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 16:09:05.901388 google-cloud-bigquery-reservation-1.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4798 2023-01-11 16:09:05.901388 google-cloud-bigquery-reservation-1.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3843 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 16:09:05.893390 google-cloud-bigquery-reservation-1.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 16:09:05.893390 google-cloud-bigquery-reservation-1.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 16:09:05.897389 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation/
--rw-rw-r--   0 root         (0)     1003     3112 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       94 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 16:09:05.897389 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/
--rw-rw-r--   0 root         (0)     1003     2938 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     6207 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       94 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 16:09:05.897389 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 16:09:05.897389 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/services/reservation_service/
--rw-rw-r--   0 root         (0)     1003      785 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/services/reservation_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   122861 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/services/reservation_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   133570 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/services/reservation_service/client.py
--rw-rw-r--   0 root         (0)     1003    26937 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/services/reservation_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 16:09:05.897389 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/services/reservation_service/transports/
--rw-rw-r--   0 root         (0)     1003     1237 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/services/reservation_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    19886 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/services/reservation_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    43751 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/services/reservation_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    44579 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/services/reservation_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 16:09:05.897389 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/types/
--rw-rw-r--   0 root         (0)     1003     2628 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    36154 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/types/reservation.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 16:09:05.901388 google-cloud-bigquery-reservation-1.9.0/google_cloud_bigquery_reservation.egg-info/
--rw-r--r--   0 root         (0)     1003     4798 2023-01-11 16:09:05.000000 google-cloud-bigquery-reservation-1.9.0/google_cloud_bigquery_reservation.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1844 2023-01-11 16:09:05.000000 google-cloud-bigquery-reservation-1.9.0/google_cloud_bigquery_reservation.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-11 16:09:05.000000 google-cloud-bigquery-reservation-1.9.0/google_cloud_bigquery_reservation.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-11 16:09:05.000000 google-cloud-bigquery-reservation-1.9.0/google_cloud_bigquery_reservation.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-11 16:09:05.000000 google-cloud-bigquery-reservation-1.9.0/google_cloud_bigquery_reservation.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-01-11 16:09:05.000000 google-cloud-bigquery-reservation-1.9.0/google_cloud_bigquery_reservation.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-11 16:09:05.000000 google-cloud-bigquery-reservation-1.9.0/google_cloud_bigquery_reservation.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-01-11 16:09:05.901388 google-cloud-bigquery-reservation-1.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3032 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 16:09:05.901388 google-cloud-bigquery-reservation-1.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/tests/__init__.py
--rw-rw-r--   0 root         (0)     1003     1018 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/tests/system.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 16:09:05.901388 google-cloud-bigquery-reservation-1.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 16:09:05.901388 google-cloud-bigquery-reservation-1.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 16:09:05.901388 google-cloud-bigquery-reservation-1.9.0/tests/unit/gapic/bigquery_reservation_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/tests/unit/gapic/bigquery_reservation_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   283198 2023-01-11 16:05:36.000000 google-cloud-bigquery-reservation-1.9.0/tests/unit/gapic/bigquery_reservation_v1/test_reservation_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:52:51.972732 google-cloud-bigquery-reservation-1.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4798 2023-01-23 15:52:51.972732 google-cloud-bigquery-reservation-1.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3843 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:52:51.960731 google-cloud-bigquery-reservation-1.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:52:51.960731 google-cloud-bigquery-reservation-1.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:52:51.964731 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation/
+-rw-rw-r--   0 root         (0)     1003     3112 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       94 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:52:51.964731 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/
+-rw-rw-r--   0 root         (0)     1003     2938 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6207 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       94 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:52:51.964731 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:52:51.968732 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/services/reservation_service/
+-rw-rw-r--   0 root         (0)     1003      785 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/services/reservation_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   122861 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/services/reservation_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   133600 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/services/reservation_service/client.py
+-rw-rw-r--   0 root         (0)     1003    26937 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/services/reservation_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:52:51.968732 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/services/reservation_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1237 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/services/reservation_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19886 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/services/reservation_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    43751 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/services/reservation_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    44579 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/services/reservation_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:52:51.968732 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2628 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    39002 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/types/reservation.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:52:51.968732 google-cloud-bigquery-reservation-1.9.1/google_cloud_bigquery_reservation.egg-info/
+-rw-r--r--   0 root         (0)     1003     4798 2023-01-23 15:52:51.000000 google-cloud-bigquery-reservation-1.9.1/google_cloud_bigquery_reservation.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1844 2023-01-23 15:52:51.000000 google-cloud-bigquery-reservation-1.9.1/google_cloud_bigquery_reservation.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 15:52:51.000000 google-cloud-bigquery-reservation-1.9.1/google_cloud_bigquery_reservation.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-01-23 15:52:51.000000 google-cloud-bigquery-reservation-1.9.1/google_cloud_bigquery_reservation.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 15:52:51.000000 google-cloud-bigquery-reservation-1.9.1/google_cloud_bigquery_reservation.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-01-23 15:52:51.000000 google-cloud-bigquery-reservation-1.9.1/google_cloud_bigquery_reservation.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-01-23 15:52:51.000000 google-cloud-bigquery-reservation-1.9.1/google_cloud_bigquery_reservation.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-01-23 15:52:51.972732 google-cloud-bigquery-reservation-1.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3032 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:52:51.972732 google-cloud-bigquery-reservation-1.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/tests/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1018 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/tests/system.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:52:51.972732 google-cloud-bigquery-reservation-1.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:52:51.972732 google-cloud-bigquery-reservation-1.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:52:51.972732 google-cloud-bigquery-reservation-1.9.1/tests/unit/gapic/bigquery_reservation_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/tests/unit/gapic/bigquery_reservation_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   283198 2023-01-23 15:49:12.000000 google-cloud-bigquery-reservation-1.9.1/tests/unit/gapic/bigquery_reservation_v1/test_reservation_service.py
```

### Comparing `google-cloud-bigquery-reservation-1.9.0/LICENSE` & `google-cloud-bigquery-reservation-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/MANIFEST.in` & `google-cloud-bigquery-reservation-1.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/PKG-INFO` & `google-cloud-bigquery-reservation-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-reservation
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Bigquery Reservation API client library
 Home-page: https://github.com/googleapis/python-bigquery-reservation
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-bigquery-reservation-1.9.0/README.rst` & `google-cloud-bigquery-reservation-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation/__init__.py` & `google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation/gapic_version.py` & `google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation/gapic_version.py`

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

### Comparing `google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/__init__.py` & `google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/gapic_metadata.json` & `google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/gapic_version.py` & `google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/gapic_version.py`

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

### Comparing `google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/services/__init__.py` & `google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/services/reservation_service/__init__.py` & `google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/services/reservation_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/services/reservation_service/async_client.py` & `google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/services/reservation_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/services/reservation_service/client.py` & `google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/services/reservation_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3111,15 +3111,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "ReservationServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/services/reservation_service/pagers.py` & `google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/services/reservation_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/services/reservation_service/transports/__init__.py` & `google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/services/reservation_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/services/reservation_service/transports/base.py` & `google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/services/reservation_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/services/reservation_service/transports/grpc.py` & `google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/services/reservation_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/services/reservation_service/transports/grpc_asyncio.py` & `google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/services/reservation_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/types/__init__.py` & `google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/google/cloud/bigquery_reservation_v1/types/reservation.py` & `google-cloud-bigquery-reservation-1.9.1/google/cloud/bigquery_reservation_v1/types/reservation.py`

 * *Files 3% similar despite different names*

```diff
@@ -205,24 +205,64 @@
             organization's default region.
     """
 
     class CommitmentPlan(proto.Enum):
         r"""Commitment plan defines the current committed period.
         Capacity commitment cannot be deleted during it's committed
         period.
+
+        Values:
+            COMMITMENT_PLAN_UNSPECIFIED (0):
+                Invalid plan value. Requests with this value will be
+                rejected with error code
+                ``google.rpc.Code.INVALID_ARGUMENT``.
+            FLEX (3):
+                Flex commitments have committed period of 1
+                minute after becoming ACTIVE. After that, they
+                are not in a committed period anymore and can be
+                removed any time.
+            TRIAL (5):
+                Trial commitments have a committed period of 182 days after
+                becoming ACTIVE. After that, they are converted to a new
+                commitment based on the ``renewal_plan``. Default
+                ``renewal_plan`` for Trial commitment is Flex so that it can
+                be deleted right after committed period ends.
+            MONTHLY (2):
+                Monthly commitments have a committed period
+                of 30 days after becoming ACTIVE. After that,
+                they are not in a committed period anymore and
+                can be removed any time.
+            ANNUAL (4):
+                Annual commitments have a committed period of 365 days after
+                becoming ACTIVE. After that they are converted to a new
+                commitment based on the renewal_plan.
         """
         COMMITMENT_PLAN_UNSPECIFIED = 0
         FLEX = 3
         TRIAL = 5
         MONTHLY = 2
         ANNUAL = 4
 
     class State(proto.Enum):
         r"""Capacity commitment can either become ACTIVE right away or
         transition from PENDING to ACTIVE or FAILED.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                Invalid state value.
+            PENDING (1):
+                Capacity commitment is pending provisioning. Pending
+                capacity commitment does not contribute to the project's
+                slot_capacity.
+            ACTIVE (2):
+                Once slots are provisioned, capacity commitment becomes
+                active. slot_count is added to the project's slot_capacity.
+            FAILED (3):
+                Capacity commitment is failed to be activated
+                by the backend.
         """
         STATE_UNSPECIFIED = 0
         PENDING = 1
         ACTIVE = 2
         FAILED = 3
 
     name: str = proto.Field(
@@ -679,24 +719,48 @@
         state (google.cloud.bigquery_reservation_v1.types.Assignment.State):
             Output only. State of the assignment.
     """
 
     class JobType(proto.Enum):
         r"""Types of job, which could be specified when using the
         reservation.
+
+        Values:
+            JOB_TYPE_UNSPECIFIED (0):
+                Invalid type. Requests with this value will be rejected with
+                error code ``google.rpc.Code.INVALID_ARGUMENT``.
+            PIPELINE (1):
+                Pipeline (load/export) jobs from the project
+                will use the reservation.
+            QUERY (2):
+                Query jobs from the project will use the
+                reservation.
+            ML_EXTERNAL (3):
+                BigQuery ML jobs that use services external
+                to BigQuery for model training. These jobs will
+                not utilize idle slots from other reservations.
         """
         JOB_TYPE_UNSPECIFIED = 0
         PIPELINE = 1
         QUERY = 2
         ML_EXTERNAL = 3
 
     class State(proto.Enum):
         r"""Assignment will remain in PENDING state if no active capacity
         commitment is present. It will become ACTIVE when some capacity
         commitment becomes active.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                Invalid state value.
+            PENDING (1):
+                Queries from assignee will be executed as
+                on-demand, if related assignment is pending.
+            ACTIVE (2):
+                Assignment is ready.
         """
         STATE_UNSPECIFIED = 0
         PENDING = 1
         ACTIVE = 2
 
     name: str = proto.Field(
         proto.STRING,
```

### Comparing `google-cloud-bigquery-reservation-1.9.0/google_cloud_bigquery_reservation.egg-info/PKG-INFO` & `google-cloud-bigquery-reservation-1.9.1/google_cloud_bigquery_reservation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-reservation
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Bigquery Reservation API client library
 Home-page: https://github.com/googleapis/python-bigquery-reservation
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-bigquery-reservation-1.9.0/google_cloud_bigquery_reservation.egg-info/SOURCES.txt` & `google-cloud-bigquery-reservation-1.9.1/google_cloud_bigquery_reservation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/setup.py` & `google-cloud-bigquery-reservation-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/tests/__init__.py` & `google-cloud-bigquery-reservation-1.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/tests/system.py` & `google-cloud-bigquery-reservation-1.9.1/tests/system.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/tests/unit/__init__.py` & `google-cloud-bigquery-reservation-1.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/tests/unit/gapic/__init__.py` & `google-cloud-bigquery-reservation-1.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/tests/unit/gapic/bigquery_reservation_v1/__init__.py` & `google-cloud-bigquery-reservation-1.9.1/tests/unit/gapic/bigquery_reservation_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-reservation-1.9.0/tests/unit/gapic/bigquery_reservation_v1/test_reservation_service.py` & `google-cloud-bigquery-reservation-1.9.1/tests/unit/gapic/bigquery_reservation_v1/test_reservation_service.py`

 * *Files identical despite different names*

