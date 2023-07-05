# Comparing `tmp/cloudpy_org-1.4.2.tar.gz` & `tmp/cloudpy_org-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpy_org-1.4.2.tar", last modified: Mon Jul  3 01:22:22 2023, max compression
+gzip compressed data, was "dist\cloudpy_org-1.4.3.tar", last modified: Wed Jul  5 08:45:56 2023, max compression
```

## Comparing `cloudpy_org-1.4.2.tar` & `cloudpy_org-1.4.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 01:22:22.196291 cloudpy_org-1.4.2/
--rw-rw-rw-   0        0        0      935 2023-07-03 01:22:22.196291 cloudpy_org-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 01:22:22.071293 cloudpy_org-1.4.2/cloudpy_org/
--rw-rw-rw-   0        0        0      130 2023-07-03 01:20:12.000000 cloudpy_org-1.4.2/cloudpy_org/__init__.py
--rw-rw-rw-   0        0        0    79159 2023-07-03 01:16:18.000000 cloudpy_org-1.4.2/cloudpy_org/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-03 01:22:22.180669 cloudpy_org-1.4.2/cloudpy_org.egg-info/
--rw-rw-rw-   0        0        0      935 2023-07-03 01:22:21.000000 cloudpy_org-1.4.2/cloudpy_org.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-03 01:22:21.000000 cloudpy_org-1.4.2/cloudpy_org.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 01:22:21.000000 cloudpy_org-1.4.2/cloudpy_org.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-07-03 01:22:21.000000 cloudpy_org-1.4.2/cloudpy_org.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-03 01:22:21.000000 cloudpy_org-1.4.2/cloudpy_org.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 01:22:22.196291 cloudpy_org-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1324 2023-07-03 01:16:43.000000 cloudpy_org-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:45:56.871904 cloudpy_org-1.4.3/
+-rw-rw-rw-   0        0        0      935 2023-07-05 08:45:56.871904 cloudpy_org-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 08:45:56.762528 cloudpy_org-1.4.3/cloudpy_org/
+-rw-rw-rw-   0        0        0      130 2023-07-03 01:20:12.000000 cloudpy_org-1.4.3/cloudpy_org/__init__.py
+-rw-rw-rw-   0        0        0    79895 2023-07-05 08:41:45.000000 cloudpy_org-1.4.3/cloudpy_org/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:45:56.840653 cloudpy_org-1.4.3/cloudpy_org.egg-info/
+-rw-rw-rw-   0        0        0      935 2023-07-05 08:45:56.000000 cloudpy_org-1.4.3/cloudpy_org.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-05 08:45:56.000000 cloudpy_org-1.4.3/cloudpy_org.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 08:45:56.000000 cloudpy_org-1.4.3/cloudpy_org.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-07-05 08:45:56.000000 cloudpy_org-1.4.3/cloudpy_org.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-05 08:45:56.000000 cloudpy_org-1.4.3/cloudpy_org.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 08:45:56.871904 cloudpy_org-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1324 2023-07-03 01:54:22.000000 cloudpy_org-1.4.3/setup.py
```

### Comparing `cloudpy_org-1.4.2/PKG-INFO` & `cloudpy_org-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy_org
-Version: 1.4.2
+Version: 1.4.3
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.4.2/cloudpy_org/tools.py` & `cloudpy_org-1.4.3/cloudpy_org/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Find documentation at https://www.cloudpy.org
 """
-cloudpy_org_version='1.4.2'
+cloudpy_org_version='1.4.3'
 import os
 import json
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
 warnings.filterwarnings('ignore')
 warnings.simplefilter('ignore')
 import pandas as pd
@@ -1210,17 +1210,17 @@
 xpt.environment = "s3"
 class aws_framework_manager:
     def __init__(self,secret_key:str,aws_auth_token:str=""):
         self.__deconstructor_token = 'JQxrs8sWqn3JIWlIL8nTlw-302SfmV7RmlZ-T-gB5c4=oiwn8TU5-NcDKzVq'
         uuu = "1V44bjdzKODcN50jdz00c4="
         self.__sc = secret_key[::-1].split(uuu)
         self.__at = aws_auth_token[::-1].split(uuu)
-        self.__cppt_construction(self.__sc[1])
+        self.cppt_construction(self.__sc[1])
         self.cppt.environment = "s3"
-        self.__ypt_construction(self.__at[1])
+        self.ypt_construction(self.__at[1])
         self.ypt.environment = "s3"
         self.general_info = {}
         self.service_name = "cloudpy-org-service-beta"
         self.delimiters = ["pZo-9xH9oEO2B2OEo","2nZzN01wtktk10N","VhMxT-9xVVZzN01w","_Shv-4F86Co981h"]
         self.general_separators = {'user_email_sep': '-0-', '@': '-1-', '.': '-2-'}
         self.special_separators = self.general_separators
         self.__service_initialized = False
@@ -1237,21 +1237,21 @@
             if i == r-1:
                 b += c[::-1][0:n]
                 c = c.replace(c[::-1][0:n][::-1],'')
         if upper:
             c = c.upper()
         return c,b
     #___________________________________________________________________
-    def __cppt_construction(self,secret_key:str=""):
+    def cppt_construction(self,secret_key:str=""):
         if len(secret_key) > 10:
             k = self.__deconstructor_token
             self.cppt = processing_tools(data=xpt.basic_dicstr_to_dict(xpt.decrypt(secret_key,self.__do(k,10,False)[1] + self.__do(k,10,False)[0][0:4])))
         else:
             self.cppt = processing_tools()
-    def __ypt_construction(self,aws_auth_token:str=""):
+    def ypt_construction(self,aws_auth_token:str=""):
         if len(aws_auth_token) > 10:
             k = self.__deconstructor_token
             self.ypt = processing_tools(data=xpt.basic_dicstr_to_dict(xpt.decrypt(aws_auth_token,self.__do(k,10,False)[1] + self.__do(k,10,False)[0][0:4])))
         else:
             self.ypt = processing_tools()
     #___________________________________________________________________
     def initialize_service(self,service_token:str,version:str=cloudpy_org_version,test_file_name:str=None):
@@ -1321,14 +1321,16 @@
     def _decorator(decorator_param):
         def inner_func(self,dk):
             k = dk + "_is_function"
             dc = "self.dx['@k'] = self.dynamic_exec(dynamic_key='@dynamic_key'@these_args)"
             dc = dc.replace("@dynamic_key",dk)\
             .replace("@k",k)\
             .replace("@these_args",self.__args_applied[dk])
+            #print("dcx:")
+            #print(dc)
             exec(dc)
             is_function = self.dx[k]
             self.dx.pop(k, None)
             rslt = None
             if dk in set(self.dx.keys()):
                 if is_function:
                     rslt = self.dx[dk]
@@ -1586,31 +1588,55 @@
                 ,'keystr_with_expiration': dat['keystr_with_expiration']
                 ,'date_id': date_id
                 ,'timestr': self.cppt.seconds_to_timestr(time_id)
                 ,'service_token': service_token}
         del dat
         return str(rslt)
 
-def aws_framework_manager_client(username_or_email:str="",pwd:str="",aws_auth_token:str="",local:bool=False):
+def aws_framework_manager_client(username_or_email:str="",pwd:str="",aws_auth_token:str="",local:bool=False,print_results:bool=False):
     url_base = "https://www.cloudpy.org/"
     if local:
         url_base = "http://localhost/"
-    url = url_base + "gen_authentication_token"
-    token = requests.post(url_base + "gen_authentication_token",json = {"username_or_email":username_or_email,"pwd":pwd} ,verify=False).text
-    if "wrong" in token.lower() or "invalid" in token.lower():
+    url_1 = url_base + "gen_authentication_token"
+    url_2 = url_base + "authenticate_with_token"
+    url_3 = url_base + "gen_service_token"
+    try:
+        token = requests.post(url_1,json = {"username_or_email":username_or_email,"pwd":pwd} ,verify=False).text
+    except:
+        token = "invalid"
+        print("Unable to generate token.")
+    if "wrong" in token.lower() or "invalid" in token.lower() or "500 Internal Server Error" in token:
         fm = None
-        print(token)
+        print("Unable to generate token.")
     else:
-        #print("token: ",token)
-        secret_key = requests.post(url_base + "authenticate_with_token",json={"token":token},verify=False).text
-        #print("secret_key: ",secret_key)
-        service_token= requests.post(url_base + "gen_service_token",json={"secret_key":secret_key},verify=False).text
-        #print("service_token: ",service_token)
-        fm = aws_framework_manager(secret_key=secret_key,aws_auth_token=aws_auth_token)
-        print(fm.initialize_service(service_token=service_token))
+        if print_results:
+            print("token: ",token)
+        try:
+            secret_key = requests.post(url_2,json={"token":token},verify=False).text
+            if print_results:
+                print("secret_key: ",secret_key)
+        except:
+            secret_key = ""
+            print("Unable to generate secret key.")
+        try:
+            service_token= requests.post(url_3,json={"token":token},verify=False).text
+            if print_results:
+                print("service_token: ",service_token)
+        except:
+            service_token = ""
+            print("Unable to generate service token.")
+        try:
+            fm = aws_framework_manager(secret_key=secret_key,aws_auth_token=aws_auth_token)
+            try:
+                message = fm.initialize_service(service_token=service_token)
+            except:
+                message = "Could not initialize service."
+            print(message)
+        except:
+            ...
     return fm
 
 def gen_aws_auth_token(user_key:str,secret:str,local:bool=False,minutes_to_expire:float=5):
     ks = "1V44bjdzKODcN50jdz00c4="
     url_base = "https://www.cloudpy.org/"
     if local:
         url_base = "http://localhost/"
```

### Comparing `cloudpy_org-1.4.2/cloudpy_org.egg-info/PKG-INFO` & `cloudpy_org-1.4.3/cloudpy_org.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy-org
-Version: 1.4.2
+Version: 1.4.3
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.4.2/setup.py` & `cloudpy_org-1.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from os import path
 
 
 long_description = 'A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.'
 
 setup(
     name="cloudpy_org",
-    version="1.4.2",
+    version="1.4.3",
     description="Cloud data pipeline organization and automation library. Includes AWS framework manager API.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://www.cloudpy.org/",
     author="cloudpy.org",
     author_email="admin@cloudpy.org",
     license="MIT",
```

