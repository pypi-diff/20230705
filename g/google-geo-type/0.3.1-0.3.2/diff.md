# Comparing `tmp/google-geo-type-0.3.1.tar.gz` & `tmp/google-geo-type-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-geo-type-0.3.1.tar", last modified: Mon Jun  5 14:00:04 2023, max compression
+gzip compressed data, was "google-geo-type-0.3.2.tar", last modified: Wed Jul  5 15:56:58 2023, max compression
```

## Comparing `google-geo-type-0.3.1.tar` & `google-geo-type-0.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:04.655304 google-geo-type-0.3.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-05 13:56:51.000000 google-geo-type-0.3.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-06-05 13:56:51.000000 google-geo-type-0.3.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4425 2023-06-05 14:00:04.655304 google-geo-type-0.3.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3527 2023-06-05 13:56:51.000000 google-geo-type-0.3.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:04.651304 google-geo-type-0.3.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:04.651304 google-geo-type-0.3.1/google/geo/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:04.651304 google-geo-type-0.3.1/google/geo/type/
--rw-rw-r--   0 root         (0)     1003      768 2023-06-05 13:56:51.000000 google-geo-type-0.3.1/google/geo/type/__init__.py
--rw-rw-r--   0 root         (0)     1003      219 2023-06-05 13:56:51.000000 google-geo-type-0.3.1/google/geo/type/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-geo-type-0.3.1/google/geo/type/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       76 2023-06-05 13:56:51.000000 google-geo-type-0.3.1/google/geo/type/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:04.651304 google-geo-type-0.3.1/google/geo/type/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-geo-type-0.3.1/google/geo/type/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:04.651304 google-geo-type-0.3.1/google/geo/type/types/
--rw-rw-r--   0 root         (0)     1003      656 2023-06-05 13:56:51.000000 google-geo-type-0.3.1/google/geo/type/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2724 2023-06-05 13:56:51.000000 google-geo-type-0.3.1/google/geo/type/types/viewport.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:04.651304 google-geo-type-0.3.1/google_geo_type.egg-info/
--rw-r--r--   0 root         (0)     1003     4425 2023-06-05 14:00:04.000000 google-geo-type-0.3.1/google_geo_type.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003      685 2023-06-05 14:00:04.000000 google-geo-type-0.3.1/google_geo_type.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-05 14:00:04.000000 google-geo-type-0.3.1/google_geo_type.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       18 2023-06-05 14:00:04.000000 google-geo-type-0.3.1/google_geo_type.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-05 14:00:04.000000 google-geo-type-0.3.1/google_geo_type.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-06-05 14:00:04.000000 google-geo-type-0.3.1/google_geo_type.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-05 14:00:04.000000 google-geo-type-0.3.1/google_geo_type.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-06-05 14:00:04.655304 google-geo-type-0.3.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2909 2023-06-05 13:56:51.000000 google-geo-type-0.3.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:04.655304 google-geo-type-0.3.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-geo-type-0.3.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:04.655304 google-geo-type-0.3.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-geo-type-0.3.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:04.655304 google-geo-type-0.3.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-geo-type-0.3.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 14:00:04.655304 google-geo-type-0.3.1/tests/unit/gapic/type/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-geo-type-0.3.1/tests/unit/gapic/type/__init__.py
--rw-rw-r--   0 root         (0)     1003      775 2023-06-05 13:56:51.000000 google-geo-type-0.3.1/tests/unit/gapic/type/test_type.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:58.095459 google-geo-type-0.3.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-geo-type-0.3.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-geo-type-0.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4425 2023-07-05 15:56:58.095459 google-geo-type-0.3.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3527 2023-07-05 15:46:59.000000 google-geo-type-0.3.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:58.091459 google-geo-type-0.3.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:58.091459 google-geo-type-0.3.2/google/geo/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:58.095459 google-geo-type-0.3.2/google/geo/type/
+-rw-rw-r--   0 root         (0)     1003      768 2023-07-05 15:46:59.000000 google-geo-type-0.3.2/google/geo/type/__init__.py
+-rw-rw-r--   0 root         (0)     1003      219 2023-07-05 15:46:59.000000 google-geo-type-0.3.2/google/geo/type/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-geo-type-0.3.2/google/geo/type/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       76 2023-07-05 15:46:59.000000 google-geo-type-0.3.2/google/geo/type/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:58.095459 google-geo-type-0.3.2/google/geo/type/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-geo-type-0.3.2/google/geo/type/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:58.095459 google-geo-type-0.3.2/google/geo/type/types/
+-rw-rw-r--   0 root         (0)     1003      656 2023-07-05 15:46:59.000000 google-geo-type-0.3.2/google/geo/type/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2724 2023-07-05 15:46:59.000000 google-geo-type-0.3.2/google/geo/type/types/viewport.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:58.095459 google-geo-type-0.3.2/google_geo_type.egg-info/
+-rw-r--r--   0 root         (0)     1003     4425 2023-07-05 15:56:58.000000 google-geo-type-0.3.2/google_geo_type.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003      685 2023-07-05 15:56:58.000000 google-geo-type-0.3.2/google_geo_type.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:56:58.000000 google-geo-type-0.3.2/google_geo_type.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       18 2023-07-05 15:56:58.000000 google-geo-type-0.3.2/google_geo_type.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:56:58.000000 google-geo-type-0.3.2/google_geo_type.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:56:58.000000 google-geo-type-0.3.2/google_geo_type.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:56:58.000000 google-geo-type-0.3.2/google_geo_type.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:56:58.095459 google-geo-type-0.3.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2909 2023-07-05 15:46:59.000000 google-geo-type-0.3.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:58.095459 google-geo-type-0.3.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-geo-type-0.3.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:58.095459 google-geo-type-0.3.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-geo-type-0.3.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:58.095459 google-geo-type-0.3.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-geo-type-0.3.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:58.095459 google-geo-type-0.3.2/tests/unit/gapic/type/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-geo-type-0.3.2/tests/unit/gapic/type/__init__.py
+-rw-rw-r--   0 root         (0)     1003      775 2023-07-05 15:46:59.000000 google-geo-type-0.3.2/tests/unit/gapic/type/test_type.py
```

### Comparing `google-geo-type-0.3.1/LICENSE` & `google-geo-type-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-geo-type-0.3.1/MANIFEST.in` & `google-geo-type-0.3.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-geo-type-0.3.1/PKG-INFO` & `google-geo-type-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-geo-type
-Version: 0.3.1
+Version: 0.3.2
 Summary: Google Geo Type API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-geo-type-0.3.1/README.rst` & `google-geo-type-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `google-geo-type-0.3.1/google/geo/type/__init__.py` & `google-geo-type-0.3.2/google/geo/type/__init__.py`

 * *Files identical despite different names*

### Comparing `google-geo-type-0.3.1/google/geo/type/gapic_version.py` & `google-geo-type-0.3.2/google/geo/type/gapic_version.py`

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
-__version__ = "0.3.1"  # {x-release-please-version}
+__version__ = "0.3.2"  # {x-release-please-version}
```

### Comparing `google-geo-type-0.3.1/google/geo/type/services/__init__.py` & `google-geo-type-0.3.2/google/geo/type/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-geo-type-0.3.1/google/geo/type/types/__init__.py` & `google-geo-type-0.3.2/google/geo/type/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-geo-type-0.3.1/google/geo/type/types/viewport.py` & `google-geo-type-0.3.2/google/geo/type/types/viewport.py`

 * *Files identical despite different names*

### Comparing `google-geo-type-0.3.1/google_geo_type.egg-info/PKG-INFO` & `google-geo-type-0.3.2/google_geo_type.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-geo-type
-Version: 0.3.1
+Version: 0.3.2
 Summary: Google Geo Type API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-geo-type-0.3.1/google_geo_type.egg-info/SOURCES.txt` & `google-geo-type-0.3.2/google_geo_type.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-geo-type-0.3.1/setup.py` & `google-geo-type-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `google-geo-type-0.3.1/tests/__init__.py` & `google-geo-type-0.3.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-geo-type-0.3.1/tests/unit/__init__.py` & `google-geo-type-0.3.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-geo-type-0.3.1/tests/unit/gapic/__init__.py` & `google-geo-type-0.3.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-geo-type-0.3.1/tests/unit/gapic/type/__init__.py` & `google-geo-type-0.3.2/tests/unit/gapic/type/__init__.py`

 * *Files identical despite different names*

### Comparing `google-geo-type-0.3.1/tests/unit/gapic/type/test_type.py` & `google-geo-type-0.3.2/tests/unit/gapic/type/test_type.py`

 * *Files identical despite different names*

