# Comparing `tmp/zibanu-django-logging-1.0.0.tar.gz` & `tmp/zibanu-django-logging-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zibanu-django-logging-1.0.0.tar", last modified: Wed Jul  5 12:31:10 2023, max compression
+gzip compressed data, was "zibanu-django-logging-1.0.1.tar", last modified: Wed Jul  5 12:37:08 2023, max compression
```

## Comparing `zibanu-django-logging-1.0.0.tar` & `zibanu-django-logging-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,38 @@
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:31:10.374578 zibanu-django-logging-1.0.0/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-logging-1.0.0/LICENSE
--rw-rw-r--   0 macercha  (1000) macercha  (1000)       62 2023-06-28 01:21:25.000000 zibanu-django-logging-1.0.0/MANIFEST.in
--rw-r--r--   0 macercha  (1000) macercha  (1000)    41393 2023-07-05 12:31:10.374578 zibanu-django-logging-1.0.0/PKG-INFO
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      172 2023-06-28 01:21:38.000000 zibanu-django-logging-1.0.0/README.md
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      923 2023-07-05 12:30:53.000000 zibanu-django-logging-1.0.0/pyproject.toml
--rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-07-05 12:31:10.374578 zibanu-django-logging-1.0.0/setup.cfg
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:31:10.365578 zibanu-django-logging-1.0.0/zibanu/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:31:10.368578 zibanu-django-logging-1.0.0/zibanu/logging/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-03-16 14:08:34.000000 zibanu-django-logging-1.0.0/zibanu/logging/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      919 2023-03-31 15:46:10.000000 zibanu-django-logging-1.0.0/zibanu/logging/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:31:10.369578 zibanu-django-logging-1.0.0/zibanu/logging/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 20:39:57.000000 zibanu-django-logging-1.0.0/zibanu/logging/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:31:10.370578 zibanu-django-logging-1.0.0/zibanu/logging/lib/events/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-logging-1.0.0/zibanu/logging/lib/events/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1016 2023-05-13 19:57:25.000000 zibanu-django-logging-1.0.0/zibanu/logging/lib/events/on_change_password.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1243 2023-03-31 15:46:10.000000 zibanu-django-logging-1.0.0/zibanu/logging/lib/events/on_login.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      975 2023-03-31 15:46:10.000000 zibanu-django-logging-1.0.0/zibanu/logging/lib/events/on_send_mail.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:31:10.371578 zibanu-django-logging-1.0.0/zibanu/logging/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:05:35.000000 zibanu-django-logging-1.0.0/zibanu/logging/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      452 2023-05-13 17:50:17.000000 zibanu-django-logging-1.0.0/zibanu/logging/lib/signals.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:31:10.372578 zibanu-django-logging-1.0.0/zibanu/logging/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1501 2023-03-15 21:32:53.000000 zibanu-django-logging-1.0.0/zibanu/logging/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1143 2023-03-31 15:46:10.000000 zibanu-django-logging-1.0.0/zibanu/logging/migrations/0002_maillog.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:33:26.000000 zibanu-django-logging-1.0.0/zibanu/logging/migrations/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1946 2023-03-31 15:46:10.000000 zibanu-django-logging-1.0.0/zibanu/logging/models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:31:10.373578 zibanu-django-logging-1.0.0/zibanu_django_logging.egg-info/
--rw-r--r--   0 macercha  (1000) macercha  (1000)    41393 2023-07-05 12:31:10.000000 zibanu-django-logging-1.0.0/zibanu_django_logging.egg-info/PKG-INFO
--rw-r--r--   0 macercha  (1000) macercha  (1000)      732 2023-07-05 12:31:10.000000 zibanu-django-logging-1.0.0/zibanu_django_logging.egg-info/SOURCES.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-07-05 12:31:10.000000 zibanu-django-logging-1.0.0/zibanu_django_logging.egg-info/dependency_links.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       83 2023-07-05 12:31:10.000000 zibanu-django-logging-1.0.0/zibanu_django_logging.egg-info/requires.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2023-07-05 12:31:10.000000 zibanu-django-logging-1.0.0/zibanu_django_logging.egg-info/top_level.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:37:08.990510 zibanu-django-logging-1.0.1/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-logging-1.0.1/LICENSE
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)       62 2023-06-28 01:21:25.000000 zibanu-django-logging-1.0.1/MANIFEST.in
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    41393 2023-07-05 12:37:08.989510 zibanu-django-logging-1.0.1/PKG-INFO
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      172 2023-06-28 01:21:38.000000 zibanu-django-logging-1.0.1/README.md
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      923 2023-07-05 12:36:11.000000 zibanu-django-logging-1.0.1/pyproject.toml
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-07-05 12:37:08.990510 zibanu-django-logging-1.0.1/setup.cfg
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:37:08.981510 zibanu-django-logging-1.0.1/zibanu/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:37:08.981510 zibanu-django-logging-1.0.1/zibanu/django/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:37:08.983510 zibanu-django-logging-1.0.1/zibanu/django/logging/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-03-16 14:08:34.000000 zibanu-django-logging-1.0.1/zibanu/django/logging/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      919 2023-03-31 15:46:10.000000 zibanu-django-logging-1.0.1/zibanu/django/logging/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:37:08.983510 zibanu-django-logging-1.0.1/zibanu/django/logging/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 20:39:57.000000 zibanu-django-logging-1.0.1/zibanu/django/logging/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:37:08.984510 zibanu-django-logging-1.0.1/zibanu/django/logging/lib/events/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-logging-1.0.1/zibanu/django/logging/lib/events/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1016 2023-05-13 19:57:25.000000 zibanu-django-logging-1.0.1/zibanu/django/logging/lib/events/on_change_password.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1243 2023-03-31 15:46:10.000000 zibanu-django-logging-1.0.1/zibanu/django/logging/lib/events/on_login.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      975 2023-03-31 15:46:10.000000 zibanu-django-logging-1.0.1/zibanu/django/logging/lib/events/on_send_mail.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:37:08.984510 zibanu-django-logging-1.0.1/zibanu/django/logging/lib/managers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:05:35.000000 zibanu-django-logging-1.0.1/zibanu/django/logging/lib/managers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      452 2023-05-13 17:50:17.000000 zibanu-django-logging-1.0.1/zibanu/django/logging/lib/signals.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:37:08.982510 zibanu-django-logging-1.0.1/zibanu/django/logging/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:37:08.982510 zibanu-django-logging-1.0.1/zibanu/django/logging/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:37:08.985510 zibanu-django-logging-1.0.1/zibanu/django/logging/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-logging-1.0.1/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1185 2023-03-31 15:46:10.000000 zibanu-django-logging-1.0.1/zibanu/django/logging/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:37:08.985510 zibanu-django-logging-1.0.1/zibanu/django/logging/migrations/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1501 2023-03-15 21:32:53.000000 zibanu-django-logging-1.0.1/zibanu/django/logging/migrations/0001_initial.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1143 2023-03-31 15:46:10.000000 zibanu-django-logging-1.0.1/zibanu/django/logging/migrations/0002_maillog.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:33:26.000000 zibanu-django-logging-1.0.1/zibanu/django/logging/migrations/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1946 2023-03-31 15:46:10.000000 zibanu-django-logging-1.0.1/zibanu/django/logging/models.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:37:08.986510 zibanu-django-logging-1.0.1/zibanu_django_logging.egg-info/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    41393 2023-07-05 12:37:08.000000 zibanu-django-logging-1.0.1/zibanu_django_logging.egg-info/PKG-INFO
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      931 2023-07-05 12:37:08.000000 zibanu-django-logging-1.0.1/zibanu_django_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-07-05 12:37:08.000000 zibanu-django-logging-1.0.1/zibanu_django_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       83 2023-07-05 12:37:08.000000 zibanu-django-logging-1.0.1/zibanu_django_logging.egg-info/requires.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2023-07-05 12:37:08.000000 zibanu-django-logging-1.0.1/zibanu_django_logging.egg-info/top_level.txt
```

### Comparing `zibanu-django-logging-1.0.0/LICENSE` & `zibanu-django-logging-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zibanu-django-logging-1.0.0/PKG-INFO` & `zibanu-django-logging-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibanu-django-logging
-Version: 1.0.0
+Version: 1.0.1
 Summary: Zibanu logging library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `zibanu-django-logging-1.0.0/pyproject.toml` & `zibanu-django-logging-1.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "zibanu-django-logging"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     {name="Mario Cerón", email="mario.ceron@cqinversiones.co"}
 ]
 description = "Zibanu logging library for django projects"
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
```

### Comparing `zibanu-django-logging-1.0.0/zibanu/logging/apps.py` & `zibanu-django-logging-1.0.1/zibanu/django/logging/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-logging-1.0.0/zibanu/logging/lib/events/__init__.py` & `zibanu-django-logging-1.0.1/zibanu/django/logging/lib/events/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-logging-1.0.0/zibanu/logging/lib/events/on_change_password.py` & `zibanu-django-logging-1.0.1/zibanu/django/logging/lib/events/on_change_password.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-logging-1.0.0/zibanu/logging/lib/events/on_login.py` & `zibanu-django-logging-1.0.1/zibanu/django/logging/lib/events/on_login.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-logging-1.0.0/zibanu/logging/lib/events/on_send_mail.py` & `zibanu-django-logging-1.0.1/zibanu/django/logging/lib/events/on_send_mail.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-logging-1.0.0/zibanu/logging/migrations/0001_initial.py` & `zibanu-django-logging-1.0.1/zibanu/django/logging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-logging-1.0.0/zibanu/logging/migrations/0002_maillog.py` & `zibanu-django-logging-1.0.1/zibanu/django/logging/migrations/0002_maillog.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-logging-1.0.0/zibanu/logging/models.py` & `zibanu-django-logging-1.0.1/zibanu/django/logging/models.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-logging-1.0.0/zibanu_django_logging.egg-info/PKG-INFO` & `zibanu-django-logging-1.0.1/zibanu_django_logging.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibanu-django-logging
-Version: 1.0.0
+Version: 1.0.1
 Summary: Zibanu logging library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `zibanu-django-logging-1.0.0/zibanu_django_logging.egg-info/SOURCES.txt` & `zibanu-django-logging-1.0.1/zibanu_django_logging.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-zibanu/logging/__init__.py
-zibanu/logging/apps.py
-zibanu/logging/models.py
-zibanu/logging/lib/__init__.py
-zibanu/logging/lib/signals.py
-zibanu/logging/lib/events/__init__.py
-zibanu/logging/lib/events/on_change_password.py
-zibanu/logging/lib/events/on_login.py
-zibanu/logging/lib/events/on_send_mail.py
-zibanu/logging/lib/managers/__init__.py
-zibanu/logging/migrations/0001_initial.py
-zibanu/logging/migrations/0002_maillog.py
-zibanu/logging/migrations/__init__.py
+zibanu/django/logging/__init__.py
+zibanu/django/logging/apps.py
+zibanu/django/logging/models.py
+zibanu/django/logging/lib/__init__.py
+zibanu/django/logging/lib/signals.py
+zibanu/django/logging/lib/events/__init__.py
+zibanu/django/logging/lib/events/on_change_password.py
+zibanu/django/logging/lib/events/on_login.py
+zibanu/django/logging/lib/events/on_send_mail.py
+zibanu/django/logging/lib/managers/__init__.py
+zibanu/django/logging/locale/es/LC_MESSAGES/django.mo
+zibanu/django/logging/locale/es/LC_MESSAGES/django.po
+zibanu/django/logging/migrations/0001_initial.py
+zibanu/django/logging/migrations/0002_maillog.py
+zibanu/django/logging/migrations/__init__.py
 zibanu_django_logging.egg-info/PKG-INFO
 zibanu_django_logging.egg-info/SOURCES.txt
 zibanu_django_logging.egg-info/dependency_links.txt
 zibanu_django_logging.egg-info/requires.txt
 zibanu_django_logging.egg-info/top_level.txt
```

