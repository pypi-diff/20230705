# Comparing `tmp/descope-1.5.3.tar.gz` & `tmp/descope-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "descope-1.5.3.tar", max compression
+gzip compressed data, was "descope-1.5.4.tar", max compression
```

## Comparing `descope-1.5.3.tar` & `descope-1.5.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1064 2023-06-28 13:50:17.971236 descope-1.5.3/LICENSE
--rw-r--r--   0        0        0    32364 2023-06-28 13:50:17.971236 descope-1.5.3/README.md
--rw-r--r--   0        0        0      531 2023-06-28 13:50:17.971236 descope-1.5.3/descope/__init__.py
--rw-r--r--   0        0        0      211 2023-06-28 13:50:17.971236 descope-1.5.3/descope/_auth_base.py
--rw-r--r--   0        0        0    21267 2023-06-28 13:50:17.971236 descope-1.5.3/descope/auth.py
--rw-r--r--   0        0        0        0 2023-06-28 13:50:17.971236 descope-1.5.3/descope/authmethod/__init__.py
--rw-r--r--   0        0        0     5352 2023-06-28 13:50:17.971236 descope-1.5.3/descope/authmethod/enchantedlink.py
--rw-r--r--   0        0        0     6211 2023-06-28 13:50:17.971236 descope-1.5.3/descope/authmethod/magiclink.py
--rw-r--r--   0        0        0     1528 2023-06-28 13:50:17.971236 descope-1.5.3/descope/authmethod/oauth.py
--rw-r--r--   0        0        0    11078 2023-06-28 13:50:17.971236 descope-1.5.3/descope/authmethod/otp.py
--rw-r--r--   0        0        0     8150 2023-06-28 13:50:17.971236 descope-1.5.3/descope/authmethod/password.py
--rw-r--r--   0        0        0     1481 2023-06-28 13:50:17.971236 descope-1.5.3/descope/authmethod/saml.py
--rw-r--r--   0        0        0     5128 2023-06-28 13:50:17.971236 descope-1.5.3/descope/authmethod/totp.py
--rw-r--r--   0        0        0     6705 2023-06-28 13:50:17.971236 descope-1.5.3/descope/authmethod/webauthn.py
--rw-r--r--   0        0        0     4266 2023-06-28 13:50:17.971236 descope-1.5.3/descope/common.py
--rw-r--r--   0        0        0    12089 2023-06-28 13:50:17.971236 descope-1.5.3/descope/descope_client.py
--rw-r--r--   0        0        0     1420 2023-06-28 13:50:17.971236 descope-1.5.3/descope/exceptions.py
--rw-r--r--   0        0        0     5809 2023-06-28 13:50:17.971236 descope-1.5.3/descope/management/access_key.py
--rw-r--r--   0        0        0     4604 2023-06-28 13:50:17.971236 descope-1.5.3/descope/management/audit.py
--rw-r--r--   0        0        0     4155 2023-06-28 13:50:17.971236 descope-1.5.3/descope/management/common.py
--rw-r--r--   0        0        0     3904 2023-06-28 13:50:17.971236 descope-1.5.3/descope/management/flow.py
--rw-r--r--   0        0        0     3971 2023-06-28 13:50:17.971236 descope-1.5.3/descope/management/group.py
--rw-r--r--   0        0        0      959 2023-06-28 13:50:17.971236 descope-1.5.3/descope/management/jwt.py
--rw-r--r--   0        0        0     2535 2023-06-28 13:50:17.971236 descope-1.5.3/descope/management/permission.py
--rw-r--r--   0        0        0     3098 2023-06-28 13:50:17.971236 descope-1.5.3/descope/management/role.py
--rw-r--r--   0        0        0     6386 2023-06-28 13:50:17.971236 descope-1.5.3/descope/management/sso_settings.py
--rw-r--r--   0        0        0     3689 2023-06-28 13:50:17.971236 descope-1.5.3/descope/management/tenant.py
--rw-r--r--   0        0        0    31376 2023-06-28 13:50:17.971236 descope-1.5.3/descope/management/user.py
--rw-r--r--   0        0        0     1710 2023-06-28 13:50:17.971236 descope-1.5.3/descope/mgmt.py
--rw-r--r--   0        0        0     1220 2023-06-28 13:50:46.119566 descope-1.5.3/pyproject.toml
--rw-r--r--   0        0        0    33384 1970-01-01 00:00:00.000000 descope-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-05 14:52:31.310171 descope-1.5.4/LICENSE
+-rw-r--r--   0        0        0    32364 2023-07-05 14:52:31.310171 descope-1.5.4/README.md
+-rw-r--r--   0        0        0      560 2023-07-05 14:52:31.310171 descope-1.5.4/descope/__init__.py
+-rw-r--r--   0        0        0      211 2023-07-05 14:52:31.310171 descope-1.5.4/descope/_auth_base.py
+-rw-r--r--   0        0        0    21253 2023-07-05 14:52:31.310171 descope-1.5.4/descope/auth.py
+-rw-r--r--   0        0        0        0 2023-07-05 14:52:31.310171 descope-1.5.4/descope/authmethod/__init__.py
+-rw-r--r--   0        0        0     5352 2023-07-05 14:52:31.310171 descope-1.5.4/descope/authmethod/enchantedlink.py
+-rw-r--r--   0        0        0     6211 2023-07-05 14:52:31.310171 descope-1.5.4/descope/authmethod/magiclink.py
+-rw-r--r--   0        0        0     1528 2023-07-05 14:52:31.310171 descope-1.5.4/descope/authmethod/oauth.py
+-rw-r--r--   0        0        0    11078 2023-07-05 14:52:31.310171 descope-1.5.4/descope/authmethod/otp.py
+-rw-r--r--   0        0        0     8150 2023-07-05 14:52:31.310171 descope-1.5.4/descope/authmethod/password.py
+-rw-r--r--   0        0        0     1481 2023-07-05 14:52:31.310171 descope-1.5.4/descope/authmethod/saml.py
+-rw-r--r--   0        0        0     5128 2023-07-05 14:52:31.310171 descope-1.5.4/descope/authmethod/totp.py
+-rw-r--r--   0        0        0     6705 2023-07-05 14:52:31.310171 descope-1.5.4/descope/authmethod/webauthn.py
+-rw-r--r--   0        0        0     4266 2023-07-05 14:52:31.310171 descope-1.5.4/descope/common.py
+-rw-r--r--   0        0        0    12089 2023-07-05 14:52:31.310171 descope-1.5.4/descope/descope_client.py
+-rw-r--r--   0        0        0     1420 2023-07-05 14:52:31.310171 descope-1.5.4/descope/exceptions.py
+-rw-r--r--   0        0        0     5809 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/access_key.py
+-rw-r--r--   0        0        0     4604 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/audit.py
+-rw-r--r--   0        0        0     4155 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/common.py
+-rw-r--r--   0        0        0     3904 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/flow.py
+-rw-r--r--   0        0        0     3971 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/group.py
+-rw-r--r--   0        0        0      959 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/jwt.py
+-rw-r--r--   0        0        0     2535 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/permission.py
+-rw-r--r--   0        0        0     3098 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/role.py
+-rw-r--r--   0        0        0     6386 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/sso_settings.py
+-rw-r--r--   0        0        0     3689 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/tenant.py
+-rw-r--r--   0        0        0    31376 2023-07-05 14:52:31.310171 descope-1.5.4/descope/management/user.py
+-rw-r--r--   0        0        0     1710 2023-07-05 14:52:31.310171 descope-1.5.4/descope/mgmt.py
+-rw-r--r--   0        0        0     1220 2023-07-05 14:52:59.885985 descope-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0    33384 1970-01-01 00:00:00.000000 descope-1.5.4/PKG-INFO
```

### Comparing `descope-1.5.3/LICENSE` & `descope-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/README.md` & `descope-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/__init__.py` & `descope-1.5.4/descope/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,12 +7,13 @@
     DeliveryMethod,
     LoginOptions,
 )
 from descope.descope_client import DescopeClient
 from descope.exceptions import (
     API_RATE_LIMIT_RETRY_AFTER_HEADER,
     ERROR_TYPE_API_RATE_LIMIT,
+    ERROR_TYPE_SERVER_ERROR,
     AuthException,
     RateLimitException,
 )
 from descope.management.common import AssociatedTenant
 from descope.management.sso_settings import AttributeMapping, RoleMapping
```

### Comparing `descope-1.5.3/descope/auth.py` & `descope-1.5.4/descope/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,15 +333,15 @@
 
         if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
             self._raise_rate_limit_exception(response)  # Raise RateLimitException
 
         raise AuthException(
             response.status_code,
             ERROR_TYPE_SERVER_ERROR,
-            f"Error: {response.reason}",
+            response.text,
         )
 
     def _fetch_public_keys(self) -> None:
         # This function called under mutex protection so no need to acquire it once again
         response = requests.get(
             f"{self.base_url}{EndpointsV2.public_key_path}/{self.project_id}",
             headers=self._get_default_headers(),
```

### Comparing `descope-1.5.3/descope/authmethod/enchantedlink.py` & `descope-1.5.4/descope/authmethod/enchantedlink.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/authmethod/magiclink.py` & `descope-1.5.4/descope/authmethod/magiclink.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/authmethod/oauth.py` & `descope-1.5.4/descope/authmethod/oauth.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/authmethod/otp.py` & `descope-1.5.4/descope/authmethod/otp.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/authmethod/password.py` & `descope-1.5.4/descope/authmethod/password.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/authmethod/saml.py` & `descope-1.5.4/descope/authmethod/saml.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/authmethod/totp.py` & `descope-1.5.4/descope/authmethod/totp.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/authmethod/webauthn.py` & `descope-1.5.4/descope/authmethod/webauthn.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/common.py` & `descope-1.5.4/descope/common.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/descope_client.py` & `descope-1.5.4/descope/descope_client.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/exceptions.py` & `descope-1.5.4/descope/exceptions.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/management/access_key.py` & `descope-1.5.4/descope/management/access_key.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/management/audit.py` & `descope-1.5.4/descope/management/audit.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/management/common.py` & `descope-1.5.4/descope/management/common.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/management/flow.py` & `descope-1.5.4/descope/management/flow.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/management/group.py` & `descope-1.5.4/descope/management/group.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/management/jwt.py` & `descope-1.5.4/descope/management/jwt.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/management/permission.py` & `descope-1.5.4/descope/management/permission.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/management/role.py` & `descope-1.5.4/descope/management/role.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/management/sso_settings.py` & `descope-1.5.4/descope/management/sso_settings.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/management/tenant.py` & `descope-1.5.4/descope/management/tenant.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/management/user.py` & `descope-1.5.4/descope/management/user.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/descope/mgmt.py` & `descope-1.5.4/descope/mgmt.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.3/pyproject.toml` & `descope-1.5.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "descope"
-version = "1.5.3"
+version = "1.5.4"
 description = "Descope Python SDK"
 authors = ["Descope <info@descope.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://descope.com/"
 repository = "https://github.com/descope/python-sdk"
 documentation = "https://docs.descope.com"
```

### Comparing `descope-1.5.3/PKG-INFO` & `descope-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: descope
-Version: 1.5.3
+Version: 1.5.4
 Summary: Descope Python SDK
 Home-page: https://descope.com/
 License: MIT
 Author: Descope
 Author-email: info@descope.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

