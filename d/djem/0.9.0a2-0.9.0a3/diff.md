# Comparing `tmp/djem-0.9.0a2.tar.gz` & `tmp/djem-0.9.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djem-0.9.0a2.tar", last modified: Wed Feb 15 21:25:59 2023, max compression
+gzip compressed data, was "djem-0.9.0a3.tar", last modified: Wed Jul  5 04:29:53 2023, max compression
```

## Comparing `djem-0.9.0a2.tar` & `djem-0.9.0a3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-15 21:25:59.304611 djem-0.9.0a2/
--rw-r--r--   0 alex      (1000) alex      (1000)     5532 2023-02-15 09:56:27.000000 djem-0.9.0a2/CHANGELOG.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     1499 2021-07-20 22:27:58.000000 djem-0.9.0a2/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)       92 2021-08-19 21:56:45.000000 djem-0.9.0a2/MANIFEST.in
--rw-rw-r--   0 alex      (1000) alex      (1000)     2463 2023-02-15 21:25:59.304611 djem-0.9.0a2/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     1437 2022-12-04 05:56:42.000000 djem-0.9.0a2/README.rst
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-15 21:25:59.296610 djem-0.9.0a2/djem/
--rw-rw-r--   0 alex      (1000) alex      (1000)      315 2023-02-15 21:25:35.000000 djem-0.9.0a2/djem/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2493 2021-07-29 20:50:47.000000 djem-0.9.0a2/djem/ajax.py
--rw-r--r--   0 alex      (1000) alex      (1000)    12284 2022-12-11 22:41:21.000000 djem-0.9.0a2/djem/auth.py
--rw-r--r--   0 alex      (1000) alex      (1000)      565 2021-07-29 20:53:04.000000 djem-0.9.0a2/djem/exceptions.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-15 21:25:59.296610 djem-0.9.0a2/djem/forms/
--rw-r--r--   0 alex      (1000) alex      (1000)      132 2021-08-05 21:53:25.000000 djem-0.9.0a2/djem/forms/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2942 2021-08-05 21:54:13.000000 djem-0.9.0a2/djem/forms/bases.py
--rw-r--r--   0 alex      (1000) alex      (1000)      559 2021-07-29 20:50:32.000000 djem-0.9.0a2/djem/forms/fields.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1855 2021-07-28 21:01:19.000000 djem-0.9.0a2/djem/middleware.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-15 21:25:59.296610 djem-0.9.0a2/djem/models/
--rw-r--r--   0 alex      (1000) alex      (1000)       82 2021-07-20 22:27:58.000000 djem-0.9.0a2/djem/models/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2936 2021-07-29 20:52:36.000000 djem-0.9.0a2/djem/models/fields.py
--rw-r--r--   0 alex      (1000) alex      (1000)    27696 2022-12-04 21:25:58.000000 djem-0.9.0a2/djem/models/models.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1398 2021-07-20 22:27:58.000000 djem-0.9.0a2/djem/pagination.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-15 21:25:59.292609 djem-0.9.0a2/djem/templates/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-15 21:25:59.300610 djem-0.9.0a2/djem/templates/djem/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-15 21:25:59.300610 djem-0.9.0a2/djem/templates/djem/csrfify_ajax/
--rw-r--r--   0 alex      (1000) alex      (1000)      452 2021-07-20 22:27:58.000000 djem-0.9.0a2/djem/templates/djem/csrfify_ajax/jquery.html
--rw-r--r--   0 alex      (1000) alex      (1000)      648 2021-07-20 22:27:58.000000 djem-0.9.0a2/djem/templates/djem/form_field.html
--rw-r--r--   0 alex      (1000) alex      (1000)      881 2023-02-15 21:17:01.000000 djem-0.9.0a2/djem/templates/djem/pagination.html
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-15 21:25:59.300610 djem-0.9.0a2/djem/templatetags/
--rw-r--r--   0 alex      (1000) alex      (1000)        0 2021-07-20 22:27:58.000000 djem-0.9.0a2/djem/templatetags/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     7551 2022-12-11 23:20:34.000000 djem-0.9.0a2/djem/templatetags/djem.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-15 21:25:59.300610 djem-0.9.0a2/djem/tests/
--rw-r--r--   0 alex      (1000) alex      (1000)      290 2021-07-20 22:27:58.000000 djem-0.9.0a2/djem/tests/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     7490 2021-08-17 22:22:26.000000 djem-0.9.0a2/djem/tests/models.py
--rw-r--r--   0 alex      (1000) alex      (1000)     9183 2021-07-28 22:03:55.000000 djem-0.9.0a2/djem/tests/test_ajax.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    85127 2022-12-12 02:12:01.000000 djem-0.9.0a2/djem/tests/test_auth.py
--rw-r--r--   0 alex      (1000) alex      (1000)    10799 2021-08-05 21:55:15.000000 djem-0.9.0a2/djem/tests/test_forms.py
--rw-r--r--   0 alex      (1000) alex      (1000)     6783 2021-07-28 21:09:47.000000 djem-0.9.0a2/djem/tests/test_middleware.py
--rw-r--r--   0 alex      (1000) alex      (1000)    83878 2021-08-23 22:06:58.000000 djem-0.9.0a2/djem/tests/test_models.py
--rw-r--r--   0 alex      (1000) alex      (1000)     4496 2021-07-29 22:12:48.000000 djem-0.9.0a2/djem/tests/test_pagination.py
--rw-r--r--   0 alex      (1000) alex      (1000)    46192 2021-07-29 22:15:35.000000 djem-0.9.0a2/djem/tests/test_templatetags.py
--rw-r--r--   0 alex      (1000) alex      (1000)     8499 2021-08-17 22:33:21.000000 djem-0.9.0a2/djem/tests/test_utils.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-15 21:25:59.304611 djem-0.9.0a2/djem/utils/
--rw-r--r--   0 alex      (1000) alex      (1000)        0 2021-07-20 22:27:58.000000 djem-0.9.0a2/djem/utils/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1123 2021-07-29 20:47:03.000000 djem-0.9.0a2/djem/utils/dev.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2086 2021-07-29 20:47:50.000000 djem-0.9.0a2/djem/utils/dt.py
--rw-r--r--   0 alex      (1000) alex      (1000)    20021 2022-12-03 01:46:16.000000 djem-0.9.0a2/djem/utils/inspect.py
--rw-r--r--   0 alex      (1000) alex      (1000)    11462 2021-07-29 20:48:17.000000 djem-0.9.0a2/djem/utils/mon.py
--rw-r--r--   0 alex      (1000) alex      (1000)    10574 2022-12-03 01:49:48.000000 djem-0.9.0a2/djem/utils/table.py
--rw-r--r--   0 alex      (1000) alex      (1000)     5539 2021-08-18 21:30:18.000000 djem-0.9.0a2/djem/utils/tests.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-15 21:25:59.296610 djem-0.9.0a2/djem.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     2463 2023-02-15 21:25:59.000000 djem-0.9.0a2/djem.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1011 2023-02-15 21:25:59.000000 djem-0.9.0a2/djem.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-02-15 21:25:59.000000 djem-0.9.0a2/djem.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       12 2023-02-15 21:25:59.000000 djem-0.9.0a2/djem.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        5 2023-02-15 21:25:59.000000 djem-0.9.0a2/djem.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)      104 2021-08-19 21:17:04.000000 djem-0.9.0a2/pyproject.toml
--rw-r--r--   0 alex      (1000) alex      (1000)     1832 2023-02-15 21:25:59.304611 djem-0.9.0a2/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-05 04:29:53.675848 djem-0.9.0a3/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5629 2023-07-05 04:12:44.000000 djem-0.9.0a3/CHANGELOG.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     1499 2021-07-20 22:27:58.000000 djem-0.9.0a3/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)       92 2021-08-19 21:56:45.000000 djem-0.9.0a3/MANIFEST.in
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2463 2023-07-05 04:29:53.675848 djem-0.9.0a3/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     1437 2022-12-04 05:56:42.000000 djem-0.9.0a3/README.rst
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-05 04:29:53.671848 djem-0.9.0a3/djem/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      383 2023-07-05 04:29:22.000000 djem-0.9.0a3/djem/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2493 2021-07-29 20:50:47.000000 djem-0.9.0a3/djem/ajax.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    12284 2022-12-11 22:41:21.000000 djem-0.9.0a3/djem/auth.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      565 2021-07-29 20:53:04.000000 djem-0.9.0a3/djem/exceptions.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-05 04:29:53.671848 djem-0.9.0a3/djem/forms/
+-rw-r--r--   0 alex      (1000) alex      (1000)      132 2021-08-05 21:53:25.000000 djem-0.9.0a3/djem/forms/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2942 2021-08-05 21:54:13.000000 djem-0.9.0a3/djem/forms/bases.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      559 2021-07-29 20:50:32.000000 djem-0.9.0a3/djem/forms/fields.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1855 2021-07-28 21:01:19.000000 djem-0.9.0a3/djem/middleware.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-05 04:29:53.671848 djem-0.9.0a3/djem/models/
+-rw-r--r--   0 alex      (1000) alex      (1000)       82 2021-07-20 22:27:58.000000 djem-0.9.0a3/djem/models/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2936 2021-07-29 20:52:36.000000 djem-0.9.0a3/djem/models/fields.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    27696 2022-12-04 21:25:58.000000 djem-0.9.0a3/djem/models/models.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1398 2021-07-20 22:27:58.000000 djem-0.9.0a3/djem/pagination.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-05 04:29:53.667848 djem-0.9.0a3/djem/templates/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-05 04:29:53.675848 djem-0.9.0a3/djem/templates/djem/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-05 04:29:53.675848 djem-0.9.0a3/djem/templates/djem/csrfify_ajax/
+-rw-r--r--   0 alex      (1000) alex      (1000)      452 2021-07-20 22:27:58.000000 djem-0.9.0a3/djem/templates/djem/csrfify_ajax/jquery.html
+-rw-r--r--   0 alex      (1000) alex      (1000)      648 2021-07-20 22:27:58.000000 djem-0.9.0a3/djem/templates/djem/form_field.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)      881 2023-07-05 04:04:27.000000 djem-0.9.0a3/djem/templates/djem/pagination.html
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-05 04:29:53.675848 djem-0.9.0a3/djem/templatetags/
+-rw-r--r--   0 alex      (1000) alex      (1000)        0 2021-07-20 22:27:58.000000 djem-0.9.0a3/djem/templatetags/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     7551 2022-12-11 23:20:34.000000 djem-0.9.0a3/djem/templatetags/djem.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-05 04:29:53.675848 djem-0.9.0a3/djem/tests/
+-rw-r--r--   0 alex      (1000) alex      (1000)      290 2021-07-20 22:27:58.000000 djem-0.9.0a3/djem/tests/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     7490 2021-08-17 22:22:26.000000 djem-0.9.0a3/djem/tests/models.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     9183 2021-07-28 22:03:55.000000 djem-0.9.0a3/djem/tests/test_ajax.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    85127 2022-12-12 02:12:01.000000 djem-0.9.0a3/djem/tests/test_auth.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    10799 2021-08-05 21:55:15.000000 djem-0.9.0a3/djem/tests/test_forms.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     6783 2021-07-28 21:09:47.000000 djem-0.9.0a3/djem/tests/test_middleware.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    83878 2021-08-23 22:06:58.000000 djem-0.9.0a3/djem/tests/test_models.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     4496 2021-07-29 22:12:48.000000 djem-0.9.0a3/djem/tests/test_pagination.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    46192 2021-07-29 22:15:35.000000 djem-0.9.0a3/djem/tests/test_templatetags.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     8839 2023-07-05 04:08:54.000000 djem-0.9.0a3/djem/tests/test_utils.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-05 04:29:53.675848 djem-0.9.0a3/djem/utils/
+-rw-r--r--   0 alex      (1000) alex      (1000)        0 2021-07-20 22:27:58.000000 djem-0.9.0a3/djem/utils/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1123 2021-07-29 20:47:03.000000 djem-0.9.0a3/djem/utils/dev.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2086 2021-07-29 20:47:50.000000 djem-0.9.0a3/djem/utils/dt.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    20021 2022-12-03 01:46:16.000000 djem-0.9.0a3/djem/utils/inspect.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    11462 2021-07-29 20:48:17.000000 djem-0.9.0a3/djem/utils/mon.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    10574 2022-12-03 01:49:48.000000 djem-0.9.0a3/djem/utils/table.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     5539 2021-08-18 21:30:18.000000 djem-0.9.0a3/djem/utils/tests.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-05 04:29:53.671848 djem-0.9.0a3/djem.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2463 2023-07-05 04:29:53.000000 djem-0.9.0a3/djem.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1011 2023-07-05 04:29:53.000000 djem-0.9.0a3/djem.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-05 04:29:53.000000 djem-0.9.0a3/djem.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       12 2023-07-05 04:29:53.000000 djem-0.9.0a3/djem.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        5 2023-07-05 04:29:53.000000 djem-0.9.0a3/djem.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)      104 2021-08-19 21:17:04.000000 djem-0.9.0a3/pyproject.toml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1832 2023-07-05 04:29:53.675848 djem-0.9.0a3/setup.cfg
```

### Comparing `djem-0.9.0a2/CHANGELOG.rst` & `djem-0.9.0a3/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Change Log
 ==========
 
 0.9.0 (unreleased)
 ==================
 
 * Improved customisability of pagination template
+* Updated ``UNDEFINED`` to ensure it cannot be deep copied (it will always be the same instance)
 
 0.8.0 (2022-12-12)
 ==================
 
 * Added compatibility with Django versions 4.0 and 4.1
 * Dropped support for Django versions below 3.2
 * Updated ``Auditable`` and ``Versionable`` to use ``self._state.adding`` to differentiate between records being added or updated
```

### Comparing `djem-0.9.0a2/LICENSE` & `djem-0.9.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/PKG-INFO` & `djem-0.9.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djem
-Version: 0.9.0a2
+Version: 0.9.0a3
 Summary: A collection of useful stuff for Django projects
 Home-page: https://github.com/oogles/djem
 Author: Alex Church
 Author-email: alex@church.id.au
 License: BSD
 Project-URL: Documentation, https://djem.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/oogles/djem/issues
```

### Comparing `djem-0.9.0a2/README.rst` & `djem-0.9.0a3/README.rst`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/ajax.py` & `djem-0.9.0a3/djem/ajax.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/auth.py` & `djem-0.9.0a3/djem/auth.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/exceptions.py` & `djem-0.9.0a3/djem/exceptions.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/forms/bases.py` & `djem-0.9.0a3/djem/forms/bases.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/forms/fields.py` & `djem-0.9.0a3/djem/forms/fields.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/middleware.py` & `djem-0.9.0a3/djem/middleware.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/models/fields.py` & `djem-0.9.0a3/djem/models/fields.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/models/models.py` & `djem-0.9.0a3/djem/models/models.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/pagination.py` & `djem-0.9.0a3/djem/pagination.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/templates/djem/form_field.html` & `djem-0.9.0a3/djem/templates/djem/form_field.html`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/templates/djem/pagination.html` & `djem-0.9.0a3/djem/templates/djem/pagination.html`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/templatetags/djem.py` & `djem-0.9.0a3/djem/templatetags/djem.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/tests/models.py` & `djem-0.9.0a3/djem/tests/models.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/tests/test_ajax.py` & `djem-0.9.0a3/djem/tests/test_ajax.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/tests/test_auth.py` & `djem-0.9.0a3/djem/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/tests/test_forms.py` & `djem-0.9.0a3/djem/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/tests/test_middleware.py` & `djem-0.9.0a3/djem/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/tests/test_models.py` & `djem-0.9.0a3/djem/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/tests/test_pagination.py` & `djem-0.9.0a3/djem/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/tests/test_templatetags.py` & `djem-0.9.0a3/djem/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/tests/test_utils.py` & `djem-0.9.0a3/djem/tests/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytz
 import warnings
+from copy import deepcopy
 
 from django.apps import apps
 from django.test import SimpleTestCase
 from django.utils import timezone
 
 from djem import UNDEFINED
 from djem.utils.dt import TimeZoneHelper
@@ -15,14 +16,27 @@
     def test_falsey(self):
         
         self.assertFalse(UNDEFINED)
     
     def test_print(self):
         
         self.assertEqual(str(UNDEFINED), '<undefined>')
+    
+    def test_deepcopy__direct(self):
+        
+        clone = deepcopy(UNDEFINED)
+        
+        self.assertIs(clone, UNDEFINED)
+    
+    def test_deepcopy__indirect(self):
+        
+        dict = {'value': UNDEFINED}
+        clone = deepcopy(dict)
+        
+        self.assertIs(clone['value'], UNDEFINED)
 
 
 class TimeZoneHelperTestCase(SimpleTestCase):
     
     def test_init__good_string(self):
         """
         Test constructing a TimeZoneHelper object with a valid timezone string.
```

### Comparing `djem-0.9.0a2/djem/utils/dev.py` & `djem-0.9.0a3/djem/utils/dev.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/utils/dt.py` & `djem-0.9.0a3/djem/utils/dt.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/utils/inspect.py` & `djem-0.9.0a3/djem/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/utils/mon.py` & `djem-0.9.0a3/djem/utils/mon.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/utils/table.py` & `djem-0.9.0a3/djem/utils/table.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem/utils/tests.py` & `djem-0.9.0a3/djem/utils/tests.py`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/djem.egg-info/PKG-INFO` & `djem-0.9.0a3/djem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djem
-Version: 0.9.0a2
+Version: 0.9.0a3
 Summary: A collection of useful stuff for Django projects
 Home-page: https://github.com/oogles/djem
 Author: Alex Church
 Author-email: alex@church.id.au
 License: BSD
 Project-URL: Documentation, https://djem.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/oogles/djem/issues
```

### Comparing `djem-0.9.0a2/djem.egg-info/SOURCES.txt` & `djem-0.9.0a3/djem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djem-0.9.0a2/setup.cfg` & `djem-0.9.0a3/setup.cfg`

 * *Files identical despite different names*

