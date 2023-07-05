# Comparing `tmp/alibabacloud_airticketopen20230117-2.0.1.tar.gz` & `tmp/alibabacloud_airticketopen20230117-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_airticketopen20230117-2.0.1.tar", last modified: Fri Jun  2 02:10:04 2023, max compression
+gzip compressed data, was "dist/alibabacloud_airticketopen20230117-3.0.0.tar", last modified: Wed Jul  5 03:52:32 2023, max compression
```

## Comparing `alibabacloud_airticketopen20230117-2.0.1.tar` & `alibabacloud_airticketopen20230117-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 02:10:04.000000 alibabacloud_airticketopen20230117-2.0.1/
--rw-r--r--   0 root         (0) root         (0)      228 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2388 2023-06-02 02:10:04.000000 alibabacloud_airticketopen20230117-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1137 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 02:10:04.000000 alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117/__init__.py
--rw-r--r--   0 root         (0) root         (0)   104846 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117/client.py
--rw-r--r--   0 root         (0) root         (0)   506516 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 02:10:04.000000 alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2388 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-02 02:10:04.000000 alibabacloud_airticketopen20230117-2.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2660 2023-06-02 02:10:03.000000 alibabacloud_airticketopen20230117-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 03:52:32.000000 alibabacloud_airticketopen20230117-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)      304 2023-07-05 03:52:31.000000 alibabacloud_airticketopen20230117-3.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-05 03:52:31.000000 alibabacloud_airticketopen20230117-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-05 03:52:31.000000 alibabacloud_airticketopen20230117-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-07-05 03:52:32.000000 alibabacloud_airticketopen20230117-3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-07-05 03:52:31.000000 alibabacloud_airticketopen20230117-3.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-07-05 03:52:31.000000 alibabacloud_airticketopen20230117-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 03:52:32.000000 alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-05 03:52:31.000000 alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104846 2023-07-05 03:52:31.000000 alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117/client.py
+-rw-r--r--   0 root         (0) root         (0)   507628 2023-07-05 03:52:31.000000 alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 03:52:32.000000 alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-07-05 03:52:32.000000 alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      500 2023-07-05 03:52:32.000000 alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 03:52:32.000000 alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-05 03:52:32.000000 alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-07-05 03:52:32.000000 alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-05 03:52:32.000000 alibabacloud_airticketopen20230117-3.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2660 2023-07-05 03:52:31.000000 alibabacloud_airticketopen20230117-3.0.0/setup.py
```

### Comparing `alibabacloud_airticketopen20230117-2.0.1/LICENSE` & `alibabacloud_airticketopen20230117-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_airticketopen20230117-2.0.1/PKG-INFO` & `alibabacloud_airticketopen20230117-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_airticketopen20230117
-Version: 2.0.1
+Version: 3.0.0
 Summary: Alibaba Cloud airticketOpen (20230117) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_airticketopen20230117-2.0.1/README-CN.md` & `alibabacloud_airticketopen20230117-3.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_airticketopen20230117-2.0.1/README.md` & `alibabacloud_airticketopen20230117-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117/client.py` & `alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117/models.py` & `alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1293,69 +1293,93 @@
 
 
 class AccountFlowListResponseBodyDataList(TeaModel):
     def __init__(
         self,
         after_available_amount: float = None,
         before_available_amount: float = None,
+        change_order_num: int = None,
         flow_id: int = None,
         gmt_create: int = None,
         gmt_modified: int = None,
         op_amount: float = None,
         op_type: int = None,
+        order_num: int = None,
+        order_type: int = None,
+        refund_order_num: int = None,
     ):
         self.after_available_amount = after_available_amount
         self.before_available_amount = before_available_amount
+        self.change_order_num = change_order_num
         self.flow_id = flow_id
         self.gmt_create = gmt_create
         self.gmt_modified = gmt_modified
         self.op_amount = op_amount
         self.op_type = op_type
+        self.order_num = order_num
+        self.order_type = order_type
+        self.refund_order_num = refund_order_num
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.after_available_amount is not None:
             result['after_available_amount'] = self.after_available_amount
         if self.before_available_amount is not None:
             result['before_available_amount'] = self.before_available_amount
+        if self.change_order_num is not None:
+            result['change_order_num'] = self.change_order_num
         if self.flow_id is not None:
             result['flow_id'] = self.flow_id
         if self.gmt_create is not None:
             result['gmt_create'] = self.gmt_create
         if self.gmt_modified is not None:
             result['gmt_modified'] = self.gmt_modified
         if self.op_amount is not None:
             result['op_amount'] = self.op_amount
         if self.op_type is not None:
             result['op_type'] = self.op_type
+        if self.order_num is not None:
+            result['order_num'] = self.order_num
+        if self.order_type is not None:
+            result['order_type'] = self.order_type
+        if self.refund_order_num is not None:
+            result['refund_order_num'] = self.refund_order_num
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('after_available_amount') is not None:
             self.after_available_amount = m.get('after_available_amount')
         if m.get('before_available_amount') is not None:
             self.before_available_amount = m.get('before_available_amount')
+        if m.get('change_order_num') is not None:
+            self.change_order_num = m.get('change_order_num')
         if m.get('flow_id') is not None:
             self.flow_id = m.get('flow_id')
         if m.get('gmt_create') is not None:
             self.gmt_create = m.get('gmt_create')
         if m.get('gmt_modified') is not None:
             self.gmt_modified = m.get('gmt_modified')
         if m.get('op_amount') is not None:
             self.op_amount = m.get('op_amount')
         if m.get('op_type') is not None:
             self.op_type = m.get('op_type')
+        if m.get('order_num') is not None:
+            self.order_num = m.get('order_num')
+        if m.get('order_type') is not None:
+            self.order_type = m.get('order_type')
+        if m.get('refund_order_num') is not None:
+            self.refund_order_num = m.get('refund_order_num')
         return self
 
 
 class AccountFlowListResponseBodyDataPagination(TeaModel):
     def __init__(
         self,
         current_page: int = None,
@@ -1443,69 +1467,69 @@
             self.pagination = temp_model.from_map(m['pagination'])
         return self
 
 
 class AccountFlowListResponseBody(TeaModel):
     def __init__(
         self,
+        request_id: str = None,
         data: AccountFlowListResponseBodyData = None,
         error_code: str = None,
         error_data: Any = None,
         error_msg: str = None,
-        request_id: str = None,
         status: int = None,
         success: bool = None,
     ):
+        self.request_id = request_id
         self.data = data
         self.error_code = error_code
         self.error_data = error_data
         self.error_msg = error_msg
-        self.request_id = request_id
         self.status = status
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
         if self.data is not None:
             result['data'] = self.data.to_map()
         if self.error_code is not None:
             result['error_code'] = self.error_code
         if self.error_data is not None:
             result['error_data'] = self.error_data
         if self.error_msg is not None:
             result['error_msg'] = self.error_msg
-        if self.request_id is not None:
-            result['request_id'] = self.request_id
         if self.status is not None:
             result['status'] = self.status
         if self.success is not None:
             result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
         if m.get('data') is not None:
             temp_model = AccountFlowListResponseBodyData()
             self.data = temp_model.from_map(m['data'])
         if m.get('error_code') is not None:
             self.error_code = m.get('error_code')
         if m.get('error_data') is not None:
             self.error_data = m.get('error_data')
         if m.get('error_msg') is not None:
             self.error_msg = m.get('error_msg')
-        if m.get('request_id') is not None:
-            self.request_id = m.get('request_id')
         if m.get('status') is not None:
             self.status = m.get('status')
         if m.get('success') is not None:
             self.success = m.get('success')
         return self
```

### Comparing `alibabacloud_airticketopen20230117-2.0.1/alibabacloud_airticketopen20230117.egg-info/PKG-INFO` & `alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-airticketopen20230117
-Version: 2.0.1
+Version: 3.0.0
 Summary: Alibaba Cloud airticketOpen (20230117) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_airticketopen20230117-2.0.1/setup.py` & `alibabacloud_airticketopen20230117-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_airticketopen20230117.
 
-Created on 02/06/2023
+Created on 05/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_airticketopen20230117"
 NAME = "alibabacloud_airticketopen20230117" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud airticketOpen (20230117) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

