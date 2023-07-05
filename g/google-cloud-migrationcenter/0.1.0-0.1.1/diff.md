# Comparing `tmp/google-cloud-migrationcenter-0.1.0.tar.gz` & `tmp/google-cloud-migrationcenter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-migrationcenter-0.1.0.tar", last modified: Thu Jun  8 15:08:45 2023, max compression
+gzip compressed data, was "google-cloud-migrationcenter-0.1.1.tar", last modified: Wed Jul  5 15:54:01 2023, max compression
```

## Comparing `google-cloud-migrationcenter-0.1.0.tar` & `google-cloud-migrationcenter-0.1.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-08 15:08:45.447062 google-cloud-migrationcenter-0.1.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4850 2023-06-08 15:08:45.447062 google-cloud-migrationcenter-0.1.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3926 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-08 15:08:45.435061 google-cloud-migrationcenter-0.1.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-08 15:08:45.435061 google-cloud-migrationcenter-0.1.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-08 15:08:45.439061 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter/
--rw-rw-r--   0 root         (0)     1003     8694 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-08 15:08:45.439061 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/
--rw-rw-r--   0 root         (0)     1003     8528 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    18730 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-08 15:08:45.439061 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-08 15:08:45.439061 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/migration_center/
--rw-rw-r--   0 root         (0)     1003      773 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/migration_center/__init__.py
--rw-rw-r--   0 root         (0)     1003   249524 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/migration_center/async_client.py
--rw-rw-r--   0 root         (0)     1003   271057 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/migration_center/client.py
--rw-rw-r--   0 root         (0)     1003    46806 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/migration_center/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-08 15:08:45.443062 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/migration_center/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/migration_center/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    29310 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/migration_center/transports/base.py
--rw-rw-r--   0 root         (0)     1003    71273 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/migration_center/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    72992 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/migration_center/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   277475 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/migration_center/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-08 15:08:45.443062 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/types/
--rw-rw-r--   0 root         (0)     1003     8248 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003   198273 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/types/migrationcenter.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-08 15:08:45.443062 google-cloud-migrationcenter-0.1.0/google_cloud_migrationcenter.egg-info/
--rw-r--r--   0 root         (0)     1003     4850 2023-06-08 15:08:45.000000 google-cloud-migrationcenter-0.1.0/google_cloud_migrationcenter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1737 2023-06-08 15:08:45.000000 google-cloud-migrationcenter-0.1.0/google_cloud_migrationcenter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-08 15:08:45.000000 google-cloud-migrationcenter-0.1.0/google_cloud_migrationcenter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-06-08 15:08:45.000000 google-cloud-migrationcenter-0.1.0/google_cloud_migrationcenter.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-08 15:08:45.000000 google-cloud-migrationcenter-0.1.0/google_cloud_migrationcenter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-06-08 15:08:45.000000 google-cloud-migrationcenter-0.1.0/google_cloud_migrationcenter.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-08 15:08:45.000000 google-cloud-migrationcenter-0.1.0/google_cloud_migrationcenter.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-06-08 15:08:45.447062 google-cloud-migrationcenter-0.1.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2956 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-08 15:08:45.443062 google-cloud-migrationcenter-0.1.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-08 15:08:45.443062 google-cloud-migrationcenter-0.1.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-08 15:08:45.443062 google-cloud-migrationcenter-0.1.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-08 15:08:45.443062 google-cloud-migrationcenter-0.1.0/tests/unit/gapic/migrationcenter_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/tests/unit/gapic/migrationcenter_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003  1152016 2023-06-08 15:05:59.000000 google-cloud-migrationcenter-0.1.0/tests/unit/gapic/migrationcenter_v1/test_migration_center.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:01.208653 google-cloud-migrationcenter-0.1.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4850 2023-07-05 15:54:01.208653 google-cloud-migrationcenter-0.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3926 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:01.200653 google-cloud-migrationcenter-0.1.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:01.200653 google-cloud-migrationcenter-0.1.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:01.200653 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter/
+-rw-rw-r--   0 root         (0)     1003     8694 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:01.204653 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/
+-rw-rw-r--   0 root         (0)     1003     8528 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18730 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:01.204653 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:01.204653 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/migration_center/
+-rw-rw-r--   0 root         (0)     1003      773 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/migration_center/__init__.py
+-rw-rw-r--   0 root         (0)     1003   249556 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/migration_center/async_client.py
+-rw-rw-r--   0 root         (0)     1003   271057 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/migration_center/client.py
+-rw-rw-r--   0 root         (0)     1003    46806 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/migration_center/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:01.204653 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/migration_center/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/migration_center/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    29310 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/migration_center/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    71273 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/migration_center/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    72992 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/migration_center/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   277463 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/migration_center/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:01.204653 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/types/
+-rw-rw-r--   0 root         (0)     1003     8248 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003   198269 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/types/migrationcenter.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:01.208653 google-cloud-migrationcenter-0.1.1/google_cloud_migrationcenter.egg-info/
+-rw-r--r--   0 root         (0)     1003     4850 2023-07-05 15:54:01.000000 google-cloud-migrationcenter-0.1.1/google_cloud_migrationcenter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1737 2023-07-05 15:54:01.000000 google-cloud-migrationcenter-0.1.1/google_cloud_migrationcenter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:01.000000 google-cloud-migrationcenter-0.1.1/google_cloud_migrationcenter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:54:01.000000 google-cloud-migrationcenter-0.1.1/google_cloud_migrationcenter.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:01.000000 google-cloud-migrationcenter-0.1.1/google_cloud_migrationcenter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:54:01.000000 google-cloud-migrationcenter-0.1.1/google_cloud_migrationcenter.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:54:01.000000 google-cloud-migrationcenter-0.1.1/google_cloud_migrationcenter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:54:01.208653 google-cloud-migrationcenter-0.1.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2956 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:01.208653 google-cloud-migrationcenter-0.1.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:01.208653 google-cloud-migrationcenter-0.1.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:01.208653 google-cloud-migrationcenter-0.1.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:01.208653 google-cloud-migrationcenter-0.1.1/tests/unit/gapic/migrationcenter_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/tests/unit/gapic/migrationcenter_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003  1152811 2023-07-05 15:46:59.000000 google-cloud-migrationcenter-0.1.1/tests/unit/gapic/migrationcenter_v1/test_migration_center.py
```

### Comparing `google-cloud-migrationcenter-0.1.0/LICENSE` & `google-cloud-migrationcenter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-migrationcenter-0.1.0/MANIFEST.in` & `google-cloud-migrationcenter-0.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-migrationcenter-0.1.0/PKG-INFO` & `google-cloud-migrationcenter-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-migrationcenter
-Version: 0.1.0
+Version: 0.1.1
 Summary: Google Cloud Migrationcenter API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-migrationcenter-0.1.0/README.rst` & `google-cloud-migrationcenter-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter/__init__.py` & `google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter/gapic_version.py` & `google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter/gapic_version.py`

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
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.1.1"  # {x-release-please-version}
```

### Comparing `google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/__init__.py` & `google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/gapic_metadata.json` & `google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/gapic_version.py` & `google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/gapic_version.py`

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
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.1.1"  # {x-release-please-version}
```

### Comparing `google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/__init__.py` & `google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/migration_center/__init__.py` & `google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/migration_center/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/migration_center/async_client.py` & `google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/migration_center/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -6154,15 +6154,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "MigrationCenterAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/migration_center/client.py` & `google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/migration_center/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/migration_center/pagers.py` & `google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/migration_center/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/migration_center/transports/__init__.py` & `google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/migration_center/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/migration_center/transports/base.py` & `google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/migration_center/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/migration_center/transports/grpc.py` & `google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/migration_center/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/migration_center/transports/grpc_asyncio.py` & `google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/migration_center/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/services/migration_center/transports/rest.py` & `google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/services/migration_center/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -6866,15 +6866,15 @@
 
             request, metadata = self._interceptor.pre_cancel_operation(
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

### Comparing `google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/types/__init__.py` & `google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-migrationcenter-0.1.0/google/cloud/migrationcenter_v1/types/migrationcenter.py` & `google-cloud-migrationcenter-0.1.1/google/cloud/migrationcenter_v1/types/migrationcenter.py`

 * *Files 0% similar despite different names*

```diff
@@ -5463,15 +5463,15 @@
     Attributes:
         field (str):
             The name of the field on which to aggregate.
         count (google.cloud.migrationcenter_v1.types.Aggregation.Count):
             Count the number of matching objects.
 
             This field is a member of `oneof`_ ``aggregation_function``.
-        sum_ (google.cloud.migrationcenter_v1.types.Aggregation.Sum):
+        sum (google.cloud.migrationcenter_v1.types.Aggregation.Sum):
             Sum over a numeric field.
 
             This field is a member of `oneof`_ ``aggregation_function``.
         histogram (google.cloud.migrationcenter_v1.types.Aggregation.Histogram):
             Creates a bucketed histogram of field values.
 
             This field is a member of `oneof`_ ``aggregation_function``.
@@ -5517,15 +5517,15 @@
     )
     count: Count = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="aggregation_function",
         message=Count,
     )
-    sum_: Sum = proto.Field(
+    sum: Sum = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="aggregation_function",
         message=Sum,
     )
     histogram: Histogram = proto.Field(
         proto.MESSAGE,
@@ -5553,15 +5553,15 @@
 
     Attributes:
         field (str):
 
         count (google.cloud.migrationcenter_v1.types.AggregationResult.Count):
 
             This field is a member of `oneof`_ ``result``.
-        sum_ (google.cloud.migrationcenter_v1.types.AggregationResult.Sum):
+        sum (google.cloud.migrationcenter_v1.types.AggregationResult.Sum):
 
             This field is a member of `oneof`_ ``result``.
         histogram (google.cloud.migrationcenter_v1.types.AggregationResult.Histogram):
 
             This field is a member of `oneof`_ ``result``.
         frequency (google.cloud.migrationcenter_v1.types.AggregationResult.Frequency):
 
@@ -5662,15 +5662,15 @@
     )
     count: Count = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="result",
         message=Count,
     )
-    sum_: Sum = proto.Field(
+    sum: Sum = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="result",
         message=Sum,
     )
     histogram: Histogram = proto.Field(
         proto.MESSAGE,
```

### Comparing `google-cloud-migrationcenter-0.1.0/google_cloud_migrationcenter.egg-info/PKG-INFO` & `google-cloud-migrationcenter-0.1.1/google_cloud_migrationcenter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-migrationcenter
-Version: 0.1.0
+Version: 0.1.1
 Summary: Google Cloud Migrationcenter API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-migrationcenter-0.1.0/google_cloud_migrationcenter.egg-info/SOURCES.txt` & `google-cloud-migrationcenter-0.1.1/google_cloud_migrationcenter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-migrationcenter-0.1.0/setup.py` & `google-cloud-migrationcenter-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-migrationcenter-0.1.0/tests/__init__.py` & `google-cloud-migrationcenter-0.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-migrationcenter-0.1.0/tests/unit/__init__.py` & `google-cloud-migrationcenter-0.1.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-migrationcenter-0.1.0/tests/unit/gapic/__init__.py` & `google-cloud-migrationcenter-0.1.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-migrationcenter-0.1.0/tests/unit/gapic/migrationcenter_v1/__init__.py` & `google-cloud-migrationcenter-0.1.1/tests/unit/gapic/migrationcenter_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-migrationcenter-0.1.0/tests/unit/gapic/migrationcenter_v1/test_migration_center.py` & `google-cloud-migrationcenter-0.1.1/tests/unit/gapic/migrationcenter_v1/test_migration_center.py`

 * *Files 0% similar despite different names*

```diff
@@ -1154,17 +1154,19 @@
                     migrationcenter.Asset(),
                     migrationcenter.Asset(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_assets(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1186,15 +1188,14 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_asset), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = migrationcenter.Asset(
             name="name_value",
             sources=["sources_value"],
             assigned_groups=["assigned_groups_value"],
-            machine_details=migrationcenter.MachineDetails(uuid="uuid_value"),
         )
         response = client.get_asset(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == migrationcenter.GetAssetRequest()
@@ -1427,15 +1428,14 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_asset), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = migrationcenter.Asset(
             name="name_value",
             sources=["sources_value"],
             assigned_groups=["assigned_groups_value"],
-            machine_details=migrationcenter.MachineDetails(uuid="uuid_value"),
         )
         response = client.update_asset(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == migrationcenter.UpdateAssetRequest()
@@ -3380,17 +3380,19 @@
                     migrationcenter.ImportJob(),
                     migrationcenter.ImportJob(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_import_jobs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3413,19 +3415,14 @@
     with mock.patch.object(type(client.transport.get_import_job), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = migrationcenter.ImportJob(
             name="name_value",
             display_name="display_name_value",
             state=migrationcenter.ImportJob.ImportJobState.IMPORT_JOB_STATE_PENDING,
             asset_source="asset_source_value",
-            validation_report=migrationcenter.ValidationReport(
-                file_validations=[
-                    migrationcenter.FileValidationReport(file_name="file_name_value")
-                ]
-            ),
         )
         response = client.get_import_job(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == migrationcenter.GetImportJobRequest()
@@ -4627,17 +4624,14 @@
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = migrationcenter.ImportDataFile(
             name="name_value",
             display_name="display_name_value",
             format_=migrationcenter.ImportJobFormat.IMPORT_JOB_FORMAT_RVTOOLS_XLSX,
             state=migrationcenter.ImportDataFile.State.CREATING,
-            upload_file_info=migrationcenter.UploadFileInfo(
-                signed_uri="signed_uri_value"
-            ),
         )
         response = client.get_import_data_file(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == migrationcenter.GetImportDataFileRequest()
@@ -5307,17 +5301,19 @@
                     migrationcenter.ImportDataFile(),
                     migrationcenter.ImportDataFile(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_import_data_files(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -6233,17 +6229,19 @@
                     migrationcenter.Group(),
                     migrationcenter.Group(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_groups(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -8109,17 +8107,19 @@
                     migrationcenter.ErrorFrame(),
                     migrationcenter.ErrorFrame(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_error_frames(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -8765,17 +8765,19 @@
                     migrationcenter.Source(),
                     migrationcenter.Source(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_sources(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -10184,17 +10186,19 @@
                     migrationcenter.PreferenceSet(),
                     migrationcenter.PreferenceSet(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_preference_sets(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -12626,17 +12630,19 @@
                     migrationcenter.ReportConfig(),
                     migrationcenter.ReportConfig(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_report_configs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -13785,17 +13791,19 @@
                     migrationcenter.Report(),
                     migrationcenter.Report(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_reports(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -14390,15 +14398,14 @@
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = migrationcenter.Asset(
             name="name_value",
             sources=["sources_value"],
             assigned_groups=["assigned_groups_value"],
-            machine_details=migrationcenter.MachineDetails(uuid="uuid_value"),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = migrationcenter.Asset.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -14921,15 +14928,14 @@
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = migrationcenter.Asset(
             name="name_value",
             sources=["sources_value"],
             assigned_groups=["assigned_groups_value"],
-            machine_details=migrationcenter.MachineDetails(uuid="uuid_value"),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = migrationcenter.Asset.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -17911,19 +17917,14 @@
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = migrationcenter.ImportJob(
             name="name_value",
             display_name="display_name_value",
             state=migrationcenter.ImportJob.ImportJobState.IMPORT_JOB_STATE_PENDING,
             asset_source="asset_source_value",
-            validation_report=migrationcenter.ValidationReport(
-                file_validations=[
-                    migrationcenter.FileValidationReport(file_name="file_name_value")
-                ]
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = migrationcenter.ImportJob.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -19368,17 +19369,14 @@
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = migrationcenter.ImportDataFile(
             name="name_value",
             display_name="display_name_value",
             format_=migrationcenter.ImportJobFormat.IMPORT_JOB_FORMAT_RVTOOLS_XLSX,
             state=migrationcenter.ImportDataFile.State.CREATING,
-            upload_file_info=migrationcenter.UploadFileInfo(
-                signed_uri="signed_uri_value"
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = migrationcenter.ImportDataFile.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

