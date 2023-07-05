# Comparing `tmp/zibanu-django-1.2.0b1.tar.gz` & `tmp/zibanu-django-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zibanu-django-1.2.0b1.tar", last modified: Mon Jun 19 16:46:45 2023, max compression
+gzip compressed data, was "zibanu-django-1.2.1.tar", last modified: Wed Jul  5 12:29:41 2023, max compression
```

## Comparing `zibanu-django-1.2.0b1.tar` & `zibanu-django-1.2.1.tar`

### file list

```diff
@@ -1,102 +1,79 @@
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.539692 zibanu-django-1.2.0b1/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-1.2.0b1/LICENSE
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      208 2023-06-19 16:39:09.000000 zibanu-django-1.2.0b1/MANIFEST.in
--rw-r--r--   0 macercha  (1000) macercha  (1000)    41394 2023-06-19 16:46:45.539692 zibanu-django-1.2.0b1/PKG-INFO
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      179 2023-06-19 16:22:53.000000 zibanu-django-1.2.0b1/README.md
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      901 2023-06-19 16:46:30.000000 zibanu-django-1.2.0b1/pyproject.toml
--rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-06-19 16:46:45.539692 zibanu-django-1.2.0b1/setup.cfg
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.525692 zibanu-django-1.2.0b1/zibanu/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      623 2022-12-10 15:21:05.000000 zibanu-django-1.2.0b1/zibanu/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.526692 zibanu-django-1.2.0b1/zibanu/django/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-11 23:08:20.000000 zibanu-django-1.2.0b1/zibanu/django/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      895 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.526692 zibanu-django-1.2.0b1/zibanu/django/db/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 18:13:01.000000 zibanu-django-1.2.0b1/zibanu/django/db/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.526692 zibanu-django-1.2.0b1/zibanu/django/db/backends/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0b1/zibanu/django/db/backends/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.527692 zibanu-django-1.2.0b1/zibanu/django/db/backends/oracle/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0b1/zibanu/django/db/backends/oracle/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1158 2023-02-07 01:58:51.000000 zibanu-django-1.2.0b1/zibanu/django/db/backends/oracle/base.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.528692 zibanu-django-1.2.0b1/zibanu/django/db/models/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      766 2023-01-17 11:51:34.000000 zibanu-django-1.2.0b1/zibanu/django/db/models/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      931 2023-03-01 18:58:00.000000 zibanu-django-1.2.0b1/zibanu/django/db/models/dated_model.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1458 2023-03-03 23:10:34.000000 zibanu-django-1.2.0b1/zibanu/django/db/models/manager.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      738 2022-12-20 14:58:49.000000 zibanu-django-1.2.0b1/zibanu/django/db/models/model.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.522692 zibanu-django-1.2.0b1/zibanu/django/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.522692 zibanu-django-1.2.0b1/zibanu/django/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.528692 zibanu-django-1.2.0b1/zibanu/django/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2274 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3598 2023-04-27 15:33:39.000000 zibanu-django-1.2.0b1/zibanu/django/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.529692 zibanu-django-1.2.0b1/zibanu/django/logging/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-03-16 14:08:34.000000 zibanu-django-1.2.0b1/zibanu/django/logging/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      919 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/logging/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.529692 zibanu-django-1.2.0b1/zibanu/django/logging/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 20:39:57.000000 zibanu-django-1.2.0b1/zibanu/django/logging/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.530692 zibanu-django-1.2.0b1/zibanu/django/logging/lib/events/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/logging/lib/events/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1016 2023-05-13 19:57:25.000000 zibanu-django-1.2.0b1/zibanu/django/logging/lib/events/on_change_password.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1243 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/logging/lib/events/on_login.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      975 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/logging/lib/events/on_send_mail.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.530692 zibanu-django-1.2.0b1/zibanu/django/logging/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:05:35.000000 zibanu-django-1.2.0b1/zibanu/django/logging/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      452 2023-05-13 17:50:17.000000 zibanu-django-1.2.0b1/zibanu/django/logging/lib/signals.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.523692 zibanu-django-1.2.0b1/zibanu/django/logging/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.523692 zibanu-django-1.2.0b1/zibanu/django/logging/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.530692 zibanu-django-1.2.0b1/zibanu/django/logging/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1185 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/logging/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.531692 zibanu-django-1.2.0b1/zibanu/django/logging/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1501 2023-03-15 21:32:53.000000 zibanu-django-1.2.0b1/zibanu/django/logging/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1143 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/logging/migrations/0002_maillog.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:33:26.000000 zibanu-django-1.2.0b1/zibanu/django/logging/migrations/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1946 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/logging/models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.531692 zibanu-django-1.2.0b1/zibanu/django/rest_framework/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 12:39:27.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1650 2023-04-28 00:41:44.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/decorators.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.532692 zibanu-django-1.2.0b1/zibanu/django/rest_framework/exceptions/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      973 2022-12-20 02:49:47.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/exceptions/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2039 2023-04-27 15:30:28.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/exceptions/api_exception.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.532692 zibanu-django-1.2.0b1/zibanu/django/rest_framework/fields/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/fields/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1142 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/fields/current_user_default.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.533692 zibanu-django-1.2.0b1/zibanu/django/rest_framework/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1560 2022-12-20 10:51:58.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-02-27 20:11:57.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/serializers/fields.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      867 2022-12-14 09:18:30.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/serializers/model_serializer.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.533692 zibanu-django-1.2.0b1/zibanu/django/rest_framework/viewsets/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-02-13 14:05:54.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/viewsets/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    10487 2023-04-28 00:47:56.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/viewsets/model_viewset.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1332 2023-02-13 14:05:54.000000 zibanu-django-1.2.0b1/zibanu/django/rest_framework/viewsets/viewset.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.534692 zibanu-django-1.2.0b1/zibanu/django/template/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-01-28 17:50:45.000000 zibanu-django-1.2.0b1/zibanu/django/template/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      663 2023-01-28 20:32:11.000000 zibanu-django-1.2.0b1/zibanu/django/template/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.534692 zibanu-django-1.2.0b1/zibanu/django/template/context_processors/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      624 2023-01-29 02:00:01.000000 zibanu-django-1.2.0b1/zibanu/django/template/context_processors/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-01-29 02:00:01.000000 zibanu-django-1.2.0b1/zibanu/django/template/context_processors/full_static_uri.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2023-01-28 20:37:34.000000 zibanu-django-1.2.0b1/zibanu/django/template/context_processors/site.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.524692 zibanu-django-1.2.0b1/zibanu/django/template/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.524692 zibanu-django-1.2.0b1/zibanu/django/template/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.535692 zibanu-django-1.2.0b1/zibanu/django/template/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      519 2023-02-09 14:42:38.000000 zibanu-django-1.2.0b1/zibanu/django/template/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1022 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/template/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.536692 zibanu-django-1.2.0b1/zibanu/django/template/templatetags/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-07 23:57:31.000000 zibanu-django-1.2.0b1/zibanu/django/template/templatetags/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1539 2023-01-29 02:38:53.000000 zibanu-django-1.2.0b1/zibanu/django/template/templatetags/static_uri.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      666 2023-02-08 00:00:29.000000 zibanu-django-1.2.0b1/zibanu/django/template/templatetags/string_concat.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2009 2023-02-16 14:53:50.000000 zibanu-django-1.2.0b1/zibanu/django/template/templatetags/subtotal_dict.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1216 2023-02-08 15:25:53.000000 zibanu-django-1.2.0b1/zibanu/django/template/templatetags/sum_dict.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.537692 zibanu-django-1.2.0b1/zibanu/django/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      863 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3332 2023-04-28 21:35:15.000000 zibanu-django-1.2.0b1/zibanu/django/utils/code_generator.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1895 2023-02-26 20:02:32.000000 zibanu-django-1.2.0b1/zibanu/django/utils/date_time.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1163 2023-03-03 13:27:43.000000 zibanu-django-1.2.0b1/zibanu/django/utils/error_messages.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     5768 2023-05-23 00:00:08.000000 zibanu-django-1.2.0b1/zibanu/django/utils/mail.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      562 2023-03-31 15:46:10.000000 zibanu-django-1.2.0b1/zibanu/django/utils/request_utils.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1080 2023-05-13 15:24:32.000000 zibanu-django-1.2.0b1/zibanu/django/utils/user.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      699 2023-03-03 13:27:43.000000 zibanu-django-1.2.0b1/zibanu/django/utils/validate_cache_code.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 16:46:45.538692 zibanu-django-1.2.0b1/zibanu_django.egg-info/
--rw-r--r--   0 macercha  (1000) macercha  (1000)    41394 2023-06-19 16:46:45.000000 zibanu-django-1.2.0b1/zibanu_django.egg-info/PKG-INFO
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2836 2023-06-19 16:46:45.000000 zibanu-django-1.2.0b1/zibanu_django.egg-info/SOURCES.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-06-19 16:46:45.000000 zibanu-django-1.2.0b1/zibanu_django.egg-info/dependency_links.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       62 2023-06-19 16:46:45.000000 zibanu-django-1.2.0b1/zibanu_django.egg-info/requires.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2023-06-19 16:46:45.000000 zibanu-django-1.2.0b1/zibanu_django.egg-info/top_level.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.306333 zibanu-django-1.2.1/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-1.2.1/LICENSE
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      208 2023-06-19 16:39:09.000000 zibanu-django-1.2.1/MANIFEST.in
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    41379 2023-07-05 12:29:41.305333 zibanu-django-1.2.1/PKG-INFO
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      169 2023-06-19 19:19:54.000000 zibanu-django-1.2.1/README.md
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      891 2023-07-05 12:26:04.000000 zibanu-django-1.2.1/pyproject.toml
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-07-05 12:29:41.306333 zibanu-django-1.2.1/setup.cfg
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.281334 zibanu-django-1.2.1/zibanu/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      623 2022-12-10 15:21:05.000000 zibanu-django-1.2.1/zibanu/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.283334 zibanu-django-1.2.1/zibanu/django/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-11 23:08:20.000000 zibanu-django-1.2.1/zibanu/django/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      895 2023-03-31 15:46:10.000000 zibanu-django-1.2.1/zibanu/django/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.283334 zibanu-django-1.2.1/zibanu/django/db/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 18:13:01.000000 zibanu-django-1.2.1/zibanu/django/db/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.284334 zibanu-django-1.2.1/zibanu/django/db/backends/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.1/zibanu/django/db/backends/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.285334 zibanu-django-1.2.1/zibanu/django/db/backends/oracle/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.1/zibanu/django/db/backends/oracle/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1158 2023-02-07 01:58:51.000000 zibanu-django-1.2.1/zibanu/django/db/backends/oracle/base.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.287334 zibanu-django-1.2.1/zibanu/django/db/models/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      766 2023-01-17 11:51:34.000000 zibanu-django-1.2.1/zibanu/django/db/models/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      931 2023-03-01 18:58:00.000000 zibanu-django-1.2.1/zibanu/django/db/models/dated_model.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1458 2023-03-03 23:10:34.000000 zibanu-django-1.2.1/zibanu/django/db/models/manager.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      738 2022-12-20 14:58:49.000000 zibanu-django-1.2.1/zibanu/django/db/models/model.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.278334 zibanu-django-1.2.1/zibanu/django/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.278334 zibanu-django-1.2.1/zibanu/django/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.288334 zibanu-django-1.2.1/zibanu/django/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2274 2023-03-31 15:46:10.000000 zibanu-django-1.2.1/zibanu/django/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3598 2023-04-27 15:33:39.000000 zibanu-django-1.2.1/zibanu/django/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.289334 zibanu-django-1.2.1/zibanu/django/rest_framework/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 12:39:27.000000 zibanu-django-1.2.1/zibanu/django/rest_framework/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1650 2023-04-28 00:41:44.000000 zibanu-django-1.2.1/zibanu/django/rest_framework/decorators.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.290334 zibanu-django-1.2.1/zibanu/django/rest_framework/exceptions/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      973 2022-12-20 02:49:47.000000 zibanu-django-1.2.1/zibanu/django/rest_framework/exceptions/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2039 2023-04-27 15:30:28.000000 zibanu-django-1.2.1/zibanu/django/rest_framework/exceptions/api_exception.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.291334 zibanu-django-1.2.1/zibanu/django/rest_framework/fields/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-03-31 15:46:10.000000 zibanu-django-1.2.1/zibanu/django/rest_framework/fields/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1142 2023-03-31 15:46:10.000000 zibanu-django-1.2.1/zibanu/django/rest_framework/fields/current_user_default.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.292334 zibanu-django-1.2.1/zibanu/django/rest_framework/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1560 2022-12-20 10:51:58.000000 zibanu-django-1.2.1/zibanu/django/rest_framework/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-02-27 20:11:57.000000 zibanu-django-1.2.1/zibanu/django/rest_framework/serializers/fields.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      867 2022-12-14 09:18:30.000000 zibanu-django-1.2.1/zibanu/django/rest_framework/serializers/model_serializer.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.293334 zibanu-django-1.2.1/zibanu/django/rest_framework/viewsets/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-02-13 14:05:54.000000 zibanu-django-1.2.1/zibanu/django/rest_framework/viewsets/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    10487 2023-04-28 00:47:56.000000 zibanu-django-1.2.1/zibanu/django/rest_framework/viewsets/model_viewset.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1332 2023-02-13 14:05:54.000000 zibanu-django-1.2.1/zibanu/django/rest_framework/viewsets/viewset.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.294334 zibanu-django-1.2.1/zibanu/django/template/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-01-28 17:50:45.000000 zibanu-django-1.2.1/zibanu/django/template/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      663 2023-01-28 20:32:11.000000 zibanu-django-1.2.1/zibanu/django/template/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.296334 zibanu-django-1.2.1/zibanu/django/template/context_processors/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      624 2023-01-29 02:00:01.000000 zibanu-django-1.2.1/zibanu/django/template/context_processors/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-01-29 02:00:01.000000 zibanu-django-1.2.1/zibanu/django/template/context_processors/full_static_uri.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2023-01-28 20:37:34.000000 zibanu-django-1.2.1/zibanu/django/template/context_processors/site.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.279334 zibanu-django-1.2.1/zibanu/django/template/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.279334 zibanu-django-1.2.1/zibanu/django/template/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.297334 zibanu-django-1.2.1/zibanu/django/template/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      519 2023-02-09 14:42:38.000000 zibanu-django-1.2.1/zibanu/django/template/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1022 2023-03-31 15:46:10.000000 zibanu-django-1.2.1/zibanu/django/template/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.299333 zibanu-django-1.2.1/zibanu/django/template/templatetags/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-07 23:57:31.000000 zibanu-django-1.2.1/zibanu/django/template/templatetags/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1539 2023-01-29 02:38:53.000000 zibanu-django-1.2.1/zibanu/django/template/templatetags/static_uri.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      666 2023-02-08 00:00:29.000000 zibanu-django-1.2.1/zibanu/django/template/templatetags/string_concat.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2009 2023-02-16 14:53:50.000000 zibanu-django-1.2.1/zibanu/django/template/templatetags/subtotal_dict.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1216 2023-02-08 15:25:53.000000 zibanu-django-1.2.1/zibanu/django/template/templatetags/sum_dict.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.303333 zibanu-django-1.2.1/zibanu/django/utils/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      863 2023-03-31 15:46:10.000000 zibanu-django-1.2.1/zibanu/django/utils/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3332 2023-04-28 21:35:15.000000 zibanu-django-1.2.1/zibanu/django/utils/code_generator.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1895 2023-02-26 20:02:32.000000 zibanu-django-1.2.1/zibanu/django/utils/date_time.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1163 2023-03-03 13:27:43.000000 zibanu-django-1.2.1/zibanu/django/utils/error_messages.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     5768 2023-05-23 00:00:08.000000 zibanu-django-1.2.1/zibanu/django/utils/mail.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      562 2023-03-31 15:46:10.000000 zibanu-django-1.2.1/zibanu/django/utils/request_utils.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1250 2023-06-19 17:29:49.000000 zibanu-django-1.2.1/zibanu/django/utils/user.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      699 2023-03-03 13:27:43.000000 zibanu-django-1.2.1/zibanu/django/utils/validate_cache_code.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 12:29:41.305333 zibanu-django-1.2.1/zibanu_django.egg-info/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    41379 2023-07-05 12:29:41.000000 zibanu-django-1.2.1/zibanu_django.egg-info/PKG-INFO
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2173 2023-07-05 12:29:41.000000 zibanu-django-1.2.1/zibanu_django.egg-info/SOURCES.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-07-05 12:29:41.000000 zibanu-django-1.2.1/zibanu_django.egg-info/dependency_links.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       62 2023-07-05 12:29:41.000000 zibanu-django-1.2.1/zibanu_django.egg-info/requires.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2023-07-05 12:29:41.000000 zibanu-django-1.2.1/zibanu_django.egg-info/top_level.txt
```

### Comparing `zibanu-django-1.2.0b1/LICENSE` & `zibanu-django-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/PKG-INFO` & `zibanu-django-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: zibanu-django
-Version: 1.2.0b1
-Summary: Zibanu authentication library for django projects
+Version: 1.2.1
+Summary: Zibanu library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -676,24 +676,24 @@
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Keywords: django,zibanu,library,auth
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Zibanu Django Authentication Module
+# Zibanu Library for Django
 
 This package or library contains some functionalities commonly used in django projects and django rest_framework projects. 
 
 ## Django db
```

### Comparing `zibanu-django-1.2.0b1/pyproject.toml` & `zibanu-django-1.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,26 +3,26 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "zibanu-django"
-version = "1.2.0-beta.1"
+version = "1.2.1"
 authors = [
     {name="Mario Cerón", email="mario.ceron@cqinversiones.co"}
 ]
-description = "Zibanu authentication library for django projects"
+description = "Zibanu library for django projects"
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3.9",
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 5 - Production/Stable",
     "Framework :: Django",
     "Framework :: Django :: 4.1",
     "Environment :: Web Environment",
     "Operating System :: OS Independent",
     "Topic :: Internet :: WWW/HTTP"
 ]
 dependencies = [
```

### Comparing `zibanu-django-1.2.0b1/zibanu/__init__.py` & `zibanu-django-1.2.1/zibanu/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/apps.py` & `zibanu-django-1.2.1/zibanu/django/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/db/backends/oracle/base.py` & `zibanu-django-1.2.1/zibanu/django/db/backends/oracle/base.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/db/models/__init__.py` & `zibanu-django-1.2.1/zibanu/django/db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/db/models/dated_model.py` & `zibanu-django-1.2.1/zibanu/django/db/models/dated_model.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/db/models/manager.py` & `zibanu-django-1.2.1/zibanu/django/db/models/manager.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/db/models/model.py` & `zibanu-django-1.2.1/zibanu/django/db/models/model.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.2.1/zibanu/django/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.2.1/zibanu/django/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/logging/apps.py` & `zibanu-django-1.2.1/zibanu/django/template/apps.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,26 +2,18 @@
 
 #  Developed by CQ Inversiones SAS. Copyright ©. 2019 - 2023. All rights reserved.
 #  Desarrollado por CQ Inversiones SAS. Copyright ©. 2019 - 2023. Todos los derechos reservado
 
 # ****************************************************************
 # IDE:          PyCharm
 # Developed by: macercha
-# Date:         10/12/22 10:23 AM
+# Date:         28/01/23 15:31
 # Project:      CFHL Transactional Backend
 # Module Name:  apps
 # Description:
 # ****************************************************************
 from django.apps import AppConfig
-from django.conf import settings
-from django.utils.translation import gettext_lazy as _
 
 
-class ZbDjangoLogging(AppConfig):
-    default_auto_field = "django.db.models.AutoField"
-    name = "zibanu.django.logging"
-    verbose_name = _("Zibanu Logging")
-    label = "zb_logging"
-
-    def ready(self):
-        # Import events for signals
-        import zibanu.django.logging.lib.events
+class ZbDjangoTemplate(AppConfig):
+    default_auto_field = 'django.db.models.BigAutoField'
+    name = 'zibanu.django.template'
```

### Comparing `zibanu-django-1.2.0b1/zibanu/django/rest_framework/decorators.py` & `zibanu-django-1.2.1/zibanu/django/rest_framework/decorators.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/rest_framework/exceptions/__init__.py` & `zibanu-django-1.2.1/zibanu/django/rest_framework/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/rest_framework/exceptions/api_exception.py` & `zibanu-django-1.2.1/zibanu/django/rest_framework/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/rest_framework/fields/__init__.py` & `zibanu-django-1.2.1/zibanu/django/rest_framework/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/rest_framework/fields/current_user_default.py` & `zibanu-django-1.2.1/zibanu/django/rest_framework/fields/current_user_default.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/rest_framework/serializers/__init__.py` & `zibanu-django-1.2.1/zibanu/django/rest_framework/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/rest_framework/serializers/fields.py` & `zibanu-django-1.2.1/zibanu/django/rest_framework/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/rest_framework/serializers/model_serializer.py` & `zibanu-django-1.2.1/zibanu/django/rest_framework/serializers/model_serializer.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/rest_framework/viewsets/__init__.py` & `zibanu-django-1.2.1/zibanu/django/rest_framework/viewsets/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/rest_framework/viewsets/model_viewset.py` & `zibanu-django-1.2.1/zibanu/django/rest_framework/viewsets/model_viewset.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/rest_framework/viewsets/viewset.py` & `zibanu-django-1.2.1/zibanu/django/rest_framework/viewsets/viewset.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/template/apps.py` & `zibanu-django-1.2.1/zibanu/django/utils/validate_cache_code.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 
 #  Developed by CQ Inversiones SAS. Copyright ©. 2019 - 2023. All rights reserved.
 #  Desarrollado por CQ Inversiones SAS. Copyright ©. 2019 - 2023. Todos los derechos reservado
 
 # ****************************************************************
 # IDE:          PyCharm
 # Developed by: macercha
-# Date:         28/01/23 15:31
+# Date:         3/03/23 8:19
 # Project:      CFHL Transactional Backend
-# Module Name:  apps
+# Module Name:  validate_cache_code
 # Description:
 # ****************************************************************
-from django.apps import AppConfig
+from django.core.cache import cache
+from typing import Any
 
 
-class ZbDjangoTemplate(AppConfig):
-    default_auto_field = 'django.db.models.BigAutoField'
-    name = 'zibanu.django.template'
+def validate_cache_code(cache_key: str, code: str, code_key: str = None):
+    if code_key is None:
+        code_key = "code"
+
```

### Comparing `zibanu-django-1.2.0b1/zibanu/django/template/context_processors/__init__.py` & `zibanu-django-1.2.1/zibanu/django/template/context_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/template/context_processors/full_static_uri.py` & `zibanu-django-1.2.1/zibanu/django/template/context_processors/full_static_uri.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/template/context_processors/site.py` & `zibanu-django-1.2.1/zibanu/django/template/context_processors/site.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/template/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.2.1/zibanu/django/template/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/template/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.2.1/zibanu/django/template/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/template/templatetags/static_uri.py` & `zibanu-django-1.2.1/zibanu/django/template/templatetags/static_uri.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/template/templatetags/string_concat.py` & `zibanu-django-1.2.1/zibanu/django/template/templatetags/string_concat.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/template/templatetags/subtotal_dict.py` & `zibanu-django-1.2.1/zibanu/django/template/templatetags/subtotal_dict.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/template/templatetags/sum_dict.py` & `zibanu-django-1.2.1/zibanu/django/template/templatetags/sum_dict.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/utils/__init__.py` & `zibanu-django-1.2.1/zibanu/django/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/utils/code_generator.py` & `zibanu-django-1.2.1/zibanu/django/utils/code_generator.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/utils/date_time.py` & `zibanu-django-1.2.1/zibanu/django/utils/date_time.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/utils/error_messages.py` & `zibanu-django-1.2.1/zibanu/django/utils/error_messages.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/utils/mail.py` & `zibanu-django-1.2.1/zibanu/django/utils/mail.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/utils/request_utils.py` & `zibanu-django-1.2.1/zibanu/django/utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0b1/zibanu/django/utils/user.py` & `zibanu-django-1.2.1/zibanu/django/utils/user.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,26 +7,33 @@
 # IDE:          PyCharm
 # Developed by: macercha
 # Date:         14/12/22 4:21 AM
 # Project:      CFHL Transactional Backend
 # Module Name:  user
 # Description:
 # ****************************************************************
+from django.contrib import auth
+from rest_framework_simplejwt.models import TokenUser
 from typing import Any
-from zibanu.django.auth.lib.utils import get_user as auth_get_user
+
 
 def get_user(user: Any) -> Any:
     """
     Function to get User objecto from TokenUser or another object.
     :param user: Any: User object to be converted
     :return: User: User object.
     """
-    return auth_get_user(user)
+    local_user = user
+    user_model = auth.get_user_model()
+    if isinstance(user, TokenUser):
+        local_user = user_model.objects.get(pk=local_user.id)
+
+    return local_user
 
 
 def get_user_object(user: Any) -> Any:
     """
     Legacy function. This function will be discontinued in future versions.
     :param user: Any: User object from request or auth to be returned
     :return: User: User object
     """
-    return get_user(user)
+    return get_user(user)
```

### Comparing `zibanu-django-1.2.0b1/zibanu_django.egg-info/PKG-INFO` & `zibanu-django-1.2.1/zibanu_django.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: zibanu-django
-Version: 1.2.0b1
-Summary: Zibanu authentication library for django projects
+Version: 1.2.1
+Summary: Zibanu library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -676,24 +676,24 @@
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Keywords: django,zibanu,library,auth
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Zibanu Django Authentication Module
+# Zibanu Library for Django
 
 This package or library contains some functionalities commonly used in django projects and django rest_framework projects. 
 
 ## Django db
```

### Comparing `zibanu-django-1.2.0b1/zibanu_django.egg-info/SOURCES.txt` & `zibanu-django-1.2.1/zibanu_django.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -11,29 +11,14 @@
 zibanu/django/db/backends/oracle/base.py
 zibanu/django/db/models/__init__.py
 zibanu/django/db/models/dated_model.py
 zibanu/django/db/models/manager.py
 zibanu/django/db/models/model.py
 zibanu/django/locale/es/LC_MESSAGES/django.mo
 zibanu/django/locale/es/LC_MESSAGES/django.po
-zibanu/django/logging/__init__.py
-zibanu/django/logging/apps.py
-zibanu/django/logging/models.py
-zibanu/django/logging/lib/__init__.py
-zibanu/django/logging/lib/signals.py
-zibanu/django/logging/lib/events/__init__.py
-zibanu/django/logging/lib/events/on_change_password.py
-zibanu/django/logging/lib/events/on_login.py
-zibanu/django/logging/lib/events/on_send_mail.py
-zibanu/django/logging/lib/managers/__init__.py
-zibanu/django/logging/locale/es/LC_MESSAGES/django.mo
-zibanu/django/logging/locale/es/LC_MESSAGES/django.po
-zibanu/django/logging/migrations/0001_initial.py
-zibanu/django/logging/migrations/0002_maillog.py
-zibanu/django/logging/migrations/__init__.py
 zibanu/django/rest_framework/__init__.py
 zibanu/django/rest_framework/decorators.py
 zibanu/django/rest_framework/exceptions/__init__.py
 zibanu/django/rest_framework/exceptions/api_exception.py
 zibanu/django/rest_framework/fields/__init__.py
 zibanu/django/rest_framework/fields/current_user_default.py
 zibanu/django/rest_framework/serializers/__init__.py
```

