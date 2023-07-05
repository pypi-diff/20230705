# Comparing `tmp/google-cloud-core-2.3.2.tar.gz` & `tmp/google-cloud-core-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-core-2.3.2.tar", last modified: Mon Jul 18 13:18:43 2022, max compression
+gzip compressed data, was "google-cloud-core-2.3.3.tar", last modified: Wed Jul  5 19:44:31 2023, max compression
```

## Comparing `google-cloud-core-2.3.2.tar` & `google-cloud-core-2.3.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-07-18 13:18:43.690238 google-cloud-core-2.3.2/
--rw-rw-r--   0 root         (0)     1003    11358 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     2289 2022-07-18 13:18:43.690238 google-cloud-core-2.3.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     1406 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-07-18 13:18:43.682238 google-cloud-core-2.3.2/google/
--rw-rw-r--   0 root         (0)     1003      796 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-07-18 13:18:43.686238 google-cloud-core-2.3.2/google/cloud/
--rw-rw-r--   0 root         (0)     1003      802 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/google/cloud/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-07-18 13:18:43.686238 google-cloud-core-2.3.2/google/cloud/_helpers/
--rw-rw-r--   0 root         (0)     1003    18628 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/google/cloud/_helpers/__init__.py
--rw-rw-r--   0 root         (0)     1003       63 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/google/cloud/_helpers/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-07-18 13:18:43.686238 google-cloud-core-2.3.2/google/cloud/_http/
--rw-rw-r--   0 root         (0)     1003    16649 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/google/cloud/_http/__init__.py
--rw-rw-r--   0 root         (0)     1003       63 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/google/cloud/_http/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-07-18 13:18:43.686238 google-cloud-core-2.3.2/google/cloud/_testing/
--rw-rw-r--   0 root         (0)     1003     3398 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/google/cloud/_testing/__init__.py
--rw-rw-r--   0 root         (0)     1003       63 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/google/cloud/_testing/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-07-18 13:18:43.686238 google-cloud-core-2.3.2/google/cloud/client/
--rw-rw-r--   0 root         (0)     1003    12266 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/google/cloud/client/__init__.py
--rw-rw-r--   0 root         (0)     1003       63 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/google/cloud/client/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-07-18 13:18:43.686238 google-cloud-core-2.3.2/google/cloud/environment_vars/
--rw-rw-r--   0 root         (0)     1003     1318 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/google/cloud/environment_vars/__init__.py
--rw-rw-r--   0 root         (0)     1003       63 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/google/cloud/environment_vars/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-07-18 13:18:43.686238 google-cloud-core-2.3.2/google/cloud/exceptions/
--rw-rw-r--   0 root         (0)     1003     2199 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/google/cloud/exceptions/__init__.py
--rw-rw-r--   0 root         (0)     1003       63 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/google/cloud/exceptions/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-07-18 13:18:43.686238 google-cloud-core-2.3.2/google/cloud/obsolete/
--rw-rw-r--   0 root         (0)     1003     1382 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/google/cloud/obsolete/__init__.py
--rw-rw-r--   0 root         (0)     1003       63 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/google/cloud/obsolete/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-07-18 13:18:43.686238 google-cloud-core-2.3.2/google/cloud/operation/
--rw-rw-r--   0 root         (0)     1003     9083 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/google/cloud/operation/__init__.py
--rw-rw-r--   0 root         (0)     1003       63 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/google/cloud/operation/py.typed
--rw-rw-r--   0 root         (0)     1003      597 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/google/cloud/version.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-07-18 13:18:43.686238 google-cloud-core-2.3.2/google_cloud_core.egg-info/
--rw-r--r--   0 root         (0)     1003     2289 2022-07-18 13:18:43.000000 google-cloud-core-2.3.2/google_cloud_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1120 2022-07-18 13:18:43.000000 google-cloud-core-2.3.2/google_cloud_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-07-18 13:18:43.000000 google-cloud-core-2.3.2/google_cloud_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-07-18 13:18:43.000000 google-cloud-core-2.3.2/google_cloud_core.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-07-18 13:18:43.000000 google-cloud-core-2.3.2/google_cloud_core.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      125 2022-07-18 13:18:43.000000 google-cloud-core-2.3.2/google_cloud_core.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-07-18 13:18:43.000000 google-cloud-core-2.3.2/google_cloud_core.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2022-07-18 13:18:43.690238 google-cloud-core-2.3.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2868 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-07-18 13:18:43.690238 google-cloud-core-2.3.2/tests/
--rw-rw-r--   0 root         (0)     1003        0 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-07-18 13:18:43.690238 google-cloud-core-2.3.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      574 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/tests/unit/__init__.py
--rw-rw-r--   0 root         (0)     1003    26852 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/tests/unit/test__helpers.py
--rw-rw-r--   0 root         (0)     1003    22015 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/tests/unit/test__http.py
--rw-rw-r--   0 root         (0)     1003    20386 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/tests/unit/test_client.py
--rw-rw-r--   0 root         (0)     1003     1034 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/tests/unit/test_obsolete.py
--rw-rw-r--   0 root         (0)     1003    14990 2022-07-18 13:16:03.000000 google-cloud-core-2.3.2/tests/unit/test_operation.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 19:44:31.220204 google-cloud-core-2.3.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     2289 2023-07-05 19:44:31.220204 google-cloud-core-2.3.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     1406 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 19:44:31.216204 google-cloud-core-2.3.3/google/
+-rw-rw-r--   0 root         (0)     1003      796 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 19:44:31.216204 google-cloud-core-2.3.3/google/cloud/
+-rw-rw-r--   0 root         (0)     1003      802 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/google/cloud/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 19:44:31.216204 google-cloud-core-2.3.3/google/cloud/_helpers/
+-rw-rw-r--   0 root         (0)     1003    18628 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/google/cloud/_helpers/__init__.py
+-rw-rw-r--   0 root         (0)     1003       63 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/google/cloud/_helpers/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 19:44:31.216204 google-cloud-core-2.3.3/google/cloud/_http/
+-rw-rw-r--   0 root         (0)     1003    16649 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/google/cloud/_http/__init__.py
+-rw-rw-r--   0 root         (0)     1003       63 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/google/cloud/_http/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 19:44:31.216204 google-cloud-core-2.3.3/google/cloud/_testing/
+-rw-rw-r--   0 root         (0)     1003     3398 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/google/cloud/_testing/__init__.py
+-rw-rw-r--   0 root         (0)     1003       63 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/google/cloud/_testing/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 19:44:31.216204 google-cloud-core-2.3.3/google/cloud/client/
+-rw-rw-r--   0 root         (0)     1003    12266 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/google/cloud/client/__init__.py
+-rw-rw-r--   0 root         (0)     1003       63 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/google/cloud/client/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 19:44:31.216204 google-cloud-core-2.3.3/google/cloud/environment_vars/
+-rw-rw-r--   0 root         (0)     1003     1318 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/google/cloud/environment_vars/__init__.py
+-rw-rw-r--   0 root         (0)     1003       63 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/google/cloud/environment_vars/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 19:44:31.216204 google-cloud-core-2.3.3/google/cloud/exceptions/
+-rw-rw-r--   0 root         (0)     1003     2199 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/google/cloud/exceptions/__init__.py
+-rw-rw-r--   0 root         (0)     1003       63 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/google/cloud/exceptions/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 19:44:31.216204 google-cloud-core-2.3.3/google/cloud/obsolete/
+-rw-rw-r--   0 root         (0)     1003     1382 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/google/cloud/obsolete/__init__.py
+-rw-rw-r--   0 root         (0)     1003       63 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/google/cloud/obsolete/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 19:44:31.220204 google-cloud-core-2.3.3/google/cloud/operation/
+-rw-rw-r--   0 root         (0)     1003     9083 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/google/cloud/operation/__init__.py
+-rw-rw-r--   0 root         (0)     1003       63 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/google/cloud/operation/py.typed
+-rw-rw-r--   0 root         (0)     1003      597 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/google/cloud/version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 19:44:31.220204 google-cloud-core-2.3.3/google_cloud_core.egg-info/
+-rw-r--r--   0 root         (0)     1003     2289 2023-07-05 19:44:31.000000 google-cloud-core-2.3.3/google_cloud_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1120 2023-07-05 19:44:31.000000 google-cloud-core-2.3.3/google_cloud_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 19:44:31.000000 google-cloud-core-2.3.3/google_cloud_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 19:44:31.000000 google-cloud-core-2.3.3/google_cloud_core.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 19:44:31.000000 google-cloud-core-2.3.3/google_cloud_core.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      125 2023-07-05 19:44:31.000000 google-cloud-core-2.3.3/google_cloud_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 19:44:31.000000 google-cloud-core-2.3.3/google_cloud_core.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 19:44:31.220204 google-cloud-core-2.3.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2868 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 19:44:31.220204 google-cloud-core-2.3.3/tests/
+-rw-rw-r--   0 root         (0)     1003        0 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 19:44:31.220204 google-cloud-core-2.3.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      574 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/tests/unit/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26852 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/tests/unit/test__helpers.py
+-rw-rw-r--   0 root         (0)     1003    22015 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/tests/unit/test__http.py
+-rw-rw-r--   0 root         (0)     1003    20386 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/tests/unit/test_client.py
+-rw-rw-r--   0 root         (0)     1003     1034 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/tests/unit/test_obsolete.py
+-rw-rw-r--   0 root         (0)     1003    14990 2023-07-05 19:41:57.000000 google-cloud-core-2.3.3/tests/unit/test_operation.py
```

### Comparing `google-cloud-core-2.3.2/LICENSE` & `google-cloud-core-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-core-2.3.2/MANIFEST.in` & `google-cloud-core-2.3.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-core-2.3.2/PKG-INFO` & `google-cloud-core-2.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-core
-Version: 2.3.2
+Version: 2.3.3
 Summary: Google Cloud API client core library
 Home-page: https://github.com/googleapis/python-cloud-core
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-core-2.3.2/README.rst` & `google-cloud-core-2.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-core-2.3.2/google/__init__.py` & `google-cloud-core-2.3.3/google/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-core-2.3.2/google/cloud/__init__.py` & `google-cloud-core-2.3.3/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-core-2.3.2/google/cloud/_helpers/__init__.py` & `google-cloud-core-2.3.3/google/cloud/_helpers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             return self._stack[-1]
 
 
 def _ensure_tuple_or_list(arg_name, tuple_or_list):
     """Ensures an input is a tuple or list.
 
     This effectively reduces the iterable types allowed to a very short
-    whitelist: list and tuple.
+    allowlist: list and tuple.
 
     :type arg_name: str
     :param arg_name: Name of argument to use in error message.
 
     :type tuple_or_list: sequence of str
     :param tuple_or_list: Sequence to be verified.
```

### Comparing `google-cloud-core-2.3.2/google/cloud/_http/__init__.py` & `google-cloud-core-2.3.3/google/cloud/_http/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-core-2.3.2/google/cloud/_testing/__init__.py` & `google-cloud-core-2.3.3/google/cloud/_testing/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-core-2.3.2/google/cloud/client/__init__.py` & `google-cloud-core-2.3.3/google/cloud/client/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-core-2.3.2/google/cloud/environment_vars/__init__.py` & `google-cloud-core-2.3.3/google/cloud/environment_vars/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-core-2.3.2/google/cloud/exceptions/__init__.py` & `google-cloud-core-2.3.3/google/cloud/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-core-2.3.2/google/cloud/obsolete/__init__.py` & `google-cloud-core-2.3.3/google/cloud/obsolete/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-core-2.3.2/google/cloud/operation/__init__.py` & `google-cloud-core-2.3.3/google/cloud/operation/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-core-2.3.2/google/cloud/version.py` & `google-cloud-core-2.3.3/google/cloud/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "2.3.2"
+__version__ = "2.3.3"
```

### Comparing `google-cloud-core-2.3.2/google_cloud_core.egg-info/PKG-INFO` & `google-cloud-core-2.3.3/google_cloud_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-core
-Version: 2.3.2
+Version: 2.3.3
 Summary: Google Cloud API client core library
 Home-page: https://github.com/googleapis/python-cloud-core
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-core-2.3.2/google_cloud_core.egg-info/SOURCES.txt` & `google-cloud-core-2.3.3/google_cloud_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-core-2.3.2/setup.py` & `google-cloud-core-2.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-core-2.3.2/tests/unit/__init__.py` & `google-cloud-core-2.3.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-core-2.3.2/tests/unit/test__helpers.py` & `google-cloud-core-2.3.3/tests/unit/test__helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-core-2.3.2/tests/unit/test__http.py` & `google-cloud-core-2.3.3/tests/unit/test__http.py`

 * *Files identical despite different names*

### Comparing `google-cloud-core-2.3.2/tests/unit/test_client.py` & `google-cloud-core-2.3.3/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-core-2.3.2/tests/unit/test_obsolete.py` & `google-cloud-core-2.3.3/tests/unit/test_obsolete.py`

 * *Files identical despite different names*

### Comparing `google-cloud-core-2.3.2/tests/unit/test_operation.py` & `google-cloud-core-2.3.3/tests/unit/test_operation.py`

 * *Files identical despite different names*

