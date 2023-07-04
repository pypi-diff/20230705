# Comparing `tmp/django-error-report-2-0.4.0a0.tar.gz` & `tmp/django-error-report-2-0.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-error-report-2-0.4.0a0.tar", last modified: Tue Jul  4 21:33:38 2023, max compression
+gzip compressed data, was "django-error-report-2-0.4.0a1.tar", last modified: Tue Jul  4 22:00:05 2023, max compression
```

## Comparing `django-error-report-2-0.4.0a0.tar` & `django-error-report-2-0.4.0a1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-04 21:33:38.346313 django-error-report-2-0.4.0a0/
--rw-r--r--   0 matmair    (501) staff       (20)     1086 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a0/LICENSE.txt
--rw-r--r--   0 matmair    (501) staff       (20)       37 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a0/MANIFEST.in
--rw-r--r--   0 matmair    (501) staff       (20)     2155 2023-07-04 21:33:38.346437 django-error-report-2-0.4.0a0/PKG-INFO
--rw-r--r--   0 matmair    (501) staff       (20)     1567 2023-07-04 21:07:36.000000 django-error-report-2-0.4.0a0/README.md
-drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-04 21:33:38.343449 django-error-report-2-0.4.0a0/django_error_report_2.egg-info/
--rw-r--r--   0 matmair    (501) staff       (20)     2155 2023-07-04 21:33:38.000000 django-error-report-2-0.4.0a0/django_error_report_2.egg-info/PKG-INFO
--rw-r--r--   0 matmair    (501) staff       (20)      582 2023-07-04 21:33:38.000000 django-error-report-2-0.4.0a0/django_error_report_2.egg-info/SOURCES.txt
--rw-r--r--   0 matmair    (501) staff       (20)        1 2023-07-04 21:33:38.000000 django-error-report-2-0.4.0a0/django_error_report_2.egg-info/dependency_links.txt
--rw-r--r--   0 matmair    (501) staff       (20)        1 2023-07-04 21:03:03.000000 django-error-report-2-0.4.0a0/django_error_report_2.egg-info/not-zip-safe
--rw-r--r--   0 matmair    (501) staff       (20)       12 2023-07-04 21:33:38.000000 django-error-report-2-0.4.0a0/django_error_report_2.egg-info/requires.txt
--rw-r--r--   0 matmair    (501) staff       (20)       13 2023-07-04 21:33:38.000000 django-error-report-2-0.4.0a0/django_error_report_2.egg-info/top_level.txt
-drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-04 21:33:38.345695 django-error-report-2-0.4.0a0/error_report/
--rw-r--r--   0 matmair    (501) staff       (20)        0 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a0/error_report/__init__.py
--rw-r--r--   0 matmair    (501) staff       (20)      853 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a0/error_report/admin.py
--rw-r--r--   0 matmair    (501) staff       (20)      180 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a0/error_report/apps.py
--rw-r--r--   0 matmair    (501) staff       (20)     1050 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a0/error_report/middleware.py
-drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-04 21:33:38.346164 django-error-report-2-0.4.0a0/error_report/migrations/
--rw-r--r--   0 matmair    (501) staff       (20)     1131 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a0/error_report/migrations/0001_initial.py
--rw-r--r--   0 matmair    (501) staff       (20)        0 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a0/error_report/migrations/__init__.py
--rw-r--r--   0 matmair    (501) staff       (20)     1750 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a0/error_report/models.py
--rw-r--r--   0 matmair    (501) staff       (20)      105 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a0/error_report/settings.py
--rw-r--r--   0 matmair    (501) staff       (20)      306 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a0/error_report/urls.py
--rw-r--r--   0 matmair    (501) staff       (20)      395 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a0/error_report/views.py
--rw-r--r--   0 matmair    (501) staff       (20)      120 2023-07-04 21:33:38.346747 django-error-report-2-0.4.0a0/setup.cfg
--rw-r--r--   0 matmair    (501) staff       (20)     1163 2023-07-04 21:33:26.000000 django-error-report-2-0.4.0a0/setup.py
+drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-04 22:00:05.199095 django-error-report-2-0.4.0a1/
+-rw-r--r--   0 matmair    (501) staff       (20)     1086 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/LICENSE.txt
+-rw-r--r--   0 matmair    (501) staff       (20)       37 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/MANIFEST.in
+-rw-r--r--   0 matmair    (501) staff       (20)     2155 2023-07-04 22:00:05.198884 django-error-report-2-0.4.0a1/PKG-INFO
+-rw-r--r--   0 matmair    (501) staff       (20)     1567 2023-07-04 21:07:36.000000 django-error-report-2-0.4.0a1/README.md
+drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-04 22:00:05.193822 django-error-report-2-0.4.0a1/django_error_report_2.egg-info/
+-rw-r--r--   0 matmair    (501) staff       (20)     2155 2023-07-04 22:00:05.000000 django-error-report-2-0.4.0a1/django_error_report_2.egg-info/PKG-INFO
+-rw-r--r--   0 matmair    (501) staff       (20)      572 2023-07-04 22:00:05.000000 django-error-report-2-0.4.0a1/django_error_report_2.egg-info/SOURCES.txt
+-rw-r--r--   0 matmair    (501) staff       (20)        1 2023-07-04 22:00:05.000000 django-error-report-2-0.4.0a1/django_error_report_2.egg-info/dependency_links.txt
+-rw-r--r--   0 matmair    (501) staff       (20)        1 2023-07-04 21:03:03.000000 django-error-report-2-0.4.0a1/django_error_report_2.egg-info/not-zip-safe
+-rw-r--r--   0 matmair    (501) staff       (20)       12 2023-07-04 22:00:05.000000 django-error-report-2-0.4.0a1/django_error_report_2.egg-info/requires.txt
+-rw-r--r--   0 matmair    (501) staff       (20)       13 2023-07-04 22:00:05.000000 django-error-report-2-0.4.0a1/django_error_report_2.egg-info/top_level.txt
+drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-04 22:00:05.196260 django-error-report-2-0.4.0a1/error_report/
+-rw-r--r--   0 matmair    (501) staff       (20)        0 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/error_report/__init__.py
+-rw-r--r--   0 matmair    (501) staff       (20)      955 2023-07-04 21:59:36.000000 django-error-report-2-0.4.0a1/error_report/admin.py
+-rw-r--r--   0 matmair    (501) staff       (20)      180 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/error_report/apps.py
+-rw-r--r--   0 matmair    (501) staff       (20)     1050 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/error_report/middleware.py
+drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-04 22:00:05.198595 django-error-report-2-0.4.0a1/error_report/migrations/
+-rw-r--r--   0 matmair    (501) staff       (20)     1131 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/error_report/migrations/0001_initial.py
+-rw-r--r--   0 matmair    (501) staff       (20)        0 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/error_report/migrations/__init__.py
+-rw-r--r--   0 matmair    (501) staff       (20)     1750 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/error_report/models.py
+-rw-r--r--   0 matmair    (501) staff       (20)      105 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/error_report/settings.py
+-rw-r--r--   0 matmair    (501) staff       (20)      306 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/error_report/urls.py
+-rw-r--r--   0 matmair    (501) staff       (20)      395 2023-07-04 20:58:50.000000 django-error-report-2-0.4.0a1/error_report/views.py
+-rw-r--r--   0 matmair    (501) staff       (20)       38 2023-07-04 22:00:05.199156 django-error-report-2-0.4.0a1/setup.cfg
+-rw-r--r--   0 matmair    (501) staff       (20)     1163 2023-07-04 21:53:56.000000 django-error-report-2-0.4.0a1/setup.py
```

### Comparing `django-error-report-2-0.4.0a0/LICENSE.txt` & `django-error-report-2-0.4.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-error-report-2-0.4.0a0/PKG-INFO` & `django-error-report-2-0.4.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-error-report-2
-Version: 0.4.0a0
+Version: 0.4.0a1
 Summary: View Django Error Report in Django Admin
 Home-page: https://github.com/matmair/django-error-report-2
 Author: M Hassan Siddiqui
 Author-email: mhassan.eeng@gmail.com
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `django-error-report-2-0.4.0a0/README.md` & `django-error-report-2-0.4.0a1/README.md`

 * *Files identical despite different names*

### Comparing `django-error-report-2-0.4.0a0/django_error_report_2.egg-info/PKG-INFO` & `django-error-report-2-0.4.0a1/django_error_report_2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-error-report-2
-Version: 0.4.0a0
+Version: 0.4.0a1
 Summary: View Django Error Report in Django Admin
 Home-page: https://github.com/matmair/django-error-report-2
 Author: M Hassan Siddiqui
 Author-email: mhassan.eeng@gmail.com
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `django-error-report-2-0.4.0a0/django_error_report_2.egg-info/SOURCES.txt` & `django-error-report-2-0.4.0a1/django_error_report_2.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE.txt
 MANIFEST.in
 README.md
-setup.cfg
 setup.py
 django_error_report_2.egg-info/PKG-INFO
 django_error_report_2.egg-info/SOURCES.txt
 django_error_report_2.egg-info/dependency_links.txt
 django_error_report_2.egg-info/not-zip-safe
 django_error_report_2.egg-info/requires.txt
 django_error_report_2.egg-info/top_level.txt
```

### Comparing `django-error-report-2-0.4.0a0/error_report/middleware.py` & `django-error-report-2-0.4.0a1/error_report/middleware.py`

 * *Files identical despite different names*

### Comparing `django-error-report-2-0.4.0a0/error_report/migrations/0001_initial.py` & `django-error-report-2-0.4.0a1/error_report/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-error-report-2-0.4.0a0/error_report/models.py` & `django-error-report-2-0.4.0a1/error_report/models.py`

 * *Files identical despite different names*

### Comparing `django-error-report-2-0.4.0a0/setup.py` & `django-error-report-2-0.4.0a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,9 +33,9 @@
     ],
     packages=find_packages(exclude=['build', 'dist', 'django_error_report.egg-info']),
     zip_safe=False,
     license="BSD License",
     install_requires=[
         'Django>=1.7'
     ],
-    version='0.4.0a0',
+    version='0.4.0a1',
 )
```

