# Comparing `tmp/google-cloud-advisorynotifications-0.2.0.tar.gz` & `tmp/google-cloud-advisorynotifications-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-advisorynotifications-0.2.0.tar", last modified: Thu Mar 30 13:46:32 2023, max compression
+gzip compressed data, was "google-cloud-advisorynotifications-0.2.1.tar", last modified: Wed Jul  5 15:49:52 2023, max compression
```

## Comparing `google-cloud-advisorynotifications-0.2.0.tar` & `google-cloud-advisorynotifications-0.2.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-30 13:46:32.627828 google-cloud-advisorynotifications-0.2.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4917 2023-03-30 13:46:32.627828 google-cloud-advisorynotifications-0.2.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3981 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-30 13:46:32.619829 google-cloud-advisorynotifications-0.2.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-30 13:46:32.619829 google-cloud-advisorynotifications-0.2.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-30 13:46:32.623829 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications/
--rw-rw-r--   0 root         (0)     1003     1684 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-30 13:46:32.623829 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/
--rw-rw-r--   0 root         (0)     1003     1499 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1508 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-30 13:46:32.623829 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-30 13:46:32.623829 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/
--rw-rw-r--   0 root         (0)     1003      825 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    19570 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    28106 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/client.py
--rw-rw-r--   0 root         (0)     1003     5956 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-30 13:46:32.627828 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/
--rw-rw-r--   0 root         (0)     1003     1617 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7257 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13030 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13277 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    17467 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-30 13:46:32.627828 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/types/
--rw-rw-r--   0 root         (0)     1003     1134 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    12969 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-30 13:46:32.627828 google-cloud-advisorynotifications-0.2.0/google_cloud_advisorynotifications.egg-info/
--rw-r--r--   0 root         (0)     1003     4917 2023-03-30 13:46:32.000000 google-cloud-advisorynotifications-0.2.0/google_cloud_advisorynotifications.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2037 2023-03-30 13:46:32.000000 google-cloud-advisorynotifications-0.2.0/google_cloud_advisorynotifications.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-30 13:46:32.000000 google-cloud-advisorynotifications-0.2.0/google_cloud_advisorynotifications.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-30 13:46:32.000000 google-cloud-advisorynotifications-0.2.0/google_cloud_advisorynotifications.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-30 13:46:32.000000 google-cloud-advisorynotifications-0.2.0/google_cloud_advisorynotifications.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-30 13:46:32.000000 google-cloud-advisorynotifications-0.2.0/google_cloud_advisorynotifications.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-30 13:46:32.000000 google-cloud-advisorynotifications-0.2.0/google_cloud_advisorynotifications.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-03-30 13:46:32.627828 google-cloud-advisorynotifications-0.2.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2974 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-30 13:46:32.627828 google-cloud-advisorynotifications-0.2.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-30 13:46:32.627828 google-cloud-advisorynotifications-0.2.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-30 13:46:32.627828 google-cloud-advisorynotifications-0.2.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-30 13:46:32.627828 google-cloud-advisorynotifications-0.2.0/tests/unit/gapic/advisorynotifications_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/tests/unit/gapic/advisorynotifications_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   103749 2023-03-30 13:44:06.000000 google-cloud-advisorynotifications-0.2.0/tests/unit/gapic/advisorynotifications_v1/test_advisory_notifications_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.968840 google-cloud-advisorynotifications-0.2.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4917 2023-07-05 15:49:52.968840 google-cloud-advisorynotifications-0.2.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3981 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.960839 google-cloud-advisorynotifications-0.2.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.960839 google-cloud-advisorynotifications-0.2.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.960839 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications/
+-rw-rw-r--   0 root         (0)     1003     1684 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.964840 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/
+-rw-rw-r--   0 root         (0)     1003     1499 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1508 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.964840 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.964840 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/
+-rw-rw-r--   0 root         (0)     1003      825 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19615 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28106 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5956 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.964840 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1617 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7257 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13030 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13277 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    17467 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.964840 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1134 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12969 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.964840 google-cloud-advisorynotifications-0.2.1/google_cloud_advisorynotifications.egg-info/
+-rw-r--r--   0 root         (0)     1003     4917 2023-07-05 15:49:52.000000 google-cloud-advisorynotifications-0.2.1/google_cloud_advisorynotifications.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2037 2023-07-05 15:49:52.000000 google-cloud-advisorynotifications-0.2.1/google_cloud_advisorynotifications.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:49:52.000000 google-cloud-advisorynotifications-0.2.1/google_cloud_advisorynotifications.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:49:52.000000 google-cloud-advisorynotifications-0.2.1/google_cloud_advisorynotifications.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:49:52.000000 google-cloud-advisorynotifications-0.2.1/google_cloud_advisorynotifications.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:49:52.000000 google-cloud-advisorynotifications-0.2.1/google_cloud_advisorynotifications.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:49:52.000000 google-cloud-advisorynotifications-0.2.1/google_cloud_advisorynotifications.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:49:52.968840 google-cloud-advisorynotifications-0.2.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2974 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.968840 google-cloud-advisorynotifications-0.2.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.968840 google-cloud-advisorynotifications-0.2.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.968840 google-cloud-advisorynotifications-0.2.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.968840 google-cloud-advisorynotifications-0.2.1/tests/unit/gapic/advisorynotifications_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/tests/unit/gapic/advisorynotifications_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   103948 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/tests/unit/gapic/advisorynotifications_v1/test_advisory_notifications_service.py
```

### Comparing `google-cloud-advisorynotifications-0.2.0/LICENSE` & `google-cloud-advisorynotifications-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.0/MANIFEST.in` & `google-cloud-advisorynotifications-0.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.0/PKG-INFO` & `google-cloud-advisorynotifications-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-advisorynotifications
-Version: 0.2.0
+Version: 0.2.1
 Summary: Google Cloud Advisorynotifications API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-advisorynotifications-0.2.0/README.rst` & `google-cloud-advisorynotifications-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications/__init__.py` & `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications/gapic_version.py` & `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,9 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.2.0"  # {x-release-please-version}
```

### Comparing `google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/__init__.py` & `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/gapic_metadata.json` & `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/gapic_version.py` & `google-cloud-advisorynotifications-0.2.1/tests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,9 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.2.0"  # {x-release-please-version}
```

### Comparing `google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/__init__.py` & `google-cloud-advisorynotifications-0.2.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/__init__.py` & `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/async_client.py` & `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -463,15 +463,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "AdvisoryNotificationsServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/client.py` & `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/pagers.py` & `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/__init__.py` & `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/base.py` & `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc.py` & `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc_asyncio.py` & `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/rest.py` & `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/types/__init__.py` & `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.0/google/cloud/advisorynotifications_v1/types/service.py` & `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.0/google_cloud_advisorynotifications.egg-info/PKG-INFO` & `google-cloud-advisorynotifications-0.2.1/google_cloud_advisorynotifications.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-advisorynotifications
-Version: 0.2.0
+Version: 0.2.1
 Summary: Google Cloud Advisorynotifications API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-advisorynotifications-0.2.0/google_cloud_advisorynotifications.egg-info/SOURCES.txt` & `google-cloud-advisorynotifications-0.2.1/google_cloud_advisorynotifications.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.0/setup.py` & `google-cloud-advisorynotifications-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.0/tests/__init__.py` & `google-cloud-advisorynotifications-0.2.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.0/tests/unit/__init__.py` & `google-cloud-advisorynotifications-0.2.1/tests/unit/gapic/advisorynotifications_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.0/tests/unit/gapic/advisorynotifications_v1/test_advisory_notifications_service.py` & `google-cloud-advisorynotifications-0.2.1/tests/unit/gapic/advisorynotifications_v1/test_advisory_notifications_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1192,17 +1192,19 @@
                     service.Notification(),
                     service.Notification(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_notifications(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

