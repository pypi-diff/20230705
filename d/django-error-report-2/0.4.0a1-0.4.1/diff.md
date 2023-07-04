# Comparing `tmp/django-error-report-2-0.4.0a1.tar.gz` & `tmp/django-error-report-2-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-error-report-2-0.4.0a1.tar", last modified: Tue Jul  4 22:00:05 2023, max compression
+gzip compressed data, was "django-error-report-2-0.4.1.tar", last modified: Tue Jul  4 22:03:21 2023, max compression
```

## Comparing `django-error-report-2-0.4.0a1.tar` & `django-error-report-2-0.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-04 22:00:05.199095 django-error-report-2-0.4.0a1/
--rw-r--r--   0 matmair    (501) staff       (20)     1086 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/LICENSE.txt
--rw-r--r--   0 matmair    (501) staff       (20)       37 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/MANIFEST.in
--rw-r--r--   0 matmair    (501) staff       (20)     2155 2023-07-04 22:00:05.198884 django-error-report-2-0.4.0a1/PKG-INFO
--rw-r--r--   0 matmair    (501) staff       (20)     1567 2023-07-04 21:07:36.000000 django-error-report-2-0.4.0a1/README.md
-drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-04 22:00:05.193822 django-error-report-2-0.4.0a1/django_error_report_2.egg-info/
--rw-r--r--   0 matmair    (501) staff       (20)     2155 2023-07-04 22:00:05.000000 django-error-report-2-0.4.0a1/django_error_report_2.egg-info/PKG-INFO
--rw-r--r--   0 matmair    (501) staff       (20)      572 2023-07-04 22:00:05.000000 django-error-report-2-0.4.0a1/django_error_report_2.egg-info/SOURCES.txt
--rw-r--r--   0 matmair    (501) staff       (20)        1 2023-07-04 22:00:05.000000 django-error-report-2-0.4.0a1/django_error_report_2.egg-info/dependency_links.txt
--rw-r--r--   0 matmair    (501) staff       (20)        1 2023-07-04 21:03:03.000000 django-error-report-2-0.4.0a1/django_error_report_2.egg-info/not-zip-safe
--rw-r--r--   0 matmair    (501) staff       (20)       12 2023-07-04 22:00:05.000000 django-error-report-2-0.4.0a1/django_error_report_2.egg-info/requires.txt
--rw-r--r--   0 matmair    (501) staff       (20)       13 2023-07-04 22:00:05.000000 django-error-report-2-0.4.0a1/django_error_report_2.egg-info/top_level.txt
-drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-04 22:00:05.196260 django-error-report-2-0.4.0a1/error_report/
--rw-r--r--   0 matmair    (501) staff       (20)        0 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/error_report/__init__.py
--rw-r--r--   0 matmair    (501) staff       (20)      955 2023-07-04 21:59:36.000000 django-error-report-2-0.4.0a1/error_report/admin.py
--rw-r--r--   0 matmair    (501) staff       (20)      180 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/error_report/apps.py
--rw-r--r--   0 matmair    (501) staff       (20)     1050 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/error_report/middleware.py
-drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-04 22:00:05.198595 django-error-report-2-0.4.0a1/error_report/migrations/
--rw-r--r--   0 matmair    (501) staff       (20)     1131 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/error_report/migrations/0001_initial.py
--rw-r--r--   0 matmair    (501) staff       (20)        0 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/error_report/migrations/__init__.py
--rw-r--r--   0 matmair    (501) staff       (20)     1750 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/error_report/models.py
--rw-r--r--   0 matmair    (501) staff       (20)      105 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/error_report/settings.py
--rw-r--r--   0 matmair    (501) staff       (20)      306 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/error_report/urls.py
--rw-r--r--   0 matmair    (501) staff       (20)      395 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/error_report/views.py
--rw-r--r--   0 matmair    (501) staff       (20)       38 2023-07-04 22:00:05.199156 django-error-report-2-0.4.0a1/setup.cfg
--rw-r--r--   0 matmair    (501) staff       (20)     1163 2023-07-04 21:53:56.000000 django-error-report-2-0.4.0a1/setup.py
+drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-04 22:03:21.195551 django-error-report-2-0.4.1/
+-rw-r--r--   0 matmair    (501) staff       (20)     1086 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/LICENSE.txt
+-rw-r--r--   0 matmair    (501) staff       (20)       37 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/MANIFEST.in
+-rw-r--r--   0 matmair    (501) staff       (20)     2153 2023-07-04 22:03:21.195354 django-error-report-2-0.4.1/PKG-INFO
+-rw-r--r--   0 matmair    (501) staff       (20)     1567 2023-07-04 21:07:36.000000 django-error-report-2-0.4.1/README.md
+drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-04 22:03:21.192123 django-error-report-2-0.4.1/django_error_report_2.egg-info/
+-rw-r--r--   0 matmair    (501) staff       (20)     2153 2023-07-04 22:03:21.000000 django-error-report-2-0.4.1/django_error_report_2.egg-info/PKG-INFO
+-rw-r--r--   0 matmair    (501) staff       (20)      572 2023-07-04 22:03:21.000000 django-error-report-2-0.4.1/django_error_report_2.egg-info/SOURCES.txt
+-rw-r--r--   0 matmair    (501) staff       (20)        1 2023-07-04 22:03:21.000000 django-error-report-2-0.4.1/django_error_report_2.egg-info/dependency_links.txt
+-rw-r--r--   0 matmair    (501) staff       (20)        1 2023-07-04 21:03:03.000000 django-error-report-2-0.4.1/django_error_report_2.egg-info/not-zip-safe
+-rw-r--r--   0 matmair    (501) staff       (20)       12 2023-07-04 22:03:21.000000 django-error-report-2-0.4.1/django_error_report_2.egg-info/requires.txt
+-rw-r--r--   0 matmair    (501) staff       (20)       13 2023-07-04 22:03:21.000000 django-error-report-2-0.4.1/django_error_report_2.egg-info/top_level.txt
+drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-04 22:03:21.194312 django-error-report-2-0.4.1/error_report/
+-rw-r--r--   0 matmair    (501) staff       (20)        0 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/error_report/__init__.py
+-rw-r--r--   0 matmair    (501) staff       (20)      955 2023-07-04 21:59:36.000000 django-error-report-2-0.4.1/error_report/admin.py
+-rw-r--r--   0 matmair    (501) staff       (20)      180 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/error_report/apps.py
+-rw-r--r--   0 matmair    (501) staff       (20)     1050 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/error_report/middleware.py
+drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-04 22:03:21.194859 django-error-report-2-0.4.1/error_report/migrations/
+-rw-r--r--   0 matmair    (501) staff       (20)     1131 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/error_report/migrations/0001_initial.py
+-rw-r--r--   0 matmair    (501) staff       (20)        0 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/error_report/migrations/__init__.py
+-rw-r--r--   0 matmair    (501) staff       (20)     1750 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/error_report/models.py
+-rw-r--r--   0 matmair    (501) staff       (20)      105 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/error_report/settings.py
+-rw-r--r--   0 matmair    (501) staff       (20)      306 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/error_report/urls.py
+-rw-r--r--   0 matmair    (501) staff       (20)      395 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/error_report/views.py
+-rw-r--r--   0 matmair    (501) staff       (20)       38 2023-07-04 22:03:21.195615 django-error-report-2-0.4.1/setup.cfg
+-rw-r--r--   0 matmair    (501) staff       (20)     1161 2023-07-04 22:02:34.000000 django-error-report-2-0.4.1/setup.py
```

### Comparing `django-error-report-2-0.4.0a1/LICENSE.txt` & `django-error-report-2-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-error-report-2-0.4.0a1/PKG-INFO` & `django-error-report-2-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-error-report-2
-Version: 0.4.0a1
+Version: 0.4.1
 Summary: View Django Error Report in Django Admin
 Home-page: https://github.com/matmair/django-error-report-2
 Author: M Hassan Siddiqui
 Author-email: mhassan.eeng@gmail.com
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `django-error-report-2-0.4.0a1/README.md` & `django-error-report-2-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `django-error-report-2-0.4.0a1/django_error_report_2.egg-info/PKG-INFO` & `django-error-report-2-0.4.1/django_error_report_2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-error-report-2
-Version: 0.4.0a1
+Version: 0.4.1
 Summary: View Django Error Report in Django Admin
 Home-page: https://github.com/matmair/django-error-report-2
 Author: M Hassan Siddiqui
 Author-email: mhassan.eeng@gmail.com
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `django-error-report-2-0.4.0a1/django_error_report_2.egg-info/SOURCES.txt` & `django-error-report-2-0.4.1/django_error_report_2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-error-report-2-0.4.0a1/error_report/admin.py` & `django-error-report-2-0.4.1/error_report/admin.py`

 * *Files identical despite different names*

### Comparing `django-error-report-2-0.4.0a1/error_report/middleware.py` & `django-error-report-2-0.4.1/error_report/middleware.py`

 * *Files identical despite different names*

### Comparing `django-error-report-2-0.4.0a1/error_report/migrations/0001_initial.py` & `django-error-report-2-0.4.1/error_report/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-error-report-2-0.4.0a1/error_report/models.py` & `django-error-report-2-0.4.1/error_report/models.py`

 * *Files identical despite different names*

### Comparing `django-error-report-2-0.4.0a1/setup.py` & `django-error-report-2-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,9 +33,9 @@
     ],
     packages=find_packages(exclude=['build', 'dist', 'django_error_report.egg-info']),
     zip_safe=False,
     license="BSD License",
     install_requires=[
         'Django>=1.7'
     ],
-    version='0.4.0a1',
+    version='0.4.1',
 )
```

