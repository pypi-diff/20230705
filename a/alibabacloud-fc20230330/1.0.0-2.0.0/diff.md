# Comparing `tmp/alibabacloud_fc20230330-1.0.0.tar.gz` & `tmp/alibabacloud_fc20230330-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_fc20230330-1.0.0.tar", last modified: Wed Jun 28 08:47:56 2023, max compression
+gzip compressed data, was "dist/alibabacloud_fc20230330-2.0.0.tar", last modified: Wed Jul  5 07:46:12 2023, max compression
```

## Comparing `alibabacloud_fc20230330-1.0.0.tar` & `alibabacloud_fc20230330-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:47:56.000000 alibabacloud_fc20230330-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-28 08:47:56.000000 alibabacloud_fc20230330-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-28 08:47:56.000000 alibabacloud_fc20230330-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2336 2023-06-28 08:47:56.000000 alibabacloud_fc20230330-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1019 2023-06-28 08:47:56.000000 alibabacloud_fc20230330-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-28 08:47:56.000000 alibabacloud_fc20230330-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:47:56.000000 alibabacloud_fc20230330-1.0.0/alibabacloud_fc20230330/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-28 08:47:56.000000 alibabacloud_fc20230330-1.0.0/alibabacloud_fc20230330/__init__.py
--rw-r--r--   0 root         (0) root         (0)   180867 2023-06-28 08:47:56.000000 alibabacloud_fc20230330-1.0.0/alibabacloud_fc20230330/client.py
--rw-r--r--   0 root         (0) root         (0)   229586 2023-06-28 08:47:56.000000 alibabacloud_fc20230330-1.0.0/alibabacloud_fc20230330/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:47:56.000000 alibabacloud_fc20230330-1.0.0/alibabacloud_fc20230330.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2336 2023-06-28 08:47:56.000000 alibabacloud_fc20230330-1.0.0/alibabacloud_fc20230330.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      399 2023-06-28 08:47:56.000000 alibabacloud_fc20230330-1.0.0/alibabacloud_fc20230330.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 08:47:56.000000 alibabacloud_fc20230330-1.0.0/alibabacloud_fc20230330.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-06-28 08:47:56.000000 alibabacloud_fc20230330-1.0.0/alibabacloud_fc20230330.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-28 08:47:56.000000 alibabacloud_fc20230330-1.0.0/alibabacloud_fc20230330.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-28 08:47:56.000000 alibabacloud_fc20230330-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2619 2023-06-28 08:47:56.000000 alibabacloud_fc20230330-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:46:12.000000 alibabacloud_fc20230330-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-05 07:46:12.000000 alibabacloud_fc20230330-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-05 07:46:12.000000 alibabacloud_fc20230330-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-05 07:46:12.000000 alibabacloud_fc20230330-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2336 2023-07-05 07:46:12.000000 alibabacloud_fc20230330-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-07-05 07:46:12.000000 alibabacloud_fc20230330-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 07:46:12.000000 alibabacloud_fc20230330-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:46:12.000000 alibabacloud_fc20230330-2.0.0/alibabacloud_fc20230330/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-05 07:46:12.000000 alibabacloud_fc20230330-2.0.0/alibabacloud_fc20230330/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   180771 2023-07-05 07:46:12.000000 alibabacloud_fc20230330-2.0.0/alibabacloud_fc20230330/client.py
+-rw-r--r--   0 root         (0) root         (0)   229097 2023-07-05 07:46:12.000000 alibabacloud_fc20230330-2.0.0/alibabacloud_fc20230330/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:46:12.000000 alibabacloud_fc20230330-2.0.0/alibabacloud_fc20230330.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2336 2023-07-05 07:46:12.000000 alibabacloud_fc20230330-2.0.0/alibabacloud_fc20230330.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2023-07-05 07:46:12.000000 alibabacloud_fc20230330-2.0.0/alibabacloud_fc20230330.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:46:12.000000 alibabacloud_fc20230330-2.0.0/alibabacloud_fc20230330.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-05 07:46:12.000000 alibabacloud_fc20230330-2.0.0/alibabacloud_fc20230330.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-05 07:46:12.000000 alibabacloud_fc20230330-2.0.0/alibabacloud_fc20230330.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-05 07:46:12.000000 alibabacloud_fc20230330-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2619 2023-07-05 07:46:12.000000 alibabacloud_fc20230330-2.0.0/setup.py
```

### Comparing `alibabacloud_fc20230330-1.0.0/LICENSE` & `alibabacloud_fc20230330-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc20230330-1.0.0/PKG-INFO` & `alibabacloud_fc20230330-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_fc20230330
-Version: 1.0.0
+Version: 2.0.0
 Summary: Alibaba Cloud Function Compute (20230330) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_fc20230330-1.0.0/README-CN.md` & `alibabacloud_fc20230330-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc20230330-1.0.0/README.md` & `alibabacloud_fc20230330-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc20230330-1.0.0/alibabacloud_fc20230330/client.py` & `alibabacloud_fc20230330-2.0.0/alibabacloud_fc20230330/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/aliases',
             method='POST',
@@ -91,15 +91,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/aliases',
             method='POST',
@@ -156,15 +156,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/custom-domains',
             method='POST',
@@ -191,15 +191,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/custom-domains',
             method='POST',
@@ -254,15 +254,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/functions',
             method='POST',
@@ -289,15 +289,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/functions',
             method='POST',
@@ -353,15 +353,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/layers/{OpenApiUtilClient.get_encode_param(layer_name)}/versions',
             method='POST',
@@ -389,15 +389,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/layers/{OpenApiUtilClient.get_encode_param(layer_name)}/versions',
             method='POST',
@@ -455,15 +455,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/triggers',
             method='POST',
@@ -491,15 +491,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/triggers',
             method='POST',
@@ -2518,16 +2518,16 @@
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
             pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/invocations',
             method='POST',
@@ -2574,16 +2574,16 @@
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
             pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/invocations',
             method='POST',
@@ -4009,15 +4009,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/versions',
             method='POST',
@@ -4045,15 +4045,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/versions',
             method='POST',
@@ -4115,15 +4115,15 @@
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
             pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/async-invoke-config',
             method='PUT',
@@ -4155,15 +4155,15 @@
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
             pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/async-invoke-config',
             method='PUT',
@@ -4221,15 +4221,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/concurrency',
             method='PUT',
@@ -4257,15 +4257,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/concurrency',
             method='PUT',
@@ -4435,15 +4435,15 @@
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
             pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/provision-config',
             method='PUT',
@@ -4475,15 +4475,15 @@
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
             pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/provision-config',
             method='PUT',
@@ -4540,15 +4540,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/tag',
             method='POST',
@@ -4575,15 +4575,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/tag',
             method='POST',
@@ -4752,15 +4752,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/aliases/{OpenApiUtilClient.get_encode_param(alias_name)}',
             method='PUT',
@@ -4789,15 +4789,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/aliases/{OpenApiUtilClient.get_encode_param(alias_name)}',
             method='PUT',
@@ -4857,15 +4857,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/custom-domains/{OpenApiUtilClient.get_encode_param(domain_name)}',
             method='PUT',
@@ -4893,15 +4893,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/custom-domains/{OpenApiUtilClient.get_encode_param(domain_name)}',
             method='PUT',
@@ -4959,15 +4959,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}',
             method='PUT',
@@ -4995,15 +4995,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}',
             method='PUT',
@@ -5062,15 +5062,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/triggers/{OpenApiUtilClient.get_encode_param(trigger_name)}',
             method='PUT',
@@ -5099,15 +5099,15 @@
         @param headers: map
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
             pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/triggers/{OpenApiUtilClient.get_encode_param(trigger_name)}',
             method='PUT',
```

### Comparing `alibabacloud_fc20230330-1.0.0/alibabacloud_fc20230330/models.py` & `alibabacloud_fc20230330-2.0.0/alibabacloud_fc20230330/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -4109,37 +4109,37 @@
             self.trigger_config = m.get('triggerConfig')
         return self
 
 
 class CreateAliasRequest(TeaModel):
     def __init__(
         self,
-        request: CreateAliasInput = None,
+        body: CreateAliasInput = None,
     ):
-        self.request = request
+        self.body = body
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = CreateAliasInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateAliasResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -4182,37 +4182,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateCustomDomainRequest(TeaModel):
     def __init__(
         self,
-        request: CreateCustomDomainInput = None,
+        body: CreateCustomDomainInput = None,
     ):
-        self.request = request
+        self.body = body
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = CreateCustomDomainInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateCustomDomainResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -4255,37 +4255,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateFunctionRequest(TeaModel):
     def __init__(
         self,
-        request: CreateFunctionInput = None,
+        body: CreateFunctionInput = None,
     ):
-        self.request = request
+        self.body = body
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = CreateFunctionInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateFunctionResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -4328,37 +4328,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateLayerVersionRequest(TeaModel):
     def __init__(
         self,
-        request: CreateLayerVersionInput = None,
+        body: CreateLayerVersionInput = None,
     ):
-        self.request = request
+        self.body = body
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = CreateLayerVersionInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateLayerVersionResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -4401,37 +4401,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateTriggerRequest(TeaModel):
     def __init__(
         self,
-        request: CreateTriggerInput = None,
+        body: CreateTriggerInput = None,
     ):
-        self.request = request
+        self.body = body
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = CreateTriggerInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateTriggerResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -5492,41 +5492,41 @@
             self.x_fc_log_type = m.get('x-fc-log-type')
         return self
 
 
 class InvokeFunctionRequest(TeaModel):
     def __init__(
         self,
+        body: BinaryIO = None,
         qualifier: str = None,
-        request: BinaryIO = None,
     ):
+        self.body = body
         self.qualifier = qualifier
-        self.request = request
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('body') is not None:
+            self.body = m.get('body')
         if m.get('qualifier') is not None:
             self.qualifier = m.get('qualifier')
-        if m.get('request') is not None:
-            self.request = m.get('request')
         return self
 
 
 class InvokeFunctionResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -6556,37 +6556,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PublishFunctionVersionRequest(TeaModel):
     def __init__(
         self,
-        request: PublishVersionInput = None,
+        body: PublishVersionInput = None,
     ):
-        self.request = request
+        self.body = body
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = PublishVersionInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PublishFunctionVersionResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -6629,43 +6629,43 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PutAsyncInvokeConfigRequest(TeaModel):
     def __init__(
         self,
+        body: PutAsyncInvokeConfigInput = None,
         qualifier: str = None,
-        request: PutAsyncInvokeConfigInput = None,
     ):
+        self.body = body
         self.qualifier = qualifier
-        self.request = request
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -6708,37 +6708,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PutConcurrencyConfigRequest(TeaModel):
     def __init__(
         self,
-        request: PutConcurrencyInput = None,
+        body: PutConcurrencyInput = None,
     ):
-        self.request = request
+        self.body = body
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = PutConcurrencyInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PutConcurrencyConfigResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -6842,43 +6842,43 @@
             self.status_code = m.get('statusCode')
         return self
 
 
 class PutProvisionConfigRequest(TeaModel):
     def __init__(
         self,
+        body: PutProvisionConfigInput = None,
         qualifier: str = None,
-        request: PutProvisionConfigInput = None,
     ):
+        self.body = body
         self.qualifier = qualifier
-        self.request = request
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -6921,37 +6921,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class TagResourceRequest(TeaModel):
     def __init__(
         self,
-        request: TagResourceInput = None,
+        body: TagResourceInput = None,
     ):
-        self.request = request
+        self.body = body
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = TagResourceInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class TagResourceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -7067,37 +7067,37 @@
             self.status_code = m.get('statusCode')
         return self
 
 
 class UpdateAliasRequest(TeaModel):
     def __init__(
         self,
-        request: UpdateAliasInput = None,
+        body: UpdateAliasInput = None,
     ):
-        self.request = request
+        self.body = body
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = UpdateAliasInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateAliasResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -7140,37 +7140,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateCustomDomainRequest(TeaModel):
     def __init__(
         self,
-        request: UpdateCustomDomainInput = None,
+        body: UpdateCustomDomainInput = None,
     ):
-        self.request = request
+        self.body = body
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = UpdateCustomDomainInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateCustomDomainResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -7213,37 +7213,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateFunctionRequest(TeaModel):
     def __init__(
         self,
-        request: UpdateFunctionInput = None,
+        body: UpdateFunctionInput = None,
     ):
-        self.request = request
+        self.body = body
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = UpdateFunctionInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateFunctionResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -7286,37 +7286,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateTriggerRequest(TeaModel):
     def __init__(
         self,
-        request: UpdateTriggerInput = None,
+        body: UpdateTriggerInput = None,
     ):
-        self.request = request
+        self.body = body
 
     def validate(self):
-        if self.request:
-            self.request.validate()
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request is not None:
-            result['request'] = self.request.to_map()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('request') is not None:
+        if m.get('body') is not None:
             temp_model = UpdateTriggerInput()
-            self.request = temp_model.from_map(m['request'])
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateTriggerResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
```

### Comparing `alibabacloud_fc20230330-1.0.0/alibabacloud_fc20230330.egg-info/PKG-INFO` & `alibabacloud_fc20230330-2.0.0/alibabacloud_fc20230330.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-fc20230330
-Version: 1.0.0
+Version: 2.0.0
 Summary: Alibaba Cloud Function Compute (20230330) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_fc20230330-1.0.0/setup.py` & `alibabacloud_fc20230330-2.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_fc20230330.
 
-Created on 28/06/2023
+Created on 05/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_fc20230330"
 NAME = "alibabacloud_fc20230330" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Function Compute (20230330) SDK Library for Python"
```

