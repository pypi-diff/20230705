# Comparing `tmp/mitol-django-openedx-1.3.0.tar.gz` & `tmp/mitol-django-openedx-2023.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitol-django-openedx-1.3.0.tar", last modified: Tue Jan 17 16:13:30 2023, max compression
+gzip compressed data, was "mitol-django-openedx-2023.1.17.tar", last modified: Wed Jul  5 16:16:56 2023, max compression
```

## Comparing `mitol-django-openedx-1.3.0.tar` & `mitol-django-openedx-2023.1.17.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:13:30.557811 mitol-django-openedx-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-01-17 16:13:29.000000 mitol-django-openedx-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-01-17 16:13:30.557811 mitol-django-openedx-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-01-17 16:13:29.000000 mitol-django-openedx-1.3.0/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:13:30.557811 mitol-django-openedx-1.3.0/mitol/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-01-17 16:13:29.000000 mitol-django-openedx-1.3.0/mitol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:13:30.557811 mitol-django-openedx-1.3.0/mitol/openedx/
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-01-17 16:13:29.000000 mitol-django-openedx-1.3.0/mitol/openedx/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      195 2023-01-17 16:13:29.000000 mitol-django-openedx-1.3.0/mitol/openedx/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-01-17 16:13:29.000000 mitol-django-openedx-1.3.0/mitol/openedx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-01-17 16:13:29.000000 mitol-django-openedx-1.3.0/mitol/openedx/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:13:29.000000 mitol-django-openedx-1.3.0/mitol/openedx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:13:30.557811 mitol-django-openedx-1.3.0/mitol/openedx/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:13:29.000000 mitol-django-openedx-1.3.0/mitol/openedx/settings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:13:30.557811 mitol-django-openedx-1.3.0/mitol/openedx/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-01-17 16:13:29.000000 mitol-django-openedx-1.3.0/mitol/openedx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      764 2023-01-17 16:13:29.000000 mitol-django-openedx-1.3.0/mitol/openedx/utils/courses.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:13:30.557811 mitol-django-openedx-1.3.0/mitol_django_openedx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-01-17 16:13:30.000000 mitol-django-openedx-1.3.0/mitol_django_openedx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-01-17 16:13:30.000000 mitol-django-openedx-1.3.0/mitol_django_openedx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 16:13:30.000000 mitol-django-openedx-1.3.0/mitol_django_openedx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-17 16:13:30.000000 mitol-django-openedx-1.3.0/mitol_django_openedx.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)       54 2023-01-17 16:13:30.000000 mitol-django-openedx-1.3.0/mitol_django_openedx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-17 16:13:30.000000 mitol-django-openedx-1.3.0/mitol_django_openedx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 16:13:30.000000 mitol-django-openedx-1.3.0/mitol_django_openedx.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-17 16:13:30.557811 mitol-django-openedx-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-01-17 16:13:29.000000 mitol-django-openedx-1.3.0/setup.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.979988 mitol-django-openedx-2023.1.17/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       12 2023-07-05 16:16:55.000000 mitol-django-openedx-2023.1.17/MANIFEST.in
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      712 2023-07-05 16:16:56.979988 mitol-django-openedx-2023.1.17/PKG-INFO
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      748 2023-07-05 16:16:55.000000 mitol-django-openedx-2023.1.17/backend_shim.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.973322 mitol-django-openedx-2023.1.17/mitol/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       56 2023-07-05 16:16:55.000000 mitol-django-openedx-2023.1.17/mitol/__init__.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.976655 mitol-django-openedx-2023.1.17/mitol/openedx/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      609 2023-07-05 16:16:55.000000 mitol-django-openedx-2023.1.17/mitol/openedx/CHANGELOG.md
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      195 2023-07-05 16:16:55.000000 mitol-django-openedx-2023.1.17/mitol/openedx/README.md
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      148 2023-07-05 16:16:55.000000 mitol-django-openedx-2023.1.17/mitol/openedx/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      665 2023-07-05 16:16:55.000000 mitol-django-openedx-2023.1.17/mitol/openedx/apps.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:55.000000 mitol-django-openedx-2023.1.17/mitol/openedx/py.typed
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.976655 mitol-django-openedx-2023.1.17/mitol/openedx/settings/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:55.000000 mitol-django-openedx-2023.1.17/mitol/openedx/settings/__init__.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.976655 mitol-django-openedx-2023.1.17/mitol/openedx/utils/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       61 2023-07-05 16:16:55.000000 mitol-django-openedx-2023.1.17/mitol/openedx/utils/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      764 2023-07-05 16:16:55.000000 mitol-django-openedx-2023.1.17/mitol/openedx/utils/courses.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.979988 mitol-django-openedx-2023.1.17/mitol_django_openedx.egg-info/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      712 2023-07-05 16:16:56.000000 mitol-django-openedx-2023.1.17/mitol_django_openedx.egg-info/PKG-INFO
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      585 2023-07-05 16:16:56.000000 mitol-django-openedx-2023.1.17/mitol_django_openedx.egg-info/SOURCES.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-07-05 16:16:56.000000 mitol-django-openedx-2023.1.17/mitol_django_openedx.egg-info/dependency_links.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        6 2023-07-05 16:16:56.000000 mitol-django-openedx-2023.1.17/mitol_django_openedx.egg-info/namespace_packages.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       54 2023-07-05 16:16:56.000000 mitol-django-openedx-2023.1.17/mitol_django_openedx.egg-info/requires.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        6 2023-07-05 16:16:56.000000 mitol-django-openedx-2023.1.17/mitol_django_openedx.egg-info/top_level.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-07-05 16:16:56.000000 mitol-django-openedx-2023.1.17/mitol_django_openedx.egg-info/zip-safe
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       38 2023-07-05 16:16:56.979988 mitol-django-openedx-2023.1.17/setup.cfg
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1505 2023-07-05 16:16:55.000000 mitol-django-openedx-2023.1.17/setup.py
```

### Comparing `mitol-django-openedx-1.3.0/PKG-INFO` & `mitol-django-openedx-2023.1.17/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mitol-django-openedx
-Version: 1.3.0
+Version: 2023.1.17
 Summary: MIT Open Learning django app extensions for edx related utilities
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
 
 mitol-django-openedx
 ---
 
 This is the Open Learning Openedx app. It provides common edx functionalities used across all our applications.
```

### Comparing `mitol-django-openedx-1.3.0/backend_shim.py` & `mitol-django-openedx-2023.1.17/backend_shim.py`

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

### Comparing `mitol-django-openedx-1.3.0/mitol/openedx/apps.py` & `mitol-django-openedx-2023.1.17/mitol/openedx/apps.py`

 * *Files identical despite different names*

### Comparing `mitol-django-openedx-1.3.0/mitol/openedx/utils/courses.py` & `mitol-django-openedx-2023.1.17/mitol/openedx/utils/courses.py`

 * *Files identical despite different names*

### Comparing `mitol-django-openedx-1.3.0/mitol_django_openedx.egg-info/PKG-INFO` & `mitol-django-openedx-2023.1.17/mitol_django_openedx.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mitol-django-openedx
-Version: 1.3.0
+Version: 2023.1.17
 Summary: MIT Open Learning django app extensions for edx related utilities
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
 
 mitol-django-openedx
 ---
 
 This is the Open Learning Openedx app. It provides common edx functionalities used across all our applications.
```

### Comparing `mitol-django-openedx-1.3.0/mitol_django_openedx.egg-info/SOURCES.txt` & `mitol-django-openedx-2023.1.17/mitol_django_openedx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitol-django-openedx-1.3.0/setup.py` & `mitol-django-openedx-2023.1.17/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,11 +46,11 @@
     },
     'packages': (
         'mitol',
         'mitol.openedx',
         'mitol.openedx.settings',
         'mitol.openedx.utils',
     ),
-    'python_requires': '>=3.7',
-    'version': '1.3.0',
+    'python_requires': '>=3.8',
+    'version': '2023.1.17',
     'zip_safe': True,
 })
```

