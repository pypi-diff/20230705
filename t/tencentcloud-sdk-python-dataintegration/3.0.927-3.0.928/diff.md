# Comparing `tmp/tencentcloud-sdk-python-dataintegration-3.0.927.tar.gz` & `tmp/tencentcloud-sdk-python-dataintegration-3.0.928.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dataintegration-3.0.927.tar", last modified: Tue Jul  4 00:19:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dataintegration-3.0.928.tar", last modified: Wed Jul  5 00:23:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dataintegration-3.0.927.tar` & `tencentcloud-sdk-python-dataintegration-3.0.928.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:19:44.000000 tencentcloud-sdk-python-dataintegration-3.0.927/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 00:19:44.000000 tencentcloud-sdk-python-dataintegration-3.0.927/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1030 2023-07-04 00:19:43.000000 tencentcloud-sdk-python-dataintegration-3.0.927/setup.py
--rw-r--r--   0 root         (0) root         (0)     1719 2023-07-04 00:19:44.000000 tencentcloud-sdk-python-dataintegration-3.0.927/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      773 2023-07-04 00:19:43.000000 tencentcloud-sdk-python-dataintegration-3.0.927/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:19:44.000000 tencentcloud-sdk-python-dataintegration-3.0.927/tencentcloud_sdk_python_dataintegration.egg-info/
--rw-r--r--   0 root         (0) root         (0)      565 2023-07-04 00:19:44.000000 tencentcloud-sdk-python-dataintegration-3.0.927/tencentcloud_sdk_python_dataintegration.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 00:19:44.000000 tencentcloud-sdk-python-dataintegration-3.0.927/tencentcloud_sdk_python_dataintegration.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1719 2023-07-04 00:19:44.000000 tencentcloud-sdk-python-dataintegration-3.0.927/tencentcloud_sdk_python_dataintegration.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 00:19:44.000000 tencentcloud-sdk-python-dataintegration-3.0.927/tencentcloud_sdk_python_dataintegration.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:19:44.000000 tencentcloud-sdk-python-dataintegration-3.0.927/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:19:44.000000 tencentcloud-sdk-python-dataintegration-3.0.927/tencentcloud/dataintegration/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:19:44.000000 tencentcloud-sdk-python-dataintegration-3.0.927/tencentcloud/dataintegration/v20220613/
--rw-r--r--   0 root         (0) root         (0)      652 2023-07-04 00:19:43.000000 tencentcloud-sdk-python-dataintegration-3.0.927/tencentcloud/dataintegration/v20220613/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-07-04 00:19:43.000000 tencentcloud-sdk-python-dataintegration-3.0.927/tencentcloud/dataintegration/v20220613/models.py
--rw-r--r--   0 root         (0) root         (0)     1910 2023-07-04 00:19:43.000000 tencentcloud-sdk-python-dataintegration-3.0.927/tencentcloud/dataintegration/v20220613/dataintegration_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:19:43.000000 tencentcloud-sdk-python-dataintegration-3.0.927/tencentcloud/dataintegration/v20220613/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:19:43.000000 tencentcloud-sdk-python-dataintegration-3.0.927/tencentcloud/dataintegration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-04 00:19:43.000000 tencentcloud-sdk-python-dataintegration-3.0.927/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:23:58.000000 tencentcloud-sdk-python-dataintegration-3.0.928/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-05 00:23:58.000000 tencentcloud-sdk-python-dataintegration-3.0.928/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1030 2023-07-05 00:23:58.000000 tencentcloud-sdk-python-dataintegration-3.0.928/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-07-05 00:23:58.000000 tencentcloud-sdk-python-dataintegration-3.0.928/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      773 2023-07-05 00:23:58.000000 tencentcloud-sdk-python-dataintegration-3.0.928/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:23:58.000000 tencentcloud-sdk-python-dataintegration-3.0.928/tencentcloud_sdk_python_dataintegration.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      565 2023-07-05 00:23:58.000000 tencentcloud-sdk-python-dataintegration-3.0.928/tencentcloud_sdk_python_dataintegration.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 00:23:58.000000 tencentcloud-sdk-python-dataintegration-3.0.928/tencentcloud_sdk_python_dataintegration.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-07-05 00:23:58.000000 tencentcloud-sdk-python-dataintegration-3.0.928/tencentcloud_sdk_python_dataintegration.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-05 00:23:58.000000 tencentcloud-sdk-python-dataintegration-3.0.928/tencentcloud_sdk_python_dataintegration.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:23:58.000000 tencentcloud-sdk-python-dataintegration-3.0.928/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:23:58.000000 tencentcloud-sdk-python-dataintegration-3.0.928/tencentcloud/dataintegration/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:23:58.000000 tencentcloud-sdk-python-dataintegration-3.0.928/tencentcloud/dataintegration/v20220613/
+-rw-r--r--   0 root         (0) root         (0)      652 2023-07-05 00:23:58.000000 tencentcloud-sdk-python-dataintegration-3.0.928/tencentcloud/dataintegration/v20220613/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-07-05 00:23:58.000000 tencentcloud-sdk-python-dataintegration-3.0.928/tencentcloud/dataintegration/v20220613/models.py
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-07-05 00:23:58.000000 tencentcloud-sdk-python-dataintegration-3.0.928/tencentcloud/dataintegration/v20220613/dataintegration_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:23:58.000000 tencentcloud-sdk-python-dataintegration-3.0.928/tencentcloud/dataintegration/v20220613/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:23:58.000000 tencentcloud-sdk-python-dataintegration-3.0.928/tencentcloud/dataintegration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-05 00:23:58.000000 tencentcloud-sdk-python-dataintegration-3.0.928/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-dataintegration-3.0.927/setup.py` & `tencentcloud-sdk-python-dataintegration-3.0.928/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dataintegration-3.0.927/PKG-INFO` & `tencentcloud-sdk-python-dataintegration-3.0.928/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dataintegration
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Dataintegration SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dataintegration-3.0.927/README.rst` & `tencentcloud-sdk-python-dataintegration-3.0.928/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dataintegration-3.0.927/tencentcloud_sdk_python_dataintegration.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-dataintegration-3.0.928/tencentcloud_sdk_python_dataintegration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dataintegration-3.0.927/tencentcloud_sdk_python_dataintegration.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dataintegration-3.0.928/tencentcloud_sdk_python_dataintegration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dataintegration
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Dataintegration SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dataintegration-3.0.927/tencentcloud/dataintegration/v20220613/errorcodes.py` & `tencentcloud-sdk-python-dataintegration-3.0.928/tencentcloud/dataintegration/v20220613/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dataintegration-3.0.927/tencentcloud/dataintegration/v20220613/models.py` & `tencentcloud-sdk-python-dataintegration-3.0.928/tencentcloud/dataintegration/v20220613/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,80 +21,130 @@
 class BatchContent(AbstractModel):
     """批量消息
 
     """
 
     def __init__(self):
         r"""
-        :param Body: 消息体
+        :param _Body: 消息体
         :type Body: str
-        :param Key: 消息的键名
+        :param _Key: 消息的键名
         :type Key: str
         """
-        self.Body = None
-        self.Key = None
+        self._Body = None
+        self._Key = None
+
+    @property
+    def Body(self):
+        return self._Body
+
+    @Body.setter
+    def Body(self, Body):
+        self._Body = Body
+
+    @property
+    def Key(self):
+        return self._Key
+
+    @Key.setter
+    def Key(self, Key):
+        self._Key = Key
 
 
     def _deserialize(self, params):
-        self.Body = params.get("Body")
-        self.Key = params.get("Key")
+        self._Body = params.get("Body")
+        self._Key = params.get("Key")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class SendMessageRequest(AbstractModel):
     """SendMessage请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param DataHubId: 接入资源ID
+        :param _DataHubId: 接入资源ID
         :type DataHubId: str
-        :param Message: 批量消息
+        :param _Message: 批量消息
         :type Message: list of BatchContent
         """
-        self.DataHubId = None
-        self.Message = None
+        self._DataHubId = None
+        self._Message = None
+
+    @property
+    def DataHubId(self):
+        return self._DataHubId
+
+    @DataHubId.setter
+    def DataHubId(self, DataHubId):
+        self._DataHubId = DataHubId
+
+    @property
+    def Message(self):
+        return self._Message
+
+    @Message.setter
+    def Message(self, Message):
+        self._Message = Message
 
 
     def _deserialize(self, params):
-        self.DataHubId = params.get("DataHubId")
+        self._DataHubId = params.get("DataHubId")
         if params.get("Message") is not None:
-            self.Message = []
+            self._Message = []
             for item in params.get("Message"):
                 obj = BatchContent()
                 obj._deserialize(item)
-                self.Message.append(obj)
+                self._Message.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class SendMessageResponse(AbstractModel):
     """SendMessage返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param MessageId: 消息ID
+        :param _MessageId: 消息ID
         :type MessageId: list of str
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
-        self.MessageId = None
-        self.RequestId = None
+        self._MessageId = None
+        self._RequestId = None
+
+    @property
+    def MessageId(self):
+        return self._MessageId
+
+    @MessageId.setter
+    def MessageId(self, MessageId):
+        self._MessageId = MessageId
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
 
 
     def _deserialize(self, params):
-        self.MessageId = params.get("MessageId")
-        self.RequestId = params.get("RequestId")
+        self._MessageId = params.get("MessageId")
+        self._RequestId = params.get("RequestId")
```

### Comparing `tencentcloud-sdk-python-dataintegration-3.0.927/tencentcloud/dataintegration/v20220613/dataintegration_client.py` & `tencentcloud-sdk-python-dataintegration-3.0.928/tencentcloud/dataintegration/v20220613/dataintegration_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dataintegration-3.0.927/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dataintegration-3.0.928/tencentcloud/__init__.py`

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

