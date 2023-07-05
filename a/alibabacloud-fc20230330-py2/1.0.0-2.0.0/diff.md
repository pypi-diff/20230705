# Comparing `tmp/alibabacloud_fc20230330_py2-1.0.0.tar.gz` & `tmp/alibabacloud_fc20230330_py2-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_fc20230330_py2-1.0.0.tar", last modified: Wed Jun 28 08:46:58 2023, max compression
+gzip compressed data, was "dist/alibabacloud_fc20230330_py2-2.0.0.tar", last modified: Wed Jul  5 07:45:30 2023, max compression
```

## Comparing `alibabacloud_fc20230330_py2-1.0.0.tar` & `alibabacloud_fc20230330_py2-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:46:58.000000 alibabacloud_fc20230330_py2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      588 2023-06-28 08:46:58.000000 alibabacloud_fc20230330_py2-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-06-28 08:46:58.000000 alibabacloud_fc20230330_py2-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2480 2023-06-28 08:46:58.000000 alibabacloud_fc20230330_py2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1030 2023-06-28 08:46:58.000000 alibabacloud_fc20230330_py2-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1113 2023-06-28 08:46:58.000000 alibabacloud_fc20230330_py2-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:46:58.000000 alibabacloud_fc20230330_py2-1.0.0/alibabacloud_fc20230330/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-28 08:46:58.000000 alibabacloud_fc20230330_py2-1.0.0/alibabacloud_fc20230330/__init__.py
--rw-r--r--   0 root         (0) root         (0)    78969 2023-06-28 08:46:58.000000 alibabacloud_fc20230330_py2-1.0.0/alibabacloud_fc20230330/client.py
--rw-r--r--   0 root         (0) root         (0)   229408 2023-06-28 08:46:58.000000 alibabacloud_fc20230330_py2-1.0.0/alibabacloud_fc20230330/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:46:58.000000 alibabacloud_fc20230330_py2-1.0.0/alibabacloud_fc20230330_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2480 2023-06-28 08:46:58.000000 alibabacloud_fc20230330_py2-1.0.0/alibabacloud_fc20230330_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      419 2023-06-28 08:46:58.000000 alibabacloud_fc20230330_py2-1.0.0/alibabacloud_fc20230330_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 08:46:58.000000 alibabacloud_fc20230330_py2-1.0.0/alibabacloud_fc20230330_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-06-28 08:46:58.000000 alibabacloud_fc20230330_py2-1.0.0/alibabacloud_fc20230330_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-28 08:46:58.000000 alibabacloud_fc20230330_py2-1.0.0/alibabacloud_fc20230330_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-28 08:46:58.000000 alibabacloud_fc20230330_py2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2912 2023-06-28 08:46:58.000000 alibabacloud_fc20230330_py2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:45:30.000000 alibabacloud_fc20230330_py2-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-05 07:45:30.000000 alibabacloud_fc20230330_py2-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-05 07:45:30.000000 alibabacloud_fc20230330_py2-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-05 07:45:30.000000 alibabacloud_fc20230330_py2-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-07-05 07:45:30.000000 alibabacloud_fc20230330_py2-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1030 2023-07-05 07:45:30.000000 alibabacloud_fc20230330_py2-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-05 07:45:30.000000 alibabacloud_fc20230330_py2-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:45:30.000000 alibabacloud_fc20230330_py2-2.0.0/alibabacloud_fc20230330/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-05 07:45:30.000000 alibabacloud_fc20230330_py2-2.0.0/alibabacloud_fc20230330/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    78921 2023-07-05 07:45:30.000000 alibabacloud_fc20230330_py2-2.0.0/alibabacloud_fc20230330/client.py
+-rw-r--r--   0 root         (0) root         (0)   228919 2023-07-05 07:45:30.000000 alibabacloud_fc20230330_py2-2.0.0/alibabacloud_fc20230330/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:45:30.000000 alibabacloud_fc20230330_py2-2.0.0/alibabacloud_fc20230330_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-07-05 07:45:30.000000 alibabacloud_fc20230330_py2-2.0.0/alibabacloud_fc20230330_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      432 2023-07-05 07:45:30.000000 alibabacloud_fc20230330_py2-2.0.0/alibabacloud_fc20230330_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:45:30.000000 alibabacloud_fc20230330_py2-2.0.0/alibabacloud_fc20230330_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-05 07:45:30.000000 alibabacloud_fc20230330_py2-2.0.0/alibabacloud_fc20230330_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-05 07:45:30.000000 alibabacloud_fc20230330_py2-2.0.0/alibabacloud_fc20230330_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-05 07:45:30.000000 alibabacloud_fc20230330_py2-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-07-05 07:45:30.000000 alibabacloud_fc20230330_py2-2.0.0/setup.py
```

### Comparing `alibabacloud_fc20230330_py2-1.0.0/LICENSE` & `alibabacloud_fc20230330_py2-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc20230330_py2-1.0.0/PKG-INFO` & `alibabacloud_fc20230330_py2-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_fc20230330_py2
-Version: 1.0.0
+Version: 2.0.0
 Summary: Alibaba Cloud Function Compute (20230330) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_fc20230330_py2-1.0.0/README-CN.md` & `alibabacloud_fc20230330_py2-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc20230330_py2-1.0.0/README.md` & `alibabacloud_fc20230330_py2-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc20230330_py2-1.0.0/alibabacloud_fc20230330/client.py` & `alibabacloud_fc20230330_py2-2.0.0/alibabacloud_fc20230330/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: CreateAliasResponse
         """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(request.request)
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='CreateAlias',
             version='2023-03-30',
             protocol='HTTPS',
             pathname='/2023-03-30/functions/%s/aliases' % TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(function_name)),
             method='POST',
@@ -92,15 +92,15 @@
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: CreateCustomDomainResponse
         """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(request.request)
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='CreateCustomDomain',
             version='2023-03-30',
             protocol='HTTPS',
             pathname='/2023-03-30/custom-domains',
             method='POST',
@@ -140,15 +140,15 @@
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: CreateFunctionResponse
         """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(request.request)
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='CreateFunction',
             version='2023-03-30',
             protocol='HTTPS',
             pathname='/2023-03-30/functions',
             method='POST',
@@ -188,15 +188,15 @@
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: CreateLayerVersionResponse
         """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(request.request)
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='CreateLayerVersion',
             version='2023-03-30',
             protocol='HTTPS',
             pathname='/2023-03-30/layers/%s/versions' % TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(layer_name)),
             method='POST',
@@ -236,15 +236,15 @@
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: CreateTriggerResponse
         """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(request.request)
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='CreateTrigger',
             version='2023-03-30',
             protocol='HTTPS',
             pathname='/2023-03-30/functions/%s/triggers' % TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(function_name)),
             method='POST',
@@ -1197,16 +1197,16 @@
         if not UtilClient.is_unset(headers.x_fc_invocation_type):
             real_headers['x-fc-invocation-type'] = UtilClient.to_jsonstring(headers.x_fc_invocation_type)
         if not UtilClient.is_unset(headers.x_fc_log_type):
             real_headers['x-fc-log-type'] = UtilClient.to_jsonstring(headers.x_fc_log_type)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             query=OpenApiUtilClient.query(query),
-            body=request.request,
-            stream=request.request
+            body=request.body,
+            stream=request.body
         )
         params = open_api_models.Params(
             action='InvokeFunction',
             version='2023-03-30',
             protocol='HTTPS',
             pathname='/2023-03-30/functions/%s/invocations' % TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(function_name)),
             method='POST',
@@ -1912,15 +1912,15 @@
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: PublishFunctionVersionResponse
         """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(request.request)
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='PublishFunctionVersion',
             version='2023-03-30',
             protocol='HTTPS',
             pathname='/2023-03-30/functions/%s/versions' % TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(function_name)),
             method='POST',
@@ -1964,15 +1964,15 @@
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.qualifier):
             query['qualifier'] = request.qualifier
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query),
-            body=OpenApiUtilClient.parse_to_map(request.request)
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='PutAsyncInvokeConfig',
             version='2023-03-30',
             protocol='HTTPS',
             pathname='/2023-03-30/functions/%s/async-invoke-config' % TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(function_name)),
             method='PUT',
@@ -2012,15 +2012,15 @@
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: PutConcurrencyConfigResponse
         """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(request.request)
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='PutConcurrencyConfig',
             version='2023-03-30',
             protocol='HTTPS',
             pathname='/2023-03-30/functions/%s/concurrency' % TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(function_name)),
             method='PUT',
@@ -2115,15 +2115,15 @@
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.qualifier):
             query['qualifier'] = request.qualifier
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query),
-            body=OpenApiUtilClient.parse_to_map(request.request)
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='PutProvisionConfig',
             version='2023-03-30',
             protocol='HTTPS',
             pathname='/2023-03-30/functions/%s/provision-config' % TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(function_name)),
             method='PUT',
@@ -2163,15 +2163,15 @@
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: TagResourceResponse
         """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(request.request)
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='TagResource',
             version='2023-03-30',
             protocol='HTTPS',
             pathname='/2023-03-30/tag',
             method='POST',
@@ -2266,15 +2266,15 @@
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: UpdateAliasResponse
         """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(request.request)
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='UpdateAlias',
             version='2023-03-30',
             protocol='HTTPS',
             pathname='/2023-03-30/functions/%s/aliases/%s' % (TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(function_name)), TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(alias_name))),
             method='PUT',
@@ -2314,15 +2314,15 @@
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: UpdateCustomDomainResponse
         """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(request.request)
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='UpdateCustomDomain',
             version='2023-03-30',
             protocol='HTTPS',
             pathname='/2023-03-30/custom-domains/%s' % TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(domain_name)),
             method='PUT',
@@ -2362,15 +2362,15 @@
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: UpdateFunctionResponse
         """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(request.request)
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='UpdateFunction',
             version='2023-03-30',
             protocol='HTTPS',
             pathname='/2023-03-30/functions/%s' % TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(function_name)),
             method='PUT',
@@ -2410,15 +2410,15 @@
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: UpdateTriggerResponse
         """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(request.request)
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='UpdateTrigger',
             version='2023-03-30',
             protocol='HTTPS',
             pathname='/2023-03-30/functions/%s/triggers/%s' % (TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(function_name)), TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(trigger_name))),
             method='PUT',
```

### Comparing `alibabacloud_fc20230330_py2-1.0.0/alibabacloud_fc20230330/models.py` & `alibabacloud_fc20230330_py2-2.0.0/alibabacloud_fc20230330/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -3636,36 +3636,36 @@
             self.match = m.get('match')
         if m.get('replacement') is not None:
             self.replacement = m.get('replacement')
         return self
 
 
 class CreateAliasRequest(TeaModel):
-    def __init__(self, request=None):
-        self.request = request  # type: CreateAliasInput
+    def __init__(self, body=None):
+        self.body = body  # type: CreateAliasInput
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super(CreateAliasRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = CreateAliasInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateAliasResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
@@ -3701,36 +3701,36 @@
         if m.get('body') is not None:
             temp_model = Alias()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateCustomDomainRequest(TeaModel):
-    def __init__(self, request=None):
-        self.request = request  # type: CreateCustomDomainInput
+    def __init__(self, body=None):
+        self.body = body  # type: CreateCustomDomainInput
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super(CreateCustomDomainRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = CreateCustomDomainInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateCustomDomainResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
@@ -3766,36 +3766,36 @@
         if m.get('body') is not None:
             temp_model = CustomDomain()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateFunctionRequest(TeaModel):
-    def __init__(self, request=None):
-        self.request = request  # type: CreateFunctionInput
+    def __init__(self, body=None):
+        self.body = body  # type: CreateFunctionInput
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super(CreateFunctionRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = CreateFunctionInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateFunctionResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
@@ -3831,36 +3831,36 @@
         if m.get('body') is not None:
             temp_model = Function()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateLayerVersionRequest(TeaModel):
-    def __init__(self, request=None):
-        self.request = request  # type: CreateLayerVersionInput
+    def __init__(self, body=None):
+        self.body = body  # type: CreateLayerVersionInput
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super(CreateLayerVersionRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = CreateLayerVersionInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateLayerVersionResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
@@ -3896,36 +3896,36 @@
         if m.get('body') is not None:
             temp_model = Layer()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateTriggerRequest(TeaModel):
-    def __init__(self, request=None):
-        self.request = request  # type: CreateTriggerInput
+    def __init__(self, body=None):
+        self.body = body  # type: CreateTriggerInput
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super(CreateTriggerRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = CreateTriggerInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateTriggerResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
@@ -4862,39 +4862,39 @@
             self.x_fc_invocation_type = m.get('x-fc-invocation-type')
         if m.get('x-fc-log-type') is not None:
             self.x_fc_log_type = m.get('x-fc-log-type')
         return self
 
 
 class InvokeFunctionRequest(TeaModel):
-    def __init__(self, qualifier=None, request=None):
+    def __init__(self, body=None, qualifier=None):
+        self.body = body  # type: READABLE
         self.qualifier = qualifier  # type: str
-        self.request = request  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(InvokeFunctionRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.body is not None:
+            result['body'] = self.body
         if self.qualifier is not None:
             result['qualifier'] = self.qualifier
-        if self.request is not None:
-            result['request'] = self.request
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('body') is not None:
+            self.body = m.get('body')
         if m.get('qualifier') is not None:
             self.qualifier = m.get('qualifier')
-        if m.get('request') is not None:
-            self.request = m.get('request')
         return self
 
 
 class InvokeFunctionResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
@@ -5798,36 +5798,36 @@
         if m.get('body') is not None:
             temp_model = ListTriggersOutput()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PublishFunctionVersionRequest(TeaModel):
-    def __init__(self, request=None):
-        self.request = request  # type: PublishVersionInput
+    def __init__(self, body=None):
+        self.body = body  # type: PublishVersionInput
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super(PublishFunctionVersionRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = PublishVersionInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PublishFunctionVersionResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
@@ -5863,41 +5863,41 @@
         if m.get('body') is not None:
             temp_model = Version()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PutAsyncInvokeConfigRequest(TeaModel):
-    def __init__(self, qualifier=None, request=None):
+    def __init__(self, body=None, qualifier=None):
+        self.body = body  # type: PutAsyncInvokeConfigInput
         self.qualifier = qualifier  # type: str
-        self.request = request  # type: PutAsyncInvokeConfigInput
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super(PutAsyncInvokeConfigRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         if self.qualifier is not None:
             result['qualifier'] = self.qualifier
-        if self.request is not None:
-            result['request'] = self.request.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('body') is not None:
+            temp_model = PutAsyncInvokeConfigInput()
+            self.body = temp_model.from_map(m['body'])
         if m.get('qualifier') is not None:
             self.qualifier = m.get('qualifier')
-        if m.get('request') is not None:
-            temp_model = PutAsyncInvokeConfigInput()
-            self.request = temp_model.from_map(m['request'])
         return self
 
 
 class PutAsyncInvokeConfigResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
@@ -5933,36 +5933,36 @@
         if m.get('body') is not None:
             temp_model = AsyncConfig()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PutConcurrencyConfigRequest(TeaModel):
-    def __init__(self, request=None):
-        self.request = request  # type: PutConcurrencyInput
+    def __init__(self, body=None):
+        self.body = body  # type: PutConcurrencyInput
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super(PutConcurrencyConfigRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = PutConcurrencyInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PutConcurrencyConfigResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
@@ -6052,41 +6052,41 @@
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         return self
 
 
 class PutProvisionConfigRequest(TeaModel):
-    def __init__(self, qualifier=None, request=None):
+    def __init__(self, body=None, qualifier=None):
+        self.body = body  # type: PutProvisionConfigInput
         self.qualifier = qualifier  # type: str
-        self.request = request  # type: PutProvisionConfigInput
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super(PutProvisionConfigRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         if self.qualifier is not None:
             result['qualifier'] = self.qualifier
-        if self.request is not None:
-            result['request'] = self.request.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('body') is not None:
+            temp_model = PutProvisionConfigInput()
+            self.body = temp_model.from_map(m['body'])
         if m.get('qualifier') is not None:
             self.qualifier = m.get('qualifier')
-        if m.get('request') is not None:
-            temp_model = PutProvisionConfigInput()
-            self.request = temp_model.from_map(m['request'])
         return self
 
 
 class PutProvisionConfigResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
@@ -6122,36 +6122,36 @@
         if m.get('body') is not None:
             temp_model = ProvisionConfig()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class TagResourceRequest(TeaModel):
-    def __init__(self, request=None):
-        self.request = request  # type: TagResourceInput
+    def __init__(self, body=None):
+        self.body = body  # type: TagResourceInput
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super(TagResourceRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = TagResourceInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class TagResourceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
@@ -6251,36 +6251,36 @@
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         return self
 
 
 class UpdateAliasRequest(TeaModel):
-    def __init__(self, request=None):
-        self.request = request  # type: UpdateAliasInput
+    def __init__(self, body=None):
+        self.body = body  # type: UpdateAliasInput
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super(UpdateAliasRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = UpdateAliasInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateAliasResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
@@ -6316,36 +6316,36 @@
         if m.get('body') is not None:
             temp_model = Alias()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateCustomDomainRequest(TeaModel):
-    def __init__(self, request=None):
-        self.request = request  # type: UpdateCustomDomainInput
+    def __init__(self, body=None):
+        self.body = body  # type: UpdateCustomDomainInput
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super(UpdateCustomDomainRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = UpdateCustomDomainInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateCustomDomainResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
@@ -6381,36 +6381,36 @@
         if m.get('body') is not None:
             temp_model = CustomDomain()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateFunctionRequest(TeaModel):
-    def __init__(self, request=None):
-        self.request = request  # type: UpdateFunctionInput
+    def __init__(self, body=None):
+        self.body = body  # type: UpdateFunctionInput
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super(UpdateFunctionRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = UpdateFunctionInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateFunctionResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
@@ -6446,36 +6446,36 @@
         if m.get('body') is not None:
             temp_model = Function()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateTriggerRequest(TeaModel):
-    def __init__(self, request=None):
-        self.request = request  # type: UpdateTriggerInput
+    def __init__(self, body=None):
+        self.body = body  # type: UpdateTriggerInput
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super(UpdateTriggerRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = UpdateTriggerInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateTriggerResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
```

### Comparing `alibabacloud_fc20230330_py2-1.0.0/alibabacloud_fc20230330_py2.egg-info/PKG-INFO` & `alibabacloud_fc20230330_py2-2.0.0/alibabacloud_fc20230330_py2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-fc20230330-py2
-Version: 1.0.0
+Version: 2.0.0
 Summary: Alibaba Cloud Function Compute (20230330) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_fc20230330_py2-1.0.0/setup.py` & `alibabacloud_fc20230330_py2-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_fc20230330_py2.
 
-Created on 28/06/2023
+Created on 05/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_fc20230330"
 NAME = "alibabacloud_fc20230330_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Function Compute (20230330) SDK Library for Python2"
```

