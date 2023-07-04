# Comparing `tmp/usermgr-0.1.0.tar.gz` & `tmp/usermgr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usermgr-0.1.0.tar", max compression
+gzip compressed data, was "usermgr-0.1.1.tar", max compression
```

## Comparing `usermgr-0.1.0.tar` & `usermgr-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2023-06-24 05:20:14.654589 usermgr-0.1.0/LICENSE
--rw-r--r--   0        0        0      396 2023-06-24 11:29:36.602405 usermgr-0.1.0/README.md
--rw-r--r--   0        0        0      588 2023-06-24 23:23:06.135821 usermgr-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      313 2023-06-24 05:20:14.654589 usermgr-0.1.0/usermgr/Factory.py
--rw-r--r--   0        0        0       22 2023-06-24 23:23:13.165818 usermgr-0.1.0/usermgr/__init__.py
--rw-r--r--   0        0        0      994 2023-06-24 13:09:02.722831 usermgr-0.1.0/usermgr/base.py
--rw-r--r--   0        0        0        0 2023-06-24 05:20:14.654589 usermgr-0.1.0/usermgr/providers/__init__.py
--rw-r--r--   0        0        0     3511 2023-06-24 23:22:03.885844 usermgr-0.1.0/usermgr/providers/cognito.py
--rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 usermgr-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-24 05:20:14.654589 usermgr-0.1.1/LICENSE
+-rw-r--r--   0        0        0      396 2023-06-24 11:29:36.602405 usermgr-0.1.1/README.md
+-rw-r--r--   0        0        0      588 2023-07-04 23:20:06.629167 usermgr-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      313 2023-06-24 05:20:14.654589 usermgr-0.1.1/usermgr/Factory.py
+-rw-r--r--   0        0        0       22 2023-07-04 23:20:00.569171 usermgr-0.1.1/usermgr/__init__.py
+-rw-r--r--   0        0        0      994 2023-06-24 13:09:02.722831 usermgr-0.1.1/usermgr/base.py
+-rw-r--r--   0        0        0        0 2023-06-24 05:20:14.654589 usermgr-0.1.1/usermgr/providers/__init__.py
+-rw-r--r--   0        0        0     3628 2023-07-04 23:18:10.049184 usermgr-0.1.1/usermgr/providers/cognito.py
+-rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 usermgr-0.1.1/PKG-INFO
```

### Comparing `usermgr-0.1.0/LICENSE` & `usermgr-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `usermgr-0.1.0/pyproject.toml` & `usermgr-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "usermgr"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["tamuto <tamuto@infodb.jp>"]
 readme = "README.md"
 homepage = "https://github.com/tamuto/usermgr"
 repository = "https://github.com/tamuto/usermgr"
 
 packages = [
```

### Comparing `usermgr-0.1.0/usermgr/base.py` & `usermgr-0.1.1/usermgr/base.py`

 * *Files identical despite different names*

### Comparing `usermgr-0.1.0/usermgr/providers/cognito.py` & `usermgr-0.1.1/usermgr/providers/cognito.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         response = self.idp.admin_create_user(
             UserPoolId=self.user_pool_id,
             Username=username,
             TemporaryPassword=password,
             UserAttributes=[{ "Name": k, "Value": v } for k, v in attrs.items()],
             MessageAction="SUPPRESS"
         )
+        sub_id = [d['Value'] for d in response['User']['Attributes'] if d['Name'] == 'sub'][0]
 
         response = self.idp.admin_initiate_auth(
             UserPoolId=self.user_pool_id,
             ClientId=self.client_id,
             AuthFlow='ADMIN_NO_SRP_AUTH',
             AuthParameters={
                 'USERNAME': username,
@@ -58,14 +59,15 @@
             ChallengeResponses={
                 'USERNAME': username,
                 'NEW_PASSWORD': password,
                 'SECRET_HASH': self._make_hash(username)
             },
             Session=session
         )
+        return sub_id
 
     def update_user(self, username, attrs):
         self.idp.admin_update_user_attributes(
             UserPoolId=self.user_pool_id,
             Username=username,
             UserAttributes=[{ "Name": k, "Value": v } for k, v in attrs.items()],
         )
```

### Comparing `usermgr-0.1.0/PKG-INFO` & `usermgr-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usermgr
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Home-page: https://github.com/tamuto/usermgr
 Author: tamuto
 Author-email: tamuto@infodb.jp
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

