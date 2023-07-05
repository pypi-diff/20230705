# Comparing `tmp/mitol-django-oauth-toolkit-extensions-1.3.0.tar.gz` & `tmp/mitol-django-oauth-toolkit-extensions-2023.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitol-django-oauth-toolkit-extensions-1.3.0.tar", last modified: Tue Jan 17 16:37:01 2023, max compression
+gzip compressed data, was "mitol-django-oauth-toolkit-extensions-2023.1.17.tar", last modified: Wed Jul  5 16:16:56 2023, max compression
```

## Comparing `mitol-django-oauth-toolkit-extensions-1.3.0.tar` & `mitol-django-oauth-toolkit-extensions-2023.1.17.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:37:01.615018 mitol-django-oauth-toolkit-extensions-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-01-17 16:37:00.000000 mitol-django-oauth-toolkit-extensions-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-01-17 16:37:01.615018 mitol-django-oauth-toolkit-extensions-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-01-17 16:37:00.000000 mitol-django-oauth-toolkit-extensions-1.3.0/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:37:01.615018 mitol-django-oauth-toolkit-extensions-1.3.0/mitol/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-01-17 16:37:00.000000 mitol-django-oauth-toolkit-extensions-1.3.0/mitol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:37:01.615018 mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/
--rw-r--r--   0 runner    (1001) docker     (122)     1852 2023-01-17 16:37:00.000000 mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-01-17 16:37:00.000000 mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-01-17 16:37:00.000000 mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-01-17 16:37:00.000000 mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)      428 2023-01-17 16:37:00.000000 mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-01-17 16:37:00.000000 mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/backends.py
--rw-r--r--   0 runner    (1001) docker     (122)     3014 2023-01-17 16:37:00.000000 mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:37:01.615018 mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1366 2023-01-17 16:37:00.000000 mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/migrations/0001_add_application_access.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:37:00.000000 mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      730 2023-01-17 16:37:00.000000 mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/models.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:37:00.000000 mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    10763 2023-01-17 16:37:00.000000 mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:37:01.615018 mitol-django-oauth-toolkit-extensions-1.3.0/mitol_django_oauth_toolkit_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-01-17 16:37:01.000000 mitol-django-oauth-toolkit-extensions-1.3.0/mitol_django_oauth_toolkit_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-01-17 16:37:01.000000 mitol-django-oauth-toolkit-extensions-1.3.0/mitol_django_oauth_toolkit_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 16:37:01.000000 mitol-django-oauth-toolkit-extensions-1.3.0/mitol_django_oauth_toolkit_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-17 16:37:01.000000 mitol-django-oauth-toolkit-extensions-1.3.0/mitol_django_oauth_toolkit_extensions.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-01-17 16:37:01.000000 mitol-django-oauth-toolkit-extensions-1.3.0/mitol_django_oauth_toolkit_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-17 16:37:01.000000 mitol-django-oauth-toolkit-extensions-1.3.0/mitol_django_oauth_toolkit_extensions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 16:37:01.000000 mitol-django-oauth-toolkit-extensions-1.3.0/mitol_django_oauth_toolkit_extensions.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-17 16:37:01.615018 mitol-django-oauth-toolkit-extensions-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2599 2023-01-17 16:37:00.000000 mitol-django-oauth-toolkit-extensions-1.3.0/setup.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.946655 mitol-django-oauth-toolkit-extensions-2023.1.17/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       12 2023-07-05 16:16:55.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/MANIFEST.in
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1653 2023-07-05 16:16:56.946655 mitol-django-oauth-toolkit-extensions-2023.1.17/PKG-INFO
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      748 2023-07-05 16:16:55.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/backend_shim.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.933321 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       56 2023-07-05 16:16:55.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/__init__.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.943322 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1820 2023-07-05 16:16:55.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/CHANGELOG.md
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1127 2023-07-05 16:16:55.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/README.md
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      214 2023-07-05 16:16:55.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      660 2023-07-05 16:16:55.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/admin.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      428 2023-07-05 16:16:55.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/apps.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1275 2023-07-05 16:16:55.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/backends.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     3014 2023-07-05 16:16:55.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/factories.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.943322 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/migrations/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1366 2023-07-05 16:16:55.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/migrations/0001_add_application_access.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:55.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/migrations/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      730 2023-07-05 16:16:55.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/models.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:55.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/py.typed
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)    10763 2023-07-05 16:16:55.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/utils.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.946655 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol_django_oauth_toolkit_extensions.egg-info/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1653 2023-07-05 16:16:56.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol_django_oauth_toolkit_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1026 2023-07-05 16:16:56.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol_django_oauth_toolkit_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-07-05 16:16:56.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol_django_oauth_toolkit_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        6 2023-07-05 16:16:56.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol_django_oauth_toolkit_extensions.egg-info/namespace_packages.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      115 2023-07-05 16:16:56.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol_django_oauth_toolkit_extensions.egg-info/requires.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        6 2023-07-05 16:16:56.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol_django_oauth_toolkit_extensions.egg-info/top_level.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-07-05 16:16:56.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/mitol_django_oauth_toolkit_extensions.egg-info/zip-safe
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       38 2023-07-05 16:16:56.946655 mitol-django-oauth-toolkit-extensions-2023.1.17/setup.cfg
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     2596 2023-07-05 16:16:55.000000 mitol-django-oauth-toolkit-extensions-2023.1.17/setup.py
```

### Comparing `mitol-django-oauth-toolkit-extensions-1.3.0/PKG-INFO` & `mitol-django-oauth-toolkit-extensions-2023.1.17/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mitol-django-oauth-toolkit-extensions
-Version: 1.3.0
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
 
 mitol-django-oauth-toolkit-extensions
 ---
 
 This is the Open Learning's extensions to `django-oauth-toolkit`.
```

### Comparing `mitol-django-oauth-toolkit-extensions-1.3.0/backend_shim.py` & `mitol-django-oauth-toolkit-extensions-2023.1.17/backend_shim.py`

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

### Comparing `mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/CHANGELOG.md` & `mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
-and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
+and this project uses date-based versioning.
 
-## [Unreleased]
+<!-- scriv-insert-here -->
 
 ## [1.3.0] - 2023-01-17
 
 ## [1.2.1] - 2022-10-31
 
 ## [1.2.0] - 2022-06-24
```

### Comparing `mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/README.md` & `mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/README.md`

 * *Files identical despite different names*

### Comparing `mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/admin.py` & `mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/admin.py`

 * *Files identical despite different names*

### Comparing `mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/backends.py` & `mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/backends.py`

 * *Files identical despite different names*

### Comparing `mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/factories.py` & `mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/factories.py`

 * *Files identical despite different names*

### Comparing `mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/migrations/0001_add_application_access.py` & `mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/migrations/0001_add_application_access.py`

 * *Files identical despite different names*

### Comparing `mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/models.py` & `mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/models.py`

 * *Files identical despite different names*

### Comparing `mitol-django-oauth-toolkit-extensions-1.3.0/mitol/oauth_toolkit_extensions/utils.py` & `mitol-django-oauth-toolkit-extensions-2023.1.17/mitol/oauth_toolkit_extensions/utils.py`

 * *Files identical despite different names*

### Comparing `mitol-django-oauth-toolkit-extensions-1.3.0/mitol_django_oauth_toolkit_extensions.egg-info/PKG-INFO` & `mitol-django-oauth-toolkit-extensions-2023.1.17/mitol_django_oauth_toolkit_extensions.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mitol-django-oauth-toolkit-extensions
-Version: 1.3.0
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
 
 mitol-django-oauth-toolkit-extensions
 ---
 
 This is the Open Learning's extensions to `django-oauth-toolkit`.
```

### Comparing `mitol-django-oauth-toolkit-extensions-1.3.0/mitol_django_oauth_toolkit_extensions.egg-info/SOURCES.txt` & `mitol-django-oauth-toolkit-extensions-2023.1.17/mitol_django_oauth_toolkit_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitol-django-oauth-toolkit-extensions-1.3.0/setup.py` & `mitol-django-oauth-toolkit-extensions-2023.1.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         'Programming Language :: Python :: 3.8',
     ],
     'description': 'MIT Open Learning django app extensions for oauth toolkit',
     'install_requires': (
         'django-oauth-toolkit>=1.3.3',
         'django<4.0,>=2.2.12',
         'factory-boy~=3.2',
-        'mitol-django-common~=2.7.0',
+        'mitol-django-common',
         'pytz>=2020.4',
         'requests>=2.20.0',
     ),
     'license': 'BSD 3-Clause License',
     'long_description': """mitol-django-oauth-toolkit-extensions
 ---
 
@@ -77,11 +77,11 @@
         ),
     },
     'packages': (
         'mitol',
         'mitol.oauth_toolkit_extensions',
         'mitol.oauth_toolkit_extensions.migrations',
     ),
-    'python_requires': '>=3.7',
-    'version': '1.3.0',
+    'python_requires': '>=3.8',
+    'version': '2023.1.17',
     'zip_safe': True,
 })
```

