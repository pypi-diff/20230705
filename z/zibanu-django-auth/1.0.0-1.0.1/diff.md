# Comparing `tmp/zibanu-django-auth-1.0.0.tar.gz` & `tmp/zibanu-django-auth-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zibanu-django-auth-1.0.0.tar", last modified: Wed Jun 28 01:11:09 2023, max compression
+gzip compressed data, was "zibanu-django-auth-1.0.1.tar", last modified: Wed Jul  5 12:49:24 2023, max compression
```

## Comparing `zibanu-django-auth-1.0.0.tar` & `zibanu-django-auth-1.0.1.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-28 01:11:09.256618 zibanu-django-auth-1.0.0/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-auth-1.0.0/LICENSE
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      109 2023-06-19 16:17:43.000000 zibanu-django-auth-1.0.0/MANIFEST.in
--rw-r--r--   0 macercha  (1000) macercha  (1000)    41389 2023-06-28 01:11:09.256618 zibanu-django-auth-1.0.0/PKG-INFO
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      179 2023-06-19 19:19:54.000000 zibanu-django-auth-1.0.0/README.md
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      905 2023-06-20 19:04:07.000000 zibanu-django-auth-1.0.0/pyproject.toml
--rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-06-28 01:11:09.257618 zibanu-django-auth-1.0.0/setup.cfg
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-28 01:11:09.236618 zibanu-django-auth-1.0.0/zibanu/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-28 01:11:09.236618 zibanu-django-auth-1.0.0/zibanu/django/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-28 01:11:09.240618 zibanu-django-auth-1.0.0/zibanu/django/auth/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:20:31.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-28 01:11:09.240618 zibanu-django-auth-1.0.0/zibanu/django/auth/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:25:30.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/api/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-28 01:11:09.243618 zibanu-django-auth-1.0.0/zibanu/django/auth/api/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      787 2023-06-19 16:01:54.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/api/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      533 2023-06-19 15:57:29.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/api/serializers/group.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      549 2023-06-19 16:00:06.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/api/serializers/permission.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      749 2023-04-27 12:00:18.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/api/serializers/profile.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3051 2023-04-27 12:17:39.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/api/serializers/token.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3944 2023-06-07 19:44:45.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/api/serializers/user.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-28 01:11:09.246618 zibanu-django-auth-1.0.0/zibanu/django/auth/api/services/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      553 2023-06-19 19:50:50.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/api/services/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1104 2023-06-19 16:01:54.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/api/services/group.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      954 2023-06-19 16:05:31.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/api/services/permission.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2012 2023-06-19 20:05:14.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/api/services/profile.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    13346 2023-06-20 15:59:00.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/api/services/user.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1245 2023-05-17 01:05:01.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-28 01:11:09.249618 zibanu-django-auth-1.0.0/zibanu/django/auth/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:32:01.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-28 01:11:09.249618 zibanu-django-auth-1.0.0/zibanu/django/auth/lib/choices/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:48:01.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/lib/choices/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-28 01:11:09.250618 zibanu-django-auth-1.0.0/zibanu/django/auth/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      314 2023-05-25 18:23:00.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1396 2023-05-17 00:58:35.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/lib/signal_events.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      412 2023-05-13 17:53:49.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/lib/signals.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      916 2023-06-19 17:31:05.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/lib/utils.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-28 01:11:09.237618 zibanu-django-auth-1.0.0/zibanu/django/auth/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-28 01:11:09.237618 zibanu-django-auth-1.0.0/zibanu/django/auth/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-28 01:11:09.250618 zibanu-django-auth-1.0.0/zibanu/django/auth/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2172 2023-06-19 20:43:36.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3203 2023-06-19 20:43:24.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-28 01:11:09.252618 zibanu-django-auth-1.0.0/zibanu/django/auth/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    24474 2023-04-11 22:39:55.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    23375 2023-04-27 14:50:20.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/migrations/0002_alter_userprofile_timezone.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:31:28.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/migrations/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1957 2023-06-19 15:42:12.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-28 01:11:09.255618 zibanu-django-auth-1.0.0/zibanu/django/auth/templates/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      487 2023-05-23 16:11:28.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/templates/change_password.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      324 2023-05-22 17:32:26.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/templates/change_password.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-05-13 16:44:16.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/templates/request-code.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-05-13 16:41:48.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/templates/request-code.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      559 2023-05-22 17:30:07.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/templates/request_password.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      346 2023-05-13 16:55:01.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/templates/request_password.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1701 2023-06-19 20:28:16.000000 zibanu-django-auth-1.0.0/zibanu/django/auth/urls.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-28 01:11:09.256618 zibanu-django-auth-1.0.0/zibanu_django_auth.egg-info/
--rw-r--r--   0 macercha  (1000) macercha  (1000)    41389 2023-06-28 01:11:09.000000 zibanu-django-auth-1.0.0/zibanu_django_auth.egg-info/PKG-INFO
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1665 2023-06-28 01:11:09.000000 zibanu-django-auth-1.0.0/zibanu_django_auth.egg-info/SOURCES.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-06-28 01:11:09.000000 zibanu-django-auth-1.0.0/zibanu_django_auth.egg-info/dependency_links.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       76 2023-06-28 01:11:09.000000 zibanu-django-auth-1.0.0/zibanu_django_auth.egg-info/requires.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2023-06-28 01:11:09.000000 zibanu-django-auth-1.0.0/zibanu_django_auth.egg-info/top_level.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:49:24.952982 zibanu-django-auth-1.0.1/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-auth-1.0.1/LICENSE
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      109 2023-06-19 16:17:43.000000 zibanu-django-auth-1.0.1/MANIFEST.in
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    41404 2023-07-05 12:49:24.952982 zibanu-django-auth-1.0.1/PKG-INFO
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      179 2023-06-19 19:19:54.000000 zibanu-django-auth-1.0.1/README.md
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      920 2023-07-05 12:48:27.000000 zibanu-django-auth-1.0.1/pyproject.toml
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-07-05 12:49:24.953982 zibanu-django-auth-1.0.1/setup.cfg
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:49:24.940982 zibanu-django-auth-1.0.1/zibanu/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:49:24.940982 zibanu-django-auth-1.0.1/zibanu/django/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:49:24.943982 zibanu-django-auth-1.0.1/zibanu/django/auth/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:20:31.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:49:24.943982 zibanu-django-auth-1.0.1/zibanu/django/auth/api/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:25:30.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/api/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:49:24.944982 zibanu-django-auth-1.0.1/zibanu/django/auth/api/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      787 2023-06-19 16:01:54.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/api/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      533 2023-06-19 15:57:29.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/api/serializers/group.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      549 2023-06-19 16:00:06.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/api/serializers/permission.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      749 2023-04-27 12:00:18.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/api/serializers/profile.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3051 2023-04-27 12:17:39.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/api/serializers/token.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3944 2023-06-07 19:44:45.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/api/serializers/user.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:49:24.948982 zibanu-django-auth-1.0.1/zibanu/django/auth/api/services/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      553 2023-06-19 19:50:50.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/api/services/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1104 2023-06-19 16:01:54.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/api/services/group.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      954 2023-06-19 16:05:31.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/api/services/permission.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2012 2023-06-19 20:05:14.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/api/services/profile.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    13346 2023-06-20 15:59:00.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/api/services/user.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1245 2023-05-17 01:05:01.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:49:24.948982 zibanu-django-auth-1.0.1/zibanu/django/auth/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:32:01.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:49:24.949982 zibanu-django-auth-1.0.1/zibanu/django/auth/lib/choices/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:48:01.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/lib/choices/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:49:24.949982 zibanu-django-auth-1.0.1/zibanu/django/auth/lib/managers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      314 2023-05-25 18:23:00.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/lib/managers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1396 2023-05-17 00:58:35.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/lib/signal_events.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      412 2023-05-13 17:53:49.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/lib/signals.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      916 2023-06-19 17:31:05.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/lib/utils.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:49:24.941982 zibanu-django-auth-1.0.1/zibanu/django/auth/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:49:24.941982 zibanu-django-auth-1.0.1/zibanu/django/auth/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:49:24.949982 zibanu-django-auth-1.0.1/zibanu/django/auth/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2172 2023-06-19 20:43:36.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3203 2023-06-19 20:43:24.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:49:24.950982 zibanu-django-auth-1.0.1/zibanu/django/auth/migrations/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    24474 2023-04-11 22:39:55.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/migrations/0001_initial.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    23375 2023-04-27 14:50:20.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/migrations/0002_alter_userprofile_timezone.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    23394 2023-07-05 12:46:29.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/migrations/0003_alter_userprofile_timezone.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:31:28.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/migrations/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1957 2023-06-19 15:42:12.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/models.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:49:24.951982 zibanu-django-auth-1.0.1/zibanu/django/auth/templates/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      487 2023-05-23 16:11:28.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/templates/change_password.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      324 2023-05-22 17:32:26.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/templates/change_password.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-05-13 16:44:16.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/templates/request-code.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-05-13 16:41:48.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/templates/request-code.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      559 2023-05-22 17:30:07.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/templates/request_password.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      346 2023-05-13 16:55:01.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/templates/request_password.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1701 2023-06-19 20:28:16.000000 zibanu-django-auth-1.0.1/zibanu/django/auth/urls.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:49:24.952982 zibanu-django-auth-1.0.1/zibanu_django_auth.egg-info/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    41404 2023-07-05 12:49:24.000000 zibanu-django-auth-1.0.1/zibanu_django_auth.egg-info/PKG-INFO
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1730 2023-07-05 12:49:24.000000 zibanu-django-auth-1.0.1/zibanu_django_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-07-05 12:49:24.000000 zibanu-django-auth-1.0.1/zibanu_django_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       76 2023-07-05 12:49:24.000000 zibanu-django-auth-1.0.1/zibanu_django_auth.egg-info/requires.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2023-07-05 12:49:24.000000 zibanu-django-auth-1.0.1/zibanu_django_auth.egg-info/top_level.txt
```

### Comparing `zibanu-django-auth-1.0.0/LICENSE` & `zibanu-django-auth-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/PKG-INFO` & `zibanu-django-auth-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: zibanu-django-auth
-Version: 1.0.0
-Summary: Zibanu library for django projects
+Version: 1.0.1
+Summary: Zibanu authentication library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `zibanu-django-auth-1.0.0/pyproject.toml` & `zibanu-django-auth-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "zibanu-django-auth"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     {name="Mario Cerón", email="mario.ceron@cqinversiones.co"}
 ]
-description = "Zibanu library for django projects"
+description = "Zibanu authentication library for django projects"
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3.9",
     "Development Status :: 5 - Production/Stable",
```

### Comparing `zibanu-django-auth-1.0.0/zibanu/django/auth/api/serializers/__init__.py` & `zibanu-django-auth-1.0.1/zibanu/django/auth/api/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/zibanu/django/auth/api/serializers/group.py` & `zibanu-django-auth-1.0.1/zibanu/django/auth/api/serializers/group.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/zibanu/django/auth/api/serializers/permission.py` & `zibanu-django-auth-1.0.1/zibanu/django/auth/api/serializers/permission.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/zibanu/django/auth/api/serializers/profile.py` & `zibanu-django-auth-1.0.1/zibanu/django/auth/api/serializers/profile.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/zibanu/django/auth/api/serializers/token.py` & `zibanu-django-auth-1.0.1/zibanu/django/auth/api/serializers/token.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/zibanu/django/auth/api/serializers/user.py` & `zibanu-django-auth-1.0.1/zibanu/django/auth/api/serializers/user.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/zibanu/django/auth/api/services/__init__.py` & `zibanu-django-auth-1.0.1/zibanu/django/auth/api/services/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/zibanu/django/auth/api/services/group.py` & `zibanu-django-auth-1.0.1/zibanu/django/auth/api/services/group.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/zibanu/django/auth/api/services/permission.py` & `zibanu-django-auth-1.0.1/zibanu/django/auth/api/services/permission.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/zibanu/django/auth/api/services/profile.py` & `zibanu-django-auth-1.0.1/zibanu/django/auth/api/services/profile.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/zibanu/django/auth/api/services/user.py` & `zibanu-django-auth-1.0.1/zibanu/django/auth/api/services/user.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/zibanu/django/auth/apps.py` & `zibanu-django-auth-1.0.1/zibanu/django/auth/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/zibanu/django/auth/lib/signal_events.py` & `zibanu-django-auth-1.0.1/zibanu/django/auth/lib/signal_events.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/zibanu/django/auth/lib/utils.py` & `zibanu-django-auth-1.0.1/zibanu/django/auth/lib/utils.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/zibanu/django/auth/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-auth-1.0.1/zibanu/django/auth/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/zibanu/django/auth/locale/es/LC_MESSAGES/django.po` & `zibanu-django-auth-1.0.1/zibanu/django/auth/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/zibanu/django/auth/migrations/0001_initial.py` & `zibanu-django-auth-1.0.1/zibanu/django/auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/zibanu/django/auth/migrations/0002_alter_userprofile_timezone.py` & `zibanu-django-auth-1.0.1/zibanu/django/auth/migrations/0002_alter_userprofile_timezone.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/zibanu/django/auth/models.py` & `zibanu-django-auth-1.0.1/zibanu/django/auth/models.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/zibanu/django/auth/templates/request_password.html` & `zibanu-django-auth-1.0.1/zibanu/django/auth/templates/request_password.html`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/zibanu/django/auth/urls.py` & `zibanu-django-auth-1.0.1/zibanu/django/auth/urls.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.0/zibanu_django_auth.egg-info/PKG-INFO` & `zibanu-django-auth-1.0.1/zibanu_django_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: zibanu-django-auth
-Version: 1.0.0
-Summary: Zibanu library for django projects
+Version: 1.0.1
+Summary: Zibanu authentication library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `zibanu-django-auth-1.0.0/zibanu_django_auth.egg-info/SOURCES.txt` & `zibanu-django-auth-1.0.1/zibanu_django_auth.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 zibanu/django/auth/lib/utils.py
 zibanu/django/auth/lib/choices/__init__.py
 zibanu/django/auth/lib/managers/__init__.py
 zibanu/django/auth/locale/es/LC_MESSAGES/django.mo
 zibanu/django/auth/locale/es/LC_MESSAGES/django.po
 zibanu/django/auth/migrations/0001_initial.py
 zibanu/django/auth/migrations/0002_alter_userprofile_timezone.py
+zibanu/django/auth/migrations/0003_alter_userprofile_timezone.py
 zibanu/django/auth/migrations/__init__.py
 zibanu/django/auth/templates/change_password.html
 zibanu/django/auth/templates/change_password.txt
 zibanu/django/auth/templates/request-code.html
 zibanu/django/auth/templates/request-code.txt
 zibanu/django/auth/templates/request_password.html
 zibanu/django/auth/templates/request_password.txt
```

