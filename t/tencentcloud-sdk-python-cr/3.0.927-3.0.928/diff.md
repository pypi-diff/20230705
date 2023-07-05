# Comparing `tmp/tencentcloud-sdk-python-cr-3.0.927.tar.gz` & `tmp/tencentcloud-sdk-python-cr-3.0.928.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cr-3.0.927.tar", last modified: Tue Jul  4 00:19:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cr-3.0.928.tar", last modified: Wed Jul  5 00:23:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cr-3.0.927.tar` & `tencentcloud-sdk-python-cr-3.0.928.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:19:02.000000 tencentcloud-sdk-python-cr-3.0.927/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:19:02.000000 tencentcloud-sdk-python-cr-3.0.927/tencentcloud_sdk_python_cr.egg-info/
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-04 00:19:02.000000 tencentcloud-sdk-python-cr-3.0.927/tencentcloud_sdk_python_cr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 00:19:02.000000 tencentcloud-sdk-python-cr-3.0.927/tencentcloud_sdk_python_cr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-04 00:19:02.000000 tencentcloud-sdk-python-cr-3.0.927/tencentcloud_sdk_python_cr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 00:19:02.000000 tencentcloud-sdk-python-cr-3.0.927/tencentcloud_sdk_python_cr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 00:19:02.000000 tencentcloud-sdk-python-cr-3.0.927/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-04 00:19:02.000000 tencentcloud-sdk-python-cr-3.0.927/setup.py
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-04 00:19:02.000000 tencentcloud-sdk-python-cr-3.0.927/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-04 00:19:02.000000 tencentcloud-sdk-python-cr-3.0.927/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:19:02.000000 tencentcloud-sdk-python-cr-3.0.927/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:19:02.000000 tencentcloud-sdk-python-cr-3.0.927/tencentcloud/cr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:19:02.000000 tencentcloud-sdk-python-cr-3.0.927/tencentcloud/cr/v20180321/
--rw-r--r--   0 root         (0) root         (0)     4158 2023-07-04 00:19:02.000000 tencentcloud-sdk-python-cr-3.0.927/tencentcloud/cr/v20180321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    26019 2023-07-04 00:19:02.000000 tencentcloud-sdk-python-cr-3.0.927/tencentcloud/cr/v20180321/cr_client.py
--rw-r--r--   0 root         (0) root         (0)    83768 2023-07-04 00:19:02.000000 tencentcloud-sdk-python-cr-3.0.927/tencentcloud/cr/v20180321/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:19:02.000000 tencentcloud-sdk-python-cr-3.0.927/tencentcloud/cr/v20180321/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:19:02.000000 tencentcloud-sdk-python-cr-3.0.927/tencentcloud/cr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-04 00:19:02.000000 tencentcloud-sdk-python-cr-3.0.927/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:23:17.000000 tencentcloud-sdk-python-cr-3.0.928/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:23:17.000000 tencentcloud-sdk-python-cr-3.0.928/tencentcloud_sdk_python_cr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-05 00:23:17.000000 tencentcloud-sdk-python-cr-3.0.928/tencentcloud_sdk_python_cr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 00:23:17.000000 tencentcloud-sdk-python-cr-3.0.928/tencentcloud_sdk_python_cr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-05 00:23:17.000000 tencentcloud-sdk-python-cr-3.0.928/tencentcloud_sdk_python_cr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-05 00:23:17.000000 tencentcloud-sdk-python-cr-3.0.928/tencentcloud_sdk_python_cr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-05 00:23:17.000000 tencentcloud-sdk-python-cr-3.0.928/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-05 00:23:17.000000 tencentcloud-sdk-python-cr-3.0.928/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-05 00:23:17.000000 tencentcloud-sdk-python-cr-3.0.928/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-05 00:23:17.000000 tencentcloud-sdk-python-cr-3.0.928/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:23:17.000000 tencentcloud-sdk-python-cr-3.0.928/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:23:17.000000 tencentcloud-sdk-python-cr-3.0.928/tencentcloud/cr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:23:17.000000 tencentcloud-sdk-python-cr-3.0.928/tencentcloud/cr/v20180321/
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-07-05 00:23:17.000000 tencentcloud-sdk-python-cr-3.0.928/tencentcloud/cr/v20180321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    26019 2023-07-05 00:23:17.000000 tencentcloud-sdk-python-cr-3.0.928/tencentcloud/cr/v20180321/cr_client.py
+-rw-r--r--   0 root         (0) root         (0)   136120 2023-07-05 00:23:17.000000 tencentcloud-sdk-python-cr-3.0.928/tencentcloud/cr/v20180321/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:23:17.000000 tencentcloud-sdk-python-cr-3.0.928/tencentcloud/cr/v20180321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:23:17.000000 tencentcloud-sdk-python-cr-3.0.928/tencentcloud/cr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-05 00:23:17.000000 tencentcloud-sdk-python-cr-3.0.928/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-cr-3.0.927/tencentcloud_sdk_python_cr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cr-3.0.928/tencentcloud_sdk_python_cr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cr
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Cr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cr-3.0.927/setup.py` & `tencentcloud-sdk-python-cr-3.0.928/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cr-3.0.927/PKG-INFO` & `tencentcloud-sdk-python-cr-3.0.928/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cr
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Cr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cr-3.0.927/README.rst` & `tencentcloud-sdk-python-cr-3.0.928/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cr-3.0.927/tencentcloud/cr/v20180321/errorcodes.py` & `tencentcloud-sdk-python-cr-3.0.928/tencentcloud/cr/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cr-3.0.927/tencentcloud/cr/v20180321/cr_client.py` & `tencentcloud-sdk-python-cr-3.0.928/tencentcloud/cr/v20180321/cr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cr-3.0.927/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cr-3.0.928/tencentcloud/__init__.py`

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

