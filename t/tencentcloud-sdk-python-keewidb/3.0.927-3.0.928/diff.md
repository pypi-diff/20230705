# Comparing `tmp/tencentcloud-sdk-python-keewidb-3.0.927.tar.gz` & `tmp/tencentcloud-sdk-python-keewidb-3.0.928.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-keewidb-3.0.927.tar", last modified: Tue Jul  4 00:24:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-keewidb-3.0.928.tar", last modified: Wed Jul  5 00:28:35 2023, max compression
```

## Comparing `tencentcloud-sdk-python-keewidb-3.0.927.tar` & `tencentcloud-sdk-python-keewidb-3.0.928.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:24:44.000000 tencentcloud-sdk-python-keewidb-3.0.927/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 00:24:44.000000 tencentcloud-sdk-python-keewidb-3.0.927/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-04 00:24:43.000000 tencentcloud-sdk-python-keewidb-3.0.927/setup.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-04 00:24:44.000000 tencentcloud-sdk-python-keewidb-3.0.927/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:24:44.000000 tencentcloud-sdk-python-keewidb-3.0.927/tencentcloud_sdk_python_keewidb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-04 00:24:44.000000 tencentcloud-sdk-python-keewidb-3.0.927/tencentcloud_sdk_python_keewidb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 00:24:44.000000 tencentcloud-sdk-python-keewidb-3.0.927/tencentcloud_sdk_python_keewidb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-04 00:24:44.000000 tencentcloud-sdk-python-keewidb-3.0.927/tencentcloud_sdk_python_keewidb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 00:24:44.000000 tencentcloud-sdk-python-keewidb-3.0.927/tencentcloud_sdk_python_keewidb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-04 00:24:43.000000 tencentcloud-sdk-python-keewidb-3.0.927/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:24:44.000000 tencentcloud-sdk-python-keewidb-3.0.927/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-04 00:24:43.000000 tencentcloud-sdk-python-keewidb-3.0.927/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:24:44.000000 tencentcloud-sdk-python-keewidb-3.0.927/tencentcloud/keewidb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:24:44.000000 tencentcloud-sdk-python-keewidb-3.0.927/tencentcloud/keewidb/v20220308/
--rw-r--r--   0 root         (0) root         (0)     5675 2023-07-04 00:24:43.000000 tencentcloud-sdk-python-keewidb-3.0.927/tencentcloud/keewidb/v20220308/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   137323 2023-07-04 00:24:43.000000 tencentcloud-sdk-python-keewidb-3.0.927/tencentcloud/keewidb/v20220308/models.py
--rw-r--r--   0 root         (0) root         (0)    37283 2023-07-04 00:24:43.000000 tencentcloud-sdk-python-keewidb-3.0.927/tencentcloud/keewidb/v20220308/keewidb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:24:43.000000 tencentcloud-sdk-python-keewidb-3.0.927/tencentcloud/keewidb/v20220308/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:24:43.000000 tencentcloud-sdk-python-keewidb-3.0.927/tencentcloud/keewidb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:28:35.000000 tencentcloud-sdk-python-keewidb-3.0.928/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-05 00:28:35.000000 tencentcloud-sdk-python-keewidb-3.0.928/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-05 00:28:35.000000 tencentcloud-sdk-python-keewidb-3.0.928/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-05 00:28:35.000000 tencentcloud-sdk-python-keewidb-3.0.928/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:28:35.000000 tencentcloud-sdk-python-keewidb-3.0.928/tencentcloud_sdk_python_keewidb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-05 00:28:35.000000 tencentcloud-sdk-python-keewidb-3.0.928/tencentcloud_sdk_python_keewidb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 00:28:35.000000 tencentcloud-sdk-python-keewidb-3.0.928/tencentcloud_sdk_python_keewidb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-05 00:28:35.000000 tencentcloud-sdk-python-keewidb-3.0.928/tencentcloud_sdk_python_keewidb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-05 00:28:35.000000 tencentcloud-sdk-python-keewidb-3.0.928/tencentcloud_sdk_python_keewidb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-05 00:28:35.000000 tencentcloud-sdk-python-keewidb-3.0.928/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:28:35.000000 tencentcloud-sdk-python-keewidb-3.0.928/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-05 00:28:35.000000 tencentcloud-sdk-python-keewidb-3.0.928/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:28:35.000000 tencentcloud-sdk-python-keewidb-3.0.928/tencentcloud/keewidb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:28:35.000000 tencentcloud-sdk-python-keewidb-3.0.928/tencentcloud/keewidb/v20220308/
+-rw-r--r--   0 root         (0) root         (0)     5675 2023-07-05 00:28:35.000000 tencentcloud-sdk-python-keewidb-3.0.928/tencentcloud/keewidb/v20220308/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   218455 2023-07-05 00:28:35.000000 tencentcloud-sdk-python-keewidb-3.0.928/tencentcloud/keewidb/v20220308/models.py
+-rw-r--r--   0 root         (0) root         (0)    37283 2023-07-05 00:28:35.000000 tencentcloud-sdk-python-keewidb-3.0.928/tencentcloud/keewidb/v20220308/keewidb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:28:35.000000 tencentcloud-sdk-python-keewidb-3.0.928/tencentcloud/keewidb/v20220308/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:28:35.000000 tencentcloud-sdk-python-keewidb-3.0.928/tencentcloud/keewidb/__init__.py
```

### Comparing `tencentcloud-sdk-python-keewidb-3.0.927/setup.py` & `tencentcloud-sdk-python-keewidb-3.0.928/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-keewidb-3.0.927/PKG-INFO` & `tencentcloud-sdk-python-keewidb-3.0.928/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-keewidb
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Keewidb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-keewidb-3.0.927/tencentcloud_sdk_python_keewidb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-keewidb-3.0.928/tencentcloud_sdk_python_keewidb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-keewidb
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Keewidb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-keewidb-3.0.927/README.rst` & `tencentcloud-sdk-python-keewidb-3.0.928/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-keewidb-3.0.927/tencentcloud/__init__.py` & `tencentcloud-sdk-python-keewidb-3.0.928/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.927'
+__version__ = '3.0.928'
```

### Comparing `tencentcloud-sdk-python-keewidb-3.0.927/tencentcloud/keewidb/v20220308/errorcodes.py` & `tencentcloud-sdk-python-keewidb-3.0.928/tencentcloud/keewidb/v20220308/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-keewidb-3.0.927/tencentcloud/keewidb/v20220308/keewidb_client.py` & `tencentcloud-sdk-python-keewidb-3.0.928/tencentcloud/keewidb/v20220308/keewidb_client.py`

 * *Files identical despite different names*

