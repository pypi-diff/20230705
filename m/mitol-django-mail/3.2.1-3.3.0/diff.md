# Comparing `tmp/mitol-django-mail-3.2.1.tar.gz` & `tmp/mitol-django-mail-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitol-django-mail-3.2.1.tar", last modified: Mon Oct 31 19:56:51 2022, max compression
+gzip compressed data, was "mitol-django-mail-3.3.0.tar", last modified: Tue Jan 17 16:15:21 2023, max compression
```

## Comparing `mitol-django-mail-3.2.1.tar` & `mitol-django-mail-3.3.0.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:51.610127 mitol-django-mail-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-31 19:56:50.000000 mitol-django-mail-3.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-10-31 19:56:51.610127 mitol-django-mail-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-10-31 19:56:50.000000 mitol-django-mail-3.2.1/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:51.606126 mitol-django-mail-3.2.1/mitol/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-10-31 19:56:50.000000 mitol-django-mail-3.2.1/mitol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:51.610127 mitol-django-mail-3.2.1/mitol/mail/
--rw-r--r--   0 runner    (1001) docker     (121)     4148 2022-10-31 19:56:50.000000 mitol-django-mail-3.2.1/mitol/mail/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     3252 2022-10-31 19:56:50.000000 mitol-django-mail-3.2.1/mitol/mail/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-31 19:56:50.000000 mitol-django-mail-3.2.1/mitol/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8303 2022-10-31 19:56:50.000000 mitol-django-mail-3.2.1/mitol/mail/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-10-31 19:56:50.000000 mitol-django-mail-3.2.1/mitol/mail/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      716 2022-10-31 19:56:50.000000 mitol-django-mail-3.2.1/mitol/mail/defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-10-31 19:56:50.000000 mitol-django-mail-3.2.1/mitol/mail/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-10-31 19:56:50.000000 mitol-django-mail-3.2.1/mitol/mail/manage.py
--rw-r--r--   0 runner    (1001) docker     (121)     2377 2022-10-31 19:56:50.000000 mitol-django-mail-3.2.1/mitol/mail/messages.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:50.000000 mitol-django-mail-3.2.1/mitol/mail/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:51.610127 mitol-django-mail-3.2.1/mitol/mail/settings/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:50.000000 mitol-django-mail-3.2.1/mitol/mail/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2010 2022-10-31 19:56:50.000000 mitol-django-mail-3.2.1/mitol/mail/settings/email.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:51.606126 mitol-django-mail-3.2.1/mitol/mail/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:51.610127 mitol-django-mail-3.2.1/mitol/mail/templates/mail/
--rw-r--r--   0 runner    (1001) docker     (121)    11199 2022-10-31 19:56:50.000000 mitol-django-mail-3.2.1/mitol/mail/templates/mail/email_base.html
--rw-r--r--   0 runner    (1001) docker     (121)     2820 2022-10-31 19:56:50.000000 mitol-django-mail-3.2.1/mitol/mail/templates/mail/email_debugger.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:51.610127 mitol-django-mail-3.2.1/mitol/mail/templates/mail/partials/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-10-31 19:56:50.000000 mitol-django-mail-3.2.1/mitol/mail/templates/mail/partials/_logo.html
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-10-31 19:56:50.000000 mitol-django-mail-3.2.1/mitol/mail/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-10-31 19:56:50.000000 mitol-django-mail-3.2.1/mitol/mail/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:51.610127 mitol-django-mail-3.2.1/mitol_django_mail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-10-31 19:56:51.000000 mitol-django-mail-3.2.1/mitol_django_mail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      790 2022-10-31 19:56:51.000000 mitol-django-mail-3.2.1/mitol_django_mail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 19:56:51.000000 mitol-django-mail-3.2.1/mitol_django_mail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-31 19:56:51.000000 mitol-django-mail-3.2.1/mitol_django_mail.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-10-31 19:56:51.000000 mitol-django-mail-3.2.1/mitol_django_mail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-31 19:56:51.000000 mitol-django-mail-3.2.1/mitol_django_mail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 19:56:51.000000 mitol-django-mail-3.2.1/mitol_django_mail.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-31 19:56:51.610127 mitol-django-mail-3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2022-10-31 19:56:50.000000 mitol-django-mail-3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:15:21.019961 mitol-django-mail-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-01-17 16:15:20.000000 mitol-django-mail-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-01-17 16:15:21.019961 mitol-django-mail-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-01-17 16:15:20.000000 mitol-django-mail-3.3.0/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:15:21.015962 mitol-django-mail-3.3.0/mitol/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-01-17 16:15:20.000000 mitol-django-mail-3.3.0/mitol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:15:21.015962 mitol-django-mail-3.3.0/mitol/mail/
+-rw-r--r--   0 runner    (1001) docker     (122)     4278 2023-01-17 16:15:20.000000 mitol-django-mail-3.3.0/mitol/mail/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3252 2023-01-17 16:15:20.000000 mitol-django-mail-3.3.0/mitol/mail/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-01-17 16:15:20.000000 mitol-django-mail-3.3.0/mitol/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8303 2023-01-17 16:15:20.000000 mitol-django-mail-3.3.0/mitol/mail/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-01-17 16:15:20.000000 mitol-django-mail-3.3.0/mitol/mail/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-01-17 16:15:20.000000 mitol-django-mail-3.3.0/mitol/mail/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-01-17 16:15:20.000000 mitol-django-mail-3.3.0/mitol/mail/forms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2377 2023-01-17 16:15:20.000000 mitol-django-mail-3.3.0/mitol/mail/messages.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:15:20.000000 mitol-django-mail-3.3.0/mitol/mail/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:15:21.015962 mitol-django-mail-3.3.0/mitol/mail/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:15:20.000000 mitol-django-mail-3.3.0/mitol/mail/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2010 2023-01-17 16:15:20.000000 mitol-django-mail-3.3.0/mitol/mail/settings/email.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:15:21.015962 mitol-django-mail-3.3.0/mitol/mail/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:15:21.015962 mitol-django-mail-3.3.0/mitol/mail/templates/mail/
+-rw-r--r--   0 runner    (1001) docker     (122)    11199 2023-01-17 16:15:20.000000 mitol-django-mail-3.3.0/mitol/mail/templates/mail/email_base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2820 2023-01-17 16:15:20.000000 mitol-django-mail-3.3.0/mitol/mail/templates/mail/email_debugger.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:15:21.019961 mitol-django-mail-3.3.0/mitol/mail/templates/mail/partials/
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-01-17 16:15:20.000000 mitol-django-mail-3.3.0/mitol/mail/templates/mail/partials/_logo.html
+-rw-r--r--   0 runner    (1001) docker     (122)      393 2023-01-17 16:15:20.000000 mitol-django-mail-3.3.0/mitol/mail/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-01-17 16:15:20.000000 mitol-django-mail-3.3.0/mitol/mail/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:15:21.019961 mitol-django-mail-3.3.0/mitol_django_mail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-01-17 16:15:21.000000 mitol-django-mail-3.3.0/mitol_django_mail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      769 2023-01-17 16:15:21.000000 mitol-django-mail-3.3.0/mitol_django_mail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 16:15:21.000000 mitol-django-mail-3.3.0/mitol_django_mail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-17 16:15:21.000000 mitol-django-mail-3.3.0/mitol_django_mail.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-01-17 16:15:21.000000 mitol-django-mail-3.3.0/mitol_django_mail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-17 16:15:21.000000 mitol-django-mail-3.3.0/mitol_django_mail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 16:15:20.000000 mitol-django-mail-3.3.0/mitol_django_mail.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-17 16:15:21.019961 mitol-django-mail-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4762 2023-01-17 16:15:20.000000 mitol-django-mail-3.3.0/setup.py
```

### Comparing `mitol-django-mail-3.2.1/backend_shim.py` & `mitol-django-mail-3.3.0/backend_shim.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 
 # DO NOT EDIT THIS FILE -- AUTOGENERATED BY PANTS
 
+import os
 import setuptools.build_meta
 
 backend = setuptools.build_meta.__legacy__
 
 dist_dir = "dist"
 build_wheel = True
 build_sdist = True
 wheel_config_settings = {
 }
 sdist_config_settings = {
 }
 
+os.makedirs(dist_dir, exist_ok=True)
 wheel_path = backend.build_wheel(dist_dir, wheel_config_settings) if build_wheel else None
 sdist_path = backend.build_sdist(dist_dir, sdist_config_settings) if build_sdist else None
 
 if wheel_path:
     print("wheel: {wheel_path}".format(wheel_path=wheel_path))
 if sdist_path:
     print("sdist: {sdist_path}".format(sdist_path=sdist_path))
```

### Comparing `mitol-django-mail-3.2.1/mitol/mail/CHANGELOG.md` & `mitol-django-mail-3.3.0/mitol/mail/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [3.3.0] - 2023-01-17
+
 ## [3.2.1] - 2022-10-31
 
 ## [3.2.0] - 2022-06-24
 
 ## [3.1.0] - 2022-05-12
 
 ### Changed
@@ -95,15 +97,16 @@
 ### Fixed
 - Attempted fix of GitHub CI pipeline
 
 ## [0.1.0] - 2020-09-29
 ### Added
 - Initial port of the `mail` app
 
-[Unreleased]: https://github.com/mitodl/ol-django/compare/mitol-django-mail/v3.2.1...HEAD
+[Unreleased]: https://github.com/mitodl/ol-django/compare/mitol-django-mail/v3.3.0...HEAD
+[3.3.0]: https://github.com/mitodl/ol-django/compare/mitol-django-mail/v3.2.1...mitol-django-mail/v3.3.0
 [3.2.1]: https://github.com/mitodl/ol-django/compare/mitol-django-mail/v3.2.0...mitol-django-mail/v3.2.1
 [3.2.0]: https://github.com/mitodl/ol-django/compare/mitol-django-mail/v3.1.0...mitol-django-mail/v3.2.0
 [3.1.0]: https://github.com/mitodl/ol-django/compare/mitol-django-mail/v3.0.1...mitol-django-mail/v3.1.0
 [3.0.1]: https://github.com/mitodl/ol-django/compare/mitol-django-mail/v3.0.0...mitol-django-mail/v3.0.1
 [3.0.0]: https://github.com/mitodl/ol-django/compare/mitol-django-mail/v2.2.0...mitol-django-mail/v3.0.0
 [2.2.0]: https://github.com/mitodl/ol-django/compare/mitol-django-mail/v2.1.0...mitol-django-mail/v2.2.0
 [2.1.0]: https://github.com/mitodl/ol-django/compare/mitol-django-mail/v2.0.0...mitol-django-mail/v2.1.0
```

### Comparing `mitol-django-mail-3.2.1/mitol/mail/README.md` & `mitol-django-mail-3.3.0/mitol/mail/README.md`

 * *Files identical despite different names*

### Comparing `mitol-django-mail-3.2.1/mitol/mail/api.py` & `mitol-django-mail-3.3.0/mitol/mail/api.py`

 * *Files identical despite different names*

### Comparing `mitol-django-mail-3.2.1/mitol/mail/defaults.py` & `mitol-django-mail-3.3.0/mitol/mail/defaults.py`

 * *Files identical despite different names*

### Comparing `mitol-django-mail-3.2.1/mitol/mail/forms.py` & `mitol-django-mail-3.3.0/mitol/mail/forms.py`

 * *Files identical despite different names*

### Comparing `mitol-django-mail-3.2.1/mitol/mail/messages.py` & `mitol-django-mail-3.3.0/mitol/mail/messages.py`

 * *Files identical despite different names*

### Comparing `mitol-django-mail-3.2.1/mitol/mail/settings/email.py` & `mitol-django-mail-3.3.0/mitol/mail/settings/email.py`

 * *Files identical despite different names*

### Comparing `mitol-django-mail-3.2.1/mitol/mail/templates/mail/email_base.html` & `mitol-django-mail-3.3.0/mitol/mail/templates/mail/email_base.html`

 * *Files identical despite different names*

### Comparing `mitol-django-mail-3.2.1/mitol/mail/templates/mail/email_debugger.html` & `mitol-django-mail-3.3.0/mitol/mail/templates/mail/email_debugger.html`

 * *Files identical despite different names*

### Comparing `mitol-django-mail-3.2.1/mitol/mail/views.py` & `mitol-django-mail-3.3.0/mitol/mail/views.py`

 * *Files identical despite different names*

### Comparing `mitol-django-mail-3.2.1/mitol_django_mail.egg-info/SOURCES.txt` & `mitol-django-mail-3.3.0/mitol_django_mail.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 mitol/mail/CHANGELOG.md
 mitol/mail/README.md
 mitol/mail/__init__.py
 mitol/mail/api.py
 mitol/mail/apps.py
 mitol/mail/defaults.py
 mitol/mail/forms.py
-mitol/mail/manage.py
 mitol/mail/messages.py
 mitol/mail/py.typed
 mitol/mail/urls.py
 mitol/mail/views.py
 mitol/mail/settings/__init__.py
 mitol/mail/settings/email.py
 mitol/mail/templates/mail/email_base.html
```

