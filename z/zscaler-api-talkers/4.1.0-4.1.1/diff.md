# Comparing `tmp/zscaler_api_talkers-4.1.0.tar.gz` & `tmp/zscaler_api_talkers-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zscaler_api_talkers-4.1.0.tar", max compression
+gzip compressed data, was "zscaler_api_talkers-4.1.1.tar", max compression
```

## Comparing `zscaler_api_talkers-4.1.0.tar` & `zscaler_api_talkers-4.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1071 2022-04-21 16:27:44.526756 zscaler_api_talkers-4.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2679 2023-06-27 21:07:15.062084 zscaler_api_talkers-4.1.0/README.md
--rw-r--r--   0        0        0      454 2023-06-27 20:53:48.702831 zscaler_api_talkers-4.1.0/pyproject.toml
--rw-r--r--   0        0        0      435 2023-06-27 20:53:48.706237 zscaler_api_talkers-4.1.0/zscaler_api_talkers/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 20:53:48.706445 zscaler_api_talkers-4.1.0/zscaler_api_talkers/models/__init__.py
--rw-r--r--   0        0        0    13788 2023-06-27 20:53:48.707682 zscaler_api_talkers-4.1.0/zscaler_api_talkers/models/models.py
--rw-r--r--   0        0        0        0 2023-06-27 20:53:48.707836 zscaler_api_talkers-4.1.0/zscaler_api_talkers/zcc_talker/__init__.py
--rw-r--r--   0        0        0     4910 2023-06-27 20:53:48.708260 zscaler_api_talkers-4.1.0/zscaler_api_talkers/zcc_talker/zcc_talker.py
--rw-r--r--   0        0        0        0 2023-06-27 20:53:48.708427 zscaler_api_talkers-4.1.0/zscaler_api_talkers/zdx_talker/__init__.py
--rw-r--r--   0        0        0    11378 2023-06-27 20:53:48.708864 zscaler_api_talkers-4.1.0/zscaler_api_talkers/zdx_talker/zdx_portaltalker.py
--rw-r--r--   0        0        0        0 2023-06-27 20:53:48.709020 zscaler_api_talkers-4.1.0/zscaler_api_talkers/zia_talker/__init__.py
--rw-r--r--   0        0        0    14967 2023-06-27 20:53:48.709468 zscaler_api_talkers-4.1.0/zscaler_api_talkers/zia_talker/zia_portaltalker.py
--rw-r--r--   0        0        0    68927 2023-06-27 20:53:48.710260 zscaler_api_talkers-4.1.0/zscaler_api_talkers/zia_talker/zia_talker.py
--rw-r--r--   0        0        0        0 2023-06-27 20:53:48.710832 zscaler_api_talkers-4.1.0/zscaler_api_talkers/zpa_talker/__init__.py
--rw-r--r--   0        0        0     2385 2023-06-27 20:53:48.711212 zscaler_api_talkers-4.1.0/zscaler_api_talkers/zpa_talker/zpa_portaltalker.py
--rw-r--r--   0        0        0    22707 2023-06-27 20:53:48.712114 zscaler_api_talkers-4.1.0/zscaler_api_talkers/zpa_talker/zpa_talker.py
--rw-r--r--   0        0        0      205 2023-06-27 20:53:48.717944 zscaler_api_talkers-4.1.0/zscaler_api_talkers/zscaler_helpers/__init__.py
--rw-r--r--   0        0        0     7782 2023-06-27 20:53:48.718457 zscaler_api_talkers-4.1.0/zscaler_api_talkers/zscaler_helpers/http_calls.py
--rw-r--r--   0        0        0     1707 2023-06-27 20:53:48.718942 zscaler_api_talkers-4.1.0/zscaler_api_talkers/zscaler_helpers/logger.py
--rw-r--r--   0        0        0     6487 2023-06-27 20:53:48.719333 zscaler_api_talkers-4.1.0/zscaler_api_talkers/zscaler_helpers/utilities.py
--rw-r--r--   0        0        0     3169 1970-01-01 00:00:00.000000 zscaler_api_talkers-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-04-21 16:27:44.526756 zscaler_api_talkers-4.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     4541 2023-07-05 00:56:15.951278 zscaler_api_talkers-4.1.1/README.md
+-rw-r--r--   0        0        0      434 2023-07-05 03:00:17.891927 zscaler_api_talkers-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0      441 2023-07-05 01:15:40.406964 zscaler_api_talkers-4.1.1/zscaler_api_talkers/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 20:53:48.707836 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zcc_talker/__init__.py
+-rw-r--r--   0        0        0     7195 2023-07-05 01:15:40.407601 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zcc_talker/zcc_talker.py
+-rw-r--r--   0        0        0        0 2023-06-27 20:53:48.708427 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zdx_talker/__init__.py
+-rw-r--r--   0        0        0    14324 2023-07-05 01:15:40.408211 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zdx_talker/zdx_portaltalker.py
+-rw-r--r--   0        0        0        0 2023-06-27 20:53:48.709020 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zia_talker/__init__.py
+-rw-r--r--   0        0        0     1144 2023-07-05 01:15:40.408775 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zia_talker/helpers.py
+-rw-r--r--   0        0        0    13788 2023-06-29 23:34:03.620027 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zia_talker/models.py
+-rw-r--r--   0        0        0    15558 2023-07-05 01:15:40.409383 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zia_talker/zia_portaltalker.py
+-rw-r--r--   0        0        0    75250 2023-07-05 01:15:40.410190 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zia_talker/zia_talker.py
+-rw-r--r--   0        0        0        0 2023-06-27 20:53:48.710832 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zpa_talker/__init__.py
+-rw-r--r--   0        0        0     3627 2023-07-05 01:15:40.410779 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zpa_talker/zpa_portaltalker.py
+-rw-r--r--   0        0        0    26074 2023-07-05 01:15:40.411442 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zpa_talker/zpa_talker.py
+-rw-r--r--   0        0        0      205 2023-07-05 00:56:15.958091 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zscaler_helpers/__init__.py
+-rw-r--r--   0        0        0     8820 2023-07-05 00:56:15.958333 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zscaler_helpers/http_calls.py
+-rw-r--r--   0        0        0     1724 2023-07-05 00:56:15.958655 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zscaler_helpers/logger.py
+-rw-r--r--   0        0        0     6482 2023-07-05 00:56:15.958902 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zscaler_helpers/utilities.py
+-rw-r--r--   0        0        0     5185 1970-01-01 00:00:00.000000 zscaler_api_talkers-4.1.1/PKG-INFO
```

### Comparing `zscaler_api_talkers-4.1.0/LICENSE.txt` & `zscaler_api_talkers-4.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-4.1.0/zscaler_api_talkers/models/models.py` & `zscaler_api_talkers-4.1.1/zscaler_api_talkers/zia_talker/models.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-4.1.0/zscaler_api_talkers/zdx_talker/zdx_portaltalker.py` & `zscaler_api_talkers-4.1.1/zscaler_api_talkers/zdx_talker/zdx_portaltalker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 import urllib
 
+import json
 import requests
-from zscaler_helpers import _request, get_user_agent, setup_logger
+from zscaler_api_talkers.zscaler_helpers import request_, get_user_agent, setup_logger
 
 logger = setup_logger(name=__name__)
 
 
 class ZdxPortalTalker:
     def __init__(
         self,
         username: str,
         password: str,
         zia_cloud: str,
     ):
+        """Class object to provide access to ZDX via web portal backend APIs.
+
+        :param username: (str) Admin username
+        :param password: (str) Admin password
+        :param zia_cloud: (str) ZIA Portal associated with this ZDX tenant. Example: "zscalerthree.net"
+        """
+        logger.warning("These API endpoints are unsupported and Zscaler can change at will and without notice.")
         self.username = username
         self.password = password
         self.base_url = "https://admin.zdxcloud.net"
         self.api_base_url = f"{self.base_url}/zdx/api/v1"
         self.headers = {
             "User-Agent": get_user_agent(),
             "X-CSRF-Token": "Fetch",
@@ -41,17 +49,18 @@
         }
         self.zia_base_url = ""  # This will be properly configured after ZIA Auth.
 
     def _authenticate(
         self,
         **kwargs,
     ):
+        """Authenticate to ZDX Web Portal"""
         url = f"{self.api_base_url}/auth"
         #  Expect 401 status code; we just want the headers/cookies that get returned.
-        result = _request(
+        result = request_(
             method="get",
             url=url,
             headers=self.headers,
             retries=1,
             wait_time=0.1,
             **kwargs,
         )
@@ -61,178 +70,232 @@
                 "X-CSRF-Token": result.headers["X-CSRF-Token"],
                 "Origin": self.base_url,
                 "Referer": f"{self.base_url}/zdx/login",
                 "Content-Type": "application/json",
             }
         )
         data = {
-            "username": f"zdx-{self.username}",
+            "username": self.username,
             "password": self.password,
         }
-        result = _request(
+        result = request_(
             method="post",
             url=url,
             headers=self.headers,
             json=data,
             cookies=self.cookie_jar,
             **kwargs,
         )
         self.cookie_jar.update(result.cookies)
 
-    def get_alerts(
+    def list_alerts(
         self,
         **kwargs,
-    ) -> requests.Response:
-        result = _request(
+    ) -> json:
+        """
+        Collect a list of ZDX Alerts.
+
+        :return: (json)
+        """
+        result = request_(
             method="get",
             url=f"{self.api_base_url}/alerts/summaries",
             headers=self.headers,
             cookies=self.cookie_jar,
             **kwargs,
         )
-        return result
+        return result.json()
 
     def delete_alert(
         self,
         data: dict,
         **kwargs,
-    ) -> requests.Response:
-        result = _request(
+    ) -> json:
+        """
+        Delete Alert.
+
+        :param data: (dict) Dict of select Alert.  # TODO: Can this just be the alert_id?
+
+        :return: (json)
+        """
+        result = request_(
             method="delete",
             url=f"{self.api_base_url}/alerts/{data['id']}",
             json=data,
             headers=self.headers,
             cookies=self.cookie_jar,
             **kwargs,
         )
-        return result
+        return result.json()
 
     def activate(
         self,
         **kwargs,
-    ) -> requests.Response:
-        result = _request(
+    ) -> json:
+        """
+        Activate Changes.
+
+        :return: (json)
+        """
+        result = request_(
             method="put",
             url=f"{self.api_base_url}/activate",
             headers=self.headers,
             cookies=self.cookie_jar,
             **kwargs,
         )
-        return result
+        return result.json()
 
-    def get_applications(
+    def list_applications(
         self,
         **kwargs,
-    ) -> requests.Response:
-        result = _request(
+    ) -> json:
+        """
+        Collect a list of ZDX Applications
+
+        :return: (json)
+        """
+        result = request_(
             method="get",
             url=f"{self.api_base_url}/applications",
             headers=self.headers,
             cookies=self.cookie_jar,
             **kwargs,
         )
-        return result
+        return result.json()
 
     def update_application(
         self,
         data: dict,
         **kwargs,
-    ) -> requests.Response:
-        result = _request(
+    ) -> json:
+        """
+        Update an Application
+
+        :return: (json)
+        """
+        result = request_(
             method="put",
             url=f"{self.api_base_url}/applications/{data['id']}",
             json=data,
             headers=self.headers,
             cookies=self.cookie_jar,
             **kwargs,
         )
-        return result
+        return result.json()
 
     def deactivate_application(
         self,
         app_id: str,
         **kwargs,
-    ) -> requests.Response:
-        result = _request(
+    ) -> json:
+        """
+        Deactivate an Application
+
+        :return: (json)
+        """
+        result = request_(
             method="put",
             url=f"{self.api_base_url}/applications/{app_id}/deactivate",
             headers=self.headers,
             cookies=self.cookie_jar,
             **kwargs,
         )
-        return result
+        return result.json()
 
     def delete_application(
         self,
         data: dict,
         **kwargs,
-    ) -> requests.Response:
-        result = _request(
+    ) -> json:
+        """
+        Delete a ZDX Application
+
+        :param data: (dict) Dict of Application  # TODO: Can this be changed to just be the app_id?
+
+        :return: json
+        """
+        result = request_(
             method="delete",
             url=f"{self.api_base_url}/applications/{data['id']}",
             json=data,
             headers=self.headers,
             cookies=self.cookie_jar,
             **kwargs,
         )
-        return result
+        return result.json()
 
-    def get_probes(
+    def list_probes(
         self,
         **kwargs,
-    ) -> requests.Response:
+    ) -> json:
+        """
+        Collect a list of ZDX Probes
+
+        :return: (json)
+        """
         parameters = {
             "pageName": "PROBES",
         }
-        result = _request(
+        result = request_(
             method="get",
             url=f"{self.api_base_url}/monitors/summary",
             params=parameters,
             headers=self.headers,
             cookies=self.cookie_jar,
             **kwargs,
         )
-        return result
+        return result.json()
 
     def delete_probe(
         self,
         app_id: str,
         probe_id: str,
         **kwargs,
-    ) -> requests.Response:
-        result = _request(
+    ) -> json:
+        """
+        Delete specific Application's Probe
+
+        :param app_id: (str) ID of Application
+        :param probe_id: (str) ID of Probe
+
+        :return: (json)
+        """
+        result = request_(
             method="delete",
             url=f"{self.api_base_url}/applications/{app_id}/monitors/{probe_id}",
             headers=self.headers,
             cookies=self.cookie_jar,
             **kwargs,
         )
-        return result
+        return result.json()
 
     def zia_authenticate(
         self,
         **kwargs,
     ):
-        """You need to cross authenticate into ZIA to work on the Admin accounts."""
-        result = _request(
+        """Cross authentication into ZIA to work on user and roles."""
+        logger.warning("Regular ZDX methods will no longer work after ZIA auth.  Create a new ZdxPortalTalker object "
+                       "if further access is needed.")
+        result = request_(
             method="post",
             url=f"{self.api_base_url}/auth/token",
             headers=self.headers,
             data=f'["{self.zia_cloud}"]',
             cookies=self.cookie_jar,
             **kwargs,
         )
         saml = result.json()
 
         payload = (
             f"SAMLResponse={urllib.parse.quote(saml['token'])}"
             f"&source=SMFALCONUI"
             f"&relay={urllib.parse.quote('#administration/admin-management')}"
         )
-        sso = _request(
+        sso = request_(
             method="post",
             url=saml["acceptedTargets"][0]["url"],
             headers=self.zia_headers,
             data=payload,
             cookies=self.cookie_jar,
             allow_redirects=False,
             **kwargs,
@@ -250,173 +313,239 @@
         self.zia_base_url = f"https://admin.{saml['cloud']}/zsapi/v1"
 
     def zia_upload_certificate(
         self,
         filename: str,
         certificate: str,
         **kwargs,
-    ) -> requests.Response:
+    ) -> json:
+        """
+        Upload a certificate to ZIA (for ZDX Admin auth)
+
+        :param filename: (str) Name representation of this cert.
+        :param certificate: (str) x509-ca-cert formatted cert.
+
+        :return: (json)
+        """
         file = [
             (
                 "fileUpload",
                 (
                     filename,
                     certificate,
                     "application/x-x509-ca-cert",
                 ),
             )
         ]
-        result = _request(
+        result = request_(
             method="post",
             url=f"{self.zia_base_url}/samlAdminSettings/uploadCert/text",
             files=file,
             headers=self.zia_headers,
             cookies=self.cookie_jar,
             **kwargs,
         )
-        return result
+        return result.json()
 
     def zia_enable_saml_sso(
         self,
         data: dict,
         **kwargs,
-    ) -> requests.Response:
+    ) -> json:
+        """
+        Enable SAML SSO
+
+        :param data: (dict)
+
+        :return: (json)
+        """
         self.zia_headers.update(
             {
                 "Content-Type": "application/json",
             }
         )
-        result = _request(
+        result = request_(
             method="put",
             url=f"{self.zia_base_url}/samlAdminSettings",
             json=data,
             headers=self.zia_headers,
             cookies=self.cookie_jar,
             **kwargs,
         )
-        return result
+        return result.json()
 
     def zia_activate(
         self,
         **kwargs,
-    ) -> requests.Response:
-        result = _request(
+    ) -> json:
+        """
+        Activate changes in ZIA Portal
+
+        :return: (json)
+        """
+        result = request_(
             method="put",
             url=f"{self.zia_base_url}/orgAdminStatus/activate",
             headers=self.zia_headers,
             cookies=self.cookie_jar,
             **kwargs,
         )
-        return result
+        return result.json()
 
-    def zia_get_admin_roles(
+    def zia_list_admin_roles(
         self,
         **kwargs,
-    ) -> requests.Response:
+    ) -> json:
+        """
+        Collect a list of Admin Roles.
+
+        :return: (json)
+        """
         parameters = {
             "includeAuditorRole": False,
             "includePartnerRole": False,
             "includeApiRole": False,
         }
-        result = _request(
+        result = request_(
             method="get",
             url=f"{self.zia_base_url}/adminRoles",
             params=parameters,
             headers=self.zia_headers,
             cookies=self.cookie_jar,
             **kwargs,
         )
-        return result
+        return result.json()
 
-    def zia_create_admin_role(
+    def zia_add_admin_role(
         self,
         data: dict,
         **kwargs,
-    ) -> requests.Response:
-        result = _request(
+    ) -> json:
+        """
+        Add an Admin Role
+
+        :param data: (dict) Admin role configuration
+
+        :return: (json)
+        """
+        result = request_(
             method="post",
             url=f"{self.zia_base_url}/adminRoles",
             json=data,
             headers=self.zia_headers,
             cookies=self.cookie_jar,
             **kwargs,
         )
-        return result
+        return result.json()
 
     def zia_delete_admin_role(
         self,
         role_id: int,
         **kwargs,
-    ) -> requests.Response:
-        result = _request(
+    ) -> json:
+        """
+        Delete an Admin Role
+
+        :param role_id: (int) ID of role
+
+        :return: (json)
+        """
+        result = request_(
             method="delete",
             url=f"{self.zia_base_url}/adminRoles/{role_id}",
             headers=self.zia_headers,
             cookies=self.cookie_jar,
             **kwargs,
         )
-        return result
+        return result.json()
 
-    def zia_get_admin_users(
+    def zia_list_admin_users(
         self,
         **kwargs,
-    ) -> requests.Response:
+    ) -> json:
+        """
+        Collect a list of ZDX Admin Users
+
+        :return: (json)
+        """
         parameters = {
-            "page": 1,
+            "page": 1,  # TODO: Change this and pageSize to an interator
             "pageSize": 100,
             "includeAuditorUsers": False,
             "includeAdminUsers": True,
         }
-        result = _request(
+        result = request_(
             method="get",
             url=f"{self.zia_base_url}/adminUsers",
             params=parameters,
             headers=self.zia_headers,
             cookies=self.cookie_jar,
             **kwargs,
         )
-        return result
+        return result.json()
 
     def zia_delete_admin_user(
         self,
         user_id: int,
         **kwargs,
-    ) -> requests.Response:
-        result = _request(
+    ) -> json:
+        """
+        Delete a ZDX Admin User
+
+        :param user_id: (int) ID of User
+
+        :return: (json)
+        """
+        result = request_(
             method="delete",
             url=f"{self.zia_base_url}/adminUsers/{user_id}",
             headers=self.zia_headers,
             cookies=self.cookie_jar,
             **kwargs,
         )
-        return result
+        return result.json()
 
-    def zia_create_admin_user(
+    def zia_add_admin_user(
         self,
         data: dict,
         **kwargs,
-    ) -> requests.Response:
-        result = _request(
+    ) -> json:
+        """
+        Add a ZDX Admin User
+
+        :param data: (dict) Dict of Admin user settings
+
+        :return: (json)
+        """
+        result = request_(
             method="post",
             url=f"{self.zia_base_url}/adminUsers",
             json=data,
             headers=self.zia_headers,
             cookies=self.cookie_jar,
             **kwargs,
         )
-        return result
+        return result.json()
 
     def zia_update_admin_user(
         self,
         data: dict,
-        user_id: str,
+        user_id: int,
         **kwargs,
-    ) -> requests.Response:
-        result = _request(
+    ) -> json:
+        """
+        Update settings for a ZDX Admin User
+
+        :param data: (dict) Settings for this admin user
+        :param user_id: (int) ID of this user  # TODO: Can't this just be in the data var?
+
+        :return: (json)
+        """
+        result = request_(
             method="put",
             url=f"{self.zia_base_url}/adminUsers/{user_id}",
             json=data,
             headers=self.zia_headers,
             cookies=self.cookie_jar,
             **kwargs,
         )
-        return result
+        return result.json()
```

### Comparing `zscaler_api_talkers-4.1.0/zscaler_api_talkers/zia_talker/zia_portaltalker.py` & `zscaler_api_talkers-4.1.1/zscaler_api_talkers/zia_talker/zia_portaltalker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,491 +1,559 @@
-import time
-from getpass import getpass
+import json
 
-from zscaler_helpers import HttpCalls
+import requests
+from zscaler_api_talkers.zscaler_helpers import HttpCalls, setup_logger, request_
+
+from .helpers import _get_seed, _obfuscate_api_key
+
+logger = setup_logger(name=__name__)
 
 
 class ZiaPortalTalker(object):
     """
     ZIA Portal API talker
     Documentation: https://help.zscaler.com/zia/zia-api/api-developer-reference-guide
     """
 
-    def __init__(self, cloud_name):
+    def __init__(
+        self,
+        cloud_name: str,
+        username: str = "",
+        password: str = "",
+    ):
         """
         Method to start the class
-        :param cloud_name: type string. Example: zscalerbeta.net, zscalerone.net, zscalertwo.net
-        zscalerthree.net, zscaler.net, zscloud.net
+
+        :param cloud_name: (str) Example: zscalerbeta.net, zscalerone.net, zscalertwo.net, zscalerthree.net,
+        zscaler.net, zscloud.net
+        :param username: (str) Client ID
+        :param password: (str) Secret Key
         """
+        self.cloud_name = cloud_name
         self.base_uri = f"https://admin.{cloud_name}/zsapi/v1"
-        self.hp_http = HttpCalls(host=self.base_uri, verify=True)
-        self.jsessionid = None
+        self.hp_http = HttpCalls(
+            host=self.base_uri,
+            verify=True,
+        )
+        self.j_session_id = None
         self.zs_session_code = None
         self.headers = None
         self.version = "0.1"
-
-    def _obfuscateApiKey(self, seed):
-        """
-        Internal method to Obfuscate the API key
-        :param seed: API key
-        :return: timestamp,obfuscated key
-        """
-        now = int(time.time() * 1000)
-        n = str(now)[-6:]
-        r = str(int(n) >> 1).zfill(6)
-        key = ""
-        for i in range(0, len(str(n)), 1):
-            key += seed[int(str(n)[i])]
-        for j in range(0, len(str(r)), 1):
-            key += seed[int(str(r)[j]) + 2]
-        return now, key
+        if username and password:
+            self.authenticate(
+                username=username,
+                password=password,
+            )
 
     def authenticate(
         self,
-        apikey,
-        username,
-        password=None,
+        username: str,
+        password: str,
     ):
         """
         Method to authenticate.
-        :param apikey: API key
-        :param username: A string that contains the email ID of the API admin
-        :param password: A string that contains the password for the API admin
-        :return:  JSESSIONID. This cookie expires by default 30 minutes from last request
-        """
-        if not password:
-            password = getpass(" Introduce password: ")
-        timestamp, key = self._obfuscateApiKey("jj7tg80fEGao")
 
+        :param username: (str) A string that contains the email ID of the API admin
+        :param password: (str) A string that contains the password for the API admin
+        """
+        timestamp, key = _obfuscate_api_key(
+            _get_seed(url=f"https://admin.{self.cloud_name}")
+        )
         payload = {
             "apiKey": key,
             "username": username,
             "password": password,
             "timestamp": timestamp,
         }
         url = "/authenticatedSession"
         response = self.hp_http.post_call(
-            url=url, payload=payload, headers={"Accept": "application/json"}
+            url=url,
+            payload=payload,
+            headers={
+                "Accept": "application/json",
+            },
         )
         if response.cookies.get("JSESSIONID"):
-            self.jsessionid = response.cookies["JSESSIONID"]
+            self.j_session_id = response.cookies["JSESSIONID"]
         else:
             raise ValueError("Invalid Credentials")
         if response.cookies.get("ZS_SESSION_CODE"):
             self.zs_session_code = response.cookies["ZS_SESSION_CODE"]
             self.headers = {
                 "Content-Type": "application/json",
                 "ZS_CUSTOM_CODE": self.zs_session_code,
             }
         else:
             raise ValueError("Invalid API key")
 
-    def add_dlpEngine(
+    def add_dlp_engine(
         self,
-        payload=None,
-        EngineExpression=None,
-        Name=None,
-        CustomDlpEngine=True,
-        PredefinedEngineName=None,
-        Description=None,
-    ):
+        payload: dict = None,
+        engine_expression: str = None,
+        name: str = None,
+        custom_dlp_engine: bool = True,
+        predefined_engine_name: bool = None,
+        description: str = None,
+    ) -> requests.Response:
         """
         Method to create a DLP engine
-        :param Name: type string. Name of the DLP ENGINE
-        :param EngineExpression: type string. Engine Expression
-        :param CustomDlpEngine: : type boolean. True if custom DLP engine
-        :param PredefinedEngineName: type boolean.
-        :param Description: type string. Description
-        :return:
+
+        :param payload: (dict?)
+        :param name: (str) Name of the DLP ENGINE
+        :param engine_expression: (str) Engine Expression
+        :param custom_dlp_engine: : (bool) True if custom DLP engine
+        :param predefined_engine_name: (bool)
+        :param description: (str) Description
+
+        :return: requests.Response object
         """
         url = "/dlpEngines"
         if payload:
             payload = payload
         else:
             payload = {
-                "EngineExpression": EngineExpression,
-                "CustomDlpEngine": CustomDlpEngine,
+                "EngineExpression": engine_expression,
+                "CustomDlpEngine": custom_dlp_engine,
             }
-            if PredefinedEngineName:
-                payload.update(PredefinedEngineName=PredefinedEngineName)
+            if predefined_engine_name:
+                payload.update(PredefinedEngineName=predefined_engine_name)
             else:
-                payload.update(Name=Name)
-
-            if Description:
-                payload.update(Description=Description)
+                payload.update(Name=name)
+            if description:
+                payload.update(Description=description)
         response = self.hp_http.post_call(
             url=url,
             payload=payload,
             headers=self.headers,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
+
         return response
 
-    def update_dlpEngine(self, payload, id):
+    def update_dlp_engine(
+        self,
+        payload: json,
+        dlp_id: int,
+    ) -> requests.Response:
         """
         Method to update a DLP engine
-        :param payload: type json. payload
-        :return:
+
+        :param payload: (json) payload
+        :param dlp_id: (int) ID
+
+        :return: requests.Response object
         """
-        url = f"/dlpEngines/{id}"
+        url = f"/dlpEngines/{dlp_id}"
         response = self.hp_http.put_call(
             url=url,
             payload=payload,
             headers=self.headers,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
+
         return response
 
-    def list_PacFiles(self):
+    def list_pac_files(self) -> json:
         """
         Method to list PAC files
-        :return: json
+
+        :return: (json)
         """
         url = f"/pacFiles"
         response = self.hp_http.get_call(
             url=url,
             headers=self.headers,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
+
         return response.json()
 
-    def add_PacFile(
+    def add_pac_file(
         self,
-        name,
-        description,
-        domain,
-        PacContent,
-        editable=True,
-        pacUrlObfuscated=True,
-    ):
+        name: str,
+        description: str,
+        domain: str,
+        pac_content: str,
+        editable: bool = True,
+        pac_url_obfuscated: bool = True,
+    ) -> json:
         """
         Method to Add a PAC file
-        :param name: type string. Name of the PAC
-        :param description: type string. Description
-        :param domain: type string. Domain
-        :param PacContent: Type string: PAC content
-        :param editable: Type boolean. Default True
-        :param pacUrlObfuscated: Type boolean. Default True
-        :return:
+
+        :param name: (str) Name of the PAC
+        :param description: (str) Description
+        :param domain: (str) Domain
+        :param pac_content: (str) PAC content
+        :param editable: (bool) Default True
+        :param pac_url_obfuscated: (bool) Default True
+
+        :return: (json)
         """
         payload = {
             "name": name,
             "editable": editable,
-            "pacContent": PacContent,
-            "pacUrlObfuscated": pacUrlObfuscated,
+            "pacContent": pac_content,
+            "pacUrlObfuscated": pac_url_obfuscated,
             "domain": domain,
             "description": description,
             "pacVerificationStatus": "VERIFY_NOERR",
         }
         url = f"/pacFiles"
         response = self.hp_http.post_call(
             url=url,
             headers=self.headers,
             payload=payload,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
+
         return response.json()
 
-    def list_malwarePolicy(self):
+    def list_malware_policy(self) -> json:
         """
         Method to list Malware Policy.  Policy > Malware Protection > Malware Policy
-        :return: json
+
+        :return: (json)
         """
         url = f"/malwarePolicy"
         response = self.hp_http.get_call(
             url=url,
             headers=self.headers,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
+
         return response.json()
 
-    def list_virusSpywareSettings(self):
+    def list_virus_spyware_settings(self) -> json:
         """
         Method to list virus, malware, adware and spyware settings.  Policy > Malware Protection > Malware Policy
-        :return: json
+
+        :return: (json)
         """
         url = f"/virusSpywareSettings"
         response = self.hp_http.get_call(
             url=url,
             headers=self.headers,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
+
         return response.json()
 
-    def list_advancedUrlFilteringSettings(self):
+    def list_advanced_url_filtering_settings(self) -> json:
         """
         Method to list Advanced Policy settings.  Policy > URL & Cloud App Control > Advanced  Policy Settings
-        :return: json
+
+        :return: (json)
         """
         url = f"/advancedUrlFilterAndCloudAppSettings"
         response = self.hp_http.get_call(
             url=url,
             headers=self.headers,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
+
         return response.json()
 
-    def list_subscriptions(self):
+    def list_subscriptions(self) -> json:
         """
         Method to list tenant subscriptions.  Administration > Company Profile > Subscriptions
-        :return: json
+
+        :return: (json)
         """
         url = f"/subscriptions"
         response = self.hp_http.get_call(
             url=url,
             headers=self.headers,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
+
         return response.json()
 
-    def list_cyberRiskScore(self):
+    def list_cyber_risk_score(self) -> json:
         """
         Method to list tenant subscriptions.  Administration > Company Profile > Subscriptions
-        :return: json
+
+        :return: (json)
         """
         url = f"/cyberRiskScore"
         response = self.hp_http.get_call(
             url=url,
             headers=self.headers,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
+
         return response.json()
 
-    def add_user_groups(self, group_name):
+    def add_user_groups(
+        self,
+        group_name,
+    ) -> json:
         """
         Creates user groups
-        :return:
-        :rtype:
+
+        :return: (json)
         """
         url = "/groups"
         payload = {"name": group_name}
         response = self.hp_http.post_call(
             url=url,
             headers=self.headers,
             payload=payload,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
+
         return response.json()
 
-    def list_samlSettings(self):
+    def list_saml_settings(self) -> json:
         """
         Method to list SAML settings.  Administration > Authentication Settings
+
+        :return: (json)
         """
         url = f"/samlSettings"
         response = self.hp_http.get_call(
             url=url,
             headers=self.headers,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
+
         return response.json()
 
-    def list_advancedSettings(self):
+    def list_advanced_settings(self) -> json:
         """
         Method to list ZIA advanced settings.  Administration > Advanced Settings
-        :return: json
+
+        :return: (json)
         """
         url = f"/advancedSettings"
         response = self.hp_http.get_call(
             url=url,
             headers=self.headers,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
+
         return response.json()
 
-    def list_idpConfig(self):
+    def list_idp_config(self) -> json:
         """
         Method to list ZIA idp configuration.  Administration > Authentication Settings > identity Providers
-        :return: json
+
+        :return: (json)
         """
         url = f"/idpConfig"
         response = self.hp_http.get_call(
             url=url,
             headers=self.headers,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
+
         return response.json()
 
-    def list_icapServers(self):
+    def list_icap_servers(self) -> json:
         """
-        Method to list ZIA icap servers.  Administration > DLP iincident Receiver > ICAP Settings
-        :return: json
+        Method to list ZIA icap servers.  Administration > DLP incident Receiver > ICAP Settings
+
+        :return: (json)
         """
         url = f"/icapServers"
         response = self.hp_http.get_call(
             url=url,
             headers=self.headers,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
+
         return response.json()
 
-    def list_authSettings(self):
+    def list_auth_settings(self) -> json:
         """
         Method to list ZIA auth settings.  Administration > Authentication Settings
-        :return: json
+
+        :return: (json)
         """
         url = f"/authSettings"
         response = self.hp_http.get_call(
             url=url,
             headers=self.headers,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
+
         return response.json()
 
-    def list_samlAdminSettings(self):
+    def list_saml_admin_settings(self) -> json:
         """
         Method to list ZIA auth settings.  Administration > Authentication Settings
-        :return: json
+
+        :return: (json)
         """
         url = f"/samlAdminSettings"
         response = self.hp_http.get_call(
             url=url,
             headers=self.headers,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
+
         return response.json()
 
-    def list_eun(self):
+    def list_eun(self) -> json:
         """
         Method to list ZIA End User Notification settings.  Administration > End User Notifications
-        :return: json
+
+        :return: (json)
         """
         url = f"/eun"
         response = self.hp_http.get_call(
             url=url,
             headers=self.headers,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
+
         return response.json()
 
-    def list_admin_password_mgt(self):
+    def list_admin_password_mgt(self) -> json:
         """
         Method to list ZIA Administrator Management password.  Administration > Administration Management
-        :return: json
+
+        :return: (json)
         """
         url = f"/passwordExpiry/settings"
         response = self.hp_http.get_call(
             url=url,
             headers=self.headers,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
+
         return response.json()
 
-    def list_apiKeys(self):
+    def list_api_keys(self) -> json:
         """
         Method to list ZIA Administrator Management password.  Administration > Administration Management
-        :return: json
+
+        :return: (json)
         """
         url = f"/apiKeys"
         response = self.hp_http.get_call(
             url=url,
             headers=self.headers,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
+
         return response.json()
 
-    def delete_group(self, groupid):
+    def delete_group(
+        self,
+        group_id: int,
+    ) -> requests.Response:
         """
         Method to delete a group given group id
-        :param groupid: type int. Group id
-        :return: HTTP response
+
+        :param group_id: (int) Group id
+
+        :return: requests.Response object
         """
-        url = f"/groups/{groupid}"
+        url = f"/groups/{group_id}"
         response = self.hp_http.delete_call(
             url=url,
             headers=self.headers,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
+
         return response
 
-    def delete_department(self, departmentid):
+    def delete_department(
+        self,
+        department_id: int,
+    ) -> json:
         """
         Method to delete a group given department
-        :param departmentid: type int. Departmentid id
-        :return: HTTP response
+
+        :param department_id: (int) Department id
+
+        :return: requests.Response object
         """
-        url = f"/departments/{departmentid}"
-        response = self.hp_http.delete_call(
-            url=url,
+        result = request_(
+            method="delete",
+            url=f"{self.base_uri}/departments/{department_id}",
             headers=self.headers,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
-        return response
 
-    def list_webApplicationRules(self):
+        return result.json()
+
+    def list_web_application_rules(self) -> json:
         """
         Method to list Cloud APP policies
-        :return:
-        :rtype:
+
+        :return: (json)
         """
         url = "/webApplicationRules"
         response = self.hp_http.get_call(
             url=url,
             headers=self.headers,
             cookies={
-                "JSESSIONID": self.jsessionid,
+                "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
+
         return response.json()
```

### Comparing `zscaler_api_talkers-4.1.0/zscaler_api_talkers/zia_talker/zia_talker.py` & `zscaler_api_talkers-4.1.1/zscaler_api_talkers/zia_talker/zia_talker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,527 +1,608 @@
+import json
 import pdb  # noqa
 import time
-from getpass import getpass
 
-from models.models import super_categories, valid_category_ids, valid_countries
-from zscaler_helpers import HttpCalls
+import requests
+from zscaler_api_talkers.zia_talker.models import (super_categories, valid_category_ids, valid_countries)
+from zscaler_api_talkers.zscaler_helpers import HttpCalls, setup_logger
+
+from .helpers import _obfuscate_api_key
+
+logger = setup_logger(name=__name__)
 
 
 class ZiaTalker(object):
     """
     ZIA API talker
     Documentation:
     https://help.zscaler.com/zia/zia-api/api-developer-reference-guide
     """
 
-    def __init__(self, cloud_name, bearer=None):
+    def __init__(
+        self,
+        cloud_name: str,
+        bearer: str = None,
+        api_key: str = "",
+        username: str = "",
+        password: str = "",
+    ):
         """
         Method to start the class
-        :param cloud_name: type string. Example: zscalerbeta.net
-        zscalerone.net, zscalertwo.net,
-        zscalerthree.net, zscaler.net, zscloud.net
-        :param bearer: Type string. OAuth2.0 Bear token
+
+        :param cloud_name: (str) Example: zscalerbeta.net, zscalerone.net, zscalertwo.net, zscalerthree.net,
+            zscaler.net, zscloud.net
+        :param bearer: (str) OAuth2.0 Bear token
         """
         self.base_uri = f"https://zsapi.{cloud_name}/api/v1"
-        self.hp_http = HttpCalls(host=self.base_uri, verify=True)
+        self.hp_http = HttpCalls(
+            host=self.base_uri,
+            verify=True,
+        )
         self.cookies = None
+        self.headers = None
         if bearer:
             self.headers = {"Authorization": f"Bearer {bearer}"}
-        else:
-            self.headers = None
-
-    def _obfuscateApiKey(self, seed: str):
-        """
-        Internal method to Obfuscate the API key
-        :param seed: API key
-        :return: timestamp,obfuscated key
-        """
-        seed = seed
-        now = int(time.time() * 1000)
-        n = str(now)[-6:]
-        r = str(int(n) >> 1).zfill(6)
-        key = ""
-        for digit in n:
-            key += seed[int(digit)]
-        for digit in r:
-            key += seed[int(digit) + 2]
-        return now, key
+        elif username and any([password, api_key]):
+            self.authenticate(
+                username=username,
+                api_key=api_key,
+                password=password,
+            )
 
     def authenticate(
         self,
-        apikey: str,
+        api_key: str,
         username: str,
         password: str = None,
-    ) -> None:
+    ):
         """
         Method to authenticate.
-        :param apikey: API key
-        :param username: A string that contains the email ID of the API admin
-        :param password: A string that contains the password for the API admin
-        :return:  JSESSIONID.
-        This cookie expires by default 30 minutes from last request
-        """
-        if not password:
-            password = getpass(" Introduce password: ")
-        timestamp, key = self._obfuscateApiKey(apikey)
 
+        :param api_key: (str) API key
+        :param username: (str) A string that contains the email ID of the API admin
+        :param password: (str) A string that contains the password for the API admin
+        """
+        timestamp, key = _obfuscate_api_key(api_key)
         payload = {
             "apiKey": key,
             "username": username,
             "password": password,
             "timestamp": timestamp,
         }
         url = "/authenticatedSession"
-        response = self.hp_http.post_call(url=url, payload=payload)
+        response = self.hp_http.post_call(
+            url=url,
+            payload=payload,
+        )
         self.cookies = {"JSESSIONID": response.cookies["JSESSIONID"]}
 
-    def authenticated_session(self):
+    def authenticated_session(self) -> json:
         """
         Checks if there is an authenticated session
-        :return: json
+
+        :return: (json)
         """
         url = "/authenticatedSession"
         response = self.hp_http.get_call(
             url,
             cookies=self.cookies,
             error_handling=True,
         )
+
         return response.json()
 
-    def end_session(self):
+    def end_session(self) -> json:
         """
-        Menthod to enf an authenticated session
-        :return: None
+        Method to end an authenticated session
+
+        :return: (json)
         """
         url = "/authenticatedSession"
         response = self.hp_http.delete_call(
-            url, cookies=self.cookies, error_handling=True, payload={}
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            payload={},
         )
+
         return response.json()
 
-    def _obtain_all(self, url: str):
+    def _obtain_all(
+        self,
+        url: str,
+    ) -> list:
         """
         Internal method that queries all pages
-        :param url:  URL
-        :return:
+
+        :param url: (str) URL
+
+        :return: (list) List of results
         """
         page = 1
         result = []
         while True:
             response = self.hp_http.get_call(
-                f"{url}&page={page}",
+                url=f"{url}&page={page}",
                 cookies=self.cookies,
                 error_handling=True,
                 headers=self.headers,
             )
             if response.json():
                 result += response.json()
                 page += 1
                 time.sleep(1)
             else:
                 break
+
         return result
 
-    def get_status(self):
+    def get_status(self) -> json:
         """
         Method to obtain the activation status for a configuration change
-        :return: json object with the status
+
+        :return: (json) JSON object with the status
         """
         url = "/status"
-        response = self.hp_http.get_call(url, cookies=self.cookies, error_handling=True)
+        response = self.hp_http.get_call(
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+        )
+
         return response.json()
 
-    def activate_status(self):
+    def activate_status(self) -> json:
         """
         Method to activate configuration changes
-        :return: json object with the status
+
+        :return: (json) JSON object with the status
         """
         url = "/status/activate"
         response = self.hp_http.post_call(
-            url, payload={}, cookies=self.cookies, error_handling=True
+            url,
+            payload={},
+            cookies=self.cookies,
+            error_handling=True,
         )
+
         return response.json()
 
     # Admin Audit Logs
 
-    def list_auditlogEntryReport(self) -> dict:
-        """
-        Gets the status of a request for an audit log report.
-        After sending a POST request to /auditlogEntryReport to
-        generate a report, you can continue to call GET /auditlogEntryReport
-        to check whether the report has finished
-        generating. Once the status is COMPLETE, you can send another GET
-        request to /auditlogEntryReport/download to
-        download the report as a CSV file.
-        :return: json
+    def list_auditlog_entry_report(self) -> json:
         """
+        Gets the status of a request for an audit log report.  After sending a POST request to /auditlogEntryReport
+        to generate a report, you can continue to call GET /auditlogEntryReport to check whether the report has
+        finished generating. Once the status is COMPLETE, you can send another GET request to
+        /auditlogEntryReport/download to download the report as a CSV file.
 
+        :return: (json)
+        """
         url = "/auditlogEntryReport"
-
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, headers=self.headers, error_handling=True
+            url,
+            cookies=self.cookies,
+            headers=self.headers,
+            error_handling=True,
         )
+
         return response.json()
 
-    def download_auditlogEntryReport(self):
-        """
-        Gets the status of a request for an audit log report. After sending a
-        POST request to /auditlogEntryReport to
-        generate a report, you can continue to call GET /auditlogEntryReport
-        to check whether the report has finished
-        generating. Once the status is COMPLETE, you can send another GET
-        request to /auditlogEntryReport/download to
-        download the report as a CSV file.
-        :return: json
+    def download_auditlog_entry_report(self) -> requests.Response:
         """
+        Gets the status of a request for an audit log report. After sending a POST request to /auditlogEntryReport
+        to generate a report, you can continue to call GET /auditlogEntryReport to check whether the report has
+        finished generating. Once the status is COMPLETE, you can send another GET request to
+        /auditlogEntryReport/download to download the report as a CSV file.
 
+        :return: (request.Response)
+        """
         url = "/auditlogEntryReport/download"
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, headers=self.headers, error_handling=True
+            url,
+            cookies=self.cookies,
+            headers=self.headers,
+            error_handling=True,
         )
+
         return response
 
-    def add_auditlogEntryReport(
+    def add_auditlog_entry_report(
         self,
-        startTime: int,
-        endTime: int,
-        actionTypes: list = None,
+        start_time: int,
+        end_time: int,
+        action_types: list = None,
         category: str = None,
         subcategories: list = None,
-        actionInterface: str = None,
-    ):
+        action_interface: str = None,
+    ) -> requests.Response:
         """
-         Creates an audit log report for the specified time period and saves
-         it as a CSV file. The report includes audit
-         information for every call made to the cloud service API during the
-         specified time period.
-         Creating a new audit log report will overwrite a previously-generated
-         report.
-        :param startTime: The timestamp, in epoch, of the admin's last login
-        :param endTime: The timestamp, in epoch, of the admin's last logout.
-        :param actionTypes: type list. The action performed by the admin in
-        the ZIA Admin Portal or API
-        :param actionResult: The outcome (i.e., Failure or Success) of an
-        actionType.
-        :param category: tyoe string. The location in the Zscaler Admin Portal
-        (i.e., Admin UI) where the actionType was performed
-        :param subcategories: type list. The area within a category where the
-        actionType was performed.
-        :param actionInterface: type string. The interface
-        (i.e., Admin UI or API) where the actionType was performed.
-        :param clientIP: type string. The source IP address for the admin
-        :param adminName: type string.  The admin's login ID
-        :return: 204 Successfull Operation
+         Creates an audit log report for the specified time period and saves it as a CSV file. The report includes
+         audit information for every call made to the cloud service API during the specified time period. Creating a
+         new audit log report will overwrite a previously-generated report.
+
+        :param start_time: (int) The timestamp, in epoch, of the admin's last login
+        :param end_time: (int) The timestamp, in epoch, of the admin's last logout.
+        :param action_types: (list) The action performed by the admin in the ZIA Admin Portal or API
+        :param category: (str) The location in the Zscaler Admin Portal (i.e., Admin UI) where the actionType was
+        performed.
+        :param subcategories: (list) The area within a category where the actionType was performed.
+        :param action_interface: (str) The interface (i.e., Admin UI or API) where the actionType was performed.
+
+        :return: (requests.Response Object) 204 Successful Operation
         """
         url = "/auditlogEntryReport"
         payload = {
-            "startTime": startTime,
-            "endTime": endTime,
+            "startTime": start_time,
+            "endTime": end_time,
         }
         if category:
             payload.update(category=category)
         if subcategories:
             payload.update(subcategories=subcategories)
-        if actionInterface:
-            payload.update(actionInterface=actionInterface)
-        if actionTypes:
-            payload.update(actionTypes=actionTypes)
+        if action_interface:
+            payload.update(actionInterface=action_interface)
+        if action_types:
+            payload.update(actionTypes=action_types)
 
         response = self.hp_http.post_call(
             url,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response
 
     # Admin & Role Management
-    def list_adminUsers(self, userId=None, query=None):
+    def list_admin_users(
+        self,
+        user_id: int = None,
+        query: str = None,
+    ) -> json:
         """
-        Gets a list of admin users. By default, auditor user
-        information is not included.
-        :param userId: user ID
-        :param query: HTTP query
-        :return:json()
+        Gets a list of admin users. By default, auditor user information is not included.
+
+        :param user_id: (int) user ID
+        :param query: (str) HTTP query  # TODO: What is this?  Looks like it is just parameters
+
+        :return: (json) JSON of results
         """
-        if userId:
-            url = f"/adminUsers/{userId}"
+        if user_id:
+            url = f"/adminUsers/{user_id}"
             return self.hp_http.get_call(
-                url, cookies=self.cookies, error_handling=True, headers=self.headers
+                url,
+                cookies=self.cookies,
+                error_handling=True,
+                headers=self.headers,
             ).json()
         else:
             if query:
                 url = f"/adminUsers?{query}?pageSize=1000"
             else:
                 url = "/adminUsers?pageSize=1000"
+
         return self._obtain_all(url)
 
-    def list_adminRoles(self, query=None):
+    def list_admin_roles(
+        self,
+        query: str = None,
+    ) -> json:
         """
         Gets a name and ID dictionary of al admin roles
-        :param query: HTTP query
-        :return: json
+
+        :param query: (str) HTTP query  # TODO: What is this?  Looks like it is just parameters
+
+        :return: (json)
         """
         if query:
             url = f"/adminRoles/lite?{query}"
         else:
             url = "/adminRoles/lite"
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
     # URL Categories
-    def list_url_categories(self, custom=False):
+    def list_url_categories(
+        self,
+        custom: bool = False,
+    ) -> json:
         """
         Gets information about all or custom URL categories
-        :param custom: Boolean, if True it will return custom categories only
-        :return: json
+
+        :param custom: (bool) If True it will return custom categories only.  Default is False.
+
+        :return: (json)
         """
 
         if custom:
             url = "/urlCategories?customOnly=true"
         else:
             url = "/urlCategories"
-        # return self._obtain_all(url)
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def list_url_categories_lite(self):
+    def list_url_categories_lite(self) -> json:
         """
         Gets a lightweight key-value list of all or custom URL categories.
+
+        :return: (json)
         """
         url = "/urlCategories/lite"
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
     def add_url_categories(
         self,
-        name,
-        superCategory,
-        type="URL_CATEGORY",
-        urls=None,
-        dbCategorizedUrls=None,
-        keywordsRetainingParentCategory=[],
-        keywords=[],
-        customCategory=False,
-        ipRanges=[],
-        ipRangesRetainingParentCategory=[],
-    ):
+        name: str,
+        super_category: str,
+        type_list: list = None,
+        urls: list = None,
+        db_categorized_urls: list = None,
+        keywords_retaining_parent_category: list = None,
+        keywords: list = None,
+        custom_category: bool = False,
+        ip_ranges: list = None,
+        ip_ranges_retaining_parent_category: list = None,
+    ) -> json:
         """
          Adds a new custom URL category.
-        :param name: type string. Name of the custom category. Possible values
-        URL_CATEGORY, TLD_CATEGORY, ALL
-        :param superCategory: type string. super category
-        :param urls: type list. List of urls
-        :param dbCategorizedUrls: type list. URL retaining parent category
-        :param keywordsRetainingParentCategory: type list. Retained custom
-        keywords from the parent URL category that is associated to a
-        URL category.
-        :param keywords: type list. Custom keywords associated to a
+
+        :param name: (str) Name of the custom category. Possible values URL_CATEGORY, TLD_CATEGORY, ALL
+        :param super_category: (str) super category
+        :param type_list: (list)
+        :param urls: (list) List of urls
+        :param db_categorized_urls: (list) URL retaining parent category
+        :param keywords_retaining_parent_category: (list) Retained custom keywords from the parent URL category that is
+        associated to a URL category.
+        :param keywords: (list) Custom keywords associated to a URL category.
+        :param custom_category: (bool) Default False. Set to True for custom category
+        :param ip_ranges: (list) Custom IP address ranges associated to a URL category
+        :param ip_ranges_retaining_parent_category: (list) The retaining parent custom IP address ranges associated to a
         URL category.
-        :param customCategory: type boolean. Default False. Set to True for
-        custom category
-        :param ipRanges: type list. Custom IP address ranges associated to a
-        URL category
-        :param ipRangesRetainingParentCategory: The retaining parent custom IP
-        address ranges associated to a URL category.
 
         :return:  json
         """
-        if keywordsRetainingParentCategory is None:
-            keywordsRetainingParentCategory = []
+        if not type_list:
+            type_list = ["URL_CATEGORY"]
 
-        if superCategory not in super_categories:
-            print("Error -> Invalid Super Category")
-            print(f"{super_categories}")
+        if keywords_retaining_parent_category is None:
+            keywords_retaining_parent_category = []
+
+        if super_category not in super_categories:
+            logger.error(f"Invalid Super Category: {super_categories}")
             raise ValueError("Invalid super category")
 
         url = "/urlCategories"
         payload = {
             "configuredName": name,
-            "customCategory": customCategory,
-            "superCategory": superCategory,
-            "keywordsRetainingParentCategory": keywordsRetainingParentCategory,
+            "customCategory": custom_category,
+            "superCategory": super_category,
+            "keywordsRetainingParentCategory": keywords_retaining_parent_category,
             "keywords": keywords,
             "urls": urls,
-            "dbCategorizedUrls": dbCategorizedUrls,
-            "ipRanges": ipRanges,
-            "ipRangesRetainingParentCategory": ipRangesRetainingParentCategory,
-            "type": type,
+            "dbCategorizedUrls": db_categorized_urls,
+            "ipRanges": ip_ranges,
+            "ipRangesRetainingParentCategory": ip_ranges_retaining_parent_category,
+            "type": type_list,
         }
         response = self.hp_http.post_call(
             url,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response.json()
 
-    def add_url_categories1(self, payload):
+    def add_raw_url_categories(
+        self,
+        payload: dict,
+    ) -> json:
         """
          Adds a new custom URL category.
-        :param payload
-        :return:  json
+
+        :param payload: (dict)
+
+        :return: (json)
         """
         url = "/urlCategories"
         response = self.hp_http.post_call(
             url,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response.json()
 
     def update_url_categories(
         self,
-        categoryId,
-        action=None,
-        configuredName=None,
-        urls=None,
-        dbCategorizedUrls=None,
-        keywords=None,
-        keywordsRetainingParentCategory=None,
-    ):
-        """
-         Updates the URL category for the specified ID. If keywords are
-         included within the request, then they
-         will replace existing ones for the specified URL category . If the
-         keywords attribute is not included the
-         request, the existing keywords are retained.
-         You can perform a full update for the specified URL category. However
-         if attributes are omitted within the
-          update request, the values for those attributes are cleared.
-
-         You can also perform an incremental update, to add or remove URLs
-         for the specified URL category using the
-         action parameter
-        :param categoryId: type string. URL id
-        :param configuredName: type string. Name of the custom category
-        :param urls: list of urls
-        :param dbCategorizedUrls: type list. URL retaining parent category
-        :param keywordsRetainingParentCategory: list of key works
-        :param action: Optional parameter. ADD_TO_LIST or REMOVE_FROM_LIST
-        :return:  json
+        category_id: str,
+        action: str = None,
+        configured_name: str = None,
+        urls: list = None,
+        db_categorized_urls: list = None,
+        keywords: list = None,
+        keywords_retaining_parent_category: list = None,
+    ) -> json:
+        """
+        Updates the URL category for the specified ID. If keywords are included within the request, then they will
+        replace existing ones for the specified URL category . If the keywords attribute is not included the request,
+        the existing keywords are retained. You can perform a full update for the specified URL category. However,
+        if attributes are omitted within the update request then clear the values for those attributes.
+
+        You can also perform an incremental update, to add or remove URLs for the specified URL category using the
+        action parameter.
+
+        :param category_id: (str) URL id
+        :param action: (str) Optional parameter. ADD_TO_LIST or REMOVE_FROM_LIST
+        :param configured_name: (str) Name of the custom category
+        :param urls: (list) List of urls
+        :param db_categorized_urls: (list) URL retaining parent category
+        :param keywords: (list)
+        :param keywords_retaining_parent_category: (list) List of key works
+
+        :return:  (json)
         """
         """if categoryId not in valid_category_ids:
             print(f'Error -> Invalid category id')
             raise ValueError("Invalid category id")"""
+        url = f"/urlCategories/{category_id}"
+        parameters = {}
 
-        if action == "ADD_TO_LIST":
-            url = f"/urlCategories/{categoryId}?action=ADD_TO_LIST"
-        elif action == "REMOVE_FROM_LIST":
-            url = f"/urlCategories/{categoryId}?action=REMOVE_FROM_LIST"
-        elif not action:
-            url = f"/urlCategories/{categoryId}"
-        else:
-            print("Error -> Invalid action")
-            print(f"{action}")
+        if action and action not in ["ADD_TO_LIST", "REMOVE_FROM_LIST"]:
+            logger.error(f"Invalid action: {action}")
             raise ValueError("Invalid action")
+        else:
+            parameters.update({"action": action})
 
         payload = {
-            "configuredName": configuredName,
+            "configuredName": configured_name,
         }
-        if keywordsRetainingParentCategory:
+        if keywords_retaining_parent_category:
             payload.update(
-                keywordsRetainingParentCategory=keywordsRetainingParentCategory
+                keywordsRetainingParentCategory=keywords_retaining_parent_category
             )
         if keywords:
             payload.update(keywords=keywords)
-        if configuredName:
-            payload.update(configuredName=configuredName)
+        if configured_name:
+            payload.update(configuredName=configured_name)
         if urls:
             payload.update(urls=urls)
-        if dbCategorizedUrls:
-            payload.update(dbCategorizedUrls=dbCategorizedUrls)
+        if db_categorized_urls:
+            payload.update(dbCategorizedUrls=db_categorized_urls)
 
         response = self.hp_http.put_call(
             url,
+            params=parameters,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response.json()
 
-    def delete_url_categories(self, categoryid):
+    def delete_url_categories(
+        self,
+        category_id: int,
+    ) -> requests.Response:
         """
-        Deletes the custom URL category for the specified ID.
-        You cannot delete a custom category while it is being used by
-        a URL policy or NSS feed. Also, predefined
-        categories cannot be deleted.
-        :param categoryid: Category ID
-        :return: json response
+        Deletes the custom URL category for the specified ID. You cannot delete a custom category while it is being
+        used by a URL policy or NSS feed. Also, predefined categories cannot be deleted.
+
+        :param category_id: (inst) Category ID
+
+        :return: (requests.Response)
         """
-        url = f"/urlCategories/{categoryid}"
+        url = f"/urlCategories/{category_id}"
         response = self.hp_http.delete_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response
 
-    def delete_urlFilteringRules(self, ruleId):
+    def delete_url_filtering_rules(
+        self,
+        rule_id: int,
+    ) -> requests.Response:
         """
-        Deletes the custom URL category for the specified ID.
-        You cannot delete a custom category while it is being used by a URL
-        policy or NSS feed. Also, predefined
-        categories cannot be deleted.
-        :param ruleId:  type int. Rule Id
-        :return: json response
+        Deletes the custom URL category for the specified ID. You cannot delete a custom category while it is being
+        used by a URL policy or NSS feed. Also, predefined categories cannot be deleted.
+
+        :param rule_id: (int) Rule Id
+
+        :return: (request.Response)
         """
-        url = f"/urlFilteringRules/{ruleId}"
+        url = f"/urlFilteringRules/{rule_id}"
         response = self.hp_http.delete_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response
 
-    def list_url_categories_urlquota(self):
+    def list_url_categories_url_quota(self) -> json:
         """
-        Gets information on the number of unique URLs that are currently
-        provisioned for your organization as well as
+        Gets information on the number of unique URLs that are currently provisioned for your organization as well as
         how many URLs you can add before reaching that number.
-        :return: json
+
+        :return: (json)
         """
         url = "/urlCategories/urlQuota"
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
-        print(response.json())
+
         return response.json()
 
-    def list_url_categories_id(self, category_id):
+    def list_url_categories_id(
+        self,
+        category_id: int,
+    ) -> json:
         """
         Gets the URL category information for the specified ID
-        :param category_id:
-        :return:
-        """
 
-        url = f"/urlCategories/{category_id}"
+        :param category_id: (int)
 
+        :return: (json)
+        """
+        url = f"/urlCategories/{category_id}"
         if category_id not in valid_category_ids:
-            print("Error -> Invalid Category ID")
-            print(f"{valid_category_ids}")
+            logger.error(f"Invalid Category ID: {category_id}")
             raise ValueError("Invalid Category ID")
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def url_lookup(self, url_list):
+    def url_lookup(
+        self,
+        url_list: list,
+    ) -> list:
         """
-        Method to look up the categorization of the
-        given list of URLs, ["abc.com","zyz.com"]
-        :param url_list: list of urls
-        :return:  json
+        Method to look up the categorization of the given list of URLs, ["abc.com","zyz.com"]
+
+        :param url_list: (list) List of urls
+        :return: (list)
         """
         result = []
         url = "/urlLookup"
         # Verify urls format
         list(set(url_list))
         # Rate limit 1/sec  and 400 hr and 100 URLs per call
         list_of_lists = [url_list[i : i + 100] for i in range(0, len(url_list), 100)]
@@ -535,264 +616,281 @@
             )
             result.append(response.json())
             time.sleep(1)
         final_result = []
         for i in result:
             for j in i:
                 final_result.append(j)
+
         return final_result
 
     # URL filtering Policies
-    def list_url_filtering_rules(
-        self,
-    ):
+    def list_url_filtering_rules(self) -> json:
         """
         Gets a list of all of URL Filtering Policy rules
-        :return:
+
+        :return: (json)
         """
         url = "/urlFilteringRules"
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def add_url_filtering_rules(
+    def add_url_filtering_rules(  # FIXME: docstring lists params that aren't options and some params I don't know what their typehint should be.
         self,
-        name,
-        order,
-        protocols,
-        state,
-        action,
-        urlcategories=[],
-        requestMethods=None,
+        name: str,
+        order: int,
+        protocols: str,
+        state: str,
+        action: str,
+        url_categories: list = None,
+        request_methods: list = None,
         description=None,
-        groups=None,
-        locations=None,
-        departments=None,
-        users=None,
-        rank=7,
-        locationGroups=None,
-        enforceTimeValidity=False,
-        validityEndTime=None,
-        validityStartTime=None,
-        validityTimeZoneId=None,
-        cbiProfileId=0,
-        blockOverride=False,
-    ):
-        """
-         Adds a URL Filtering Policy rule.
-         If you are using the Admin Rank feature, refer to About Admin Rank
-         to determine which value to provide for rank
-         when adding a policy rule. If you are not using Admin Rank, the
-         rank value must be 7.
-        :param name: type string.  Name of the rule
-        :param order: type integer. Rule order
-        :param protocols: type string. Possible values
-        SMRULEF_ZPA_BROKERS_RULE, ANY_RULE, TCP_RULE, UDP_RULE, DOHTTPS_RULE,
-        TUNNELSSL_RULE,
-        HTTP_PROXY, FOHTTP_RULE, FTP_RULE, HTTPS_RULE, HTTP_RULE,
-        SSL_RULE, TUNNEL_RULE
-        :param locations: type list. Each element is a  dictionary:
-        Name-ID pairs of locations for which rule must be applied
-        :param groups: type list. Name-ID pairs of groups for which
-        rule must be applied
-        :param departments:type list. Name-ID pairs of departments
-        for which rule will be applied
-        :param users: type list. Name-ID pairs of users for which rule must
-        be applied
-        :param urlcategories: type list. List of URL categories for which rule
-        must be applied
-        :param admin_rack:Admin rank of the admin who creates this rule
-        :param timewindows: type list. Name-ID pairs of time interval
-        during which rule must be enforced.
-        :param requestmethods: type list. Request method for which the rule
-        must be applied. If not set, rule will be applied to all
-         methods
-        :param endUserNotificationUrl: type string. URL of end user
-        notification page to be displayed when the rule is matched. Not
-        applicable if either
-        'overrideUsers' or 'overrideGroups' is specified.
-        :param overrideusers: Name-ID pairs of users for which this rule can
-        be overridden. Applicable only if
-         blockOverride is set to 'true', action is 'BLOCK' and overrideGroups
-         is not set.If this overrideUsers is not
-         set, 'BLOCK' action can be overridden for any user.
-        :param overridegroups: Name-ID pairs of groups for which this
-        rule can be overridden. Applicable only if
-        blockOverride is set to 'true' and action is 'BLOCK'. If this
-        overrideGroups is not set, 'BLOCK' action can be
-        overridden for any group
-        :param blockOverride: boolean: When set to true, a 'BLOCK' action
-        triggered by the rule could be overridden.
-        If true and both overrideGroup and overrideUsers are not set, the
-        BLOCK triggered by this rule could be
-        overridden for any users. If blockOverride is not set, 'BLOCK'
-        action cannot be overridden.
-        :param description: Additional information about the URL Filtering rule
-        :param state: enabled/disabled
-        :param action: Allow, Caution, Block
+        groups: list = None,
+        locations: list = None,
+        departments: list = None,
+        users: list = None,
+        rank: int = 7,
+        location_groups=None,
+        enforce_time_validity: bool = False,
+        validity_end_time=None,
+        validity_start_time=None,
+        validity_time_zone_id=None,
+        cbi_profile_id: int = 0,
+        block_override: bool = False,
+    ) -> json:
+        """
+         Adds a URL Filtering Policy rule. If you are using the Rank feature, refer to About Admin Rank to
+         determine which value to provide for rank when adding a policy rule. If you are not using Admin Rank,
+         the rank value must be 7.
+
+        :param name: (str)  Name of the rule
+        :param order: (int) Rule order
+        :param protocols: (str) Possible values: SMRULEF_ZPA_BROKERS_RULE, ANY_RULE, TCP_RULE, UDP_RULE,
+        DOHTTPS_RULE, TUNNELSSL_RULE, HTTP_PROXY, FOHTTP_RULE, FTP_RULE, HTTPS_RULE, HTTP_RULE, SSL_RULE, TUNNEL_RULE
+        :param state: (str) enabled/disabled
+        :param action: (str) Allow, Caution, Block
+        :param url_categories: (list) List of URL categories for which rule must be applied
+        :param request_methods: (list) Request method for which the rule must be applied. If not set, rule will be
+        applied to all methods
+        :param description: (str) Additional information about the URL Filtering rule
+        :param groups: (list) Name-ID pairs of groups for which rule must be applied
+        :param locations: (list) Each element is a dictionary: Name-ID pairs of locations for which rule must be applied
+        :param departments: (list) Name-ID pairs of departments for which rule will be applied
+        :param users: (list) Name-ID pairs of users for which rule must be applied
+        :param rank: (int) Admin rank of the admin who creates this rule
+        :param location_groups:
+        :param enforce_time_validity: (bool)
+        :param validity_end_time:
+        :param validity_start_time:
+        :param validity_time_zone_id:
+        :param cbi_profile_id: (int)
+        :param block_override: (bool) When set to true, a 'BLOCK' action triggered by the rule could be overridden.
+        If true and both overrideGroup and overrideUsers are not set, the BLOCK triggered by this rule could be
+        overridden for any users. If blockOverride is not set, 'BLOCK' action cannot be overridden.
+
+        :param timewindows: (list) Name-ID pairs of time interval during which rule must be enforced.
+        :param endUserNotificationUrl: (str) URL of end user notification page to be displayed when the rule
+        is matched. Not applicable if either 'overrideUsers' or 'overrideGroups' is specified.
+        :param overrideusers: Name-ID pairs of users for which this rule can be overridden. Applicable only if
+        blockOverride is set to 'true', action is 'BLOCK' and overrideGroups is not set.If this overrideUsers is not
+        set, 'BLOCK' action can be overridden for any user.
+        :param overridegroups: Name-ID pairs of groups for which this rule can be overridden. Applicable only if
+        blockOverride is set to 'true' and action is 'BLOCK'. If this overrideGroups is not set, 'BLOCK' action can
+        be overridden for any group
+
         :return:
         """
         url = "/urlFilteringRules"
         payload = {
-            "blockOverride": blockOverride,
-            "cbiProfileId": cbiProfileId,
+            "blockOverride": block_override,
+            "cbiProfileId": cbi_profile_id,
             "description": description,
-            "enforceTimeValidity": enforceTimeValidity,
+            "enforceTimeValidity": enforce_time_validity,
             "name": name,
             "order": order,
             "protocols": protocols,
-            "urlCategories": urlcategories,
+            "urlCategories": url_categories,
             "state": state,
             "rank": rank,
             "action": action,
         }
         if locations:
             payload.update(locations=locations)
-        if locationGroups:
-            payload.update(locationGroups=locationGroups)
+        if location_groups:
+            payload.update(locationGroups=location_groups)
         if groups:
             payload.update(groups=groups)
         if departments:
             payload.update(departments=departments)
         if users:
             payload.update(users=users)
-        if requestMethods:
-            payload.update(requestMethods=requestMethods)
-        if enforceTimeValidity:
-            payload.update(validityStartTime=validityStartTime)
-            payload.update(validityEndTime=validityEndTime)
-            payload.update(validityTimeZoneId=validityTimeZoneId)
-
-        print(payload)
+        if request_methods:
+            payload.update(requestMethods=request_methods)
+        if enforce_time_validity:
+            payload.update(validityStartTime=validity_start_time)
+            payload.update(validityEndTime=validity_end_time)
+            payload.update(validityTimeZoneId=validity_time_zone_id)
 
         response = self.hp_http.post_call(
             url,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response.json()
 
     # User Management
 
-    def list_departments(self, department_id=""):
+    def list_departments(
+        self,
+        department_id: int = None,
+    ) -> json or list:
         """
-        Gets a list of departments. The search parameters find matching values
-        within the "name" or "comments"
-        attributes.
-        if ID, gets the department for the specified ID
-        :param department_id: department ID
-        :return:json()
+        Gets a list of departments. The search parameters find matching values within the "name" or "comments"
+        attributes. if ID, gets the department for the specified ID
+
+        :param department_id: (int) department ID
+
+        :return: (json or list)
         """
 
-        if department_id:
-            url = "/departments"
+        if not department_id:
+            url = "/departments?pageSize=10000"
+            return self._obtain_all(url)
         else:
             url = f"/departments/{department_id}"
+            response = self.hp_http.get_call(
+                url,
+                cookies=self.cookies,
+                error_handling=True,
+                headers=self.headers,
+            )
+            return response.json()
 
-        response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
-        )
-        return response.json()
-
-    def list_groups(self, group_id=None):
+    def list_groups(
+        self,
+        group_id: int = None,
+    ) -> json or list:
         """
-        Gets a list of groups
-        if ID, gets the group for the specified ID
+        Gets a list of groups if ID, gets the group for the specified ID
+
         :param group_id: group ID
-        :return:json()
+
+        :return: (json)
         """
         if not group_id:
             url = "/groups?pageSize=10000"
             return self._obtain_all(url)
         else:
             url = f"/groups/{group_id}"
             response = self.hp_http.get_call(
-                url, cookies=self.cookies, error_handling=True, headers=self.headers
+                url,
+                cookies=self.cookies,
+                error_handling=True,
+                headers=self.headers,
             )
+            return response.json()
 
-        return response.json()
-
-    def list_users(self, user_id=None, query=None):
+    def list_users(
+        self,
+        user_id: int = None,
+        query: str = None,
+    ) -> json or list:
         """
-        Gets a list of all users and allows user filtering
-        by name, department, or group.
-        The name search parameter performs a partial match. The dept and group
-        parameters perform a 'starts with' match.
-        if ID, gets user information for the specified ID
-        :param user_id: user ID
-        :return:json()
+        Gets a list of all users and allows user filtering by name, department, or group. The name search parameter
+        performs a partial match. The dept and group parameters perform a 'starts with' match. if ID,
+        gets user information for the specified ID
+
+        :param user_id: (int) user ID
+        :param query: (str)
+
+        :return: (json or list)
         """
+        url = "/users?pageSize=1000"
         if user_id:
             url = f"/users/{user_id}"
             return self.hp_http.get_call(
-                url, cookies=self.cookies, error_handling=True, headers=self.headers
+                url,
+                cookies=self.cookies,
+                error_handling=True,
+                headers=self.headers,
             ).json()
-        else:
-            if query:
-                url = f"/users?{query}&pageSize=1000"
-                return self.hp_http.get_call(
-                    url, cookies=self.cookies, error_handling=True, headers=self.headers
-                ).json()
-            else:
-                url = "/users?pageSize=1000"
+        elif query:
+            url = f"/users?{query}&pageSize=1000"
+            return self.hp_http.get_call(
+                url,
+                cookies=self.cookies,
+                error_handling=True,
+                headers=self.headers,
+            ).json()
+
         return self._obtain_all(url)
 
     def add_users(
         self,
-        name,
-        email,
-        groups,
-        department,
-        comments,
-        password,
-        adminuser=False,
-    ):
-        """
-        Adds a new user. A user can belong to multiple groups,
-        but can only belong to one department.
+        name: str,
+        email: str,
+        groups: list,
+        department: dict,
+        comments: str,
+        password: str,
+        admin_user: bool = False,
+    ) -> json:
+        """
+        Adds a new user. A user can belong to multiple groups, but can only belong to one department.
+
+        :param name: (str) user name
+        :param email: (str) user email address
+        :param groups: (list) List each member is a dictionary, key id, value name [{"id":1234, "name":"guest-wifi"}]
+        :param department: (dict) key is the id and value is the name {"id":1234, "name":"guests"}
+        :param comments: (str) Comments
+        :param password: (str) Password,
+        :param admin_user: (bool) True if user is admin user. default False
 
-        :param name: string, user name
-        :param email: string user email address
-        :param groups: list. each member is a dictionary, key id, value name
-        [{"id":1234, "name":"guest-wifi"}]
-        :param department: dictionary, key is the id and value is the name
-        {"id":1234, "name":"guests"}
-        :param comments: string, comments
-        :param password: string password,
-        :param adminuser: True if user is admin user. default False
-        :return: Json
+        :return: (json)
         """
         url = "/users"
         payload = {
             "name": name,
             "email": email,
             "groups": groups,
             "department": department,
             "comments": comments,
             "password": password,
-            "adminUser": adminuser,
+            "adminUser": admin_user,
         }
         response = self.hp_http.post_call(
             url,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response.json()
 
-    def delete_bulk_users(self, user_ids):
+    def delete_bulk_users(
+        self,
+        user_ids: list,
+    ) -> json:
         """
-        Bulk delete users up to a maximum of 500 users per request.
-        The response returns the user IDs that were
+        Bulk delete users up to a maximum of 500 users per request. The response returns the user IDs that were
         successfully deleted.
-        :param user_ids:  List of user IDS to be deleted
+
+        :param user_ids: (list) List of user IDS to be deleted.  Max 500 per bulk delete.
+
+        :return: (json)
         """
         url = "/users/bulkDelete"
         if len(user_ids) < 500:
             payload = {"ids": user_ids}
             response = self.hp_http.post_call(
                 url,
                 payload=payload,
@@ -802,566 +900,741 @@
             )
             return response.json()
         else:
             raise ValueError("Maximum 500 users per request")
 
     # Location Management
 
-    def list_locations(self, locationId=None):
+    def list_locations(
+        self,
+        location_id: int = None,
+    ) -> json:
         """
-        Gets locations only, not sub-locations. When a location matches
-        the given search parameter criteria only its
+        Gets locations only, not sub-locations. When a location matches the given search parameter criteria only its
         parent location is included in the result set, not its sub-locations.
-        :param locationId: Location id
+
+        :param location_id: (int) Location id
+
+        :return: (json)
         """
-        if locationId:
-            url = f"/locations/{locationId}"
-        else:
-            url = "/locations"
+        url = "/locations"
+        if location_id:
+            url = f"/locations/{location_id}"
+
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def list_sublocations(self, locationId):
+    def list_sublocations(
+        self,
+        location_id: int,
+    ) -> json:
         """
-        Gets the sub-location information
-        for the location with the specified ID
-        :param locationId: Location id
+        Gets the sub-location information for the location with the specified ID
+
+        :param location_id: (int) Location id
+
+        :return: (json)
         """
-        if locationId:
-            url = f"/locations/{locationId}/sublocations"
-        else:
-            url = "/locations"
+        url = "/locations"
+        if location_id:
+            url = f"/locations/{location_id}/sublocations"
+
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def list_locationsgroups(
-        self,
-    ):
+    def list_locations_groups(self) -> json:
         """
         Gets information on location groups
-        :param locationgroupId: Location group id
+
+        :return: (json)
         """
         url = "/locations/groups"
-        print(url)
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def delete_bulk_locations(self, locationIds):
+    def delete_bulk_locations(
+        self,
+        location_ids: list,
+    ) -> json:
         """
-        Bulk delete locations up to a maximum of 100 users per request.
-        The response returns the location IDs that were successfully deleted.
-        :param locationIds: list of location IDs
+        Bulk delete locations up to a maximum of 100 users per request. The response returns the location IDs that
+        were successfully deleted.
+
+        :param location_ids: (list) List of location IDs
+
+        :return: (json)
         """
         url = "/locations/bulkDelete"
-        if len(locationIds) < 100:
-            payload = {"ids": locationIds}
+        if len(location_ids) < 100:
+            payload = {"ids": location_ids}
             response = self.hp_http.post_call(
                 url,
                 payload=payload,
                 cookies=self.cookies,
                 error_handling=True,
                 headers=self.headers,
             )
             return response.json()
         else:
             raise ValueError("Maximum 100 locations per request")
 
-    def delete_locations(self, locationId):
+    def delete_locations(
+        self,
+        location_id: int,
+    ) -> requests.Response:
         """
         Deletes the location or sub-location for the specified ID
-        :param locationId: location ID
-        """
-        url = f"/locations/{locationId}"
 
+        :param location_id: (int) location ID
+
+        :return: (request.Response object)
+        """
+        url = f"/locations/{location_id}"
         response = self.hp_http.delete_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response
 
     #   Traffic Forwarding
 
-    def list_greTunnels(self, greTunnelId=None):
+    def list_gre_tunnels(
+        self,
+        gre_tunnel_id: int = None,
+    ) -> json:
         """
         Gets the GRE tunnel information for the specified ID
-        :param greTunnelId: Optional. The unique identifier for the GRE tunnel
+
+        :param gre_tunnel_id: (int) Optional. The unique identifier for the GRE tunnel
+
+        :return: (json)
         """
-        if greTunnelId:
-            url = f"/greTunnels/{greTunnelId}"
-        else:
-            url = "/greTunnels"
+        url = "/greTunnels"
+        if gre_tunnel_id:
+            url = f"/greTunnels/{gre_tunnel_id}"
+
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def add_greTunnels(
+    def add_gre_tunnels(
         self,
-        sourceIp,
-        primaryDestVip,
-        secondaryDestVip,
-        internalIpRange,
-        withinCountry,
-        comment,
-        ipUnnumbered,
-    ):
+        source_ip: str,
+        primary_dest_vip: dict,
+        secondary_dest_vip: dict,
+        internal_ip_range: str,
+        within_country: bool,
+        comment: str,
+        ip_unnumbered: bool,
+    ) -> json:
         """
         Adds a GRE tunnel configuration.
-        :param sourceIp: type string. The source IP address of the
-        GRE tunnel. This is typically a static IP address in
-         the organization or SD-WAN. This IP address must be provisioned
-         within the Zscaler service using the /staticIP
-         endpoint.
-        :param primaryDestVip: type dictionary. {id:value} where value is
-        integer: Unique identifier of the GRE primary
-         VIP
-        :param secondaryDestVip: type dictionary. {id:value} where value is
-        integer: Unique identifier of the GRE
-        secondary VIP
-        :param internalIpRange: type string. The start of the internal IP
-        address in /29 CIDR range
-        :param withinCountry: type boolean. Restrict the data center virtual
-        IP addresses (VIPs) only to those within
-        the same country as the source IP address
-        :param comment: type string. Additional information about
-        this GRE tunnel
-        :param ipUnnumbered:This is required to support the automated SD-WAN
-        provisioning of GRE tunnels, when set to
-        true gre_tun_ip and gre_tun_id are set to null
-        :return:
+
+        :param source_ip: (str) The source IP address of the GRE tunnel. This is typically a static IP address in the
+        organization or SD-WAN. This IP address must be provisioned within the Zscaler service using the /staticIP
+        endpoint.
+        :param primary_dest_vip: (dict) {id:value} where value is integer: Unique identifier of the GRE primary VIP
+        :param secondary_dest_vip: (dict) {id:value} where value is integer: Unique identifier of the GRE secondary VIP
+        :param internal_ip_range: (str) The start of the internal IP address in /29 CIDR range
+        :param within_country: (bool) Restrict the data center virtual IP addresses (VIPs) only to those within the
+        same country as the source IP address
+        :param comment: (str) Additional information about this GRE tunnel
+        :param ip_unnumbered: (bool?) This is required to support the automated SD-WAN provisioning of GRE tunnels,
+        when set to True gre_tun_ip and gre_tun_id are set to null
+
+        :return: (json)
         """
         url = "/greTunnels"
         payload = {
-            "sourceIp": sourceIp,
-            "primaryDestVip": primaryDestVip,
-            "secondaryDestVip": secondaryDestVip,
-            "internalIpRange": internalIpRange,
-            "withinCountry": withinCountry,
+            "sourceIp": source_ip,
+            "primaryDestVip": primary_dest_vip,
+            "secondaryDestVip": secondary_dest_vip,
+            "internalIpRange": internal_ip_range,
+            "withinCountry": within_country,
             "comment": comment,
-            "ipUnnumbered": ipUnnumbered,
+            "ipUnnumbered": ip_unnumbered,
         }
         response = self.hp_http.post_call(
             url,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response.json()
 
-    def list_gre_validateAndGetAvailableInternalIpRanges(self):
+    def list_gre_validate_and_get_available_internal_ip_ranges(self) -> json:
         """
         Gets the next available GRE tunnel internal IP address ranges
-        :return: list of available IP addresses
+
+        :return: (json) List of available IP addresses
         """
         url = "/greTunnels/availableInternalIpRanges"
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def list_gre_recommended_vips(self, query):
+    def list_gre_recommended_vips(
+        self,
+        query: str,
+    ) -> json:
         """
-        Gets a list of recommended GRE tunnel virtual IP addresses (VIPs),
-        based on source IP address or latitude/longitude coordinates.
-        :param query: type string. URL query. Example:
-        :return: list of available IP addresses
+        Gets a list of recommended GRE tunnel virtual IP addresses (VIPs), based on source IP address or
+        latitude/longitude coordinates.
+
+        :param query: (str) URL query. Example:
+
+        :return: (json) List of available IP addresses
         """
         url = f"/vips/recommendedList?{query}"
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def list_gre_validate_ip(self, ip):
+    def list_gre_validate_ip(
+        self,
+        ip: str,
+    ) -> json:
         """
-        Gets the static IP address and location mapping information for the
-        specified GRE tunnel
-        IP address
-        :param ip: type string. IP address of the GRE tunnel.
-        :return:
+        Gets the static IP address and location mapping information for the specified GRE tunnel IP address
+
+        :param ip: (str) IP address of the GRE tunnel.
+
+        :return: (json)
         """
         url = f"/greTunnels/validateIP/{ip}"
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def list_vpnCredentials(self, vpnId=None):
+    def list_vpn_credentials(
+        self,
+        vpn_id: int = None,
+    ) -> json:
         """
         Gets VPN credentials that can be associated to locations.
-        :param vpnId: Optional. If specified, get VPN credentials for
-        the specified ID.
+
+        :param vpn_id: (int) Optional. If specified, get VPN credentials for the specified ID.
         """
-        if vpnId:
-            url = f"/vpnCredentials/{vpnId}"
-        else:
-            url = "/vpnCredentials"
+        url = "/vpnCredentials"
+        if vpn_id:
+            url = f"/vpnCredentials/{vpn_id}"
+
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def add_vpnCredentials(
+    def add_vpn_credentials(
         self,
-        fqdn,
-        preSharedKey,
-        type="UFQDN",
-        comments=None,
-    ):
+        fqdn: str,
+        pre_shared_key: str,
+        auth_type: str = "UFQDN",
+        comments: str = None,
+    ) -> json:
         """
         Adds VPN credentials that can be associated to locations.
-        :param fqdn: type string. Example abc@domain.com
-        :param preSharedKey: type string. Pre-shared key. This is a
-        required field for UFQDN and IP auth type
-        :param type: type string VPN authentication type.
+
+        :param fqdn: (str) Example abc@domain.com
+        :param pre_shared_key: (str) Pre-shared key. This is a required field for UFQDN and IP auth type
+        :param auth_type: (str) VPN authentication type.
         valid options CN, IP, UFQDN,XAUTH
-        :param comments: type string. Additional information
-        about this VPN credential.
-        :return:
+        :param comments: (str) Additional information about this VPN credential.
+
+        :return: (json)
         """
         url = "/vpnCredentials"
-        payload = {"type": type, "fqdn": fqdn, "preSharedKey": preSharedKey}
+        payload = {
+            "type": auth_type,
+            "fqdn": fqdn,
+            "preSharedKey": pre_shared_key,
+        }
         if comments:
             payload.update(comments=comments)
         response = self.hp_http.post_call(
             url,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response.json()
 
-    def delete_vpnCredentials(self, vpnId):
+    def delete_vpn_credentials(
+        self,
+        vpn_id: int,
+    ) -> requests.Response:  # TODO: Move to returning json
         """
         Deletes the VPN credentials for the specified ID.
-        :param vpnId: type integer. The unique identifier
-        for the VPN credential.
-        :return:
-        """
-        url = f"/vpnCredentials/{vpnId}"
 
+        :param vpn_id: (int) The unique identifier for the VPN credential.
+
+        :return: (requests.Response object)
+        """
+        url = f"/vpnCredentials/{vpn_id}"
         response = self.hp_http.delete_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response
 
-    def list_staticIP(self, IPId=None):
+    def list_static_ip(
+        self,
+        ip_id: int = None,
+    ) -> json:
         """
         Gets all provisioned static IP addresses.
-        :param IPId: Optional. If specified, get IP address
-        for the specified id
+
+        :param ip_id: (str) Optional. If specified, get IP address for the specified id
+
+        :return: (json)
         """
-        if IPId:
-            url = f"/staticIP/{IPId}"
-        else:
-            url = "/staticIP"
+        url = "/staticIP"
+        if ip_id:
+            url = f"/staticIP/{ip_id}"
+
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def add_staticIP(
+    def add_static_ip(
         self,
-        ipAddress,
-        geoOverrride=False,
-        routableIP=True,
-        latitude=0,
-        longitude=0,
-        comment="",
-    ):
+        ip_address: str,
+        geo_override: bool = False,
+        routable_ip: bool = True,
+        latitude: float = 0,
+        longitude: float = 0,
+        comment: str = "",
+    ) -> json:
         """
         Adds a static IP address
-        :param ipAddress: String. The satic IP address
-        :param geoOverrride: Boolean. If not set, geographic
-        coordinates and city are automatically determined from
-        the IP address. Otherwise, the latitude and longitude
-        coordinates must be provided.
-        :param routableIP: Boolean. Indicates whether a non-RFC 1918
-        IP address is publicly routable. This attribute is
-        ignored if there is no ZIA Private Service Edge associated to
-        the organization.
-        :param latitude: Required only if the geoOverride attribute is set.
-        Latitude with 7 digit precision after
-        decimal point, ranges between -90 and 90 degrees.
-        :param longitude: Required only if the geoOverride attribute is set.
-        Longitude with 7 digit precision after
-        decimal point, ranges between -180 and 180 degrees.
-        :param comment: String Additional information about this static
-        IP address
+
+        :param ip_address: (str) The static IP address
+        :param geo_override: (bool) If not set, geographic coordinates and city are automatically determined from the
+        IP address. Otherwise, the latitude and longitude coordinates must be provided.
+        :param routable_ip: (bool) Indicates whether a non-RFC 1918 IP address is publicly routable. This attribute is
+        ignored if there is no ZIA Private Service Edge associated to the organization.
+        :param latitude: (float) Required only if the geoOverride attribute is set. Latitude with 7 digit precision
+        after decimal point, ranges between -90 and 90 degrees.
+        :param longitude: (float) Required only if the geoOverride attribute is set. Longitude with 7 digit precision
+        after decimal point, ranges between -180 and 180 degrees.
+        :param comment: (str) Additional information about this static IP address
+
+        :return: (json)
         """
         url = "/staticIP"
-
         payload = {
-            "ipAddress": ipAddress,
+            "ipAddress": ip_address,
             "latitude": latitude,
             "longitude": longitude,
-            "routableIP": routableIP,
+            "routableIP": routable_ip,
             "comment": comment,
         }
-        if geoOverrride:
-            payload.update(geoOverrride=geoOverrride)
+        if geo_override:
+            payload.update(geoOverrride=geo_override)
             payload.update(latitude=latitude)
             payload.update(longitude=longitude)
 
         response = self.hp_http.post_call(
             url,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response.json()
 
-    def delete_staticIP(self, Id):
+    def delete_static_ip(
+        self,
+        ip_address_id: int,
+    ) -> requests.Response:
         """
         Deletes the static IP address for the specified ID.
-        :param Id: type integer. The unique identifier for the
-        provisioned static IP address.
-        :return: json
+
+        :param ip_address_id: (int) The unique identifier for the provisioned static IP address.
+
+        :return: (request.Response object))
         """
-        url = f"/staticIP/{Id}"
+        url = f"/staticIP/{ip_address_id}"
         response = self.hp_http.delete_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
 
         return response
 
     # User Authentication Settings
-    def list_exemptedUrls(self):
+    def list_exempted_urls(self) -> json:
         """
         Gets a list of URLs that were exempted from cookie authentication
+
+        :return: (json)
         """
         url = "/authSettings/exemptedUrls"
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def add_exemptedUrls(self, urls):
+    def add_exempted_urls(
+        self,
+        urls: list,
+    ) -> json:
         """
         Adds URLs to the cookie authentication exempt list to the list
-        :param urls: List of urls. Example ['url1','url2']
+
+        :param urls: (list) List of urls. Example ['url1','url2']
+
+        :return: (json)
         """
         url = "/authSettings/exemptedUrls?action=ADD_TO_LIST"
         payload = {"urls": urls}
         response = self.hp_http.post_call(
             url,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response.json()
 
-    def delete_exemptedUrls(self, urls):
+    def delete_exempted_urls(
+        self,
+        urls: list,
+    ) -> json:
         """
         Removed URLs to the cookie authentication exempt list to the list
-        :param urls: List of urls. Example ['url1','url2']
+
+        :param urls: (list) List of urls. Example ['url1','url2']
+
+        :return: (json)
         """
-        url = "/authSettings/exemptedUrls?action=REMOVE_FROM_LIST"
+        url = "/authSettings/exemptedUrls"
+        parameters = {"action": "REMOVE_FROM_LIST"}
         payload = {"urls": urls}
         response = self.hp_http.post_call(
             url,
+            params=parameters,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response.json()
 
     # Security Policy Settings
 
-    def list_security_whitelisted_urls(self):
+    def list_security_whitelisted_urls(self) -> json:
         """
         Gets a list of white-listed URLs
+
+        :return: (json)
         """
         url = "/security"
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def update_security_whitelisted_urls(self, urls):
+    def update_security_whitelisted_urls(
+        self,
+        urls: list,
+    ) -> json:
         """
-        Updates the list of white-listed URLs. This will overwrite
-        a previously-generated white list.
-        If you need to completely erase the white list, submit an empty list.
-        :param urls: list of urls ['www.zscaler.com', 'www.example.com']
+        Updates the list of white-listed URLs. This will overwrite a previously-generated white list. If you need to
+        completely erase the white list, submit an empty list.
+
+        :param urls: (list) List of urls ['www.zscaler.com', 'www.example.com']
+
+        :return: (json)
         """
         url = "/security"
         payload = {"whitelistUrls": urls}
         response = self.hp_http.put_call(
             url,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response.json()
 
-    def list_security_blacklisted_urls(self):
+    def list_security_blacklisted_urls(self) -> json:
         """
         Gets a list of white-listed URLs
+
+        :return: (json)
         """
         url = "/security/advanced"
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def update_security_blacklisted_urls(self, urls):
+    def update_security_blacklisted_urls(
+        self,
+        urls: list,
+    ) -> json:
         """
-        Updates the list of black-listed URLs. This will overwrite
-        a previously-generated black list.
-        If you need to completely erase the black list, submit an empty list.
+        Updates the list of black-listed URLs. This will overwrite a previously-generated black list. If you need to
+        completely erase the black list, submit an empty list.
+
+        :param urls: (list)
+
+        :return: (json)
         """
         url = "/security/advanced"
         payload = {"blacklistUrls": urls}
         response = self.hp_http.put_call(
             url,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response.json()
 
-    def add_security_blacklistUrls(self, urls):
+    def add_security_blacklist_urls(
+        self,
+        urls: list,
+    ) -> requests.Response:  # TODO: Move to return json
         """
-        :param urls: list of urls
         Adds a URL from the black list. To add a URL to the black list.
+
+        :param urls: (list) List of urls
+
+        :return: (request.Response object)
         """
-        url = "/security/advanced/blacklistUrls?action=ADD_TO_LIST"
+        url = "/security/advanced/blacklistUrls"
+        parameters = {"action": "ADD_TO_LIST"}
         payload = {"blacklistUrls": urls}
         response = self.hp_http.post_call(
             url,
             payload=payload,
+            params=parameters,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response
 
-    def remove_security_blacklistUrls(self, urls):
+    def remove_security_blacklist_urls(
+        self,
+        urls: list,
+    ) -> json:
         """
         Removes a URL from the black list.
-        :param urls: List of urls
+
+        :param urls: (list) List of urls
+
+        :return: (json)
         """
-        url = "/security/advanced/blacklistUrls?action=REMOVE_FROM_LIST"
+        url = "/security/advanced/blacklistUrls"
+        parameters = {"action" "REMOVE_FROM_LIST"}
         payload = {"blacklistUrls": urls}
         response = self.hp_http.post_call(
             url,
             payload=payload,
+            params=parameters,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response.json()
 
     # DLP Policies
 
-    def list_dlpDictionaries(self, dlpDicId=None):
+    def list_dlp_dictionaries(
+        self,
+        dlp_dic_id: int = None,
+    ) -> json:
         """
         Gets a list of all DLP Dictionaries.
-        :param dlpDicId: type int. dlp dictionary id ( optional parameter)
+
+        :param dlp_dic_id: (int) dlp dictionary id ( optional parameter)
+
+        :return: (json)
         """
-        if dlpDicId:
-            url = f"/dlpDictionaries/{dlpDicId}"
-        else:
-            url = "/dlpDictionaries"
+        url = "/dlpDictionaries"
+        if dlp_dic_id:
+            url = f"/dlpDictionaries/{dlp_dic_id}"
+
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def list_dlpDictionaries_lite(self):
+    def list_dlp_dictionaries_lite(self) -> json:
         """
         Gets a list of all DLP Dictionary names and ID's only. T
-        """
 
+        :return: (json)
+        """
         url = "/dlpDictionaries/lite"
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def validateDlpPattern(self, pattern):
+    def validate_dlp_pattern(
+        self,
+        pattern: str,
+    ) -> json:
         """
-        Validates the pattern used by a Pattern and Phrases DLP
-        dictionary type, and provides error information if the
-        pattern is invalid.
-        :param pattern: Regex pattern
-        :return: json
+        Validates the pattern used by a Pattern and Phrases DLP dictionary type, and provides error information if
+        the pattern is invalid.
+
+        :param pattern: (str) Regex pattern
+
+        :return: (json)
         """
         payload = pattern
         url = "/dlpDictionaries/validateDlpPattern"
         response = self.hp_http.post_call(
             url,
             cookies=self.cookies,
-            payload=payload,
+            payload=payload,  # TODO: payload is typically dict but here it is str?
             error_handling=True,
             headers=self.headers,
         )
+
         return response.json()
 
-    def delete_dlp_dictionaries(self, dlpDicId):
+    def delete_dlp_dictionaries(
+        self,
+        dlp_dic_id: int,
+    ) -> requests.Response:
         """
-        Deletes the custom DLP category for the specified ID.
-        You cannot delete predefined DLP dictionaries.
-        You cannot delete a custom dictionary while it is being used by a
-        DLP Engine or policy. Also, predefined
-        DLP dictionaries cannot be deleted.
-        :param dlpDicId: dlp dictionary ID
-        :return: json response
+        Deletes the custom DLP category for the specified ID. You cannot delete predefined DLP dictionaries. You
+        cannot delete a custom dictionary while it is being used by a DLP Engine or policy. Also, predefined DLP
+        dictionaries cannot be deleted.
+
+        :param dlp_dic_id: (int) dlp dictionary ID
+
+        :return: (requests.Response object)
         """
-        url = f"/dlpDictionaries/{dlpDicId}"
+        url = f"/dlpDictionaries/{dlp_dic_id}"
         response = self.hp_http.delete_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response
 
-    def add_dlpDictionaries(
+    def add_dlp_dictionaries(
         self,
-        dlpdicname,
-        customPhraseMatchType="MATCH_ANY_CUSTOM_PHRASE_PATTERN_DICTIONARY",
-        description=None,
-        phrases=None,
-        patterns=None,
-    ):
-        """
-        Adds a new custom DLP dictionary that uses either
-        Patterns and/or Phrases.
-        :param dlpdicname: type string.name
-        :param phrases: type list. list of phrases
-        :phrases valid example:[{
-        "action": "PHRASE_COUNT_TYPE_UNIQUE",
-        "phrase": "string"
-        }, {
-        "action": "PHRASE_COUNT_TYPE_UNIQUE",
-        "phrase": "string"
-        }]
-        :param patterns: type list. list of patterns
-        :patterns valid example:[{
-        "action": "PATTERN_COUNT_TYPE_UNIQUE",
-        "phrase": "string"
-        }, {
-        "action": "PATTERN_COUNT_TYPE_UNIQUE",
-        "phrase": "string"
-        }]
-        :param customPhraseMatchType: type string.customPhraseMatchType
-        :param description: description
-        """
+        dlp_dic_name: str,
+        custom_phrase_match_type: str = "MATCH_ANY_CUSTOM_PHRASE_PATTERN_DICTIONARY",
+        description: str = None,
+        phrases: list = None,
+        patterns: list = None,
+    ) -> json:
+        """
+        Adds a new custom DLP dictionary that uses either Patterns and/or Phrases.
+
+        :param dlp_dic_name: (str) Name
+        :param custom_phrase_match_type: (str) customPhraseMatchType
+        :param description: (str) description
+        :param phrases: (list) list of phrases. valid example:[
+        {"action": "PHRASE_COUNT_TYPE_UNIQUE", "phrase": "string"},
+        {"action": "PHRASE_COUNT_TYPE_UNIQUE", "phrase": "string"}
+        ]
+        :param patterns: (list) list of patterns. valid example:[
+        {"action": "PATTERN_COUNT_TYPE_UNIQUE", "phrase": "string"},
+        {"action": "PATTERN_COUNT_TYPE_UNIQUE", "phrase": "string"}
+        ]
 
+        :return: (json)
+        """
         if phrases is not None:
             for i in phrases:
                 if i["action"] not in [
                     "PHRASE_COUNT_TYPE_UNIQUE",
                     "PHRASE_COUNT_TYPE_ALL",
                 ]:
                     raise ValueError("Invalid action")
@@ -1369,661 +1642,829 @@
             for k in patterns:
                 if k["action"] not in [
                     "PATTERN_COUNT_TYPE_UNIQUE",
                     "PATTERN_COUNT_TYPE_ALL",
                 ]:
                     raise ValueError("Invalid action")
 
-        if customPhraseMatchType not in [
+        if custom_phrase_match_type not in [
             "MATCH_ALL_CUSTOM_PHRASE_PATTERN_DICTIONARY",
             "MATCH_ANY_CUSTOM_PHRASE_PATTERN_DICTIONARY",
         ]:
             raise ValueError("Invalid customPhraseMatchType")
 
         url = "/dlpDictionaries"
         payload = {
-            "name": dlpdicname,
+            "name": dlp_dic_name,
             "description": description,
             "confidenceThreshold": None,
-            "customPhraseMatchType": customPhraseMatchType,
+            "customPhraseMatchType": custom_phrase_match_type,
             "dictionaryType": "PATTERNS_AND_PHRASES",
             "phrases": phrases,
             "patterns": patterns,
         }
         response = self.hp_http.post_call(
             url,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response.json()
 
-    def list_dlpEngines(self, dlpEngineId=None):
+    def list_dlp_engines(
+        self,
+        dlp_engine_id: int = None,
+    ) -> json:
         """
         Get a list of DLP engines.
-        :param dlpEngineId: type integer. Optinal value.
-        The unique identifier for the DLP engine
-        :return: json
+
+        :param dlp_engine_id: (int) Optional value. The unique identifier for the DLP engine
+
+        :return: (json)
         """
-        if dlpEngineId:
-            url = f"/dlpEngines/{dlpEngineId}"
-        else:
-            url = "/dlpEngines"
+        url = "/dlpEngines"
+        if dlp_engine_id:
+            url = f"/dlpEngines/{dlp_engine_id}"
+
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def list_dlpExactDataMatchSchemas(self):
+    def list_dlp_exact_data_match_schemas(self) -> json:
         """
-        Exact Data Match (EDM) templates (or EDM schemas) allow the
-        Zscaler service to identify a record from a structured
-        data source that matches predefined criteria. Using the Index Tool,
-        you can create an EDM template that allows
-        you to define this criteria (i.e., define the tokens) for your data
-        records by importing a CSV file.
-        After the data is defined and submitted within the tool, you can then
-        apply the EDM template to a custom DLP
-        dictionary or engine. This endpoint gets the EDM templates for all
-        Index Tools used by the organization
+        Exact Data Match (EDM) templates (or EDM schemas) allow the Zscaler service to identify a record from a
+        structured data source that matches predefined criteria. Using the Index Tool, you can create an EDM template
+        that allows you to define the criteria (i.e., define the tokens) for your data records by importing a CSV
+        file. After the data is defined and submitted within the tool, you can then apply the EDM template to a custom
+        DLP dictionary or engine. This endpoint gets the EDM templates for all Index Tools used by the organization
 
-        :return: json
+        :return: (json)
         """
         url = "/dlpExactDataMatchSchemas"
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def list_dlpNotificationTemplates(self, templateId=None):
+    def list_dlp_notification_templates(
+        self,
+        template_id: int = None,
+    ) -> json:
         """
         Gets a list of DLP notification templates
-        :param templateId: type integer. Optional value. The unique identifier
-        for a DLP notification template
-        :return: json
+
+        :param template_id: (int) Optional value. The unique identifier for a DLP notification template
+
+        :return: (json)
         """
-        if templateId:
-            url = f"/dlpNotificationTemplates/{templateId}"
-        else:
-            url = "/dlpNotificationTemplates"
+        url = "/dlpNotificationTemplates"
+        if template_id:
+            url = f"/dlpNotificationTemplates/{template_id}"
+
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def add_dlpNotificationTemplates(
+    def add_dlp_notification_templates(
         self,
-        name,
-        subject,
-        plainTextMessage,
-        htmlMessage,
-        attachContent=True,
-        tlsEnabled=True,
-    ):
-        """
-
-        :param name: type string. The DLP notification template name
-        :param subject: type string. The Subject line that is displayed
-        within the DLP notification template
-        :param plainTextMessage: type string. The temaplte for the plain text
-        UTF-8 message body that must be displayed
-        in the DLP notification email.
-        :param htmlMessage: type string. The template for the HTML message
-        body that myst tbe displayed in the DLP
+        name: str,
+        subject: str,
+        plain_text_message: str,
+        html_message: str,
+        attach_content: bool = True,
+        tls_enabled: bool = True,
+    ) -> json:
+        """
+        :param name: (str) The DLP notification template name
+        :param subject: (str) The Subject line that is displayed within the DLP notification template
+        :param plain_text_message: (str) The template for the plain text UTF-8 message body that must be displayed in
+        the DLP notification email.
+        :param html_message: (str) The template for the HTML message body that myst tbe displayed in the DLP
         notification email
-        :param attachContent: type boolean. if set to True, the content that
-        is violation is attached to the DLP
+        :param attach_content: (bool) if set to True, the content that is violation is attached to the DLP
         notification email
-        :patam tlsEnabled: type boolean. If set to True tls will be used to
-        send email.
-        :return:
+        :param tls_enabled: (bool) If set to True tls will be used to send email.
+
+        :return: (json)
         """
         url = "/dlpNotificationTemplates"
         payload = {
             "name": name,
             "subject": subject,
-            "tlsEnabled": tlsEnabled,
-            "attachContent": attachContent,
-            "plainTextMessage": plainTextMessage,
-            "htmlMessage": htmlMessage,
+            "tlsEnabled": tls_enabled,
+            "attachContent": attach_content,
+            "plainTextMessage": plain_text_message,
+            "htmlMessage": html_message,
         }
         response = self.hp_http.post_call(
             url,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response.json()
 
-    def delete_dlpNotificationTemplates(self, templateId):
+    def delete_dlp_notification_templates(
+        self,
+        template_id: int,
+    ) -> requests.Response:  # TODO: return json instead
         """
         Deletes a DLP notification template
-        :param templateId: type int. the unique identifies for
-        the DLP notification template
-        :return: json
+
+        :param template_id: (int) The unique identifies for the DLP notification template
+        :return: (requests.Response Object)
         """
-        url = f"/dlpNotificationTemplates/{templateId}"
+        url = f"/dlpNotificationTemplates/{template_id}"
         response = self.hp_http.delete_call(
-            url=url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url=url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response
 
-    def list_icapServer(self, icapServerId=None):
+    def list_icap_server(
+        self,
+        icap_server_id: int = None,
+    ) -> json:
         """
         Gets a list of DLP notification templates
-        :param icapServerId: type integer. Optional value. The unique
-        identifier for the DLP server using ICAP
-        :return: json
+
+        :param icap_server_id: (int) Optional value. The unique identifier for the DLP server using ICAP
+
+        :return: (json)
         """
-        if icapServerId:
-            url = f"/icapServers/{icapServerId}"
-        else:
-            url = "/icapServers"
+        url = "/icapServers"
+        if icap_server_id:
+            url = f"/icapServers/{icap_server_id}"
+
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def list_idmprofile(self, profileId=None):
+    def list_idm_profile(
+        self,
+        profile_id: int = None,
+    ) -> json:
         """
-        List all the IDM templates for all Index Tools
-        used by the organization. If profileId, it lists the
-        IDM template information for the specified ID.
-        :param profileId: type integer. Optional value. The unique
-        identifier for the IDM template (or profile)
-        :return: json
+        List all the IDM templates for all Index Tools used by the organization. If profileId, it lists the IDM
+        template information for the specified ID.
+
+        :param profile_id: (int) Optional value. The unique identifier for the IDM template (or profile)
+
+        :return: (json)
         """
-        if profileId:
-            url = f"/idmprofile/{profileId}"
+        if profile_id:
+            url = f"/idmprofile/{profile_id}"
         else:
             url = "/idmprofile"
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def list_webDlpRules(self, ruleId=None):
+    def list_web_dlp_rules(
+        self,
+        rule_id: int = None,
+    ) -> json:
         """
-        list DLP policy rules, excluding SaaS Security API DLP policy rules.
-        If ruleId, list DLP policy rule
+        list DLP policy rules, excluding SaaS Security API DLP policy rules. If ruleId, list DLP policy rule
         information for the specified ID
-        :param ruleId: type integer. Optional value.
-        The unique identifier for theDLP rule
-        :return: json
+
+        :param rule_id: (int) Optional value. The unique identifier for theDLP rule
+
+        :return: (json)
         """
-        if ruleId:
-            url = f"/webDlpRules/{ruleId}"
-        else:
-            url = "/webDlpRules"
+        url = "/webDlpRules"
+        if rule_id:
+            url = f"/webDlpRules/{rule_id}"
+
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def delete_webDlpRules(self, ruleId):
+    def delete_web_dlp_rules(
+        self,
+        rule_id: int,
+    ) -> json:
         """
-        Deletes a DLP policy rule. This endpoint is not applicable
-        to SaaS Security API DLP policy rules.
-        :param ruleId: type integer. The unique identifier for the
-        DLP policy rule.
-        :return: json
+        Deletes a DLP policy rule. This endpoint is not applicable to SaaS Security API DLP policy rules.
+
+        :param rule_id: (int) The unique identifier for the DLP policy rule.
+
+        :return: (json)
         """
-        url = f"/webDlpRules/{ruleId}"
+        url = f"/webDlpRules/{rule_id}"
         response = self.hp_http.delete_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
     # Firewall Policies
 
-    def list_networkServices(self, serviceId=None):
+    def list_network_services(
+        self,
+        service_id: int = None,
+    ) -> json:
         """
-        Gets a list of all network service groups. The search parameters
-        find matching values within the "name" or
+        Gets a list of all network service groups. The search parameters find matching values within the "name" or
         "description" attributes.
+
+        :param service_id: (int)
+
+        :return: (json)
         """
-        if serviceId:
-            url = f"/networkServices/{serviceId}"
-        else:
-            url = "/networkServices"
+        url = "/networkServices"
+        if service_id:
+            url = f"/networkServices/{service_id}"
+
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def add_networkServices(
+    def add_network_services(
         self,
-        name,
-        tag=None,
-        srcTcpPorts=None,
-        destTcpPorts=None,
-        srcUdpPorts=None,
-        destUdpPorts=None,
-        type="CUSTOM",
-        description=None,
-        isNameL10nTag=False,
-    ):
+        name: str,
+        tag: str = None,
+        src_tcp_ports: list = None,
+        dest_tcp_ports: list = None,
+        src_udp_ports: list = None,
+        dest_udp_ports: list = None,
+        service_type: str = "CUSTOM",
+        description: str = None,
+        is_name_l10n_tag: bool = False,
+    ) -> requests.Response:  # TODO: return json
         """
         Adds a new network service.
-        :param name: type string. Name
-        :param tag: type string
-        :param srcTcpPorts: type list. Each element
-        is [{"start": int, "end": int}]
-        :param destTcpPorts: type list. Each element
-        is [{"start": int, "end": int}]
-        :param srcUdpPorts: type list. Each element
-        is [{"start": int, "end": int}]
-        :param destUdpPorts: type list. Each element
-        is [{"start": int, "end": int}]
-        :param type: type string. STANDARD|PREDEFINE|CUSTOM
-        :param description: type string. Description
-        :param isNameL10nTag: type boolean.
-        :return: json response from API
+
+        :param name: (str) Name
+        :param tag: (str)
+        :param src_tcp_ports:(list) Each element is [{"start": int, "end": int}]
+        :param dest_tcp_ports:(list) Each element is [{"start": int, "end": int}]
+        :param src_udp_ports:(list) Each element is [{"start": int, "end": int}]
+        :param dest_udp_ports:(list) Each element is [{"start": int, "end": int}]
+        :param service_type: (str) STANDARD|PREDEFINE|CUSTOM
+        :param description: (str) Description
+        :param is_name_l10n_tag: (bool)
+
+        :return: (requests.Response Object)
         """
         url = "/networkServices"
-
         payload = {
             "id": 0,
             "name": name,
             "tag": tag,
-            "srcTcpPorts": srcTcpPorts,
-            "destTcpPorts": destTcpPorts,
-            "srcUdpPorts": srcUdpPorts,
-            "destUdpPorts": destUdpPorts,
-            "type": type,
+            "srcTcpPorts": src_tcp_ports,
+            "destTcpPorts": dest_tcp_ports,
+            "srcUdpPorts": src_udp_ports,
+            "destUdpPorts": dest_udp_ports,
+            "type": service_type,
             "description": description,
-            "isNameL10nTag": isNameL10nTag,
+            "isNameL10nTag": is_name_l10n_tag,
         }
-        print(payload)
         response = self.hp_http.post_call(
             url,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response
 
-    def delete_networkServices(self, serviceid):
+    def delete_network_services(
+        self,
+        service_id: int,
+    ) -> requests.Response:
         """
+        :param service_id: (int) The unique identifier for the network service
 
-        :param serviceid: type int. The unique identifier
-        for the network service
-        :return: json
+        :return: (requests.Response Object)
         """
-        url = f"/networkServices/{serviceid}"
+        url = f"/networkServices/{service_id}"
         response = self.hp_http.delete_call(
-            url, cookies=self.cookies, error_handling=False, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=False,
+            headers=self.headers,
         )
+
         return response
 
-    def list_firewallFilteringRules(self, ruleId=None):
+    def list_firewall_filtering_rules(
+        self,
+        rule_id: int = None,
+    ) -> json:
         """
         Gets all rules in the Firewall Filtering policy.
+
+        :param rule_id: (int)
+
+        :return: (json)
         """
-        if ruleId:
-            url = f"/firewallFilteringRules/{ruleId}"
-        else:
-            url = "/firewallFilteringRules"
+        url = "/firewallFilteringRules"
+        if rule_id:
+            url = f"/firewallFilteringRules/{rule_id}"
+
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def add_firewallFilteringRules(
+    def add_firewall_filtering_rules(
         self,
-        name,
-        order,
-        state,
-        action,
-        description=None,
-        defaultRule=False,
-        predefined=False,
-        srcIps=None,
-        destAddresses=None,
-        destIpGroups=None,
-        srcIpGroups=None,
-        destIpCategories=None,
+        name: str,
+        order: int,
+        state: str,
+        action: str,
+        description: str = None,
+        default_rule: bool = False,
+        predefined: bool = False,
+        src_ips: list = None,
+        dest_addresses: list = None,
+        dest_ip_groups: list = None,
+        src_ip_groups: list = None,
+        dest_ip_categories: list = None,
         labels=None,
-        nwServices=None,
-        rank=0,
+        nw_services: list = None,
+        rank: int = 0,
         **kwargs,
-    ):
-        """
-        :param name: type str,  Name of the Firewall
-        Filtering policy rule ["String"]
-        :param order: type int, Rule order number of the
-        Firewall Filtering policy rule
-        :param state: type str, Possible values : DISABLED or  ENABLED
-        :param action: type str, Possible values: ALLOW, BLOCK_DROP,
-        BLOCK_RESET, BLOCK_ICMP, EVAL_NWAPP
-        :param rank: type int, Admin rank of the Firewall Filtering policy rule
-        :param description: type str, Additional information about the rule
-        :param defaultRule: Default is false.If set to true,
-        the default rule is applied
-        :param predefined: Boolean
-        :param srcIps: type list, List of source IP addresses
-        :param destAddresses: type list. List of destination addresses
-        :param destIpGroups: type list: List of user-definied
-        destination IP address groups
-        :param srcIpGroups: type list: List of user defined source
-        IP address groups
-        :param destIpCategories: type list: list of destination IP categories
-        :param nwServices: type list. List of user-defined network services
-        on whih the rule is applied
-        :return: Default is false.If set to true, a predefined rule is applied
+    ) -> requests.Response:
         """
+        :param name: (str) Name of the Firewall Filtering policy rule ["String"]
+        :param order: (int), Rule order number of the Firewall Filtering policy rule
+        :param state: (str) Possible values : DISABLED or  ENABLED
+        :param action: (str) Possible values: ALLOW, BLOCK_DROP, BLOCK_RESET, BLOCK_ICMP, EVAL_NWAPP
+        :param description: (str) Additional information about the rule
+        :param default_rule: (bool) Default is false.If set to true, the default rule is applied
+        :param predefined: (bool)
+        :param src_ips: (list) List of source IP addresses
+        :param dest_addresses: (list) List of destination addresses
+        :param dest_ip_groups: (list) List of user-defined destination IP address groups
+        :param src_ip_groups: (list) List of user defined source IP address groups
+        :param dest_ip_categories:(list) list of destination IP categories
+        :param labels: (?)
+        :param nw_services: (list) List of user-defined network services on with the rule is applied
+        :param rank: (int), Admin rank of the Firewall Filtering policy rule
 
+        :return: (requests.Response Object)
+        """
         url = "/firewallFilteringRules"
         payload = {
             "accessControl": "READ_WRITE",
             "enableFullLogging": False,
             "name": name,
             "order": order,
             "rank": rank,
             "action": action,
             "state": state,
             "predefined": predefined,
-            "defaultRule": defaultRule,
+            "defaultRule": default_rule,
             "description": description,
         }
-        if srcIps:
-            payload.update(srcIps=srcIps)
-        if srcIpGroups:
-            payload.update(srcIpGroups=srcIpGroups)
-        if destAddresses:
-            payload.update(destAddresses=destAddresses)
-        if destIpGroups:
-            payload.update(destIpGroups=destIpGroups)
+        if src_ips:
+            payload.update(srcIps=src_ips)
+        if src_ip_groups:
+            payload.update(srcIpGroups=src_ip_groups)
+        if dest_addresses:
+            payload.update(destAddresses=dest_addresses)
+        if dest_ip_groups:
+            payload.update(destIpGroups=dest_ip_groups)
         if labels:
             payload.update(labels=labels)
-        if destIpCategories:
-            payload.update(destIpCategories=destIpCategories)
-        if nwServices:
-            payload.update(nwServices=nwServices)
+        if dest_ip_categories:
+            payload.update(destIpCategories=dest_ip_categories)
+        if nw_services:
+            payload.update(nwServices=nw_services)
         response = self.hp_http.post_call(
             url,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response
 
-    def delete_firewallFIlteringRules(self, ruleId):
+    def delete_firewall_f_iltering_rules(
+        self,
+        rule_id: int,
+    ) -> requests.Response:
         """
         Deletes a Firewall Filtering policy rule for the specified ID.
 
-        :param ruleId: type integer: The unique identifier for the policy rule
-        :return: json
+        :param rule_id: (int) The unique identifier for the policy rule
+
+        :return: (requests.Response Object)
         """
-        url = f"/firewallFilteringRules/{ruleId}"
+        url = f"/firewallFilteringRules/{rule_id}"
         response = self.hp_http.delete_call(
-            url, cookies=self.cookies, error_handling=False, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=False,
+            headers=self.headers,
         )
+
         return response
 
-    def list_ipSourceGroups(self, ipGroupId=None):
+    def list_ip_source_groups(
+        self,
+        ip_group_id: int = None,
+    ) -> json:
         """
-        Gets a list of all IP source groups. The search parameters find
-        matching values within the "name" or
+        Gets a list of all IP source groups. The search parameters find matching values within the "name" or
         "description" attributes.
-        :param ipGroupId: Option ip group id
+
+        :param ip_group_id: (int) Option ip group id
+
+        :return: (json)
         """
-        if ipGroupId:
-            url = f"/ipSourceGroups/{ipGroupId}"
-        else:
-            url = "/ipSourceGroups"
+        url = "/ipSourceGroups"
+        if ip_group_id:
+            url = f"/ipSourceGroups/{ip_group_id}"
+
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def list_ipSourceGroups_lite(
-        self,
-    ):
+    def list_ip_source_groups_lite(self) -> json:
         """
         Gets a name and ID dictionary of all IP source groups
-        :return:
+
+        :return: (json)
         """
         url = "/ipSourceGroups/lite"
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def list_ipDestinationGroups(self, ipGroupId=None):
+    def list_ip_destination_groups(
+        self,
+        ip_group_id: int = None,
+    ) -> json:
         """
-        Gets a list of all IP source groups. The search parameters
-        find matching values within the "name" or
+        Gets a list of all IP source groups. The search parameters find matching values within the "name" or
         "description" attributes.
-        :param ipGroupId: Option ip group id
+
+        :param ip_group_id: (int) Option ip group id
+
+        :return: (json)
         """
-        if ipGroupId:
-            url = f"/ipDestinationGroups/{ipGroupId}"
-        else:
-            url = "/ipDestinationGroups/"
+        url = "/ipDestinationGroups/"
+        if ip_group_id:
+            url = f"/ipDestinationGroups/{ip_group_id}"
+
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def list_ipDestinationGroups_lite(self):
+    def list_ip_destination_groups_lite(self) -> json:
         """
         Gets a name and ID dictionary of all IP destination groups
-        return json
-        """
 
+        :return: (json)
+        """
         url = "/ipDestinationGroups/lite"
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def add_ipSourceGroups(self, name, ipAddresses, description=None):
-        """
-        :param name: mame
-        :param ipAddresses: list of IP addresses
-        :param description: description
-        """
+    def add_ip_source_groups(
+        self,
+        name: str,
+        ip_addresses: list,
+        description: str = None,
+    ) -> json:
+        """
+        :param name: (str) Name
+        :param ip_addresses: (list) List of IP addresses
+        :param description: (str) description
 
+        :return: (json)
+        """
         url = "/ipSourceGroups"
-        payload = {"name": name, "ipAddresses": ipAddresses, "description": description}
+        payload = {
+            "name": name,
+            "ipAddresses": ip_addresses,
+            "description": description,
+        }
         response = self.hp_http.post_call(
             url,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response.json()
 
-    def delete_ipSourceGroups(self, ipGroupId):
+    def delete_ip_source_groups(
+        self,
+        ip_group_id: int,
+    ) -> requests.Response:
         """
         Deletes the IP source group for the specified ID
-        :param ipGroupId:  type int. The unique identifies
-        for the IP source group
-        :return: json
+
+        :param ip_group_id: (int) The unique identifies for the IP source group
+
+        :return: (requests.Response Object)
         """
-        url = f"/ipSourceGroups/{ipGroupId}"
+        url = f"/ipSourceGroups/{ip_group_id}"
         response = self.hp_http.delete_call(
             url,
             cookies=self.cookies,
             error_handling=True,
             payload={},
             headers=self.headers,
         )
+
         return response
 
-    def delete_ipDestinationGroups(self, ipGroupId):
+    def delete_ip_destination_groups(
+        self,
+        ip_group_id: int,
+    ) -> requests.Response:
         """
         Deletes the IP destination group for the specified ID
-        :param ipGroupId:  type int. The uniquye identifies
-        for the IP source group
-        :return: json
+
+        :param ip_group_id: (int) The unique identifies for the IP source group
+
+        :return: (requests.Response Object)
         """
-        url = f"/ipDestinationGroups/{ipGroupId}"
+        url = f"/ipDestinationGroups/{ip_group_id}"
         response = self.hp_http.delete_call(
             url,
             cookies=self.cookies,
             error_handling=True,
             payload={},
             headers=self.headers,
         )
+
         return response
 
-    def add_ipDestinationGroups(
-        self, name, type, addresses, ipCategories=None, countries=None, description=None
-    ):
-        """
-        :param name: mame
-        :param type: Destination IP group type.
-        Either DSTN_IP or  DSTN_FQDN or DSTN_DOMAIN
-        :param addresses: List of Destination IP addresses within the group.
-        :param description: description
-        :param ipCategories: List of Destination IP address URL categories.
-        You can identify destination based
+    def add_ip_destination_groups(
+        self,
+        name: str,
+        dest_ip_group_type: str,
+        addresses: list,
+        ip_categories: list = None,
+        countries: list = None,
+        description: str = None,
+    ) -> json:
+        """
+        :param name: (str) Name
+        :param dest_ip_group_type: (str) Destination IP group type. Either DSTN_IP or  DSTN_FQDN or DSTN_DOMAIN
+        :param addresses: (list) List of Destination IP addresses within the group.
+        :param ip_categories: (list) List of Destination IP address URL categories. You can identify destination based
         on the URL category of the domain. Default value ANY
-        :param countries: list of destination IP address countries.
-        You can identify destinations based on the location
-        of a server.Default value ANY
-        """
-        if type not in ["DSTN_IP", "DSTN_FQDN", "DSTN_DOMAIN"]:
+        :param countries: (list) List of destination IP address countries. You can identify destinations based on
+        the location of a server.Default value ANY
+        :param description: (str) description
+        """
+        if dest_ip_group_type not in [
+            "DSTN_IP",
+            "DSTN_FQDN",
+            "DSTN_DOMAIN",
+        ]:
             raise ValueError("Invalid destination type ")
         if countries:
             for i in countries:
                 if i not in valid_countries:
                     raise ValueError("Invalid country ")
         else:
             countries = []
 
-        if ipCategories:
-            for j in ipCategories:
+        if ip_categories:
+            for j in ip_categories:
                 if j not in valid_category_ids:
                     raise ValueError("Invalid country ")
         else:
-            ipCategories = []
+            ip_categories = []
 
         url = "/ipDestinationGroups"
         payload = {
             "name": name,
-            "type": type,
+            "type": dest_ip_group_type,
             "addresses": addresses,
-            "ipCategories": ipCategories,
+            "ipCategories": ip_categories,
             "countries": countries,
             "description": description,
         }
-        print(payload)
         response = self.hp_http.post_call(
             url,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response.json()
 
     # Device Groups
 
-    def list_devices_groups(self, query=None):
+    def list_devices_groups(
+        self,
+        query: str = None,
+    ) -> json:
         """
         Gets a list of device groups
-        :param query:
-        :return: List
+
+        :param query: (str)
+
+        :return: (json)
         """
+        url = "/deviceGroups"
         if query:
             url = f"/deviceGroups?{query}"
-        else:
-            url = "/deviceGroups"
 
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def list_devices(self, query=None):
+    def list_devices(
+        self,
+        query: str = None,
+    ) -> json:
         """
-        Gets a list of devices. Any given search parameters will be applied
-        during device search. Search parameters are
-         based on device name, model, owner, OS type, and OS version.
-         The devices listed can also be restricted to return
-         information only for ones belonging to specific users.
-        :param query:
-        :return: List
+        Gets a list of devices. Any given search parameters will be applied during device search. Search parameters
+        are based on device name, model, owner, OS type, and OS version. The devices listed can also be restricted
+        to return information only for ones belonging to specific users.
+
+        :param query: (str)
+
+        :return: (json)
         """
+        url = "/deviceGroups/devices"
         if query:
             url = f"/deviceGroups/devices?{query}"
-        else:
-            url = "/deviceGroups/devices"
 
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
     # Rule Labels
-    def list_rule_labels(self, ruleLabelId=None):
+    def list_rule_labels(
+        self,
+        rule_label_id: int = None,
+    ) -> json:
         """
         Gets rule label information for the specified ID
-        :param ruleLabelId:
-        :return: List
-        """
-        if ruleLabelId:
-            url = f"/ruleLabels/{ruleLabelId}"
 
-        else:
-            url = "/ruleLabels?pageSize=1000"
+        :param rule_label_id: (int)
+
+        :return: (json)
+        """
+        url = "/ruleLabels?pageSize=1000"
+        if rule_label_id:
+            url = f"/ruleLabels/{rule_label_id}"
 
         response = self.hp_http.get_call(
-            url, cookies=self.cookies, error_handling=True, headers=self.headers
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
         )
+
         return response.json()
 
-    def add_rule_label(self, payload):
+    def add_rule_label(
+        self,
+        payload: dict,
+    ) -> json:
         """
         Adds new rule labels with the given name
-        :param name: name
-        :param description: description
+        :param name: (str) name  # FIXME: Not in passed attributes.
+        :param description: (str) description  # FIXME: Not in passed attributes.
+        :param payload: (dict)
         """
         url = "/ruleLabels"
         response = self.hp_http.post_call(
             url,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
             payload=payload,
         )
+
         return response.json()
 
-    def update_call(self, url, payload):
+    def update_call(
+        self,
+        url: str,
+        payload: json,
+    ) -> json:
         """
-        Generic PUT call. This call will overwrite all the
-        configuration with the new payload
-        :param url: url of Zscaler API call
-        :param payload: type json. Payload
+        Generic PUT call. This call will overwrite all the configuration with the new payload
+
+        :param url: (str) url of Zscaler API call
+        :param payload: (json) Payload
+
+        :return: (json)
         """
         response = self.hp_http.put_call(
             url,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response.json()
 
-    def add_call(self, url, payload):
+    def add_call(
+        self,
+        url: str,
+        payload: json,
+    ) -> json:
         """
-        Generic POST call. This call will add all the
-        configuration with the new payload
-        :param url: url of Zscaler API call
-        :param payload: type json. Payload
+        Generic POST call. This call will add all the configuration with the new payload
+
+        :param url: (str) url of Zscaler API call
+        :param payload: (json) Payload
+
+        :return: (json)
         """
         response = self.hp_http.post_call(
             url,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
+
         return response.json()
```

### Comparing `zscaler_api_talkers-4.1.0/zscaler_api_talkers/zscaler_helpers/http_calls.py` & `zscaler_api_talkers-4.1.1/zscaler_api_talkers/zscaler_helpers/http_calls.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,121 +1,183 @@
-import pdb
-
 import requests
+from .logger import setup_logger
+
+logger = setup_logger(name=__name__)
+
+
+def _zia_http_codes(response: requests.Response):
+    """
+    Internal method to display HTTP error handling and response codes. For more information, please refer to
+    https://help.zscaler.com/zia/about-error-handling
+
+    :param response: (requests.Response Object)
+    """
+    if response.status_code in [200, 201, 202, 204]:
+        return
+    elif response.status_code == 401:
+        raise ValueError(
+            f"{response.status_code} :Session is not authenticated or timed out"
+        )
+    elif response.status_code == 403:
+        raise ValueError(
+            f"{response.status_code} :API key disabled or SKU subscription missing or user role has not access"
+        )
+    elif response.status_code == 404:
+        raise ValueError("Resource does not exist")
+    elif response.status_code == 409:
+        raise ValueError(
+            "Request could not be processed because of possible edit conflict occurred"
+        )
+    elif response.status_code == 415:
+        raise ValueError("Unsupported media type")
+    elif response.status_code == 429:
+        raise ValueError("Exceeded the rate limit or quota")
+    elif response.status_code == 500:
+        raise ValueError("Unexpected error")
+    elif response.status_code == 503:
+        raise ValueError("Service is temporarily unavailable")
+    else:
+        print(response.content)
+        raise ValueError(f"Unexpected HTTP response code: {response.status_code}")
 
 
 class HttpCalls(object):
     """
     class to Perform HTTP calls
     """
 
-    def __init__(self, host, header=None, verify=True):
+    def __init__(
+        self,
+        host: str,
+        header: dict = None,
+        verify: bool = True,
+    ):
         """
         to start this instance, host IP address or fqdn is required
-        :param host: IP address or fqdn
-        :param header: dictionary. HTTP header
-        :param verify: Boolean. True to verify ssl cert with in HTTP call
+
+        :param host: (str) IP address or fqdn
+        :param header: (dict) HTTP header
+        :param verify: (bool) True to verify ssl cert with in HTTP call
         """
         self.version = "1.1"
         self.host = host
         self.headers = {"Content-type": "application/json", "Cache-Control": "no-cache"}
         if header:
             self.headers.update(header)
         self.cookies = None
         self.verify = verify
 
     def get_call(
-        self, url, cookies=None, headers=None, params=None, error_handling=False
-    ):
+        self,
+        url: str,
+        cookies: dict = None,
+        headers: dict = None,
+        params: dict = None,
+        error_handling: bool = False,
+    ) -> requests.Response:
         """
         Method to perform a GET HTTP  call
-        :param url: url
-        :param cookies: cookies
-        :param headers: Additional HTTP headers
-        :param params: Key,Value parameters in the URL after a question mark
-        :param error_handling: Boolean, when TRUE will use Zscaler HTTP codes
-        :return: response
+
+        :param url: (str) url
+        :param cookies: (str) cookies
+        :param headers: (dict) Additional HTTP headers
+        :param params: (dict) Key,Value parameters in the URL after a question mark
+        :param error_handling: (bool) when TRUE will use Zscaler HTTP codes
+
+        :return: (requests.Response Object)
         """
         full_url = f"{self.host}{url}"
         if headers:
             self.headers.update(headers)
         try:
             response = requests.get(
                 url=full_url,
                 headers=self.headers,
                 cookies=cookies,
                 params=params,
                 verify=self.verify,
             )
             if error_handling:
-                self._zia_http_codes(response)
+                _zia_http_codes(response)
             else:
                 if response.status_code not in [200, 201, 204]:
                     raise ValueError(f"{response.status_code} -> {response.content}")
             return response
         except requests.HTTPError as e:
             raise ValueError(e)
 
     def post_call(
         self,
-        url,
-        payload,
-        headers=None,
-        cookies=None,
-        error_handling=False,
-        urlencoded=False,
-    ):
+        url: str,
+        payload: dict,
+        params: dict = None,
+        headers: dict = None,
+        cookies: dict = None,
+        error_handling: bool = False,
+        urlencoded: bool = False,
+    ) -> requests.Response:
         """
         Method to perform an HTTP POST call
-        :param url: url
-        :param cookies: cookies
-        :param error_handling: Boolean, when TRUE will use Zscaler HTTP codes
-        :return: response
+
+        :param url: (str) url
+        :param payload: (dict)
+        :param params: (dict)
+        :param headers: (dict)
+        :param cookies: (str) cookies
+        :param error_handling: (bool) when TRUE will use Zscaler HTTP codes
+        :param urlencoded: (bool)
+
+        :return: (requests.Response Object)
         """
         full_url = f"{self.host}{url}"
         try:
             if urlencoded:
                 url_encoded_headers = headers
                 response = requests.post(
                     url=full_url,
+                    params=params,
                     headers=url_encoded_headers,
                     cookies=cookies,
                     data=payload,
                     verify=self.verify,
                 )
             else:
                 if headers:
                     self.headers.update(headers)
                 response = requests.post(
                     url=full_url,
+                    params=params,
                     headers=self.headers,
                     cookies=cookies,
                     json=payload,
                     verify=self.verify,
                 )
             if error_handling:
-                self._zia_http_codes(response)
+                _zia_http_codes(response)
             else:
                 if response.status_code not in [200, 201, 204]:
                     raise ValueError(f"{response.status_code} -> {response.content}")
             return response
         except requests.HTTPError as e:
             raise ValueError(e)
 
     def patch_call(
         self,
-        url,
-        payload,
-        cookies=None,
-    ):
+        url: str,
+        payload: dict,
+        cookies: dict = None,
+    ) -> requests.Response:
         """
         Method to perform an HTTP PATH call
-        :param url: url
-        :param cookies: cookies
-        :return: response
+
+        :param url: (str) url
+        :param payload: (dict)
+        :param cookies: (str) cookies
+
+        :return: (requests.Response Object)
         """
         full_url = f"{self.host}{url}"
         try:
             response = requests.patch(
                 url=full_url,
                 headers=self.headers,
                 cookies=cookies,
@@ -124,105 +186,92 @@
             )
             if response.status_code not in [200, 201, 204]:
                 raise ValueError(response.status_code)
             return response
         except requests.HTTPError as e:
             raise ValueError(e)
 
-    def put_call(self, url, payload, headers=None, cookies=None, error_handling=False):
+    def put_call(
+        self,
+        url: str,
+        payload: dict,
+        params: dict = None,
+        headers: dict = None,
+        cookies: dict = None,
+        error_handling: bool = False,
+    ) -> requests.Response:
         """
         Method to perform an HTTP PUT call
-        :param url: url
-        :param cookies: cookies
-        :param error_handling: Boolean, when TRUE will use Zscaler HTTP codes
-        :return: response
+
+        :param url: (str) url
+        :param params: (dict) Parameters to add to url
+        :param payload: (dict)
+        :param headers: (dict)
+        :param cookies: (str) cookies
+        :param error_handling: (bool) when TRUE will use Zscaler HTTP codes
+
+        :return: (requests.Response Object)
         """
         full_url = f"{self.host}{url}"
         if headers:
             self.headers.update(headers)
         try:
             response = requests.put(
                 url=full_url,
+                params=params,
                 headers=self.headers,
                 cookies=cookies,
                 json=payload,
                 verify=self.verify,
             )
             if error_handling:
-                self._zia_http_codes(response)
+                _zia_http_codes(response)
             else:
                 if response.status_code not in [200, 201, 204]:
                     try:
                         raise ValueError(
                             f"HTTPS Response code {response.status_code} : {response.json()}"
                         )
                     except ValueError:
                         raise ValueError(response.status_code)
             return response
         except requests.HTTPError as e:
             raise ValueError(e)
 
     def delete_call(
-        self, url, payload=None, headers=None, cookies=None, error_handling=False
-    ):
+        self,
+        url: str,
+        payload: dict = None,
+        headers: dict = None,
+        cookies: dict = None,
+        error_handling: bool = False,
+    ) -> requests.Response:
         """
         Method to perform an HTTP DELETE call
-        :param url: url
-        :param payload: json payload
-        :param cookies: cookies
-        :param error_handling: Boolean, when TRUE will use Zscaler HTTP codes
-        :return: response
+
+        :param url: (str) url
+        :param payload: (dict) json payload
+        :param headers: (dict)
+        :param cookies: (str) cookies
+        :param error_handling: (bool) when TRUE will use Zscaler HTTP codes
+
+        :return: (requests.Response Object)
         """
         full_url = f"{self.host}{url}"
         if headers:
             self.headers.update(headers)
         try:
             response = requests.delete(
                 url=full_url,
                 headers=self.headers,
                 cookies=cookies,
                 json=payload,
                 verify=self.verify,
             )
             if error_handling:
-                self._zia_http_codes(response)
+                _zia_http_codes(response)
             else:
                 if response.status_code not in [200, 201, 204]:
                     raise ValueError(response.status_code)
             return response
         except requests.HTTPError as e:
             raise ValueError(e)
-
-    def _zia_http_codes(self, response):
-        """
-        Internal method to display HTTP error handling and response codes
-        For more information, please refer to https://help.zscaler.com/zia/about-error-handling
-        :param response:
-        :return: None
-        """
-        if response.status_code in [200, 201, 202, 204]:
-            return
-        elif response.status_code == 401:
-            raise ValueError(
-                f"{response.status_code} :Session is not authenticated or timed out"
-            )
-        elif response.status_code == 403:
-            raise ValueError(
-                f"{response.status_code} :API key disabled or SKU subscription missing or user role has not access"
-            )
-        elif response.status_code == 404:
-            raise ValueError("Resource does not exist")
-        elif response.status_code == 409:
-            raise ValueError(
-                "Request could not be processed because of possible edit conflict occurred"
-            )
-        elif response.status_code == 415:
-            raise ValueError("Unsupported media type")
-        elif response.status_code == 429:
-            raise ValueError("Exceeded the rate limit or quota")
-        elif response.status_code == 500:
-            raise ValueError("Unexpected error")
-        elif response.status_code == 503:
-            raise ValueError("Service is temporarily unavailable")
-        else:
-            print(response.content)
-            raise ValueError(f"Unexpected HTTP response code: {response.status_code}")
```

### Comparing `zscaler_api_talkers-4.1.0/zscaler_api_talkers/zscaler_helpers/logger.py` & `zscaler_api_talkers-4.1.1/zscaler_api_talkers/zscaler_helpers/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,48 +2,51 @@
 import os
 from logging.handlers import RotatingFileHandler
 
 
 def setup_logger(
     name: str,
     level: str = os.getenv("LOGGING_LEVEL", "info"),
-    log_filename: str = "output.log",
+    log_filename: str = None,
     max_log_size: int = 10 * 1024 * 1024,  # 10 MB
     backup_count: int = 3,
 ) -> logging.Logger:
     """
     To set up as many loggers as you want
 
     Args:
         name (str): Name of logger
         level (str): os.getenv("LOGGING_LEVEL"). Defaults to 'info'.
-        log_filename (str): Name and Path of log file.  Defaults to "output.log"
+        log_filename (str): Name and Path of log file.
         max_log_size (int): Defaults to 10MB
         backup_count (int): Default to 3
 
     Return:
         Logger Object
     """
-    handler_stream = logging.StreamHandler()
-    handler_file = RotatingFileHandler(
-        log_filename,
-        maxBytes=max_log_size,
-        backupCount=backup_count,
-    )
+    logger = logging.getLogger(name)
+
     formatter = logging.Formatter(
         fmt="{asctime} {name}.{funcName} {levelname} {message}",
         datefmt="%Y%m%d %H:%M:%S",
         style="{",
     )
-    handler_stream.setFormatter(formatter)
-    handler_file.setFormatter(formatter)
 
-    logger = logging.getLogger(name)
+    if log_filename:
+        handler_file = RotatingFileHandler(
+            log_filename,
+            maxBytes=max_log_size,
+            backupCount=backup_count,
+        )
+        handler_file.setFormatter(formatter)
+        logger.addHandler(handler_file)
+
+    handler_stream = logging.StreamHandler()
+    handler_stream.setFormatter(formatter)
     logger.addHandler(handler_stream)
-    logger.addHandler(handler_file)
 
     log_level = logging.INFO
     level = level.lower()
     if level == "notset":
         log_level = logging.NOTSET
     elif level == "debug":
         log_level = logging.DEBUG
```

### Comparing `zscaler_api_talkers-4.1.0/zscaler_api_talkers/zscaler_helpers/utilities.py` & `zscaler_api_talkers-4.1.1/zscaler_api_talkers/zscaler_helpers/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 logger = setup_logger(name=__name__)
 
 
 def get_user_agent() -> str:
     return "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/46.0.2490.86 Safari/537.36"
 
 
-def _request(
+def request_(
     method: str,
     url: str,
     retries: int = 10,
     wait_time: float = 5,
     silence_logs: bool = False,
     **kwargs,
 ) -> requests.Response:
@@ -80,15 +80,15 @@
             result = requests.request(
                 method=method.upper(),
                 url=url,
                 **{k: v for k, v in kwargs.items() if k in passable_options},
             )
             if result.status_code < 400:
                 break  # Only stop looping if the status_code is reported as not an error.
-        except requests.exceptions.SSLError as e:
+        except requests.exceptions.SSLError:
             if not silence_logs:
                 logger.debug("Disabling SSL verification for the next request attempt.")
             kwargs.update(
                 {
                     "verify": False,
                 }
             )
```

