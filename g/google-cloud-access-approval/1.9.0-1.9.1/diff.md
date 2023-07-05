# Comparing `tmp/google-cloud-access-approval-1.9.0.tar.gz` & `tmp/google-cloud-access-approval-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-access-approval-1.9.0.tar", last modified: Mon Nov 14 21:05:22 2022, max compression
+gzip compressed data, was "google-cloud-access-approval-1.9.1.tar", last modified: Thu Dec  8 14:45:30 2022, max compression
```

## Comparing `google-cloud-access-approval-1.9.0.tar` & `google-cloud-access-approval-1.9.1.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-11-14 21:05:22.855257 google-cloud-access-approval-1.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4604 2022-11-14 21:05:22.855257 google-cloud-access-approval-1.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3715 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-11-14 21:05:22.847257 google-cloud-access-approval-1.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-11-14 21:05:22.851257 google-cloud-access-approval-1.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-11-14 21:05:22.851257 google-cloud-access-approval-1.9.0/google/cloud/accessapproval/
--rw-rw-r--   0 root         (0)     1003     2363 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/google/cloud/accessapproval/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/google/cloud/accessapproval/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/google/cloud/accessapproval/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-11-14 21:05:22.851257 google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/
--rw-rw-r--   0 root         (0)     1003     2198 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3191 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       89 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-11-14 21:05:22.851257 google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-11-14 21:05:22.855257 google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/services/access_approval/
--rw-rw-r--   0 root         (0)     1003      769 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/services/access_approval/__init__.py
--rw-rw-r--   0 root         (0)     1003    49904 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/services/access_approval/async_client.py
--rw-rw-r--   0 root         (0)     1003    60239 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/services/access_approval/client.py
--rw-rw-r--   0 root         (0)     1003     6088 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/services/access_approval/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-11-14 21:05:22.855257 google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/services/access_approval/transports/
--rw-rw-r--   0 root         (0)     1003     1193 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/services/access_approval/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11552 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/services/access_approval/transports/base.py
--rw-rw-r--   0 root         (0)     1003    25688 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/services/access_approval/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    26096 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/services/access_approval/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-11-14 21:05:22.855257 google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/types/
--rw-rw-r--   0 root         (0)     1003     1927 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    25371 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/types/accessapproval.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-11-14 21:05:22.855257 google-cloud-access-approval-1.9.0/google_cloud_access_approval.egg-info/
--rw-r--r--   0 root         (0)     1003     4604 2022-11-14 21:05:22.000000 google-cloud-access-approval-1.9.0/google_cloud_access_approval.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1592 2022-11-14 21:05:22.000000 google-cloud-access-approval-1.9.0/google_cloud_access_approval.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-11-14 21:05:22.000000 google-cloud-access-approval-1.9.0/google_cloud_access_approval.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-11-14 21:05:22.000000 google-cloud-access-approval-1.9.0/google_cloud_access_approval.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-11-14 21:05:22.000000 google-cloud-access-approval-1.9.0/google_cloud_access_approval.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      232 2022-11-14 21:05:22.000000 google-cloud-access-approval-1.9.0/google_cloud_access_approval.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-11-14 21:05:22.000000 google-cloud-access-approval-1.9.0/google_cloud_access_approval.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2022-11-14 21:05:22.859257 google-cloud-access-approval-1.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2873 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-11-14 21:05:22.855257 google-cloud-access-approval-1.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-11-14 21:05:22.855257 google-cloud-access-approval-1.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-11-14 21:05:22.855257 google-cloud-access-approval-1.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-11-14 21:05:22.855257 google-cloud-access-approval-1.9.0/tests/unit/gapic/accessapproval_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/tests/unit/gapic/accessapproval_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   133933 2022-11-14 21:02:46.000000 google-cloud-access-approval-1.9.0/tests/unit/gapic/accessapproval_v1/test_access_approval.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-08 14:45:30.649868 google-cloud-access-approval-1.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4604 2022-12-08 14:45:30.649868 google-cloud-access-approval-1.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3715 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-08 14:45:30.641868 google-cloud-access-approval-1.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-08 14:45:30.641868 google-cloud-access-approval-1.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-08 14:45:30.645868 google-cloud-access-approval-1.9.1/google/cloud/accessapproval/
+-rw-rw-r--   0 root         (0)     1003     2363 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/google/cloud/accessapproval/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/google/cloud/accessapproval/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/google/cloud/accessapproval/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-08 14:45:30.645868 google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/
+-rw-rw-r--   0 root         (0)     1003     2198 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3191 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-08 14:45:30.645868 google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-08 14:45:30.645868 google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/services/access_approval/
+-rw-rw-r--   0 root         (0)     1003      769 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/services/access_approval/__init__.py
+-rw-rw-r--   0 root         (0)     1003    49989 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/services/access_approval/async_client.py
+-rw-rw-r--   0 root         (0)     1003    60324 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/services/access_approval/client.py
+-rw-rw-r--   0 root         (0)     1003     6088 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/services/access_approval/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-08 14:45:30.645868 google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/services/access_approval/transports/
+-rw-rw-r--   0 root         (0)     1003     1193 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/services/access_approval/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11420 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/services/access_approval/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    25688 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/services/access_approval/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    26096 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/services/access_approval/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-08 14:45:30.649868 google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1927 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25371 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/types/accessapproval.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-08 14:45:30.649868 google-cloud-access-approval-1.9.1/google_cloud_access_approval.egg-info/
+-rw-r--r--   0 root         (0)     1003     4604 2022-12-08 14:45:30.000000 google-cloud-access-approval-1.9.1/google_cloud_access_approval.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1640 2022-12-08 14:45:30.000000 google-cloud-access-approval-1.9.1/google_cloud_access_approval.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-12-08 14:45:30.000000 google-cloud-access-approval-1.9.1/google_cloud_access_approval.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-12-08 14:45:30.000000 google-cloud-access-approval-1.9.1/google_cloud_access_approval.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-12-08 14:45:30.000000 google-cloud-access-approval-1.9.1/google_cloud_access_approval.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      257 2022-12-08 14:45:30.000000 google-cloud-access-approval-1.9.1/google_cloud_access_approval.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-12-08 14:45:30.000000 google-cloud-access-approval-1.9.1/google_cloud_access_approval.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2022-12-08 14:45:30.649868 google-cloud-access-approval-1.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2898 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-08 14:45:30.649868 google-cloud-access-approval-1.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-08 14:45:30.649868 google-cloud-access-approval-1.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-08 14:45:30.649868 google-cloud-access-approval-1.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-08 14:45:30.649868 google-cloud-access-approval-1.9.1/tests/unit/gapic/accessapproval_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/tests/unit/gapic/accessapproval_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   133933 2022-12-08 14:42:52.000000 google-cloud-access-approval-1.9.1/tests/unit/gapic/accessapproval_v1/test_access_approval.py
```

### Comparing `google-cloud-access-approval-1.9.0/LICENSE` & `google-cloud-access-approval-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-access-approval-1.9.0/MANIFEST.in` & `google-cloud-access-approval-1.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-access-approval-1.9.0/PKG-INFO` & `google-cloud-access-approval-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-access-approval
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Access Approval API client library
 Home-page: https://github.com/googleapis/python-access-approval
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-access-approval-1.9.0/README.rst` & `google-cloud-access-approval-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-access-approval-1.9.0/google/cloud/accessapproval/__init__.py` & `google-cloud-access-approval-1.9.1/google/cloud/accessapproval/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-access-approval-1.9.0/google/cloud/accessapproval/gapic_version.py` & `google-cloud-access-approval-1.9.1/google/cloud/accessapproval/gapic_version.py`

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

### Comparing `google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/__init__.py` & `google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/gapic_metadata.json` & `google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/services/__init__.py` & `google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/services/access_approval/__init__.py` & `google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/services/access_approval/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/services/access_approval/async_client.py` & `google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/services/access_approval/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.accessapproval_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.protobuf import field_mask_pb2  # type: ignore
@@ -269,15 +270,15 @@
         self,
         request: Optional[
             Union[accessapproval.ListApprovalRequestsMessage, dict]
         ] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Optional[float] = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListApprovalRequestsAsyncPager:
         r"""Lists approval requests associated with a project,
         folder, or organization. Approval requests can be
         filtered by state (pending, active, dismissed). The
         order is reverse chronological.
 
@@ -396,15 +397,15 @@
 
     async def get_approval_request(
         self,
         request: Optional[Union[accessapproval.GetApprovalRequestMessage, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Optional[float] = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> accessapproval.ApprovalRequest:
         r"""Gets an approval request. Returns NOT_FOUND if the request does
         not exist.
 
         .. code-block:: python
 
@@ -507,15 +508,15 @@
     async def approve_approval_request(
         self,
         request: Optional[
             Union[accessapproval.ApproveApprovalRequestMessage, dict]
         ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Optional[float] = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> accessapproval.ApprovalRequest:
         r"""Approves a request and returns the updated ApprovalRequest.
 
         Returns NOT_FOUND if the request does not exist. Returns
         FAILED_PRECONDITION if the request exists but is not in a
         pending state.
@@ -592,15 +593,15 @@
     async def dismiss_approval_request(
         self,
         request: Optional[
             Union[accessapproval.DismissApprovalRequestMessage, dict]
         ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Optional[float] = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> accessapproval.ApprovalRequest:
         r"""Dismisses a request. Returns the updated ApprovalRequest.
 
         NOTE: This does not deny access to the resource if another
         request has been made and approved. It is equivalent in effect
         to ignoring the request altogether.
@@ -682,15 +683,15 @@
     async def invalidate_approval_request(
         self,
         request: Optional[
             Union[accessapproval.InvalidateApprovalRequestMessage, dict]
         ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Optional[float] = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> accessapproval.ApprovalRequest:
         r"""Invalidates an existing ApprovalRequest. Returns the updated
         ApprovalRequest.
 
         NOTE: This does not deny access to the resource if another
         request has been made and approved. It only invalidates a single
@@ -772,15 +773,15 @@
         self,
         request: Optional[
             Union[accessapproval.GetAccessApprovalSettingsMessage, dict]
         ] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Optional[float] = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> accessapproval.AccessApprovalSettings:
         r"""Gets the settings associated with a project, folder,
         or organization.
 
         .. code-block:: python
 
@@ -888,15 +889,15 @@
         request: Optional[
             Union[accessapproval.UpdateAccessApprovalSettingsMessage, dict]
         ] = None,
         *,
         settings: Optional[accessapproval.AccessApprovalSettings] = None,
         update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Optional[float] = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> accessapproval.AccessApprovalSettings:
         r"""Updates the settings associated with a project, folder, or
         organization. Settings to update are determined by the value of
         field_mask.
 
         .. code-block:: python
@@ -1012,15 +1013,15 @@
         self,
         request: Optional[
             Union[accessapproval.DeleteAccessApprovalSettingsMessage, dict]
         ] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Optional[float] = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
         r"""Deletes the settings associated with a project,
         folder, or organization. This will have the effect of
         disabling Access Approval for the project, folder, or
         organization, but only if all ancestors also have Access
         Approval disabled. If Access Approval is enabled at a
@@ -1110,15 +1111,15 @@
         self,
         request: Optional[
             Union[accessapproval.GetAccessApprovalServiceAccountMessage, dict]
         ] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Optional[float] = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> accessapproval.AccessApprovalServiceAccount:
         r"""Retrieves the service account that is used by Access
         Approval to access KMS keys for signing approved
         approval requests.
 
         .. code-block:: python
@@ -1216,18 +1217,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-access-approval",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("AccessApprovalAsyncClient",)
```

### Comparing `google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/services/access_approval/client.py` & `google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/services/access_approval/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,16 @@
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.accessapproval_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.protobuf import field_mask_pb2  # type: ignore
@@ -510,15 +511,15 @@
         self,
         request: Optional[
             Union[accessapproval.ListApprovalRequestsMessage, dict]
         ] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Optional[float] = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListApprovalRequestsPager:
         r"""Lists approval requests associated with a project,
         folder, or organization. Approval requests can be
         filtered by state (pending, active, dismissed). The
         order is reverse chronological.
 
@@ -628,15 +629,15 @@
 
     def get_approval_request(
         self,
         request: Optional[Union[accessapproval.GetApprovalRequestMessage, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Optional[float] = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> accessapproval.ApprovalRequest:
         r"""Gets an approval request. Returns NOT_FOUND if the request does
         not exist.
 
         .. code-block:: python
 
@@ -730,15 +731,15 @@
     def approve_approval_request(
         self,
         request: Optional[
             Union[accessapproval.ApproveApprovalRequestMessage, dict]
         ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Optional[float] = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> accessapproval.ApprovalRequest:
         r"""Approves a request and returns the updated ApprovalRequest.
 
         Returns NOT_FOUND if the request does not exist. Returns
         FAILED_PRECONDITION if the request exists but is not in a
         pending state.
@@ -816,15 +817,15 @@
     def dismiss_approval_request(
         self,
         request: Optional[
             Union[accessapproval.DismissApprovalRequestMessage, dict]
         ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Optional[float] = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> accessapproval.ApprovalRequest:
         r"""Dismisses a request. Returns the updated ApprovalRequest.
 
         NOTE: This does not deny access to the resource if another
         request has been made and approved. It is equivalent in effect
         to ignoring the request altogether.
@@ -907,15 +908,15 @@
     def invalidate_approval_request(
         self,
         request: Optional[
             Union[accessapproval.InvalidateApprovalRequestMessage, dict]
         ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Optional[float] = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> accessapproval.ApprovalRequest:
         r"""Invalidates an existing ApprovalRequest. Returns the updated
         ApprovalRequest.
 
         NOTE: This does not deny access to the resource if another
         request has been made and approved. It only invalidates a single
@@ -1000,15 +1001,15 @@
         self,
         request: Optional[
             Union[accessapproval.GetAccessApprovalSettingsMessage, dict]
         ] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Optional[float] = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> accessapproval.AccessApprovalSettings:
         r"""Gets the settings associated with a project, folder,
         or organization.
 
         .. code-block:: python
 
@@ -1109,15 +1110,15 @@
         request: Optional[
             Union[accessapproval.UpdateAccessApprovalSettingsMessage, dict]
         ] = None,
         *,
         settings: Optional[accessapproval.AccessApprovalSettings] = None,
         update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Optional[float] = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> accessapproval.AccessApprovalSettings:
         r"""Updates the settings associated with a project, folder, or
         organization. Settings to update are determined by the value of
         field_mask.
 
         .. code-block:: python
@@ -1235,15 +1236,15 @@
         self,
         request: Optional[
             Union[accessapproval.DeleteAccessApprovalSettingsMessage, dict]
         ] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Optional[float] = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
         r"""Deletes the settings associated with a project,
         folder, or organization. This will have the effect of
         disabling Access Approval for the project, folder, or
         organization, but only if all ancestors also have Access
         Approval disabled. If Access Approval is enabled at a
@@ -1335,15 +1336,15 @@
         self,
         request: Optional[
             Union[accessapproval.GetAccessApprovalServiceAccountMessage, dict]
         ] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Optional[float] = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> accessapproval.AccessApprovalServiceAccount:
         r"""Retrieves the service account that is used by Access
         Approval to access KMS keys for signing approved
         approval requests.
 
         .. code-block:: python
@@ -1452,18 +1453,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-access-approval",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("AccessApprovalClient",)
```

### Comparing `google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/services/access_approval/pagers.py` & `google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/services/access_approval/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/services/access_approval/transports/__init__.py` & `google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/services/access_approval/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/services/access_approval/transports/base.py` & `google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/services/access_approval/transports/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,26 +20,21 @@
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
-import pkg_resources
 
+from google.cloud.accessapproval_v1 import gapic_version as package_version
 from google.cloud.accessapproval_v1.types import accessapproval
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-access-approval",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class AccessApprovalTransport(abc.ABC):
     """Abstract transport class for AccessApproval."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
```

### Comparing `google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/services/access_approval/transports/grpc.py` & `google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/services/access_approval/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/services/access_approval/transports/grpc_asyncio.py` & `google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/services/access_approval/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/types/__init__.py` & `google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-access-approval-1.9.0/google/cloud/accessapproval_v1/types/accessapproval.py` & `google-cloud-access-approval-1.9.1/google/cloud/accessapproval_v1/types/accessapproval.py`

 * *Files identical despite different names*

### Comparing `google-cloud-access-approval-1.9.0/google_cloud_access_approval.egg-info/PKG-INFO` & `google-cloud-access-approval-1.9.1/google_cloud_access_approval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-access-approval
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Access Approval API client library
 Home-page: https://github.com/googleapis/python-access-approval
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-access-approval-1.9.0/google_cloud_access_approval.egg-info/SOURCES.txt` & `google-cloud-access-approval-1.9.1/google_cloud_access_approval.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.cfg
 setup.py
 google/cloud/accessapproval/__init__.py
 google/cloud/accessapproval/gapic_version.py
 google/cloud/accessapproval/py.typed
 google/cloud/accessapproval_v1/__init__.py
 google/cloud/accessapproval_v1/gapic_metadata.json
+google/cloud/accessapproval_v1/gapic_version.py
 google/cloud/accessapproval_v1/py.typed
 google/cloud/accessapproval_v1/services/__init__.py
 google/cloud/accessapproval_v1/services/access_approval/__init__.py
 google/cloud/accessapproval_v1/services/access_approval/async_client.py
 google/cloud/accessapproval_v1/services/access_approval/client.py
 google/cloud/accessapproval_v1/services/access_approval/pagers.py
 google/cloud/accessapproval_v1/services/access_approval/transports/__init__.py
```

### Comparing `google-cloud-access-approval-1.9.0/setup.py` & `google-cloud-access-approval-1.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 if version[0] == "0":
     release_status = "Development Status :: 4 - Beta"
 else:
     release_status = "Development Status :: 5 - Production/Stable"
 
 dependencies = [
-    "google-api-core[grpc] >= 1.33.2, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
+    "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
 url = "https://github.com/googleapis/python-access-approval"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `google-cloud-access-approval-1.9.0/tests/__init__.py` & `google-cloud-access-approval-1.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-access-approval-1.9.0/tests/unit/__init__.py` & `google-cloud-access-approval-1.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-access-approval-1.9.0/tests/unit/gapic/__init__.py` & `google-cloud-access-approval-1.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-access-approval-1.9.0/tests/unit/gapic/accessapproval_v1/__init__.py` & `google-cloud-access-approval-1.9.1/tests/unit/gapic/accessapproval_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-access-approval-1.9.0/tests/unit/gapic/accessapproval_v1/test_access_approval.py` & `google-cloud-access-approval-1.9.1/tests/unit/gapic/accessapproval_v1/test_access_approval.py`

 * *Files identical despite different names*

