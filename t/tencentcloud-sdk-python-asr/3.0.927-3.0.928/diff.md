# Comparing `tmp/tencentcloud-sdk-python-asr-3.0.927.tar.gz` & `tmp/tencentcloud-sdk-python-asr-3.0.928.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.927.tar", last modified: Tue Jul  4 00:14:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.928.tar", last modified: Wed Jul  5 00:18:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-asr-3.0.927.tar` & `tencentcloud-sdk-python-asr-3.0.928.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:14:43.000000 tencentcloud-sdk-python-asr-3.0.927/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 00:14:43.000000 tencentcloud-sdk-python-asr-3.0.927/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:14:43.000000 tencentcloud-sdk-python-asr-3.0.927/tencentcloud_sdk_python_asr.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-04 00:14:43.000000 tencentcloud-sdk-python-asr-3.0.927/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 00:14:43.000000 tencentcloud-sdk-python-asr-3.0.927/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 00:14:43.000000 tencentcloud-sdk-python-asr-3.0.927/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 00:14:43.000000 tencentcloud-sdk-python-asr-3.0.927/tencentcloud_sdk_python_asr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-04 00:14:43.000000 tencentcloud-sdk-python-asr-3.0.927/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 00:14:43.000000 tencentcloud-sdk-python-asr-3.0.927/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-04 00:14:43.000000 tencentcloud-sdk-python-asr-3.0.927/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:14:43.000000 tencentcloud-sdk-python-asr-3.0.927/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-04 00:14:43.000000 tencentcloud-sdk-python-asr-3.0.927/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:14:43.000000 tencentcloud-sdk-python-asr-3.0.927/tencentcloud/asr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:14:43.000000 tencentcloud-sdk-python-asr-3.0.927/tencentcloud/asr/v20190614/
--rw-r--r--   0 root         (0) root         (0)     6520 2023-07-04 00:14:43.000000 tencentcloud-sdk-python-asr-3.0.927/tencentcloud/asr/v20190614/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    64222 2023-07-04 00:14:43.000000 tencentcloud-sdk-python-asr-3.0.927/tencentcloud/asr/v20190614/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:14:43.000000 tencentcloud-sdk-python-asr-3.0.927/tencentcloud/asr/v20190614/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24910 2023-07-04 00:14:43.000000 tencentcloud-sdk-python-asr-3.0.927/tencentcloud/asr/v20190614/asr_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:14:43.000000 tencentcloud-sdk-python-asr-3.0.927/tencentcloud/asr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:18:38.000000 tencentcloud-sdk-python-asr-3.0.928/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-05 00:18:38.000000 tencentcloud-sdk-python-asr-3.0.928/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:18:38.000000 tencentcloud-sdk-python-asr-3.0.928/tencentcloud_sdk_python_asr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-05 00:18:38.000000 tencentcloud-sdk-python-asr-3.0.928/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 00:18:38.000000 tencentcloud-sdk-python-asr-3.0.928/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-05 00:18:38.000000 tencentcloud-sdk-python-asr-3.0.928/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-05 00:18:38.000000 tencentcloud-sdk-python-asr-3.0.928/tencentcloud_sdk_python_asr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-05 00:18:38.000000 tencentcloud-sdk-python-asr-3.0.928/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-05 00:18:38.000000 tencentcloud-sdk-python-asr-3.0.928/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-05 00:18:38.000000 tencentcloud-sdk-python-asr-3.0.928/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:18:38.000000 tencentcloud-sdk-python-asr-3.0.928/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-05 00:18:38.000000 tencentcloud-sdk-python-asr-3.0.928/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:18:38.000000 tencentcloud-sdk-python-asr-3.0.928/tencentcloud/asr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:18:38.000000 tencentcloud-sdk-python-asr-3.0.928/tencentcloud/asr/v20190614/
+-rw-r--r--   0 root         (0) root         (0)     7371 2023-07-05 00:18:38.000000 tencentcloud-sdk-python-asr-3.0.928/tencentcloud/asr/v20190614/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   110859 2023-07-05 00:18:38.000000 tencentcloud-sdk-python-asr-3.0.928/tencentcloud/asr/v20190614/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:18:38.000000 tencentcloud-sdk-python-asr-3.0.928/tencentcloud/asr/v20190614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29291 2023-07-05 00:18:38.000000 tencentcloud-sdk-python-asr-3.0.928/tencentcloud/asr/v20190614/asr_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:18:38.000000 tencentcloud-sdk-python-asr-3.0.928/tencentcloud/asr/__init__.py
```

### Comparing `tencentcloud-sdk-python-asr-3.0.927/tencentcloud_sdk_python_asr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.928/tencentcloud_sdk_python_asr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.927/setup.py` & `tencentcloud-sdk-python-asr-3.0.928/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.927/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.928/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.927/README.rst` & `tencentcloud-sdk-python-asr-3.0.928/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.927/tencentcloud/__init__.py` & `tencentcloud-sdk-python-asr-3.0.928/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-asr-3.0.927/tencentcloud/asr/v20190614/errorcodes.py` & `tencentcloud-sdk-python-asr-3.0.928/tencentcloud/asr/v20190614/errorcodes.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 
 # 识别失败。
 FAILEDOPERATION_ERRORRECOGNIZE = 'FailedOperation.ErrorRecognize'
 
 # 错误的TaskId。
 FAILEDOPERATION_NOSUCHTASK = 'FailedOperation.NoSuchTask'
 
+# 不存在的说话人id
+FAILEDOPERATION_NOTEXISTENTVOICEPRINTID = 'FailedOperation.NotExistentVoicePrintId'
+
 # 账号因为欠费停止服务，请在腾讯云账户充值。
 FAILEDOPERATION_SERVICEISOLATE = 'FailedOperation.ServiceIsolate'
 
 # 账号本月免费额度已用完。
 FAILEDOPERATION_USERHASNOFREEAMOUNT = 'FailedOperation.UserHasNoFreeAmount'
 
 # 服务未开通，请在腾讯云官网语音识别控制台开通服务。
@@ -82,17 +85,35 @@
 
 # 访问数据库失败。
 INTERNALERROR_FAILACCESSDATABASE = 'InternalError.FailAccessDatabase'
 
 # 访问Redis失败。
 INTERNALERROR_FAILACCESSREDIS = 'InternalError.FailAccessRedis'
 
+# 说话人注册接口失败
+INTERNALERROR_FAILEDVOICEPRINTENROLL = 'InternalError.FailedVoicePrintEnroll'
+
+# 说话人验证接口失败
+INTERNALERROR_FAILEDVOICEPRINTVERIFY = 'InternalError.FailedVoicePrintVerify'
+
 # 请求标签接口出错
 INTERNALERROR_TAGREQUESTERROR = 'InternalError.TagRequestError'
 
+# 说话人音频处理失败
+INTERNALERROR_VOICEPRINTAUDIOFAILED = 'InternalError.VoicePrintAudioFailed'
+
+# 传入音频解码失败
+INTERNALERROR_VOICEPRINTDECODEFAILED = 'InternalError.VoicePrintDecodeFailed'
+
+# 说话人ID注册失败
+INTERNALERROR_VOICEPRINTENROLLFAILED = 'InternalError.VoicePrintEnrollFailed'
+
+# 说话人验证失败
+INTERNALERROR_VOICEPRINTVERIFYFAILED = 'InternalError.VoicePrintVerifyFailed'
+
 # 参数错误。
 INVALIDPARAMETER = 'InvalidParameter'
 
 # 请求数据长度无效。
 INVALIDPARAMETER_ERRORCONTENTLENGTH = 'InvalidParameter.ErrorContentlength'
 
 # 参数不全。
@@ -178,14 +199,17 @@
 
 # 上线模型个数已到限制。
 LIMITEXCEEDED_ONLINEFULL = 'LimitExceeded.OnlineFull'
 
 # 热词表数量已到账号限制。
 LIMITEXCEEDED_VOCABFULL = 'LimitExceeded.VocabFull'
 
+# 说话人ID创建数量达到上限
+LIMITEXCEEDED_VOICEPRINTFULL = 'LimitExceeded.VoicePrintFull'
+
 # 缺少参数错误。
 MISSINGPARAMETER = 'MissingParameter'
 
 # 请求的次数超过了频率限制。
 REQUESTLIMITEXCEEDED = 'RequestLimitExceeded'
 
 # 超出请求频率。
```

### Comparing `tencentcloud-sdk-python-asr-3.0.927/tencentcloud/asr/v20190614/asr_client.py` & `tencentcloud-sdk-python-asr-3.0.928/tencentcloud/asr/v20190614/asr_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -505,8 +505,106 @@
             model = models.UpdateAsrVocabResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def VoicePrintDelete(self, request):
+        """本接口用于以删除已经注册的说话人信息（删除之后，原有的说话人ID和说话人音频数据都会失效）
+
+        :param request: Request instance for VoicePrintDelete.
+        :type request: :class:`tencentcloud.asr.v20190614.models.VoicePrintDeleteRequest`
+        :rtype: :class:`tencentcloud.asr.v20190614.models.VoicePrintDeleteResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("VoicePrintDelete", params, headers=headers)
+            response = json.loads(body)
+            model = models.VoicePrintDeleteResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def VoicePrintEnroll(self, request):
+        """说话人注册接口用于注册一个指定音频，生成一个唯一的说话人id，后续可通过说话人验证接口验证其它音频和已有的说话人ID匹配度，注册时可指定说话人昵称，方便标识说话人ID，  说话人昵称可重复配置。
+        （注: 一个appid最多可以注册1000个说话人ID，一个说话人ID仅支持一条音频注册，后续可通过更新接口进行更新）
+
+        使用须知
+        支持的输入格式：编码文件(PCM, WAV)、16 bit采样位数、单声道（mono）。
+
+        支持的音频采样率：16000 Hz。
+
+        :param request: Request instance for VoicePrintEnroll.
+        :type request: :class:`tencentcloud.asr.v20190614.models.VoicePrintEnrollRequest`
+        :rtype: :class:`tencentcloud.asr.v20190614.models.VoicePrintEnrollResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("VoicePrintEnroll", params, headers=headers)
+            response = json.loads(body)
+            model = models.VoicePrintEnrollResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def VoicePrintUpdate(self, request):
+        """本接口用于更新和覆盖已注册的音频数据和说话人昵称，更新后原有的音频数据将失效。
+
+        :param request: Request instance for VoicePrintUpdate.
+        :type request: :class:`tencentcloud.asr.v20190614.models.VoicePrintUpdateRequest`
+        :rtype: :class:`tencentcloud.asr.v20190614.models.VoicePrintUpdateResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("VoicePrintUpdate", params, headers=headers)
+            response = json.loads(body)
+            model = models.VoicePrintUpdateResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def VoicePrintVerify(self, request):
+        """本接口用于校验传入音频与已注册音频的匹配程度，通过指定说话人ID（VoicePrintId）和一段音频进行音频和说话人的匹配度判断
+
+        :param request: Request instance for VoicePrintVerify.
+        :type request: :class:`tencentcloud.asr.v20190614.models.VoicePrintVerifyRequest`
+        :rtype: :class:`tencentcloud.asr.v20190614.models.VoicePrintVerifyResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("VoicePrintVerify", params, headers=headers)
+            response = json.loads(body)
+            model = models.VoicePrintVerifyResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
                 raise TencentCloudSDKException(e.message, e.message)
```

