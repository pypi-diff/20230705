# Comparing `tmp/google-cloud-essential-contacts-1.5.2.tar.gz` & `tmp/google-cloud-essential-contacts-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-essential-contacts-1.5.2.tar", last modified: Thu Jun 22 18:46:26 2023, max compression
+gzip compressed data, was "google-cloud-essential-contacts-1.5.3.tar", last modified: Wed Jul  5 15:53:01 2023, max compression
```

## Comparing `google-cloud-essential-contacts-1.5.2.tar` & `google-cloud-essential-contacts-1.5.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.909608 google-cloud-essential-contacts-1.5.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4863 2023-06-22 18:46:26.909608 google-cloud-essential-contacts-1.5.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3920 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.897609 google-cloud-essential-contacts-1.5.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.897609 google-cloud-essential-contacts-1.5.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.901608 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts/
--rw-rw-r--   0 root         (0)     1003     1835 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       92 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.901608 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/
--rw-rw-r--   0 root         (0)     1003     1616 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3282 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       92 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.901608 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.905608 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/
--rw-rw-r--   0 root         (0)     1003      809 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    39816 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    48954 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/client.py
--rw-rw-r--   0 root         (0)     1003    10815 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.905608 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/
--rw-rw-r--   0 root         (0)     1003     1561 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9298 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18645 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19035 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    42857 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.905608 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/types/
--rw-rw-r--   0 root         (0)     1003     1211 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3467 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/types/enums.py
--rw-rw-r--   0 root         (0)     1003    12529 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.905608 google-cloud-essential-contacts-1.5.2/google_cloud_essential_contacts.egg-info/
--rw-r--r--   0 root         (0)     1003     4863 2023-06-22 18:46:26.000000 google-cloud-essential-contacts-1.5.2/google_cloud_essential_contacts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1973 2023-06-22 18:46:26.000000 google-cloud-essential-contacts-1.5.2/google_cloud_essential_contacts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-22 18:46:26.000000 google-cloud-essential-contacts-1.5.2/google_cloud_essential_contacts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-06-22 18:46:26.000000 google-cloud-essential-contacts-1.5.2/google_cloud_essential_contacts.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-22 18:46:26.000000 google-cloud-essential-contacts-1.5.2/google_cloud_essential_contacts.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-06-22 18:46:26.000000 google-cloud-essential-contacts-1.5.2/google_cloud_essential_contacts.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-22 18:46:26.000000 google-cloud-essential-contacts-1.5.2/google_cloud_essential_contacts.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-06-22 18:46:26.909608 google-cloud-essential-contacts-1.5.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2965 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.905608 google-cloud-essential-contacts-1.5.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.905608 google-cloud-essential-contacts-1.5.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.909608 google-cloud-essential-contacts-1.5.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.909608 google-cloud-essential-contacts-1.5.2/tests/unit/gapic/essential_contacts_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/tests/unit/gapic/essential_contacts_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   193125 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/tests/unit/gapic/essential_contacts_v1/test_essential_contacts_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:01.617357 google-cloud-essential-contacts-1.5.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4863 2023-07-05 15:53:01.617357 google-cloud-essential-contacts-1.5.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3920 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:01.609357 google-cloud-essential-contacts-1.5.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:01.609357 google-cloud-essential-contacts-1.5.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:01.613357 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts/
+-rw-rw-r--   0 root         (0)     1003     1835 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       92 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:01.613357 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/
+-rw-rw-r--   0 root         (0)     1003     1616 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3282 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       92 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:01.613357 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:01.613357 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/essential_contacts_service/
+-rw-rw-r--   0 root         (0)     1003      809 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/essential_contacts_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    39857 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/essential_contacts_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    48954 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/essential_contacts_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10815 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/essential_contacts_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:01.617357 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1561 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9298 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18645 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19035 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    42857 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:01.617357 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1211 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3467 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/types/enums.py
+-rw-rw-r--   0 root         (0)     1003    12529 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:01.617357 google-cloud-essential-contacts-1.5.3/google_cloud_essential_contacts.egg-info/
+-rw-r--r--   0 root         (0)     1003     4863 2023-07-05 15:53:01.000000 google-cloud-essential-contacts-1.5.3/google_cloud_essential_contacts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1973 2023-07-05 15:53:01.000000 google-cloud-essential-contacts-1.5.3/google_cloud_essential_contacts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:01.000000 google-cloud-essential-contacts-1.5.3/google_cloud_essential_contacts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:53:01.000000 google-cloud-essential-contacts-1.5.3/google_cloud_essential_contacts.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:01.000000 google-cloud-essential-contacts-1.5.3/google_cloud_essential_contacts.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:53:01.000000 google-cloud-essential-contacts-1.5.3/google_cloud_essential_contacts.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:53:01.000000 google-cloud-essential-contacts-1.5.3/google_cloud_essential_contacts.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:53:01.617357 google-cloud-essential-contacts-1.5.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2965 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:01.617357 google-cloud-essential-contacts-1.5.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:01.617357 google-cloud-essential-contacts-1.5.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:01.617357 google-cloud-essential-contacts-1.5.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:01.617357 google-cloud-essential-contacts-1.5.3/tests/unit/gapic/essential_contacts_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/tests/unit/gapic/essential_contacts_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   193523 2023-07-05 15:46:58.000000 google-cloud-essential-contacts-1.5.3/tests/unit/gapic/essential_contacts_v1/test_essential_contacts_service.py
```

### Comparing `google-cloud-essential-contacts-1.5.2/LICENSE` & `google-cloud-essential-contacts-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/MANIFEST.in` & `google-cloud-essential-contacts-1.5.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/PKG-INFO` & `google-cloud-essential-contacts-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-essential-contacts
-Version: 1.5.2
+Version: 1.5.3
 Summary: Google Cloud Essential Contacts API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-essential-contacts-1.5.2/README.rst` & `google-cloud-essential-contacts-1.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts/__init__.py` & `google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts/gapic_version.py` & `google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts/gapic_version.py`

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
-__version__ = "1.5.2"  # {x-release-please-version}
+__version__ = "1.5.3"  # {x-release-please-version}
```

### Comparing `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/__init__.py` & `google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/gapic_metadata.json` & `google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/gapic_version.py` & `google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/gapic_version.py`

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
-__version__ = "1.5.2"  # {x-release-please-version}
+__version__ = "1.5.3"  # {x-release-please-version}
```

### Comparing `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/__init__.py` & `google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/__init__.py` & `google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/essential_contacts_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/async_client.py` & `google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/essential_contacts_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -959,15 +959,15 @@
         await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "EssentialContactsServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/client.py` & `google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/essential_contacts_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/pagers.py` & `google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/essential_contacts_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/__init__.py` & `google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/base.py` & `google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/grpc.py` & `google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/grpc_asyncio.py` & `google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/rest.py` & `google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/types/__init__.py` & `google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/types/enums.py` & `google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/types/enums.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/types/service.py` & `google-cloud-essential-contacts-1.5.3/google/cloud/essential_contacts_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/google_cloud_essential_contacts.egg-info/PKG-INFO` & `google-cloud-essential-contacts-1.5.3/google_cloud_essential_contacts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-essential-contacts
-Version: 1.5.2
+Version: 1.5.3
 Summary: Google Cloud Essential Contacts API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-essential-contacts-1.5.2/google_cloud_essential_contacts.egg-info/SOURCES.txt` & `google-cloud-essential-contacts-1.5.3/google_cloud_essential_contacts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/setup.py` & `google-cloud-essential-contacts-1.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/tests/__init__.py` & `google-cloud-essential-contacts-1.5.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/tests/unit/__init__.py` & `google-cloud-essential-contacts-1.5.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/tests/unit/gapic/__init__.py` & `google-cloud-essential-contacts-1.5.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/tests/unit/gapic/essential_contacts_v1/__init__.py` & `google-cloud-essential-contacts-1.5.3/tests/unit/gapic/essential_contacts_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.2/tests/unit/gapic/essential_contacts_v1/test_essential_contacts_service.py` & `google-cloud-essential-contacts-1.5.3/tests/unit/gapic/essential_contacts_v1/test_essential_contacts_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1681,17 +1681,19 @@
                     service.Contact(),
                     service.Contact(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_contacts(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2487,17 +2489,19 @@
                     service.Contact(),
                     service.Contact(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.compute_contacts(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

