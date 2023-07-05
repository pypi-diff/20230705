# Comparing `tmp/google-area120-tables-0.8.2.tar.gz` & `tmp/google-area120-tables-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-area120-tables-0.8.2.tar", last modified: Mon Oct 10 18:21:15 2022, max compression
+gzip compressed data, was "google-area120-tables-0.9.0.tar", last modified: Tue Nov  8 20:31:25 2022, max compression
```

## Comparing `google-area120-tables-0.8.2.tar` & `google-area120-tables-0.9.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:21:15.360624 google-area120-tables-0.8.2/
--rw-rw-r--   0 root         (0)     1003    11358 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4317 2022-10-10 18:21:15.360624 google-area120-tables-0.8.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3586 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:21:15.352621 google-area120-tables-0.8.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:21:15.352621 google-area120-tables-0.8.2/google/area120/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:21:15.356623 google-area120-tables-0.8.2/google/area120/tables/
--rw-rw-r--   0 root         (0)     1003     2096 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/google/area120/tables/__init__.py
--rw-rw-r--   0 root         (0)     1003       82 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/google/area120/tables/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:21:15.356623 google-area120-tables-0.8.2/google/area120/tables_v1alpha1/
--rw-rw-r--   0 root         (0)     1003     1932 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/google/area120/tables_v1alpha1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4911 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/google/area120/tables_v1alpha1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       82 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/google/area120/tables_v1alpha1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:21:15.356623 google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:21:15.356623 google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/tables_service/
--rw-rw-r--   0 root         (0)     1003      765 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/tables_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    53247 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/tables_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    64576 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/tables_service/client.py
--rw-rw-r--   0 root         (0)     1003    15452 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/tables_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:21:15.360624 google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/tables_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/tables_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10877 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/tables_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    23694 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/tables_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    24240 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/tables_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    62935 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/tables_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:21:15.360624 google-area120-tables-0.8.2/google/area120/tables_v1alpha1/types/
--rw-rw-r--   0 root         (0)     1003     1783 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/google/area120/tables_v1alpha1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    18490 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/google/area120/tables_v1alpha1/types/tables.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:21:15.360624 google-area120-tables-0.8.2/google_area120_tables.egg-info/
--rw-r--r--   0 root         (0)     1003     4317 2022-10-10 18:21:15.000000 google-area120-tables-0.8.2/google_area120_tables.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1539 2022-10-10 18:21:15.000000 google-area120-tables-0.8.2/google_area120_tables.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 18:21:15.000000 google-area120-tables-0.8.2/google_area120_tables.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       22 2022-10-10 18:21:15.000000 google-area120-tables-0.8.2/google_area120_tables.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 18:21:15.000000 google-area120-tables-0.8.2/google_area120_tables.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      232 2022-10-10 18:21:15.000000 google-area120-tables-0.8.2/google_area120_tables.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-10-10 18:21:15.000000 google-area120-tables-0.8.2/google_area120_tables.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2022-10-10 18:21:15.360624 google-area120-tables-0.8.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2231 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:21:15.360624 google-area120-tables-0.8.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:21:15.360624 google-area120-tables-0.8.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:21:15.360624 google-area120-tables-0.8.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:21:15.360624 google-area120-tables-0.8.2/tests/unit/gapic/tables_v1alpha1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/tests/unit/gapic/tables_v1alpha1/__init__.py
--rw-rw-r--   0 root         (0)     1003   253738 2022-10-10 18:17:38.000000 google-area120-tables-0.8.2/tests/unit/gapic/tables_v1alpha1/test_tables_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-08 20:31:25.274805 google-area120-tables-0.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4447 2022-11-08 20:31:25.274805 google-area120-tables-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3586 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-08 20:31:25.266806 google-area120-tables-0.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-08 20:31:25.266806 google-area120-tables-0.9.0/google/area120/
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-08 20:31:25.270805 google-area120-tables-0.9.0/google/area120/tables/
+-rw-rw-r--   0 root         (0)     1003     2207 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/google/area120/tables/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/google/area120/tables/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/google/area120/tables/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-08 20:31:25.270805 google-area120-tables-0.9.0/google/area120/tables_v1alpha1/
+-rw-rw-r--   0 root         (0)     1003     2043 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/google/area120/tables_v1alpha1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4911 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/google/area120/tables_v1alpha1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       82 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/google/area120/tables_v1alpha1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-08 20:31:25.270805 google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-08 20:31:25.270805 google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/tables_service/
+-rw-rw-r--   0 root         (0)     1003      765 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/tables_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    53247 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/tables_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    64698 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/tables_service/client.py
+-rw-rw-r--   0 root         (0)     1003    15452 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/tables_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-08 20:31:25.274805 google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/tables_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/tables_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10877 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/tables_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    23694 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/tables_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    24240 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/tables_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    62935 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/tables_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-08 20:31:25.274805 google-area120-tables-0.9.0/google/area120/tables_v1alpha1/types/
+-rw-rw-r--   0 root         (0)     1003     1783 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/google/area120/tables_v1alpha1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18490 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/google/area120/tables_v1alpha1/types/tables.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-08 20:31:25.274805 google-area120-tables-0.9.0/google_area120_tables.egg-info/
+-rw-r--r--   0 root         (0)     1003     4447 2022-11-08 20:31:25.000000 google-area120-tables-0.9.0/google_area120_tables.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1578 2022-11-08 20:31:25.000000 google-area120-tables-0.9.0/google_area120_tables.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-11-08 20:31:25.000000 google-area120-tables-0.9.0/google_area120_tables.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-11-08 20:31:25.000000 google-area120-tables-0.9.0/google_area120_tables.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-11-08 20:31:25.000000 google-area120-tables-0.9.0/google_area120_tables.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      232 2022-11-08 20:31:25.000000 google-area120-tables-0.9.0/google_area120_tables.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-11-08 20:31:25.000000 google-area120-tables-0.9.0/google_area120_tables.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2022-11-08 20:31:25.274805 google-area120-tables-0.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2846 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-08 20:31:25.274805 google-area120-tables-0.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-08 20:31:25.274805 google-area120-tables-0.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-08 20:31:25.274805 google-area120-tables-0.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-08 20:31:25.274805 google-area120-tables-0.9.0/tests/unit/gapic/tables_v1alpha1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/tests/unit/gapic/tables_v1alpha1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   253738 2022-11-08 20:27:57.000000 google-area120-tables-0.9.0/tests/unit/gapic/tables_v1alpha1/test_tables_service.py
```

### Comparing `google-area120-tables-0.8.2/LICENSE` & `google-area120-tables-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-area120-tables-0.8.2/MANIFEST.in` & `google-area120-tables-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-area120-tables-0.8.2/PKG-INFO` & `google-area120-tables-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: google-area120-tables
-Version: 0.8.2
+Version: 0.9.0
+Summary: Google Area120 Tables API client library
 Home-page: https://github.com/googleapis/python-area120-tables
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 License-File: LICENSE
 
 Python Client for Area 120 Tables API
 =====================================
 
 |preview| |pypi| |versions|
```

### Comparing `google-area120-tables-0.8.2/README.rst` & `google-area120-tables-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-area120-tables-0.8.2/google/area120/tables/__init__.py` & `google-area120-tables-0.9.0/google/area120/tables/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.area120.tables import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from google.area120.tables_v1alpha1.services.tables_service.async_client import (
     TablesServiceAsyncClient,
 )
 from google.area120.tables_v1alpha1.services.tables_service.client import (
     TablesServiceClient,
 )
```

### Comparing `google-area120-tables-0.8.2/google/area120/tables_v1alpha1/__init__.py` & `google-area120-tables-0.9.0/google/area120/tables_v1alpha1/types/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-from .services.tables_service import TablesServiceAsyncClient, TablesServiceClient
-from .types.tables import (
+from .tables import (
     BatchCreateRowsRequest,
     BatchCreateRowsResponse,
     BatchDeleteRowsRequest,
     BatchUpdateRowsRequest,
     BatchUpdateRowsResponse,
     ColumnDescription,
     CreateRowRequest,
@@ -40,15 +38,14 @@
     Table,
     UpdateRowRequest,
     View,
     Workspace,
 )
 
 __all__ = (
-    "TablesServiceAsyncClient",
     "BatchCreateRowsRequest",
     "BatchCreateRowsResponse",
     "BatchDeleteRowsRequest",
     "BatchUpdateRowsRequest",
     "BatchUpdateRowsResponse",
     "ColumnDescription",
     "CreateRowRequest",
@@ -63,12 +60,11 @@
     "ListTablesResponse",
     "ListWorkspacesRequest",
     "ListWorkspacesResponse",
     "LookupDetails",
     "RelationshipDetails",
     "Row",
     "Table",
-    "TablesServiceClient",
     "UpdateRowRequest",
-    "View",
     "Workspace",
+    "View",
 )
```

### Comparing `google-area120-tables-0.8.2/google/area120/tables_v1alpha1/gapic_metadata.json` & `google-area120-tables-0.9.0/google/area120/tables_v1alpha1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/__init__.py` & `google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/tables_service/__init__.py` & `google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/tables_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/tables_service/async_client.py` & `google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/tables_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/tables_service/client.py` & `google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/tables_service/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union, cast
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
@@ -371,15 +371,15 @@
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, TablesServiceTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the tables service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -388,15 +388,15 @@
                 credentials from the environment.
             transport (Union[str, TablesServiceTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
                 NOTE: "rest" transport functionality is currently in a
                 beta state (preview). We welcome your feedback via an
                 issue in this library's source repository.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -418,14 +418,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
```

### Comparing `google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/tables_service/pagers.py` & `google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/tables_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/tables_service/transports/__init__.py` & `google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/tables_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/tables_service/transports/base.py` & `google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/tables_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/tables_service/transports/grpc.py` & `google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/tables_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/tables_service/transports/grpc_asyncio.py` & `google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/tables_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-area120-tables-0.8.2/google/area120/tables_v1alpha1/services/tables_service/transports/rest.py` & `google-area120-tables-0.9.0/google/area120/tables_v1alpha1/services/tables_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-area120-tables-0.8.2/google/area120/tables_v1alpha1/types/__init__.py` & `google-area120-tables-0.9.0/google/area120/tables_v1alpha1/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from .tables import (
+from google.area120.tables import gapic_version as package_version
+
+__version__ = package_version.__version__
+
+
+from .services.tables_service import TablesServiceAsyncClient, TablesServiceClient
+from .types.tables import (
     BatchCreateRowsRequest,
     BatchCreateRowsResponse,
     BatchDeleteRowsRequest,
     BatchUpdateRowsRequest,
     BatchUpdateRowsResponse,
     ColumnDescription,
     CreateRowRequest,
@@ -38,14 +44,15 @@
     Table,
     UpdateRowRequest,
     View,
     Workspace,
 )
 
 __all__ = (
+    "TablesServiceAsyncClient",
     "BatchCreateRowsRequest",
     "BatchCreateRowsResponse",
     "BatchDeleteRowsRequest",
     "BatchUpdateRowsRequest",
     "BatchUpdateRowsResponse",
     "ColumnDescription",
     "CreateRowRequest",
@@ -60,11 +67,12 @@
     "ListTablesResponse",
     "ListWorkspacesRequest",
     "ListWorkspacesResponse",
     "LookupDetails",
     "RelationshipDetails",
     "Row",
     "Table",
+    "TablesServiceClient",
     "UpdateRowRequest",
-    "Workspace",
     "View",
+    "Workspace",
 )
```

### Comparing `google-area120-tables-0.8.2/google/area120/tables_v1alpha1/types/tables.py` & `google-area120-tables-0.9.0/google/area120/tables_v1alpha1/types/tables.py`

 * *Files identical despite different names*

### Comparing `google-area120-tables-0.8.2/google_area120_tables.egg-info/PKG-INFO` & `google-area120-tables-0.9.0/google_area120_tables.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: google-area120-tables
-Version: 0.8.2
+Version: 0.9.0
+Summary: Google Area120 Tables API client library
 Home-page: https://github.com/googleapis/python-area120-tables
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 License-File: LICENSE
 
 Python Client for Area 120 Tables API
 =====================================
 
 |preview| |pypi| |versions|
```

### Comparing `google-area120-tables-0.8.2/google_area120_tables.egg-info/SOURCES.txt` & `google-area120-tables-0.9.0/google_area120_tables.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 google/area120/tables/__init__.py
+google/area120/tables/gapic_version.py
 google/area120/tables/py.typed
 google/area120/tables_v1alpha1/__init__.py
 google/area120/tables_v1alpha1/gapic_metadata.json
 google/area120/tables_v1alpha1/py.typed
 google/area120/tables_v1alpha1/services/__init__.py
 google/area120/tables_v1alpha1/services/tables_service/__init__.py
 google/area120/tables_v1alpha1/services/tables_service/async_client.py
```

### Comparing `google-area120-tables-0.8.2/setup.py` & `google-area120-tables-0.9.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,90 @@
 # -*- coding: utf-8 -*-
-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
 import io
 import os
 
 import setuptools  # type: ignore
 
-version = "0.8.2"
+package_root = os.path.abspath(os.path.dirname(__file__))
+
+name = "google-area120-tables"
+
+
+description = "Google Area120 Tables API client library"
+
+version = {}
+with open(os.path.join(package_root, "google/area120/tables/gapic_version.py")) as fp:
+    exec(fp.read(), version)
+version = version["__version__"]
+
+if version[0] == "0":
+    release_status = "Development Status :: 4 - Beta"
+else:
+    release_status = "Development Status :: 5 - Production/Stable"
+
+dependencies = [
+    "google-api-core[grpc] >= 1.33.2, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
+    "proto-plus >= 1.22.0, <2.0.0dev",
+    "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
+]
+url = "https://github.com/googleapis/python-area120-tables"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
+packages = [
+    package
+    for package in setuptools.PEP420PackageFinder.find()
+    if package.startswith("google")
+]
+
+namespaces = ["google"]
+if "google.cloud" in packages:
+    namespaces.append("google.cloud")
 
 setuptools.setup(
-    name="google-area120-tables",
+    name=name,
     version=version,
+    description=description,
     long_description=readme,
     author="Google LLC",
     author_email="googleapis-packages@google.com",
     license="Apache 2.0",
-    url="https://github.com/googleapis/python-area120-tables",
-    packages=[
-        package
-        for package in setuptools.PEP420PackageFinder.find()
-        if package.startswith("google")
-    ],
-    namespace_packages=("google", "google.area120"),
-    platforms="Posix; MacOS X; Windows",
-    include_package_data=True,
-    install_requires=(
-        "google-api-core[grpc] >= 1.33.2, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
-        "proto-plus >= 1.22.0, <2.0.0dev",
-        "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
-    ),
-    python_requires=">=3.7",
+    url=url,
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        release_status,
         "Intended Audience :: Developers",
-        "Operating System :: OS Independent",
+        "License :: OSI Approved :: Apache Software License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Operating System :: OS Independent",
         "Topic :: Internet",
-        "Topic :: Software Development :: Libraries :: Python Modules",
     ],
+    platforms="Posix; MacOS X; Windows",
+    packages=packages,
+    python_requires=">=3.7",
+    namespace_packages=namespaces,
+    install_requires=dependencies,
+    include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `google-area120-tables-0.8.2/tests/__init__.py` & `google-area120-tables-0.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-area120-tables-0.8.2/tests/unit/__init__.py` & `google-area120-tables-0.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-area120-tables-0.8.2/tests/unit/gapic/__init__.py` & `google-area120-tables-0.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-area120-tables-0.8.2/tests/unit/gapic/tables_v1alpha1/__init__.py` & `google-area120-tables-0.9.0/tests/unit/gapic/tables_v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-area120-tables-0.8.2/tests/unit/gapic/tables_v1alpha1/test_tables_service.py` & `google-area120-tables-0.9.0/tests/unit/gapic/tables_v1alpha1/test_tables_service.py`

 * *Files identical despite different names*

