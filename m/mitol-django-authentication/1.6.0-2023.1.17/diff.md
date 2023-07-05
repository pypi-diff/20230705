# Comparing `tmp/mitol-django-authentication-1.6.0.tar.gz` & `tmp/mitol-django-authentication-2023.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitol-django-authentication-1.6.0.tar", last modified: Tue Jan 17 16:18:02 2023, max compression
+gzip compressed data, was "mitol-django-authentication-2023.1.17.tar", last modified: Wed Jul  5 16:16:57 2023, max compression
```

## Comparing `mitol-django-authentication-1.6.0.tar` & `mitol-django-authentication-2023.1.17.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:18:02.559208 mitol-django-authentication-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-01-17 16:18:01.000000 mitol-django-authentication-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      927 2023-01-17 16:18:02.559208 mitol-django-authentication-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-01-17 16:18:01.000000 mitol-django-authentication-1.6.0/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:18:02.559208 mitol-django-authentication-1.6.0/mitol/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-01-17 16:18:01.000000 mitol-django-authentication-1.6.0/mitol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:18:02.559208 mitol-django-authentication-1.6.0/mitol/authentication/
--rw-r--r--   0 runner    (1001) docker     (122)     3632 2023-01-17 16:18:01.000000 mitol-django-authentication-1.6.0/mitol/authentication/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      415 2023-01-17 16:18:01.000000 mitol-django-authentication-1.6.0/mitol/authentication/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-01-17 16:18:01.000000 mitol-django-authentication-1.6.0/mitol/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-01-17 16:18:01.000000 mitol-django-authentication-1.6.0/mitol/authentication/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:18:02.559208 mitol-django-authentication-1.6.0/mitol/authentication/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:18:01.000000 mitol-django-authentication-1.6.0/mitol/authentication/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:18:01.000000 mitol-django-authentication-1.6.0/mitol/authentication/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:18:02.559208 mitol-django-authentication-1.6.0/mitol/authentication/serializers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:18:01.000000 mitol-django-authentication-1.6.0/mitol/authentication/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1097 2023-01-17 16:18:01.000000 mitol-django-authentication-1.6.0/mitol/authentication/serializers/djoser_serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:18:02.559208 mitol-django-authentication-1.6.0/mitol/authentication/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:18:01.000000 mitol-django-authentication-1.6.0/mitol/authentication/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1244 2023-01-17 16:18:01.000000 mitol-django-authentication-1.6.0/mitol/authentication/settings/djoser_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     3268 2023-01-17 16:18:01.000000 mitol-django-authentication-1.6.0/mitol/authentication/settings/touchstone.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:18:02.559208 mitol-django-authentication-1.6.0/mitol/authentication/urls/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:18:01.000000 mitol-django-authentication-1.6.0/mitol/authentication/urls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      636 2023-01-17 16:18:01.000000 mitol-django-authentication-1.6.0/mitol/authentication/urls/djoser_urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-01-17 16:18:01.000000 mitol-django-authentication-1.6.0/mitol/authentication/urls/saml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:18:02.559208 mitol-django-authentication-1.6.0/mitol/authentication/views/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:18:01.000000 mitol-django-authentication-1.6.0/mitol/authentication/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2516 2023-01-17 16:18:01.000000 mitol-django-authentication-1.6.0/mitol/authentication/views/djoser_views.py
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-01-17 16:18:01.000000 mitol-django-authentication-1.6.0/mitol/authentication/views/saml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:18:02.559208 mitol-django-authentication-1.6.0/mitol_django_authentication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      927 2023-01-17 16:18:02.000000 mitol-django-authentication-1.6.0/mitol_django_authentication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-01-17 16:18:02.000000 mitol-django-authentication-1.6.0/mitol_django_authentication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 16:18:02.000000 mitol-django-authentication-1.6.0/mitol_django_authentication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-17 16:18:02.000000 mitol-django-authentication-1.6.0/mitol_django_authentication.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-01-17 16:18:02.000000 mitol-django-authentication-1.6.0/mitol_django_authentication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-17 16:18:02.000000 mitol-django-authentication-1.6.0/mitol_django_authentication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 16:18:02.000000 mitol-django-authentication-1.6.0/mitol_django_authentication.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-17 16:18:02.559208 mitol-django-authentication-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-01-17 16:18:01.000000 mitol-django-authentication-1.6.0/setup.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:57.676660 mitol-django-authentication-2023.1.17/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       12 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/MANIFEST.in
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      931 2023-07-05 16:16:57.676660 mitol-django-authentication-2023.1.17/PKG-INFO
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      748 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/backend_shim.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:57.673326 mitol-django-authentication-2023.1.17/mitol/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       56 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol/__init__.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:57.673326 mitol-django-authentication-2023.1.17/mitol/authentication/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1492 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol/authentication/CHANGELOG.md
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      415 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol/authentication/README.md
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      108 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol/authentication/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      716 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol/authentication/apps.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:57.673326 mitol-django-authentication-2023.1.17/mitol/authentication/migrations/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol/authentication/migrations/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol/authentication/py.typed
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:57.673326 mitol-django-authentication-2023.1.17/mitol/authentication/serializers/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol/authentication/serializers/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1097 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol/authentication/serializers/djoser_serializers.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:57.676660 mitol-django-authentication-2023.1.17/mitol/authentication/settings/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol/authentication/settings/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1244 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol/authentication/settings/djoser_settings.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     3268 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol/authentication/settings/touchstone.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:57.676660 mitol-django-authentication-2023.1.17/mitol/authentication/urls/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol/authentication/urls/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      636 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol/authentication/urls/djoser_urls.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      217 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol/authentication/urls/saml.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:57.676660 mitol-django-authentication-2023.1.17/mitol/authentication/views/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol/authentication/views/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     2516 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol/authentication/views/djoser_views.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      558 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol/authentication/views/saml.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:57.676660 mitol-django-authentication-2023.1.17/mitol_django_authentication.egg-info/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      931 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol_django_authentication.egg-info/PKG-INFO
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1080 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol_django_authentication.egg-info/SOURCES.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol_django_authentication.egg-info/dependency_links.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        6 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol_django_authentication.egg-info/namespace_packages.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      149 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol_django_authentication.egg-info/requires.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        6 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol_django_authentication.egg-info/top_level.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/mitol_django_authentication.egg-info/zip-safe
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       38 2023-07-05 16:16:57.676660 mitol-django-authentication-2023.1.17/setup.cfg
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     2029 2023-07-05 16:16:57.000000 mitol-django-authentication-2023.1.17/setup.py
```

### Comparing `mitol-django-authentication-1.6.0/PKG-INFO` & `mitol-django-authentication-2023.1.17/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mitol-django-authentication
-Version: 1.6.0
+Version: 2023.1.17
 Summary: MIT Open Learning django app extensions for oauth toolkit
 License: BSD 3-Clause License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 mitol-django-authentication
 ---
 
 This is the Open Learning Django Authentication app. It provides a few key features around authentication:
```

### Comparing `mitol-django-authentication-1.6.0/backend_shim.py` & `mitol-django-authentication-2023.1.17/backend_shim.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 build_wheel = True
 build_sdist = True
 wheel_config_settings = {
 }
 sdist_config_settings = {
 }
 
-os.makedirs(dist_dir, exist_ok=True)
+# Python 2.7 doesn't have the exist_ok arg on os.makedirs().
+try:
+    os.makedirs(dist_dir)
+except OSError as e:
+    if e.errno != errno.EEXIST:
+        raise
+
 wheel_path = backend.build_wheel(dist_dir, wheel_config_settings) if build_wheel else None
 sdist_path = backend.build_sdist(dist_dir, sdist_config_settings) if build_sdist else None
 
 if wheel_path:
     print("wheel: {wheel_path}".format(wheel_path=wheel_path))
 if sdist_path:
     print("sdist: {sdist_path}".format(sdist_path=sdist_path))
```

### Comparing `mitol-django-authentication-1.6.0/mitol/authentication/apps.py` & `mitol-django-authentication-2023.1.17/mitol/authentication/apps.py`

 * *Files identical despite different names*

### Comparing `mitol-django-authentication-1.6.0/mitol/authentication/serializers/djoser_serializers.py` & `mitol-django-authentication-2023.1.17/mitol/authentication/serializers/djoser_serializers.py`

 * *Files identical despite different names*

### Comparing `mitol-django-authentication-1.6.0/mitol/authentication/settings/djoser_settings.py` & `mitol-django-authentication-2023.1.17/mitol/authentication/settings/djoser_settings.py`

 * *Files identical despite different names*

### Comparing `mitol-django-authentication-1.6.0/mitol/authentication/settings/touchstone.py` & `mitol-django-authentication-2023.1.17/mitol/authentication/settings/touchstone.py`

 * *Files identical despite different names*

### Comparing `mitol-django-authentication-1.6.0/mitol/authentication/urls/djoser_urls.py` & `mitol-django-authentication-2023.1.17/mitol/authentication/urls/djoser_urls.py`

 * *Files identical despite different names*

### Comparing `mitol-django-authentication-1.6.0/mitol/authentication/views/djoser_views.py` & `mitol-django-authentication-2023.1.17/mitol/authentication/views/djoser_views.py`

 * *Files identical despite different names*

### Comparing `mitol-django-authentication-1.6.0/mitol/authentication/views/saml.py` & `mitol-django-authentication-2023.1.17/mitol/authentication/views/saml.py`

 * *Files identical despite different names*

### Comparing `mitol-django-authentication-1.6.0/mitol_django_authentication.egg-info/PKG-INFO` & `mitol-django-authentication-2023.1.17/mitol_django_authentication.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mitol-django-authentication
-Version: 1.6.0
+Version: 2023.1.17
 Summary: MIT Open Learning django app extensions for oauth toolkit
 License: BSD 3-Clause License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 mitol-django-authentication
 ---
 
 This is the Open Learning Django Authentication app. It provides a few key features around authentication:
```

### Comparing `mitol-django-authentication-1.6.0/mitol_django_authentication.egg-info/SOURCES.txt` & `mitol-django-authentication-2023.1.17/mitol_django_authentication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitol-django-authentication-1.6.0/setup.py` & `mitol-django-authentication-2023.1.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     ],
     'description': 'MIT Open Learning django app extensions for oauth toolkit',
     'install_requires': (
         'django-anymail>=6.0',
         'django<4.0,>=2.2.12',
         'djangorestframework>=3.0.0',
         'djoser==2.1.0',
-        'mitol-django-common~=2.7.0',
-        'mitol-django-mail~=3.3.0',
+        'mitol-django-common',
+        'mitol-django-mail',
         'social-auth-app-django>=3.1.0',
     ),
     'license': 'BSD 3-Clause License',
     'long_description': """mitol-django-authentication
 ---
 
 This is the Open Learning Django Authentication app. It provides a few key features around authentication:
@@ -57,11 +57,11 @@
         'mitol.authentication',
         'mitol.authentication.migrations',
         'mitol.authentication.serializers',
         'mitol.authentication.settings',
         'mitol.authentication.urls',
         'mitol.authentication.views',
     ),
-    'python_requires': '>=3.7',
-    'version': '1.6.0',
+    'python_requires': '>=3.8',
+    'version': '2023.1.17',
     'zip_safe': True,
 })
```

