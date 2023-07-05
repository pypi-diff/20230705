# Comparing `tmp/antchain_yunqing-4.0.5.tar.gz` & `tmp/antchain_yunqing-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_yunqing-4.0.5.tar", last modified: Tue Jul  4 09:50:02 2023, max compression
+gzip compressed data, was "dist/antchain_yunqing-4.0.6.tar", last modified: Wed Jul  5 09:49:44 2023, max compression
```

## Comparing `antchain_yunqing-4.0.5.tar` & `antchain_yunqing-4.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:50:02.000000 antchain_yunqing-4.0.5/
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-04 09:50:01.000000 antchain_yunqing-4.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-04 09:50:01.000000 antchain_yunqing-4.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2186 2023-07-04 09:50:02.000000 antchain_yunqing-4.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      816 2023-07-04 09:50:01.000000 antchain_yunqing-4.0.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1002 2023-07-04 09:50:01.000000 antchain_yunqing-4.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:50:02.000000 antchain_yunqing-4.0.5/antchain_sdk_yunqing/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 09:50:01.000000 antchain_yunqing-4.0.5/antchain_sdk_yunqing/__init__.py
--rw-r--r--   0 root         (0) root         (0)   197878 2023-07-04 09:50:01.000000 antchain_yunqing-4.0.5/antchain_sdk_yunqing/client.py
--rw-r--r--   0 root         (0) root         (0)   566684 2023-07-04 09:50:01.000000 antchain_yunqing-4.0.5/antchain_sdk_yunqing/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:50:02.000000 antchain_yunqing-4.0.5/antchain_yunqing.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2186 2023-07-04 09:50:02.000000 antchain_yunqing-4.0.5/antchain_yunqing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      355 2023-07-04 09:50:02.000000 antchain_yunqing-4.0.5/antchain_yunqing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 09:50:02.000000 antchain_yunqing-4.0.5/antchain_yunqing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-04 09:50:02.000000 antchain_yunqing-4.0.5/antchain_yunqing.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 09:50:02.000000 antchain_yunqing-4.0.5/antchain_yunqing.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 09:50:02.000000 antchain_yunqing-4.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2508 2023-07-04 09:50:01.000000 antchain_yunqing-4.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 09:49:44.000000 antchain_yunqing-4.0.6/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-05 09:49:44.000000 antchain_yunqing-4.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-05 09:49:44.000000 antchain_yunqing-4.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-07-05 09:49:44.000000 antchain_yunqing-4.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      816 2023-07-05 09:49:44.000000 antchain_yunqing-4.0.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-07-05 09:49:44.000000 antchain_yunqing-4.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 09:49:44.000000 antchain_yunqing-4.0.6/antchain_sdk_yunqing/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-05 09:49:44.000000 antchain_yunqing-4.0.6/antchain_sdk_yunqing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   197878 2023-07-05 09:49:44.000000 antchain_yunqing-4.0.6/antchain_sdk_yunqing/client.py
+-rw-r--r--   0 root         (0) root         (0)   566684 2023-07-05 09:49:44.000000 antchain_yunqing-4.0.6/antchain_sdk_yunqing/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 09:49:44.000000 antchain_yunqing-4.0.6/antchain_yunqing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-07-05 09:49:44.000000 antchain_yunqing-4.0.6/antchain_yunqing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      355 2023-07-05 09:49:44.000000 antchain_yunqing-4.0.6/antchain_yunqing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 09:49:44.000000 antchain_yunqing-4.0.6/antchain_yunqing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-05 09:49:44.000000 antchain_yunqing-4.0.6/antchain_yunqing.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-05 09:49:44.000000 antchain_yunqing-4.0.6/antchain_yunqing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-05 09:49:44.000000 antchain_yunqing-4.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-07-05 09:49:44.000000 antchain_yunqing-4.0.6/setup.py
```

### Comparing `antchain_yunqing-4.0.5/LICENSE` & `antchain_yunqing-4.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_yunqing-4.0.5/PKG-INFO` & `antchain_yunqing-4.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_yunqing
-Version: 4.0.5
+Version: 4.0.6
 Summary: Ant Chain YUNQING SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_yunqing-4.0.5/README-CN.md` & `antchain_yunqing-4.0.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_yunqing-4.0.5/README.md` & `antchain_yunqing-4.0.6/README.md`

 * *Files identical despite different names*

### Comparing `antchain_yunqing-4.0.5/antchain_sdk_yunqing/client.py` & `antchain_yunqing-4.0.6/antchain_sdk_yunqing/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '4.0.5',
+                    'sdk_version': '4.0.6',
                     '_prod_code': 'YUNQING',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '4.0.5',
+                    'sdk_version': '4.0.6',
                     '_prod_code': 'YUNQING',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_yunqing-4.0.5/antchain_sdk_yunqing/models.py` & `antchain_yunqing-4.0.6/antchain_sdk_yunqing/models.py`

 * *Files identical despite different names*

### Comparing `antchain_yunqing-4.0.5/antchain_yunqing.egg-info/PKG-INFO` & `antchain_yunqing-4.0.6/antchain_yunqing.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-yunqing
-Version: 4.0.5
+Version: 4.0.6
 Summary: Ant Chain YUNQING SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_yunqing-4.0.5/setup.py` & `antchain_yunqing-4.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_yunqing.
 
-Created on 04/07/2023
+Created on 05/07/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_yunqing"
 NAME = "antchain_yunqing" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain YUNQING SDK Library for Python"
```

