# Comparing `tmp/asconnect-3.0.1.tar.gz` & `tmp/asconnect-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asconnect-3.0.1.tar", max compression
+gzip compressed data, was "asconnect-3.0.2.tar", max compression
```

## Comparing `asconnect-3.0.1.tar` & `asconnect-3.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1141 2023-05-29 02:27:05.304589 asconnect-3.0.1/LICENSE
--rw-r--r--   0        0        0     4502 2023-05-29 02:27:05.304589 asconnect-3.0.1/README.md
--rwxr-xr-x   0        0        0      297 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/__init__.py
--rw-r--r--   0        0        0     3165 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/altool.py
--rwxr-xr-x   0        0        0     3406 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/app_client.py
--rwxr-xr-x   0        0        0     5930 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/app_info_client.py
--rwxr-xr-x   0        0        0    10487 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/beta_review_client.py
--rwxr-xr-x   0        0        0     6296 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/build_client.py
--rwxr-xr-x   0        0        0     2301 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/client.py
--rw-r--r--   0        0        0     1301 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/exceptions.py
--rwxr-xr-x   0        0        0    12747 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/httpclient.py
--rw-r--r--   0        0        0      537 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/__init__.py
--rw-r--r--   0        0        0     2166 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/app_info.py
--rw-r--r--   0        0        0     4313 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/app_store.py
--rw-r--r--   0        0        0      933 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/app_store_version_localizations.py
--rw-r--r--   0        0        0     2721 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/apps.py
--rw-r--r--   0        0        0     1178 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/beta_app_review.py
--rw-r--r--   0        0        0     1866 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/beta_detail.py
--rw-r--r--   0        0        0     1277 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/beta_groups.py
--rw-r--r--   0        0        0     1225 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/builds.py
--rw-r--r--   0        0        0     1221 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/common.py
--rw-r--r--   0        0        0      978 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/idfa.py
--rw-r--r--   0        0        0     1373 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/localization.py
--rw-r--r--   0        0        0     4556 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/screenshots.py
--rw-r--r--   0        0        0     1364 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/users.py
--rwxr-xr-x   0        0        0     9963 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/screenshot_client.py
--rw-r--r--   0        0        0      352 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/sorting.py
--rwxr-xr-x   0        0        0     1216 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/users_client.py
--rw-r--r--   0        0        0     2219 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/utilities.py
--rwxr-xr-x   0        0        0    16470 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/version_client.py
--rw-r--r--   0        0        0     1342 2023-05-29 02:27:05.304589 asconnect-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     5662 1970-01-01 00:00:00.000000 asconnect-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1141 2023-07-05 06:01:18.578653 asconnect-3.0.2/LICENSE
+-rw-r--r--   0        0        0     4502 2023-07-05 06:01:18.578653 asconnect-3.0.2/README.md
+-rwxr-xr-x   0        0        0      297 2023-07-05 06:01:18.578653 asconnect-3.0.2/asconnect/__init__.py
+-rw-r--r--   0        0        0     3165 2023-07-05 06:01:18.578653 asconnect-3.0.2/asconnect/altool.py
+-rwxr-xr-x   0        0        0     3406 2023-07-05 06:01:18.578653 asconnect-3.0.2/asconnect/app_client.py
+-rwxr-xr-x   0        0        0     5930 2023-07-05 06:01:18.578653 asconnect-3.0.2/asconnect/app_info_client.py
+-rwxr-xr-x   0        0        0    10487 2023-07-05 06:01:18.578653 asconnect-3.0.2/asconnect/beta_review_client.py
+-rwxr-xr-x   0        0        0     6296 2023-07-05 06:01:18.578653 asconnect-3.0.2/asconnect/build_client.py
+-rwxr-xr-x   0        0        0     2301 2023-07-05 06:01:18.578653 asconnect-3.0.2/asconnect/client.py
+-rw-r--r--   0        0        0     1301 2023-07-05 06:01:18.578653 asconnect-3.0.2/asconnect/exceptions.py
+-rwxr-xr-x   0        0        0    12747 2023-07-05 06:01:18.578653 asconnect-3.0.2/asconnect/httpclient.py
+-rw-r--r--   0        0        0      537 2023-07-05 06:01:18.578653 asconnect-3.0.2/asconnect/models/__init__.py
+-rw-r--r--   0        0        0     2166 2023-07-05 06:01:18.578653 asconnect-3.0.2/asconnect/models/app_info.py
+-rw-r--r--   0        0        0     4313 2023-07-05 06:01:18.578653 asconnect-3.0.2/asconnect/models/app_store.py
+-rw-r--r--   0        0        0      933 2023-07-05 06:01:18.578653 asconnect-3.0.2/asconnect/models/app_store_version_localizations.py
+-rw-r--r--   0        0        0     2721 2023-07-05 06:01:18.578653 asconnect-3.0.2/asconnect/models/apps.py
+-rw-r--r--   0        0        0     1178 2023-07-05 06:01:18.578653 asconnect-3.0.2/asconnect/models/beta_app_review.py
+-rw-r--r--   0        0        0     1866 2023-07-05 06:01:18.578653 asconnect-3.0.2/asconnect/models/beta_detail.py
+-rw-r--r--   0        0        0     1277 2023-07-05 06:01:18.578653 asconnect-3.0.2/asconnect/models/beta_groups.py
+-rw-r--r--   0        0        0     1225 2023-07-05 06:01:18.578653 asconnect-3.0.2/asconnect/models/builds.py
+-rw-r--r--   0        0        0     1221 2023-07-05 06:01:18.578653 asconnect-3.0.2/asconnect/models/common.py
+-rw-r--r--   0        0        0      978 2023-07-05 06:01:18.578653 asconnect-3.0.2/asconnect/models/idfa.py
+-rw-r--r--   0        0        0     1373 2023-07-05 06:01:18.578653 asconnect-3.0.2/asconnect/models/localization.py
+-rw-r--r--   0        0        0     4556 2023-07-05 06:01:18.582653 asconnect-3.0.2/asconnect/models/screenshots.py
+-rw-r--r--   0        0        0     1364 2023-07-05 06:01:18.582653 asconnect-3.0.2/asconnect/models/users.py
+-rwxr-xr-x   0        0        0     9963 2023-07-05 06:01:18.582653 asconnect-3.0.2/asconnect/screenshot_client.py
+-rw-r--r--   0        0        0      352 2023-07-05 06:01:18.582653 asconnect-3.0.2/asconnect/sorting.py
+-rwxr-xr-x   0        0        0     1216 2023-07-05 06:01:18.582653 asconnect-3.0.2/asconnect/users_client.py
+-rw-r--r--   0        0        0     2219 2023-07-05 06:01:18.582653 asconnect-3.0.2/asconnect/utilities.py
+-rwxr-xr-x   0        0        0    16470 2023-07-05 06:01:18.582653 asconnect-3.0.2/asconnect/version_client.py
+-rw-r--r--   0        0        0     1343 2023-07-05 06:01:18.582653 asconnect-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5654 1970-01-01 00:00:00.000000 asconnect-3.0.2/PKG-INFO
```

### Comparing `asconnect-3.0.1/LICENSE` & `asconnect-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/README.md` & `asconnect-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/altool.py` & `asconnect-3.0.2/asconnect/altool.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/app_client.py` & `asconnect-3.0.2/asconnect/app_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/app_info_client.py` & `asconnect-3.0.2/asconnect/app_info_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/beta_review_client.py` & `asconnect-3.0.2/asconnect/beta_review_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/build_client.py` & `asconnect-3.0.2/asconnect/build_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/client.py` & `asconnect-3.0.2/asconnect/client.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/exceptions.py` & `asconnect-3.0.2/asconnect/exceptions.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/httpclient.py` & `asconnect-3.0.2/asconnect/httpclient.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/models/__init__.py` & `asconnect-3.0.2/asconnect/models/__init__.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/models/app_info.py` & `asconnect-3.0.2/asconnect/models/app_info.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/models/app_store.py` & `asconnect-3.0.2/asconnect/models/app_store.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/models/app_store_version_localizations.py` & `asconnect-3.0.2/asconnect/models/app_store_version_localizations.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/models/apps.py` & `asconnect-3.0.2/asconnect/models/apps.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/models/beta_app_review.py` & `asconnect-3.0.2/asconnect/models/beta_app_review.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/models/beta_detail.py` & `asconnect-3.0.2/asconnect/models/beta_detail.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/models/beta_groups.py` & `asconnect-3.0.2/asconnect/models/beta_groups.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/models/builds.py` & `asconnect-3.0.2/asconnect/models/builds.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/models/common.py` & `asconnect-3.0.2/asconnect/models/common.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/models/idfa.py` & `asconnect-3.0.2/asconnect/models/idfa.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/models/localization.py` & `asconnect-3.0.2/asconnect/models/localization.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/models/screenshots.py` & `asconnect-3.0.2/asconnect/models/screenshots.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/models/users.py` & `asconnect-3.0.2/asconnect/models/users.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/screenshot_client.py` & `asconnect-3.0.2/asconnect/screenshot_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/users_client.py` & `asconnect-3.0.2/asconnect/users_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/utilities.py` & `asconnect-3.0.2/asconnect/utilities.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/asconnect/version_client.py` & `asconnect-3.0.2/asconnect/version_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.1/pyproject.toml` & `asconnect-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asconnect"
-version = "3.0.1"
+version = "3.0.2"
 description = "A wrapper around the Apple App Store Connect APIs"
 
 license = "MIT"
 
 authors = [
     "Dale Myers <dalemy@microsoft.com>"
 ]
@@ -28,15 +28,15 @@
     'Programming Language :: Python :: 3.11',
     'Topic :: Software Development',
     'Topic :: Utilities'
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-cryptography = "^40.0.0"
+cryptography = ">=40,<42"
 deserialize = "^2.0.1"
 pyjwt = "^2.6.0"
 requests = "^2.28.2"
 tenacity = "^8.2.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
```

### Comparing `asconnect-3.0.1/PKG-INFO` & `asconnect-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asconnect
-Version: 3.0.1
+Version: 3.0.2
 Summary: A wrapper around the Apple App Store Connect APIs
 Home-page: https://github.com/microsoft/asconnect
 License: MIT
 Keywords: apple,app store,itunes,connect
 Author: Dale Myers
 Author-email: dalemy@microsoft.com
 Requires-Python: >=3.8,<4.0
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Dist: cryptography (>=40.0.0,<41.0.0)
+Requires-Dist: cryptography (>=40,<42)
 Requires-Dist: deserialize (>=2.0.1,<3.0.0)
 Requires-Dist: pyjwt (>=2.6.0,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Project-URL: Repository, https://github.com/microsoft/asconnect
 Description-Content-Type: text/markdown
```

