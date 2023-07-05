# Comparing `tmp/mitol-django-digital-credentials-3.2.1.tar.gz` & `tmp/mitol-django-digital-credentials-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitol-django-digital-credentials-3.2.1.tar", last modified: Mon Oct 31 19:58:38 2022, max compression
+gzip compressed data, was "mitol-django-digital-credentials-3.3.0.tar", last modified: Tue Jan 17 16:34:04 2023, max compression
```

## Comparing `mitol-django-digital-credentials-3.2.1.tar` & `mitol-django-digital-credentials-3.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:58:38.275142 mitol-django-digital-credentials-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-10-31 19:58:38.275142 mitol-django-digital-credentials-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:58:38.271142 mitol-django-digital-credentials-3.2.1/mitol/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/mitol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:58:38.271142 mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/
--rw-r--r--   0 runner    (1001) docker     (121)     4075 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     4196 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:58:38.271142 mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     4379 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/migrations/0001_add_digital_credentials_models.py
--rw-r--r--   0 runner    (1001) docker     (121)      991 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/migrations/0002_rename_courseware_to_credentialed.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1872 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)     2525 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/models.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     2283 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/requests_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3282 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1670 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:58:38.275142 mitol-django-digital-credentials-3.2.1/mitol_django_digital_credentials.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-10-31 19:58:38.000000 mitol-django-digital-credentials-3.2.1/mitol_django_digital_credentials.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-10-31 19:58:38.000000 mitol-django-digital-credentials-3.2.1/mitol_django_digital_credentials.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 19:58:38.000000 mitol-django-digital-credentials-3.2.1/mitol_django_digital_credentials.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-31 19:58:38.000000 mitol-django-digital-credentials-3.2.1/mitol_django_digital_credentials.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-10-31 19:58:38.000000 mitol-django-digital-credentials-3.2.1/mitol_django_digital_credentials.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-31 19:58:38.000000 mitol-django-digital-credentials-3.2.1/mitol_django_digital_credentials.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 19:58:38.000000 mitol-django-digital-credentials-3.2.1/mitol_django_digital_credentials.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-31 19:58:38.275142 mitol-django-digital-credentials-3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-10-31 19:58:37.000000 mitol-django-digital-credentials-3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:34:04.870816 mitol-django-digital-credentials-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-01-17 16:34:04.870816 mitol-django-digital-credentials-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:34:04.870816 mitol-django-digital-credentials-3.3.0/mitol/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:34:04.870816 mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/
+-rw-r--r--   0 runner    (1001) docker     (122)     4233 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4196 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:34:04.870816 mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     4379 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/migrations/0001_add_digital_credentials_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      991 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/migrations/0002_rename_courseware_to_credentialed.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2525 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/requests_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3282 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      990 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1670 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:34:04.870816 mitol-django-digital-credentials-3.3.0/mitol_django_digital_credentials.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol_django_digital_credentials.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol_django_digital_credentials.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol_django_digital_credentials.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol_django_digital_credentials.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol_django_digital_credentials.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol_django_digital_credentials.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/mitol_django_digital_credentials.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-17 16:34:04.870816 mitol-django-digital-credentials-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2755 2023-01-17 16:34:04.000000 mitol-django-digital-credentials-3.3.0/setup.py
```

### Comparing `mitol-django-digital-credentials-3.2.1/backend_shim.py` & `mitol-django-digital-credentials-3.3.0/backend_shim.py`

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

### Comparing `mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/CHANGELOG.md` & `mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/CHANGELOG.md`

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
@@ -81,15 +83,16 @@
 
 ## [0.1.0] - 2020-11-16
 
 ### Added
 - Added HMAC Signature + Digest Headers support
 - Added `mitol-django-digital-credentials` app
 
-[Unreleased]: https://github.com/mitodl/ol-django/compare/mitol-django-digitalcredentials/v3.2.1...HEAD
+[Unreleased]: https://github.com/mitodl/ol-django/compare/mitol-django-digitalcredentials/v3.3.0...HEAD
+[3.3.0]: https://github.com/mitodl/ol-django/compare/mitol-django-digitalcredentials/v3.2.1...mitol-django-digitalcredentials/v3.3.0
 [3.2.1]: https://github.com/mitodl/ol-django/compare/mitol-django-digitalcredentials/v3.2.0...mitol-django-digitalcredentials/v3.2.1
 [3.2.0]: https://github.com/mitodl/ol-django/compare/mitol-django-digitalcredentials/v3.1.0...mitol-django-digitalcredentials/v3.2.0
 [3.1.0]: https://github.com/mitodl/ol-django/compare/mitol-django-digitalcredentials/v3.0.1...mitol-django-digitalcredentials/v3.1.0
 [3.0.1]: https://github.com/mitodl/ol-django/compare/mitol-django-digitalcredentials/v3.0.0...mitol-django-digitalcredentials/v3.0.1
 [3.0.0]: https://github.com/mitodl/ol-django/compare/mitol-django-digitalcredentials/v2.0.0...mitol-django-digitalcredentials/v3.0.0
 [2.0.0]: https://github.com/mitodl/ol-django/compare/mitol-django-digital-credentials/v0.1.0...mitol-django-digital-credentials/v2.0.0
 [1.4.1]: https://github.com/mitodl/ol-django/compare/mitol-django-digital-credentials/v0.1.0...mitol-django-digital-credentials/v1.4.1
```

### Comparing `mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/README.md` & `mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/README.md`

 * *Files identical despite different names*

### Comparing `mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/admin.py` & `mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/admin.py`

 * *Files identical despite different names*

### Comparing `mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/apps.py` & `mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/apps.py`

 * *Files identical despite different names*

### Comparing `mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/backend.py` & `mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/backend.py`

 * *Files identical despite different names*

### Comparing `mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/factories.py` & `mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/factories.py`

 * *Files identical despite different names*

### Comparing `mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/migrations/0001_add_digital_credentials_models.py` & `mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/migrations/0001_add_digital_credentials_models.py`

 * *Files identical despite different names*

### Comparing `mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/migrations/0002_rename_courseware_to_credentialed.py` & `mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/migrations/0002_rename_courseware_to_credentialed.py`

 * *Files identical despite different names*

### Comparing `mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/mixins.py` & `mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/mixins.py`

 * *Files identical despite different names*

### Comparing `mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/models.py` & `mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/models.py`

 * *Files identical despite different names*

### Comparing `mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/requests_utils.py` & `mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/requests_utils.py`

 * *Files identical despite different names*

### Comparing `mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/serializers.py` & `mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/serializers.py`

 * *Files identical despite different names*

### Comparing `mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/settings.py` & `mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/settings.py`

 * *Files identical despite different names*

### Comparing `mitol-django-digital-credentials-3.2.1/mitol/digitalcredentials/views.py` & `mitol-django-digital-credentials-3.3.0/mitol/digitalcredentials/views.py`

 * *Files identical despite different names*

### Comparing `mitol-django-digital-credentials-3.2.1/mitol_django_digital_credentials.egg-info/SOURCES.txt` & `mitol-django-digital-credentials-3.3.0/mitol_django_digital_credentials.egg-info/SOURCES.txt`

 * *Files identical despite different names*

