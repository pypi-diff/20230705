# Comparing `tmp/django-appwrite-1.3.1.tar.gz` & `tmp/django-appwrite-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-appwrite-1.3.1.tar", last modified: Thu Mar 16 01:39:53 2023, max compression
+gzip compressed data, was "django-appwrite-1.4.0.tar", last modified: Wed Jul  5 00:21:14 2023, max compression
```

## Comparing `django-appwrite-1.3.1.tar` & `django-appwrite-1.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 01:39:53.733873 django-appwrite-1.3.1/
--rw-rw-rw-   0        0        0     1067 2023-02-08 00:02:52.000000 django-appwrite-1.3.1/LICENSE
--rw-rw-rw-   0        0        0     6205 2023-03-16 01:39:53.732921 django-appwrite-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     5069 2023-02-11 00:48:26.000000 django-appwrite-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-16 01:39:53.713833 django-appwrite-1.3.1/django_appwrite/
--rw-rw-rw-   0        0        0        0 2023-02-08 00:08:32.000000 django-appwrite-1.3.1/django_appwrite/__init__.py
--rw-rw-rw-   0        0        0     4056 2023-03-16 01:31:12.000000 django-appwrite-1.3.1/django_appwrite/middleware.py
-drwxrwxrwx   0        0        0        0 2023-03-16 01:39:53.731873 django-appwrite-1.3.1/django_appwrite/tests/
--rw-rw-rw-   0        0        0        0 2023-02-08 00:27:32.000000 django-appwrite-1.3.1/django_appwrite/tests/__init__.py
--rw-rw-rw-   0        0        0     1476 2023-02-09 23:54:28.000000 django-appwrite-1.3.1/django_appwrite/tests/test_middleware.py
-drwxrwxrwx   0        0        0        0 2023-03-16 01:39:53.730908 django-appwrite-1.3.1/django_appwrite.egg-info/
--rw-rw-rw-   0        0        0     6205 2023-03-16 01:39:53.000000 django-appwrite-1.3.1/django_appwrite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-03-16 01:39:53.000000 django-appwrite-1.3.1/django_appwrite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 01:39:53.000000 django-appwrite-1.3.1/django_appwrite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-03-16 01:39:53.000000 django-appwrite-1.3.1/django_appwrite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-03-16 01:39:53.000000 django-appwrite-1.3.1/django_appwrite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-16 01:39:53.733873 django-appwrite-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1587 2023-03-16 01:39:50.000000 django-appwrite-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 00:21:14.881458 django-appwrite-1.4.0/
+-rw-rw-rw-   0        0        0     1067 2023-02-08 00:02:52.000000 django-appwrite-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0     6095 2023-07-05 00:21:14.880460 django-appwrite-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4959 2023-07-04 22:24:13.000000 django-appwrite-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 00:21:14.857461 django-appwrite-1.4.0/django_appwrite/
+-rw-rw-rw-   0        0        0        0 2023-02-08 00:08:32.000000 django-appwrite-1.4.0/django_appwrite/__init__.py
+-rw-rw-rw-   0        0        0     4270 2023-07-04 22:20:06.000000 django-appwrite-1.4.0/django_appwrite/middleware.py
+drwxrwxrwx   0        0        0        0 2023-07-05 00:21:14.879506 django-appwrite-1.4.0/django_appwrite/tests/
+-rw-rw-rw-   0        0        0        0 2023-02-08 00:27:32.000000 django-appwrite-1.4.0/django_appwrite/tests/__init__.py
+-rw-rw-rw-   0        0        0     1476 2023-02-09 23:54:28.000000 django-appwrite-1.4.0/django_appwrite/tests/test_middleware.py
+drwxrwxrwx   0        0        0        0 2023-07-05 00:21:14.878459 django-appwrite-1.4.0/django_appwrite.egg-info/
+-rw-rw-rw-   0        0        0     6095 2023-07-05 00:21:14.000000 django-appwrite-1.4.0/django_appwrite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-07-05 00:21:14.000000 django-appwrite-1.4.0/django_appwrite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 00:21:14.000000 django-appwrite-1.4.0/django_appwrite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-05 00:21:14.000000 django-appwrite-1.4.0/django_appwrite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-05 00:21:14.000000 django-appwrite-1.4.0/django_appwrite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 00:21:14.881458 django-appwrite-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1587 2023-07-05 00:17:16.000000 django-appwrite-1.4.0/setup.py
```

### Comparing `django-appwrite-1.3.1/LICENSE` & `django-appwrite-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-appwrite-1.3.1/PKG-INFO` & `django-appwrite-1.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-appwrite
-Version: 1.3.1
+Version: 1.4.0
 Summary: Django Middleware to authenticate users with Appwrite
 Home-page: https://github.com/khashashin/django-appwrite
-Author: Yusup Khasbulatov
+Author: Yusuf Khasbulatov
 License: MIT
 Project-URL: Documentation, https://github.com/khashashin/django-appwrite/blob/main/README.md
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, https://patreon.com/khashashin
 Project-URL: Source, https://github.com/khashashin/django-appwrite
 Project-URL: Tracker, https://github.com/khashashin/django-appwrite/issues
 Keywords: appwrite auth django
@@ -71,48 +71,45 @@
 ```
 | Setting            | Default            | Description                                                                                                                                                                                                           |
 |--------------------|--------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `PROJECT_ENDPOINT` |                    | The endpoint of your Appwrite project. You can find this in the Appwrite console under Settings > General.                                                                                                            |
 | `PROJECT_ID`       |                    | The ID of your Appwrite project. You can find this in the Appwrite console under Settings > General.                                                                                                                  |
 | `PROJECT_API_KEY`  |                    | The API key of your Appwrite project. You can find this in the Appwrite console under Settings > API Keys.                                                                                                            |
 | `AUTH_HEADER`      | HTTP_AUTHORIZATION | The header name that will be used to get the JWT from the authorization header. The value of this header should be `Bearer [JWT]`                                                                                     |
-| `USER_ID_HEADER`   | HTTP_USER_ID       | The header name that will be used to store the user ID.                                                                                                                                                               |
 | `VERIFY_EMAIL`     | False              | If set to `True`, the middleware will check if the user's email address has been verified in Appwrite before authenticating the user. If the email address has not been verified, the user will not be authenticated. |
 | `VERIFY_PHONE`     | False              | If set to `True`, the middleware will check if the user's phone number has been verified in Appwrite before authenticating the user. If the phone number has not been verified, the user will not be authenticated.   |
+| `PREFIX_EMAIL`     |                    | The prefix to use for the email address when checking if the user's email address has been verified. This is useful if you are integrating django_appwrite to existing projects that already have users.              |
 
 ## How it works
-This middleware class will get the user ID from the header specified in the `USER_ID_HEADER` setting.
-It will then use this user ID to retrieve the user information from Appwrite using the `Users` service.
-If a user is found, it will create a Django user if it doesn't exist, and authenticate the user.
+This middleware class will authorize the user by checking the JWT in the `Authorization` header. The JWT is obtained from the `Authorization` header and is then sent to the Appwrite API to verify the JWT. If the JWT is valid, the user will be authenticated.
 
 Please note that this middleware is intended to be used in conjunction with the Appwrite client-side SDK to authorize users on the frontend, and does not provide any APIs for user authentication on its own.
 
 ## Example
 This is an example of how you can configure your frontend to use this middleware. Note that this example uses the [axios](https://axios-http.com/) library.
 
 ```javascript
-// axios interceptor to add the user ID to the request header
+// axios interceptor to add jwt to the request header
 import axios from 'axios';
 import { Client, Account } from 'appwrite';
 
 const client = new Client()
     .setEndpoint('https://example.com/v1')
     .setProject('PROJECT_ID')
     .setKey('PROJECT_API_KEY');
     
 const account = new Account(client);
 
 axios.interceptors.request.use(async (config) => {
-    // get the user_id and jwt from your auth service/provider
-    const { user_id, jwt } = await yourAuthService();
+    // get jwt from your auth service/provider
+    const { jwt } = await yourAuthService();
     
     config.headers = {
         ...config.headers,
-        Authorization: `Bearer ${jwt}`,
-        'User-ID': user_id,
+        Authorization: `Bearer ${jwt}`
     }
     
     return config;
 });
 ```
 
 ## License
```

### Comparing `django-appwrite-1.3.1/README.md` & `django-appwrite-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -45,48 +45,45 @@
 ```
 | Setting            | Default            | Description                                                                                                                                                                                                           |
 |--------------------|--------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `PROJECT_ENDPOINT` |                    | The endpoint of your Appwrite project. You can find this in the Appwrite console under Settings > General.                                                                                                            |
 | `PROJECT_ID`       |                    | The ID of your Appwrite project. You can find this in the Appwrite console under Settings > General.                                                                                                                  |
 | `PROJECT_API_KEY`  |                    | The API key of your Appwrite project. You can find this in the Appwrite console under Settings > API Keys.                                                                                                            |
 | `AUTH_HEADER`      | HTTP_AUTHORIZATION | The header name that will be used to get the JWT from the authorization header. The value of this header should be `Bearer [JWT]`                                                                                     |
-| `USER_ID_HEADER`   | HTTP_USER_ID       | The header name that will be used to store the user ID.                                                                                                                                                               |
 | `VERIFY_EMAIL`     | False              | If set to `True`, the middleware will check if the user's email address has been verified in Appwrite before authenticating the user. If the email address has not been verified, the user will not be authenticated. |
 | `VERIFY_PHONE`     | False              | If set to `True`, the middleware will check if the user's phone number has been verified in Appwrite before authenticating the user. If the phone number has not been verified, the user will not be authenticated.   |
+| `PREFIX_EMAIL`     |                    | The prefix to use for the email address when checking if the user's email address has been verified. This is useful if you are integrating django_appwrite to existing projects that already have users.              |
 
 ## How it works
-This middleware class will get the user ID from the header specified in the `USER_ID_HEADER` setting.
-It will then use this user ID to retrieve the user information from Appwrite using the `Users` service.
-If a user is found, it will create a Django user if it doesn't exist, and authenticate the user.
+This middleware class will authorize the user by checking the JWT in the `Authorization` header. The JWT is obtained from the `Authorization` header and is then sent to the Appwrite API to verify the JWT. If the JWT is valid, the user will be authenticated.
 
 Please note that this middleware is intended to be used in conjunction with the Appwrite client-side SDK to authorize users on the frontend, and does not provide any APIs for user authentication on its own.
 
 ## Example
 This is an example of how you can configure your frontend to use this middleware. Note that this example uses the [axios](https://axios-http.com/) library.
 
 ```javascript
-// axios interceptor to add the user ID to the request header
+// axios interceptor to add jwt to the request header
 import axios from 'axios';
 import { Client, Account } from 'appwrite';
 
 const client = new Client()
     .setEndpoint('https://example.com/v1')
     .setProject('PROJECT_ID')
     .setKey('PROJECT_API_KEY');
     
 const account = new Account(client);
 
 axios.interceptors.request.use(async (config) => {
-    // get the user_id and jwt from your auth service/provider
-    const { user_id, jwt } = await yourAuthService();
+    // get jwt from your auth service/provider
+    const { jwt } = await yourAuthService();
     
     config.headers = {
         ...config.headers,
-        Authorization: `Bearer ${jwt}`,
-        'User-ID': user_id,
+        Authorization: `Bearer ${jwt}`
     }
     
     return config;
 });
 ```
 
 ## License
```

### Comparing `django-appwrite-1.3.1/django_appwrite/middleware.py` & `django-appwrite-1.4.0/django_appwrite/middleware.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,85 +4,96 @@
 from appwrite.client import Client
 from appwrite.services.account import Account
 from django.utils.deprecation import MiddlewareMixin
 
 User = get_user_model()
 
 
+def log_error(e):
+    import logging
+    logger = logging.getLogger('django')
+    logger.error('Error: ', e)
+
+
 class AppwriteMiddleware(MiddlewareMixin):
     def __init__(self, get_response):
+        super().__init__(get_response)
         self.get_response = get_response
 
         # Try to retrieve the required Appwrite settings from the Django settings file
         try:
             project_endpoint = settings.APPWRITE.get('PROJECT_ENDPOINT')
             project_id = settings.APPWRITE.get('PROJECT_ID')
             project_key = settings.APPWRITE.get('PROJECT_API_KEY')
             self.auth_header = settings.APPWRITE.get('AUTH_HEADER', 'HTTP_AUTHORIZATION')
-            self.user_id_header = settings.APPWRITE.get('USER_ID_HEADER', 'HTTP_USER_ID')
             self.verify_email = settings.APPWRITE.get('VERIFY_EMAIL', False)
             self.verify_phone = settings.APPWRITE.get('VERIFY_PHONE', False)
+            self.prefix_email = settings.APPWRITE.get('PREFIX_EMAIL', '')
         except AttributeError:
             raise Exception("""
                 Make sure you have the following settings in your Django settings file:
                 APPWRITE = {
                     'PROJECT_ENDPOINT': 'https://example.com/v1',
                     'PROJECT_ID': 'PROJECT_ID',
                     'PROJECT_API_KEY': 'PROJECT_API_KEY',
-                    'USER_ID_HEADER': '[USER_ID]',
                 }
             """)
 
         # Initialize Appwrite client
-        self.client = (Client()
-                       .set_endpoint(project_endpoint)
-                       .set_project(project_id)
-                       .set_key(project_key))
+        try:
+            self.client = (Client()
+                           .set_endpoint(project_endpoint)
+                           .set_project(project_id)
+                           .set_key(project_key))
+        except Exception as e:
+            if settings.DEBUG:
+                log_error(e)
 
     def __call__(self, request, *args, **kwargs):
         try:
-            # Get the user ID from the header
-            user_id = request.META.get(self.user_id_header, '')
+            # Get the jwt from the header
             auth_header = request.META.get(self.auth_header, '')
             jwt = auth_header.replace('Bearer ', '')
         except Exception as e:
-            print('Error: ', e)
+            if settings.DEBUG:
+                log_error(e)
             return self.get_response(request)
 
         user_info = None
-        # If the user ID header is present
-        if user_id and jwt:
+        # If the jwt header is present
+        if jwt:
             try:
                 # Get the user information from Appwrite
                 self.client.set_jwt(jwt)
                 user_info = Account(self.client).get()
             except Exception as e:
-                print('Error: ', e)
+                if settings.DEBUG:
+                    log_error(e)
                 # Return the response without doing anything
                 return self.get_response(request)
 
         # If the user information was retrieved successfully
         if user_info:
 
             # If the user has not verified their email, return the response without doing anything
             if self.verify_email and not user_info['emailVerification']:
                 return self.get_response(request)
 
             # If the user has not verified their phone, return the response without doing anything
             if self.verify_phone and not user_info['phoneVerification']:
                 return self.get_response(request)
 
-            email = user_info['email']
-            password = settings.SECRET_KEY+user_id
+            email = self.prefix_email + user_info['email']
+            password = settings.SECRET_KEY + user_info['$id']
             # Get the Django user by its email
             user = User.objects.filter(username=email).first()
 
             # If the user doesn't exist, create it
             if not user:
-                user = User.objects.create_user(
+                User.objects.create_user(
                     username=email,
                     password=password,
                     email=email)
 
             # Authenticate the user using the email as the username
             user = authenticate(request, username=email, password=password)
```

### Comparing `django-appwrite-1.3.1/django_appwrite/tests/test_middleware.py` & `django-appwrite-1.4.0/django_appwrite/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-appwrite-1.3.1/django_appwrite.egg-info/PKG-INFO` & `django-appwrite-1.4.0/django_appwrite.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-appwrite
-Version: 1.3.1
+Version: 1.4.0
 Summary: Django Middleware to authenticate users with Appwrite
 Home-page: https://github.com/khashashin/django-appwrite
-Author: Yusup Khasbulatov
+Author: Yusuf Khasbulatov
 License: MIT
 Project-URL: Documentation, https://github.com/khashashin/django-appwrite/blob/main/README.md
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, https://patreon.com/khashashin
 Project-URL: Source, https://github.com/khashashin/django-appwrite
 Project-URL: Tracker, https://github.com/khashashin/django-appwrite/issues
 Keywords: appwrite auth django
@@ -71,48 +71,45 @@
 ```
 | Setting            | Default            | Description                                                                                                                                                                                                           |
 |--------------------|--------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `PROJECT_ENDPOINT` |                    | The endpoint of your Appwrite project. You can find this in the Appwrite console under Settings > General.                                                                                                            |
 | `PROJECT_ID`       |                    | The ID of your Appwrite project. You can find this in the Appwrite console under Settings > General.                                                                                                                  |
 | `PROJECT_API_KEY`  |                    | The API key of your Appwrite project. You can find this in the Appwrite console under Settings > API Keys.                                                                                                            |
 | `AUTH_HEADER`      | HTTP_AUTHORIZATION | The header name that will be used to get the JWT from the authorization header. The value of this header should be `Bearer [JWT]`                                                                                     |
-| `USER_ID_HEADER`   | HTTP_USER_ID       | The header name that will be used to store the user ID.                                                                                                                                                               |
 | `VERIFY_EMAIL`     | False              | If set to `True`, the middleware will check if the user's email address has been verified in Appwrite before authenticating the user. If the email address has not been verified, the user will not be authenticated. |
 | `VERIFY_PHONE`     | False              | If set to `True`, the middleware will check if the user's phone number has been verified in Appwrite before authenticating the user. If the phone number has not been verified, the user will not be authenticated.   |
+| `PREFIX_EMAIL`     |                    | The prefix to use for the email address when checking if the user's email address has been verified. This is useful if you are integrating django_appwrite to existing projects that already have users.              |
 
 ## How it works
-This middleware class will get the user ID from the header specified in the `USER_ID_HEADER` setting.
-It will then use this user ID to retrieve the user information from Appwrite using the `Users` service.
-If a user is found, it will create a Django user if it doesn't exist, and authenticate the user.
+This middleware class will authorize the user by checking the JWT in the `Authorization` header. The JWT is obtained from the `Authorization` header and is then sent to the Appwrite API to verify the JWT. If the JWT is valid, the user will be authenticated.
 
 Please note that this middleware is intended to be used in conjunction with the Appwrite client-side SDK to authorize users on the frontend, and does not provide any APIs for user authentication on its own.
 
 ## Example
 This is an example of how you can configure your frontend to use this middleware. Note that this example uses the [axios](https://axios-http.com/) library.
 
 ```javascript
-// axios interceptor to add the user ID to the request header
+// axios interceptor to add jwt to the request header
 import axios from 'axios';
 import { Client, Account } from 'appwrite';
 
 const client = new Client()
     .setEndpoint('https://example.com/v1')
     .setProject('PROJECT_ID')
     .setKey('PROJECT_API_KEY');
     
 const account = new Account(client);
 
 axios.interceptors.request.use(async (config) => {
-    // get the user_id and jwt from your auth service/provider
-    const { user_id, jwt } = await yourAuthService();
+    // get jwt from your auth service/provider
+    const { jwt } = await yourAuthService();
     
     config.headers = {
         ...config.headers,
-        Authorization: `Bearer ${jwt}`,
-        'User-ID': user_id,
+        Authorization: `Bearer ${jwt}`
     }
     
     return config;
 });
 ```
 
 ## License
```

### Comparing `django-appwrite-1.3.1/setup.py` & `django-appwrite-1.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='django-appwrite',
-    version='1.3.1',
+    version='1.4.0',
     description='Django Middleware to authenticate users with Appwrite',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(exclude=("tests",)),
     package_dir={'django_appwrite': 'django_appwrite'},
     install_requires=['appwrite', 'django'],
     license='MIT',
-    author='Yusup Khasbulatov',
+    author='Yusuf Khasbulatov',
     readme='README.md',
     keywords="appwrite auth django",
     url='https://github.com/khashashin/django-appwrite',
     project_urls={
         'Documentation': 'https://github.com/khashashin/django-appwrite/blob/main/README.md',
         'Funding': 'https://donate.pypi.org',
         'Say Thanks!': 'https://patreon.com/khashashin',
```

