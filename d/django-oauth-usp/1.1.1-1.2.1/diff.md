# Comparing `tmp/django_oauth_usp-1.1.1.tar.gz` & `tmp/django_oauth_usp-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_oauth_usp-1.1.1.tar", max compression
+gzip compressed data, was "django_oauth_usp-1.2.1.tar", max compression
```

## Comparing `django_oauth_usp-1.1.1.tar` & `django_oauth_usp-1.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1068 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/LICENSE
--rw-r--r--   0        0        0     1761 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/__init__.py
--rw-r--r--   0        0        0      402 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/admin.py
--rw-r--r--   0        0        0      108 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/apps.py
--rw-r--r--   0        0        0     3123 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/managers.py
--rw-r--r--   0        0        0      555 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/middleware.py
--rw-r--r--   0        0        0     2557 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/migrations/__init__.py
--rw-r--r--   0        0        0     2289 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/models.py
--rw-r--r--   0        0        0     1395 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/oauth.py
--rw-r--r--   0        0        0      180 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/templates/main.html
--rw-r--r--   0        0        0      624 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/templates/user.html
--rw-r--r--   0        0        0        0 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/tests/__init__.py
--rw-r--r--   0        0        0     1076 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/tests/faker.py
--rw-r--r--   0        0        0     1985 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/tests/mock.py
--rw-r--r--   0        0        0      346 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/tests/test_accounts_admin.py
--rw-r--r--   0        0        0      324 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/tests/test_accounts_manager.py
--rw-r--r--   0        0        0     2964 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/tests/test_accounts_models.py
--rw-r--r--   0        0        0     1224 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/tests/test_accounts_transform.py
--rw-r--r--   0        0        0     4494 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/tests/test_accounts_views.py
--rw-r--r--   0        0        0     1213 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/tests/test_oauth.py
--rw-r--r--   0        0        0      912 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/tests/test_user_middleware.py
--rw-r--r--   0        0        0      764 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/transform.py
--rw-r--r--   0        0        0      361 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/urls.py
--rw-r--r--   0        0        0     2720 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/accounts/views.py
--rw-r--r--   0        0        0     2316 2023-06-28 10:48:52.546683 django_oauth_usp-1.1.1/django_oauth_usp/settings.py
--rw-r--r--   0        0        0      115 2023-06-28 10:48:52.550016 django_oauth_usp-1.1.1/django_oauth_usp/urls.py
--rw-r--r--   0        0        0      536 2023-06-28 11:17:22.154848 django_oauth_usp-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2312 1970-01-01 00:00:00.000000 django_oauth_usp-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-03 19:42:21.440019 django_oauth_usp-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1780 2023-07-03 19:42:21.440019 django_oauth_usp-1.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/__init__.py
+-rw-r--r--   0        0        0      402 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/admin.py
+-rw-r--r--   0        0        0      108 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/apps.py
+-rw-r--r--   0        0        0     3122 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/managers.py
+-rw-r--r--   0        0        0      555 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/middleware.py
+-rw-r--r--   0        0        0     2557 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/migrations/__init__.py
+-rw-r--r--   0        0        0     2288 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/models.py
+-rw-r--r--   0        0        0     1395 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/oauth.py
+-rw-r--r--   0        0        0      180 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/templates/main.html
+-rw-r--r--   0        0        0      624 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/templates/user.html
+-rw-r--r--   0        0        0        0 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/__init__.py
+-rw-r--r--   0        0        0     1076 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/faker.py
+-rw-r--r--   0        0        0     1985 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/mock.py
+-rw-r--r--   0        0        0      346 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_accounts_admin.py
+-rw-r--r--   0        0        0      324 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_accounts_manager.py
+-rw-r--r--   0        0        0     2964 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_accounts_models.py
+-rw-r--r--   0        0        0     1224 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_accounts_transform.py
+-rw-r--r--   0        0        0     4535 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_accounts_views.py
+-rw-r--r--   0        0        0     1440 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_oauth.py
+-rw-r--r--   0        0        0      912 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_user_middleware.py
+-rw-r--r--   0        0        0      764 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/transform.py
+-rw-r--r--   0        0        0      361 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/urls.py
+-rw-r--r--   0        0        0     2720 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/views.py
+-rw-r--r--   0        0        0     2316 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/settings.py
+-rw-r--r--   0        0        0      115 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/urls.py
+-rw-r--r--   0        0        0      965 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 django_oauth_usp-1.2.1/PKG-INFO
```

### Comparing `django_oauth_usp-1.1.1/LICENSE` & `django_oauth_usp-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.1.1/README.md` & `django_oauth_usp-1.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,54 +3,54 @@
 ================
 
 Este pacote permite que usuários façam login utilizando a senha única USP.
 
 Além da autenticação OAuth este pacote também possui migrations para o armazenamento dos
 usuários no banco de dados.
 
-É recomendado que a estas migrations sejam rodaddas antes de qualquer outra migration, devido
+É recomendado que a estas migrations sejam rodadas antes de qualquer outra migration, devido
 a dificuldade de alteração do model User depois de realizada a primeira migration:
 `Using a custom user model when starting a project`__
 
 __ https://docs.djangoproject.com/en/3.1/topics/auth/customizing/#using-a-custom-user-model-when-starting-a-project
 
 Quick start
 -----------
 
 1. Adicione "django_oauth_usp" em INSTALLED_APPS no arquivo settings.py::
 
     INSTALLED_APPS = [
         ...
-        'polls',
+        'django_oauth_usp.accounts',
     ]
 
 2. Adicone o Middleware OAuthUspMiddleware::
 
     MIDDLEWARE = [
         ...
         'django_oauth_usp.accounts.middleware.OAuthUspMiddleware',
     ]
 
 3. No arquivo settings.py, informe o Model que será utilizado para armazenar os usuários::
 
-        AUTH_USER_MODEL= 'django_oauth_usp.UserModel'
+        AUTH_USER_MODEL= 'accounts.UserModel'
 
 4. Defina os parâmetro para OAuth::
 
-    OAUTH_CALLBACK_ID = callback_id_da_aplicação
+    OAUTH_CALLBACK_ID = 'callback_id_da_aplicação'
 
     AUTHLIB_OAUTH_CLIENTS = {
         'usp': {
-            'client_id': meu_client_id,
-            'client_secret': meu_secret_key
+            'client_id': 'meu_client_id',
+            'client_secret': 'meu_secret_key'
         }
     }
 
     #Rota utilizada para a view accounts_authorize
-    REDIRECT_URI = /auth/authorize
+    REDIRECT_URI = '/auth/authorize'
 
     #Lista com o código das unidades que poderão ter acesso.
     ALLOWED_UNIDADES = [12, 13, 14]
 5. Rode as migrations::
 
     python manage.py migrate
```

### Comparing `django_oauth_usp-1.1.1/django_oauth_usp/accounts/managers.py` & `django_oauth_usp-1.2.1/django_oauth_usp/accounts/managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.contrib.auth.models import BaseUserManager
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from django.utils import timezone
 
 
 class UserManager(BaseUserManager):
     def _create_user(self, login, name, user_type, main_email, password,
                      is_staff, is_superuser, **extra_fields):
```

### Comparing `django_oauth_usp-1.1.1/django_oauth_usp/accounts/middleware.py` & `django_oauth_usp-1.2.1/django_oauth_usp/accounts/middleware.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.1.1/django_oauth_usp/accounts/migrations/0001_initial.py` & `django_oauth_usp-1.2.1/django_oauth_usp/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.1.1/django_oauth_usp/accounts/models.py` & `django_oauth_usp-1.2.1/django_oauth_usp/accounts/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from django.db import models
 from django.contrib.auth.models import AbstractBaseUser, PermissionsMixin
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from django.core.mail import send_mail
 from django.conf import settings
 
 from .managers import UserManager
 
 
 class UserModel(AbstractBaseUser, PermissionsMixin):
```

### Comparing `django_oauth_usp-1.1.1/django_oauth_usp/accounts/oauth.py` & `django_oauth_usp-1.2.1/django_oauth_usp/accounts/oauth.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.1.1/django_oauth_usp/accounts/templates/user.html` & `django_oauth_usp-1.2.1/django_oauth_usp/accounts/templates/user.html`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.1.1/django_oauth_usp/accounts/tests/faker.py` & `django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/faker.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.1.1/django_oauth_usp/accounts/tests/mock.py` & `django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/mock.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.1.1/django_oauth_usp/accounts/tests/test_accounts_models.py` & `django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_accounts_models.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.1.1/django_oauth_usp/accounts/tests/test_accounts_transform.py` & `django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_accounts_transform.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.1.1/django_oauth_usp/accounts/tests/test_accounts_views.py` & `django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_accounts_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,25 +36,26 @@
 
 
 class AuthorizeViewTest(TestCase):
     @mock_oauth
     def setUp(self):
         self.request = HttpRequest()
         query = QueryDict(
-            'oauth_token=12345oauth & oauth_verifier=12345veriifer')
+            'oauth_token=12345oauth&oauth_verifier=12345veriifer')
 
         self.request.GET = query
 
         session = SessionStore()
         setattr(self.request, 'session', session)
 
         request_token = dict(
             oauth_token='token123', oauth_token_secret='oauth_token_secret123',
             oauth_verifier='verifier123')
-        self.request.session['_usp_authlib_request_token_'] = request_token
+        data = {"data": {"request_token": request_token}}
+        self.request.session['_state_usp_12345oauth'] = data
 
         user = UserModel.objects.create_user(**user_data)
         setattr(user, 'wsuserid', 'oiuasd098')
         setattr(self.request, 'user', user)
 
         self.obj = OAuthAuthorize()
```

### Comparing `django_oauth_usp-1.1.1/django_oauth_usp/accounts/tests/test_user_middleware.py` & `django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_user_middleware.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.1.1/django_oauth_usp/accounts/transform.py` & `django_oauth_usp-1.2.1/django_oauth_usp/accounts/transform.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.1.1/django_oauth_usp/accounts/views.py` & `django_oauth_usp-1.2.1/django_oauth_usp/accounts/views.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.1.1/django_oauth_usp/settings.py` & `django_oauth_usp-1.2.1/django_oauth_usp/settings.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.1.1/PKG-INFO` & `django_oauth_usp-1.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,80 @@
 Metadata-Version: 2.1
 Name: django-oauth-usp
-Version: 1.1.1
-Summary: Autenticação com a senha única utilizando oauth
+Version: 1.2.1
+Summary: 
 License: MIT
 Author: Marcelo Schneider
 Author-email: schenider.fei@gmail.com
 Requires-Python: >=3.10,<4.0
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Authlib (>=1.2.1,<2.0.0)
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Requires-Dist: authlib (>=1.2.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 ================
 Django OAuth USP
 ================
 
 Este pacote permite que usuários façam login utilizando a senha única USP.
 
 Além da autenticação OAuth este pacote também possui migrations para o armazenamento dos
 usuários no banco de dados.
 
-É recomendado que a estas migrations sejam rodaddas antes de qualquer outra migration, devido
+É recomendado que a estas migrations sejam rodadas antes de qualquer outra migration, devido
 a dificuldade de alteração do model User depois de realizada a primeira migration:
 `Using a custom user model when starting a project`__
 
 __ https://docs.djangoproject.com/en/3.1/topics/auth/customizing/#using-a-custom-user-model-when-starting-a-project
 
 Quick start
 -----------
 
 1. Adicione "django_oauth_usp" em INSTALLED_APPS no arquivo settings.py::
 
     INSTALLED_APPS = [
         ...
-        'polls',
+        'django_oauth_usp.accounts',
     ]
 
 2. Adicone o Middleware OAuthUspMiddleware::
 
     MIDDLEWARE = [
         ...
         'django_oauth_usp.accounts.middleware.OAuthUspMiddleware',
     ]
 
 3. No arquivo settings.py, informe o Model que será utilizado para armazenar os usuários::
 
-        AUTH_USER_MODEL= 'django_oauth_usp.UserModel'
+        AUTH_USER_MODEL= 'accounts.UserModel'
 
 4. Defina os parâmetro para OAuth::
 
-    OAUTH_CALLBACK_ID = callback_id_da_aplicação
+    OAUTH_CALLBACK_ID = 'callback_id_da_aplicação'
 
     AUTHLIB_OAUTH_CLIENTS = {
         'usp': {
-            'client_id': meu_client_id,
-            'client_secret': meu_secret_key
+            'client_id': 'meu_client_id',
+            'client_secret': 'meu_secret_key'
         }
     }
 
     #Rota utilizada para a view accounts_authorize
-    REDIRECT_URI = /auth/authorize
+    REDIRECT_URI = '/auth/authorize'
 
     #Lista com o código das unidades que poderão ter acesso.
     ALLOWED_UNIDADES = [12, 13, 14]
 5. Rode as migrations::
 
     python manage.py migrate
```

