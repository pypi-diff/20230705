# Comparing `tmp/leanit-mweb-23.6.9.tar.gz` & `tmp/leanit-mweb-23.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leanit-mweb-23.6.9.tar", last modified: Fri Jun  9 14:23:17 2023, max compression
+gzip compressed data, was "leanit-mweb-23.7.1.tar", last modified: Wed Jul  5 12:33:37 2023, max compression
```

## Comparing `leanit-mweb-23.6.9.tar` & `leanit-mweb-23.7.1.tar`

### file list

```diff
@@ -1,38 +1,90 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-09 14:23:17.447745 leanit-mweb-23.6.9/
--rw-rw-r--   0 martin    (1000) martin    (1000)      962 2023-05-08 15:13:45.000000 leanit-mweb-23.6.9/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)      533 2023-06-09 14:23:17.447745 leanit-mweb-23.6.9/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)       24 2023-05-08 15:14:30.000000 leanit-mweb-23.6.9/README.md
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-09 14:23:17.423746 leanit-mweb-23.6.9/leanit_mweb/
--rw-rw-r--   0 martin    (1000) martin    (1000)    12246 2023-06-07 07:42:38.000000 leanit-mweb-23.6.9/leanit_mweb/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2509 2023-05-17 08:12:08.000000 leanit-mweb-23.6.9/leanit_mweb/auth.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      449 2023-05-08 06:49:29.000000 leanit-mweb-23.6.9/leanit_mweb/form.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-09 14:23:17.431746 leanit-mweb-23.6.9/leanit_mweb/jinja_template/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1023 2023-06-09 09:26:15.000000 leanit-mweb-23.6.9/leanit_mweb/jinja_template/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4134 2023-05-01 18:09:47.000000 leanit-mweb-23.6.9/leanit_mweb/jinja_template/loaders.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2002 2023-05-17 14:10:35.000000 leanit-mweb-23.6.9/leanit_mweb/manage.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-09 14:23:17.435746 leanit-mweb-23.6.9/leanit_mweb/messaging/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-19 13:00:21.000000 leanit-mweb-23.6.9/leanit_mweb/messaging/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-19 13:00:37.000000 leanit-mweb-23.6.9/leanit_mweb/messaging/base.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-09 14:23:17.439746 leanit-mweb-23.6.9/leanit_mweb/orm/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-07 11:08:10.000000 leanit-mweb-23.6.9/leanit_mweb/orm/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      205 2023-05-07 11:45:37.000000 leanit-mweb-23.6.9/leanit_mweb/orm/exception.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1838 2023-05-19 15:33:21.000000 leanit-mweb-23.6.9/leanit_mweb/orm/fields.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    13816 2023-06-06 14:35:40.000000 leanit-mweb-23.6.9/leanit_mweb/orm/model.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      914 2023-05-07 12:15:52.000000 leanit-mweb-23.6.9/leanit_mweb/orm/password.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1060 2023-05-01 12:48:02.000000 leanit-mweb-23.6.9/leanit_mweb/staticfiles.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-09 14:23:17.439746 leanit-mweb-23.6.9/leanit_mweb/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)      267 2023-05-26 13:54:10.000000 leanit-mweb-23.6.9/leanit_mweb/tests/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2241 2023-06-06 11:14:00.000000 leanit-mweb-23.6.9/leanit_mweb/thread.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1789 2023-06-07 11:04:54.000000 leanit-mweb-23.6.9/leanit_mweb/utils.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-09 14:23:17.447745 leanit-mweb-23.6.9/leanit_mweb/views/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-17 08:14:19.000000 leanit-mweb-23.6.9/leanit_mweb/views/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1120 2023-05-17 08:19:41.000000 leanit-mweb-23.6.9/leanit_mweb/views/auth.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10540 2023-05-23 15:19:29.000000 leanit-mweb-23.6.9/leanit_mweb/yuga.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-09 14:23:17.431746 leanit-mweb-23.6.9/leanit_mweb.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)      533 2023-06-09 14:23:17.000000 leanit-mweb-23.6.9/leanit_mweb.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      739 2023-06-09 14:23:17.000000 leanit-mweb-23.6.9/leanit_mweb.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-09 14:23:17.000000 leanit-mweb-23.6.9/leanit_mweb.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      513 2023-06-09 14:23:17.000000 leanit-mweb-23.6.9/leanit_mweb.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       12 2023-06-09 14:23:17.000000 leanit-mweb-23.6.9/leanit_mweb.egg-info/top_level.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-06-09 14:23:17.447745 leanit-mweb-23.6.9/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)     1854 2023-06-09 14:23:16.000000 leanit-mweb-23.6.9/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.943405 leanit-mweb-23.7.1/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      962 2023-05-08 15:13:45.000000 leanit-mweb-23.7.1/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2430 2023-07-05 12:33:37.943405 leanit-mweb-23.7.1/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1921 2023-06-21 11:11:08.000000 leanit-mweb-23.7.1/README.md
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.927406 leanit-mweb-23.7.1/leanit_mweb.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2430 2023-07-05 12:33:37.000000 leanit-mweb-23.7.1/leanit_mweb.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1593 2023-07-05 12:33:37.000000 leanit-mweb-23.7.1/leanit_mweb.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-07-05 12:33:37.000000 leanit-mweb-23.7.1/leanit_mweb.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      549 2023-07-05 12:33:37.000000 leanit-mweb-23.7.1/leanit_mweb.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       11 2023-07-05 12:33:37.000000 leanit-mweb-23.7.1/leanit_mweb.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.927406 leanit-mweb-23.7.1/mweb/
+-rw-rw-r--   0 martin    (1000) martin    (1000)    14635 2023-07-01 09:20:47.000000 leanit-mweb-23.7.1/mweb/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.931406 leanit-mweb-23.7.1/mweb/auth/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:18:02.000000 leanit-mweb-23.7.1/mweb/auth/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.931406 leanit-mweb-23.7.1/mweb/auth/sso/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:23:33.000000 leanit-mweb-23.7.1/mweb/auth/sso/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      381 2023-06-30 09:43:07.000000 leanit-mweb-23.7.1/mweb/auth/sso/base.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.931406 leanit-mweb-23.7.1/mweb/auth/sso/microsoft/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5760 2023-07-04 12:23:22.000000 leanit-mweb-23.7.1/mweb/auth/sso/microsoft/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      449 2023-05-08 06:49:29.000000 leanit-mweb-23.7.1/mweb/form.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.931406 leanit-mweb-23.7.1/mweb/jinja_template/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2001 2023-07-05 12:31:10.000000 leanit-mweb-23.7.1/mweb/jinja_template/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4134 2023-05-01 18:09:47.000000 leanit-mweb-23.7.1/mweb/jinja_template/loaders.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1995 2023-06-30 11:57:20.000000 leanit-mweb-23.7.1/mweb/manage.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.931406 leanit-mweb-23.7.1/mweb/messaging/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-19 13:00:21.000000 leanit-mweb-23.7.1/mweb/messaging/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-19 13:00:37.000000 leanit-mweb-23.7.1/mweb/messaging/base.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.931406 leanit-mweb-23.7.1/mweb/orm/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-07 11:08:10.000000 leanit-mweb-23.7.1/mweb/orm/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      205 2023-05-07 11:45:37.000000 leanit-mweb-23.7.1/mweb/orm/exception.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.935406 leanit-mweb-23.7.1/mweb/orm/fields/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2809 2023-06-30 13:17:38.000000 leanit-mweb-23.7.1/mweb/orm/fields/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      402 2023-06-30 11:55:37.000000 leanit-mweb-23.7.1/mweb/orm/fields/snowflake.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    17508 2023-07-05 09:48:32.000000 leanit-mweb-23.7.1/mweb/orm/model.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      914 2023-05-07 12:15:52.000000 leanit-mweb-23.7.1/mweb/orm/password.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.935406 leanit-mweb-23.7.1/mweb/security/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      564 2023-06-27 15:25:35.000000 leanit-mweb-23.7.1/mweb/security/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2135 2023-06-30 09:59:15.000000 leanit-mweb-23.7.1/mweb/security/jwt.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1060 2023-05-01 12:48:02.000000 leanit-mweb-23.7.1/mweb/staticfiles.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2745 2023-06-14 06:12:52.000000 leanit-mweb-23.7.1/mweb/testutils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2241 2023-06-06 11:14:00.000000 leanit-mweb-23.7.1/mweb/thread.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.935406 leanit-mweb-23.7.1/mweb/utils/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2906 2023-07-01 08:58:49.000000 leanit-mweb-23.7.1/mweb/utils/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.935406 leanit-mweb-23.7.1/mweb/utils/id/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:02:22.000000 leanit-mweb-23.7.1/mweb/utils/id/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1345 2023-06-30 09:04:34.000000 leanit-mweb-23.7.1/mweb/utils/id/snowflakeid.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      931 2023-07-05 09:13:08.000000 leanit-mweb-23.7.1/mweb/utils/log_catcher.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)       19 2023-07-05 12:33:37.000000 leanit-mweb-23.7.1/mweb/version.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.935406 leanit-mweb-23.7.1/mweb/views/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-17 08:14:19.000000 leanit-mweb-23.7.1/mweb/views/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1092 2023-06-30 11:57:20.000000 leanit-mweb-23.7.1/mweb/views/auth.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6900 2023-07-05 10:05:44.000000 leanit-mweb-23.7.1/mweb/views/model.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10602 2023-07-05 10:55:32.000000 leanit-mweb-23.7.1/mweb/yuga.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-07-05 12:33:37.943405 leanit-mweb-23.7.1/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1912 2023-07-05 12:33:37.000000 leanit-mweb-23.7.1/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.935406 leanit-mweb-23.7.1/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 12:07:34.000000 leanit-mweb-23.7.1/tests/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.935406 leanit-mweb-23.7.1/tests/auth/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:29:21.000000 leanit-mweb-23.7.1/tests/auth/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.935406 leanit-mweb-23.7.1/tests/auth/sso/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:29:21.000000 leanit-mweb-23.7.1/tests/auth/sso/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.939406 leanit-mweb-23.7.1/tests/auth/sso/microsoft/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      210 2023-06-30 09:30:02.000000 leanit-mweb-23.7.1/tests/auth/sso/microsoft/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1824 2023-06-30 09:36:45.000000 leanit-mweb-23.7.1/tests/auth/sso/microsoft/test_auth_callback.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1797 2023-06-30 09:36:45.000000 leanit-mweb-23.7.1/tests/auth/sso/microsoft/test_build_auth_url.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      591 2023-06-30 09:30:07.000000 leanit-mweb-23.7.1/tests/auth/sso/microsoft/test_code.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.939406 leanit-mweb-23.7.1/tests/orm/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-14 06:24:31.000000 leanit-mweb-23.7.1/tests/orm/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.939406 leanit-mweb-23.7.1/tests/orm/fields/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-14 07:10:28.000000 leanit-mweb-23.7.1/tests/orm/fields/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      706 2023-06-30 11:55:37.000000 leanit-mweb-23.7.1/tests/orm/fields/test_StringField.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.939406 leanit-mweb-23.7.1/tests/orm/model/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-14 06:24:39.000000 leanit-mweb-23.7.1/tests/orm/model/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1158 2023-06-30 12:03:34.000000 leanit-mweb-23.7.1/tests/orm/model/test_delete_all.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.939406 leanit-mweb-23.7.1/tests/resources/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       76 2023-07-02 16:02:44.000000 leanit-mweb-23.7.1/tests/resources/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.939406 leanit-mweb-23.7.1/tests/security/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-28 15:18:34.000000 leanit-mweb-23.7.1/tests/security/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1110 2023-06-29 11:38:56.000000 leanit-mweb-23.7.1/tests/security/test_jwt.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      685 2023-06-29 11:18:38.000000 leanit-mweb-23.7.1/tests/security/test_sign.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.943405 leanit-mweb-23.7.1/tests/utils/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-29 11:22:08.000000 leanit-mweb-23.7.1/tests/utils/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1836 2023-06-30 11:57:20.000000 leanit-mweb-23.7.1/tests/utils/test_form.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      537 2023-06-30 09:05:14.000000 leanit-mweb-23.7.1/tests/utils/test_snowflake.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      469 2023-07-01 08:58:49.000000 leanit-mweb-23.7.1/tests/utils/test_unflatten.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.943405 leanit-mweb-23.7.1/tests/views/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-07-02 15:26:48.000000 leanit-mweb-23.7.1/tests/views/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 12:33:37.943405 leanit-mweb-23.7.1/tests/views/model/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-07-02 15:26:56.000000 leanit-mweb-23.7.1/tests/views/model/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9069 2023-07-03 08:51:42.000000 leanit-mweb-23.7.1/tests/views/model/test_paging.py
```

### Comparing `leanit-mweb-23.6.9/LICENSE` & `leanit-mweb-23.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.6.9/leanit_mweb/__init__.py` & `leanit-mweb-23.7.1/mweb/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 from __future__ import annotations
+import logging
+from pprint import pprint
+
+from mweb.version import VERSION
+
+logger = logging.getLogger(__name__)
+
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    pass
 
 import base64
+import importlib
 import logging
 import os
+import pkgutil
 import sys
 from collections import defaultdict
-from datetime import timedelta, datetime
-from os.path import isabs, abspath
-from pprint import pprint
+from os.path import isdir
 
 import yaml
-from fastapi import FastAPI, Depends, HTTPException
-from jose import jwt, JWTError
-
-from leanit_mweb.jinja_template import Jinja2Templates
-from leanit_mweb.jinja_template.loaders import FileSystemLoader
-from leanit_mweb.utils import merge_dict
-
+from fastapi import FastAPI
 
-from leanit_mweb.yuga import YugabytedbThreadPool
-from starlette import status
+from mweb.jinja_template import Jinja2Templates
+from mweb.jinja_template.loaders import FileSystemLoader
+from mweb.utils import merge_dict
+from mweb.yuga import YugabytedbThreadPool
 
 logger = logging.getLogger(__name__)
 
-from typing import TYPE_CHECKING, Dict, Annotated, Any
+from typing import TYPE_CHECKING, Dict, Any
 
 if TYPE_CHECKING:
-    from leanit_mweb.orm.model import Model
+    from mweb.orm import Model
 
 config: Dict = None
 db: YugabytedbThreadPool = None
 loader: FileSystemLoader = None
 templates: Jinja2Templates = None
 
 # auth
@@ -41,28 +48,34 @@
 oauth2_scheme = None
 auth_user_model = None
 
 app = None
 
 class App(FastAPI):
 
-    def __init__(self, app_root: str, enable_static=False):
+    def __init__(self, app_root: str):
+        logger.info(f"Initializing mweb app version={VERSION}")
+
         global config, app
         app = self
 
         self.app_root = app_root
+        self.db: YugabytedbThreadPool = None
 
         config = self.config = self._read_config()
+        self.secret_key = config.get("mweb", {}).get("secret_key", None)
 
         super().__init__()
 
-        if enable_static:
+        # static files
+        static_dir = f"{app_root}/static"
+        if isdir(static_dir):
             # mount static files
-            from leanit_mweb.staticfiles import StaticFiles
-            self.mount("/static", StaticFiles(directory=f"{app_root}/static"), name="static")
+            from mweb.staticfiles import StaticFiles
+            self.mount("/static", StaticFiles(directory=static_dir), name="static")
 
     def enable_auth(self, user_model):
         """
         :param user_model: Model class for user
         :type user_model: Model
         :return:
         """
@@ -78,34 +91,48 @@
 
         algorithm = auth_config.get("algorithm", "HS256")
         access_token_expire_minutes = auth_config.get("access_token_expire_minutes", 30)
 
         from passlib.context import CryptContext
         pwd_context = CryptContext(schemes=["bcrypt"], deprecated="auto")
 
-        from fastapi.security import OAuth2PasswordBearer, OAuth2PasswordRequestForm
+        from fastapi.security import OAuth2PasswordBearer
         oauth2_scheme = oauth2_scheme = OAuth2PasswordBearer(tokenUrl="token")
 
         auth_user_model = user_model
 
     def enable_db(self):
         global db
 
         db_config = config["db"]
         pool_config = db_config.get("pool", {})
-        db = YugabytedbThreadPool(
+        db = self.db = YugabytedbThreadPool(
             min_workers=pool_config.get("min_workers", 1),
             max_workers=pool_config.get("max_workers", 10),
         )
         db.migrate(migration_dir=f"{self.app_root}/migrations")
 
         # get all subclasses of Model
-        from leanit_mweb.orm.model import Model
+        from mweb.orm.model import Model
+
+        # loader
+        module_name = self.__module__ # "mium_frontend"
+        models_module_name = f"{module_name}.model"
+        models_module = None
+        try:
+            models_module = importlib.import_module(models_module_name)
+        except ImportError:
+            logger.debug(f"no models package found for {module_name} ({models_module_name})")
+        if models_module:
+            for importer, modname, ispkg in pkgutil.walk_packages(path=models_module.__path__, prefix=models_module.__name__+'.'):
+                module = importlib.import_module(modname)
+
         # initialize all models
         for cls in Model.__subclasses__():  # type: Model
+            logger.debug(f"initialize model {cls.__name__}")
             cls._initialize()
 
         # initialize objects
         init_objects = db_config.get("init_objects", [])
         if init_objects:
             def _handle_object(obj_cls, query: Dict, obj_attributes: Dict):
                 obj = obj_cls.get(**query)
@@ -183,15 +210,14 @@
             }
 
             if "traces_sample_rate" in sentry_config:
                 sentry_kwargs["traces_sample_rate"] = float(sentry_config["traces_sample_rate"])
             if "environment" in sentry_config:
                 sentry_kwargs["environment"] = sentry_config["environment"]
 
-            pprint(sentry_kwargs)
             sentry_sdk.init(**sentry_kwargs)
 
     def enable_tracing(self):
         tracing_config = config.get("tracing", {})
         if not tracing_config.get("enabled", False):
             logger.info("Tracing is disabled")
             return
@@ -259,15 +285,14 @@
             )
 
         # instrument fastapi
         from opentelemetry.instrumentation.fastapi import FastAPIInstrumentor
         FastAPIInstrumentor.instrument_app(self, tracer_provider=tracer_provider)
 
         # instrument aiohttp
-        import aiohttp
         from opentelemetry.instrumentation.aiohttp_client import (
             AioHttpClientInstrumentor
         )
 
         # Enable instrumentation
         AioHttpClientInstrumentor().instrument()
 
@@ -321,21 +346,57 @@
                 sub_config = yaml.safe_load(f)
                 if sub_config:
                     merge_dict(source=sub_config, destination=config_data)
 
         return config_data
 
     def setup(self) -> None:
+        logger.info("Setting up application")
         super().setup()
 
+        # self._patch_starlette()
+
         if "db" in config:
             self.enable_db()
 
         global loader, templates
         loader = FileSystemLoader(f"{self.app_root}/templates")
         templates = Jinja2Templates(directory=f"{self.app_root}/templates", loader=loader)
 
         if "tracing" in config:
             self.enable_tracing()
 
         self.enable_sentry()
         self.initialize()
+
+    def load_views(self):
+        """
+        Load all views from the views package (recursively). This is done to ensure that all views are loaded.
+        :return:
+        """
+        # import views
+        module_name = self.__module__  # "mium_frontend"
+        views_module_name = f"{module_name}.views"
+        views_module = None
+        try:
+            views_module = importlib.import_module(views_module_name)
+        except ImportError as e:
+            logger.info(f"no views package found for {module_name}: {e}")
+
+        if views_module:
+            for importer, modname, ispkg in pkgutil.walk_packages(path=views_module.__path__,
+                                                                  prefix=views_module.__name__ + '.'):
+                module = importlib.import_module(modname)
+
+        # validate views
+        from mweb.views.model import ModelView
+        model_views = ModelView.__subclasses__()
+
+        for model_view_class in model_views:
+            self._validate_model_view(model_view_class)
+
+    def _validate_model_view(self, model_view_class):
+        # check if every primary key property is in the list of fields
+        if model_view_class.list_fields:
+            for pk_field_name in model_view_class.model._pk:
+                if pk_field_name not in model_view_class.list_fields:
+                    raise ValueError(f"primary key field {pk_field_name} of model {model_view_class.model.__name__} is not in list_fields of {model_view_class.__name__} defined in {model_view_class.__module__}")
```

### Comparing `leanit-mweb-23.6.9/leanit_mweb/auth.py` & `leanit-mweb-23.7.1/mweb/utils/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,82 +1,84 @@
 from __future__ import annotations
 import logging
-
+from starlette.requests import Request
 logger = logging.getLogger(__name__)
-import logging
-from datetime import timedelta, datetime
-
-import leanit_mweb
 
-from fastapi import Depends, HTTPException
-from fastapi.security import OAuth2PasswordBearer, OAuth2PasswordRequestForm
-from jose import jwt, JWTError
-from passlib.context import CryptContext
-from pydantic import BaseModel
-from starlette import status
-
-from typing import TYPE_CHECKING, Annotated, Dict
+from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     pass
 
-class Token(BaseModel):
-    access_token: str
-    token_type: str
-
-def get_password_hash(password):
-    return leanit_mweb.pwd_context.hash(password)
-
-def verify_password(plain_password, hashed_password):
-    return leanit_mweb.pwd_context.verify(plain_password, hashed_password)
-
-def authenticate_user(username: str, password: str):
-    """
-    Authenticate user, return user if authenticated, False otherwise
-    :param username:
-    :param password:
-    :return:
-    """
-    users = leanit_mweb.auth_user_model.filter(name=username)
-    if not users:
-        print("No user found")
-        return False
-    user = users[0]
-    if not user:
-        return False
-    if not leanit_mweb.pwd_context.verify(password, user.password):
-        return False
-    return user
-
-def create_access_token(data: dict, expires_delta: timedelta | None = None):
-    to_encode = data.copy()
-    if expires_delta:
-        expire = datetime.utcnow() + expires_delta
+def camelCaseToSnakeCase(name):
+    return ''.join(['_'+i.lower() if i.isupper() else i for i in name]).lstrip('_')
+
+def flatten(data: tuple, delimiter: str = ',') -> str:
+    """
+    Convert a tuple of pairs to a delimited list.
+
+    :param data: A tuple of pairs.
+    :type data: tuple
+    :param delimiter: The delimiter used to join the output list. Defaults to ','.
+    :type delimiter: str
+    :return: A delimited list of strings, where each element of the input tuple is represented by two elements in the output list.
+    :rtype: str
+    """
+    flattened_data = [str(item) for sublist in data for item in sublist]
+    result = delimiter.join(flattened_data)
+    return result
+
+def merge_dict(source, destination):
+    """
+    run me with nosetests --with-doctest file.py
+
+    >>> a = { 'first' : { 'all_rows' : { 'pass' : 'dog', 'number' : '1' } } }
+    >>> b = { 'first' : { 'all_rows' : { 'fail' : 'cat', 'number' : '5' } } }
+    >>> merge(b, a) == { 'first' : { 'all_rows' : { 'pass' : 'dog', 'fail' : 'cat', 'number' : '5' } } }
+    True
+    """
+    for key, value in source.items():
+        if isinstance(value, dict):
+            # get node or create one
+            node = destination.setdefault(key, {})
+            merge_dict(value, node)
+        elif isinstance(value, list):
+            # get node or create one
+            node = destination.setdefault(key, [])
+            for item in value:
+                if item not in node:
+                    node.append(item)
+        else:
+            destination[key] = value
+
+    return destination
+
+def remote_ip(request: Request):
+    """
+    Return the remote ip address of the request depending on the ip_mode config.
+    """
+    from mweb import config
+    ip_mode = config.get("mweb", {}).get("ip_mode", "remote_addr")
+
+    if ip_mode == "remote_addr":
+        return request.client.host
+    elif ip_mode == "x_forwarded_for":
+        return request.headers.get("x-forwarded-for", request.client.host)
+    elif ip_mode == "cloudflare":
+        return request.headers.get("cf-connecting-ip", request.client.host)
     else:
-        expire = datetime.utcnow() + timedelta(minutes=15)
-    to_encode.update({"exp": expire})
-    encoded_jwt = jwt.encode(to_encode, leanit_mweb.secret_key, algorithm=leanit_mweb.algorithm)
-    return encoded_jwt
-
-
-async def get_current_user(token: Annotated[str, Depends(leanit_mweb.oauth2_scheme)]):
-    credentials_exception = HTTPException(
-        status_code=status.HTTP_401_UNAUTHORIZED,
-        detail="Could not validate credentials",
-        headers={"WWW-Authenticate": "Bearer"},
-    )
-    try:
-        payload = jwt.decode(token, leanit_mweb.secret_key, algorithms=[leanit_mweb.algorithm])
-        user_id: str = payload.get("sub")
-        if user_id is None:
-            raise credentials_exception
-    except JWTError:
-        raise credentials_exception
-    user = leanit_mweb.auth_user_model.get(id=user_id)
-    if user is None:
-        raise credentials_exception
-    return user
-
-async def get_current_active_user(
-    current_user: Annotated[Dict, Depends(get_current_user)]
-) -> Dict[str, str]:
-    return current_user.to_dict()
+        raise NotImplementedError(f"Unknown ip_mode: {ip_mode}")
+
+
+def unflatten(data: str, delimiter: str = ',') -> tuple:
+    """
+    Convert a delimited list to a tuple of pairs.
+
+    :param data: A delimited list of strings.
+    :type data: str
+    :param delimiter: The delimiter used to split the input string. Defaults to ','.
+    :type delimiter: str
+    :return: A tuple of pairs, where each pair contains two elements from the input list.
+    :rtype: tuple
+    """
+    split_data = data.split(delimiter)
+    result = tuple((split_data[i], split_data[i+1]) for i in range(0, len(split_data), 2))
+    return result
```

### Comparing `leanit-mweb-23.6.9/leanit_mweb/jinja_template/loaders.py` & `leanit-mweb-23.7.1/mweb/jinja_template/loaders.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.6.9/leanit_mweb/manage.py` & `leanit-mweb-23.7.1/mweb/manage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import logging
 import os
 import time
 from os.path import isfile, join
 
-import leanit_mweb
+import mweb
 
 logger = logging.getLogger(__name__)
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     pass
```

### Comparing `leanit-mweb-23.6.9/leanit_mweb/orm/fields.py` & `leanit-mweb-23.7.1/mweb/orm/fields/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import json
 import logging
 import re
 
 from ulid import ULID
 
-from leanit_mweb.orm.exception import ValidationFailedException
+from mweb.orm.exception import ValidationFailedException
 
 logger = logging.getLogger(__name__)
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     pass
@@ -52,15 +52,31 @@
 
 
 class IntegerField(Field):
     pass
 
 
 class StringField(Field):
-    pass
+    def __init__(self, min_length=None, max_length=None, default=None, alphabet=None, choices=None):
+        super().__init__(default=default)
+        self.min_length = min_length
+        self.max_length = max_length
+        self.alphabet = alphabet
+        self.choices = choices
+
+    def validate(self, value):
+        if self.min_length is not None and len(value) < self.min_length:
+            raise ValidationFailedException(f"String is too short: '{value}'")
+        if self.max_length is not None and len(value) > self.max_length:
+            raise ValidationFailedException(f"String is too long: '{value}'")
+        if self.alphabet is not None and not set(value).issubset(set(self.alphabet)):
+            raise ValidationFailedException(f"String contains invalid characters: '{value}'")
+        if self.choices is not None and value not in self.choices:
+            raise ValidationFailedException(f"String is not in choices: '{value}'")
+        return super().validate(value)
 
 
 class EmailField(StringField):
     pattern = re.compile(r'^[\w\.-]+@[\w\.-]+\.\w+$')
 
     def validate(self, value):
         # validate email
@@ -82,7 +98,8 @@
     pass
 
 class JsonField(StringField):
     # psycopg2 handles reads correctly and automatically converts json to python dict
     # but it does not handle writes correctly, so we need to convert python dict to json string
     def to_db(self, value):
         return json.dumps(value)
+
```

### Comparing `leanit-mweb-23.6.9/leanit_mweb/orm/password.py` & `leanit-mweb-23.7.1/mweb/orm/password.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.6.9/leanit_mweb/staticfiles.py` & `leanit-mweb-23.7.1/mweb/staticfiles.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.6.9/leanit_mweb/thread.py` & `leanit-mweb-23.7.1/mweb/thread.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.6.9/leanit_mweb/views/auth.py` & `leanit-mweb-23.7.1/mweb/views/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 logger = logging.getLogger(__name__)
 
 from typing import TYPE_CHECKING, Annotated
 
 if TYPE_CHECKING:
     pass
 
-import leanit_mweb
-from leanit_mweb.auth import Token, authenticate_user, create_access_token
+import mweb
+from mweb.auth import Token, authenticate_user, create_access_token
 
-@leanit_mweb.app.post("/token2", response_model=Token)
+@mweb.app.post("/token2", response_model=Token)
 async def login_for_access_token(
     form_data: Annotated[OAuth2PasswordRequestForm, Depends()]
 ):
     user = authenticate_user(form_data.username, form_data.password)
     if not user:
         raise HTTPException(
             status_code=status.HTTP_401_UNAUTHORIZED,
             detail="Incorrect username or password",
             headers={"WWW-Authenticate": "Bearer"},
         )
-    access_token_expires = timedelta(minutes=leanit_mweb.access_token_expire_minutes)
+    access_token_expires = timedelta(minutes=mweb.access_token_expire_minutes)
     access_token = create_access_token(
         data={"sub": user.id}, expires_delta=access_token_expires
     )
     return {"access_token": access_token, "token_type": "bearer"}
```

### Comparing `leanit-mweb-23.6.9/leanit_mweb/yuga.py` & `leanit-mweb-23.7.1/mweb/yuga.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from __future__ import annotations
 import logging
 import threading
 from concurrent.futures import ThreadPoolExecutor
 from os import listdir, chmod
 from time import time, perf_counter
 
+import asyncio
 import psycopg2
 from opentelemetry import trace, context
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.trace import SpanKind
 from psycopg2 import connection, InterfaceError
 from psycopg2.extensions import ISOLATION_LEVEL_SERIALIZABLE, ISOLATION_LEVEL_REPEATABLE_READ
 from psycopg2.pool import ThreadedConnectionPool
+import psycopg2.errors
 
-import leanit_mweb
-from leanit_mweb.thread import AdvancedThreadPoolExecutor
+import mweb
+import mweb
+from mweb.thread import AdvancedThreadPoolExecutor
 
 tracer = trace.get_tracer(__name__)
 logger = logging.getLogger(__name__)
 
 
 from typing import TYPE_CHECKING, Iterable, Dict, Union
 
@@ -42,19 +45,19 @@
 
 
 def _initialize():
     thread_name = threading.current_thread().name
     logger.info(f"[{thread_name}] Initializing YugabyteDB connection pool")
 
     kwargs = dict(
-        dbname=leanit_mweb.config['db']['dbname'],
-        host=leanit_mweb.config['db']['host'],
-        port=leanit_mweb.config['db']['port'],
-        user=leanit_mweb.config['db']['user'],
-        password=leanit_mweb.config['db']['password'],
+        dbname=mweb.config['db']['dbname'],
+        host=mweb.config['db']['host'],
+        port=mweb.config['db']['port'],
+        user=mweb.config['db']['user'],
+        password=mweb.config['db']['password'],
         # load_balance='true',
 
         # Controls whether client-side TCP keepalives are used. The default value is 1, meaning on, but you can change
         # this to 0, meaning off, if keepalives are not wanted.
         keepalives=1,
         # Controls the number of seconds of inactivity after which TCP should send a keepalive message to the server.
         # A value of zero uses the system default.
@@ -62,43 +65,43 @@
         # Controls the number of seconds after which a TCP keepalive message that is not acknowledged by the server
         # should be retransmitted. A value of zero uses the system default.
         keepalives_interval=5,
         # Controls the number of TCP keepalives that can be lost before the client's connection to the server is
         # considered dead. A value of zero uses the system default.
         keepalives_count=2,
     )
-    if 'sslmode' in leanit_mweb.config['db']:
-        kwargs['sslmode'] = leanit_mweb.config['db']['sslmode']
-    if 'sslcert' in leanit_mweb.config['db']:
-        sslcert = leanit_mweb.config['db']['sslcert']
+    if 'sslmode' in mweb.config['db']:
+        kwargs['sslmode'] = mweb.config['db']['sslmode']
+    if 'sslcert' in mweb.config['db']:
+        sslcert = mweb.config['db']['sslcert']
         if"BEGIN CERTIFICATE" in sslcert:
             # assume it's a certificate
             sslcert_path = f"/tmp/{kwargs['dbname']}-{thread_name}-sslcert.crt"
             with open(sslcert_path, "w") as f:
                 f.write(sslcert.strip())
         else:
             # assume it's a file path
             sslcert_path = sslcert
 
         kwargs['sslcert'] = sslcert_path
-    if 'sslkey' in leanit_mweb.config['db']:
-        sslkey = leanit_mweb.config['db']['sslkey']
+    if 'sslkey' in mweb.config['db']:
+        sslkey = mweb.config['db']['sslkey']
         if "PRIVATE KEY" in sslkey:
             # assume it's a private key
             sslkey_path = f"/tmp/{kwargs['dbname']}-{thread_name}-sslkey.key"
             with open(sslkey_path, "w") as f:
                 chmod(sslkey_path, 0o600)
                 f.write(sslkey.strip())
         else:
             # assume it's a file path
             sslkey_path = sslkey
 
         kwargs['sslkey'] = sslkey_path
-    if 'sslrootcert' in leanit_mweb.config['db']:
-        sslrootcert = leanit_mweb.config['db']['sslrootcert']
+    if 'sslrootcert' in mweb.config['db']:
+        sslrootcert = mweb.config['db']['sslrootcert']
         if "BEGIN CERTIFICATE" in sslrootcert:
             # assume it's a certificate
             sslrootcert_path = f"/tmp/{kwargs['dbname']}-{thread_name}-sslrootcert.crt"
             with open(sslrootcert_path, "w") as f:
                 f.write(sslrootcert.strip())
 
         else:
@@ -138,17 +141,22 @@
         :param sql: might contain %s placeholders (vars=Iterable) or %(name)s placeholders (vars=Dict)
         :param vars: Iterable or Dict
         :return:
         """
         f = self.submit(self.submit_sql, sql, vars, tracing_context)
         return f.result()
 
+    async def execute_async(self, sql: str, vars: Union[Dict, Iterable]=None, tracing_context=None):
+        if not tracing_context:
+            tracing_context = context.get_current()
+        return await asyncio.get_event_loop().run_in_executor(self, self.submit_sql, sql, vars, tracing_context)
+
     def submit_sql(self, sql: str, vars: Union[Dict, Iterable]=None, tracing_context=None):
         """
-        This function is executed in a thread
+        This function is executed in a thread. It is blocking.
 
         :param sql: might contain %s placeholders (vars=Iterable) or %(name)s placeholders (vars=Dict)
         :param vars: Iterable or Dict
         :return:
         """
         # tracing
         if tracing_context:
@@ -171,18 +179,14 @@
 
                     cursor.execute(sql, vars)
 
                     result = None
                     if sql_command == 'SELECT':
                         result = cursor.fetchall()
 
-                    # else:
-                    #     with tracer.start_as_current_span("db.commit", kind=SpanKind.INTERNAL) as span:  # type: trace.Span
-                    #         conn.commit()
-
                     # everything is fine, break out of the while loop
                     break
             except psycopg2.errors.SerializationFailure as e:
                 error_message = " ".join([line.strip() for line in str(e).splitlines()])
                 logger.error(f"[{threading.current_thread().name}] Error executing SQL: sql='{sql}' error={e.__class__.__name__} message='{error_message}'")
                 try:
                     with tracer.start_as_current_span("db.rollback", kind=SpanKind.INTERNAL) as span:  # type: trace.Span
```

### Comparing `leanit-mweb-23.6.9/leanit_mweb.egg-info/requires.txt` & `leanit-mweb-23.7.1/leanit_mweb.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 python-multipart~=0.0
 wtforms~=3.0
 email_validator~=2.0
 multidict~=6.0
 psycopg2-yugabytedb~=2.9
 PyYAML~=6.0
 python-ulid~=1.1
+snowflake-id~=0.0
 aiohttp~=3.7
+aioresponses~=0.7
 bcrypt~=4.0
 passlib~=1.7
 python-jose[cryptography]~=3.3
 opentelemetry-api~=1.18
 opentelemetry-sdk~=1.18
 opentelemetry-instrumentation-aiohttp-client~=0.39b0
 opentelemetry-instrumentation-fastapi~=0.39b0
```

### Comparing `leanit-mweb-23.6.9/setup.py` & `leanit-mweb-23.7.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '23.6.9'
+VERSION = '23.7.1'
 DESCRIPTION = 'Web framework'
 LONG_DESCRIPTION = 'Web framework'
 
 # Setting up
 setup(
     name="leanit-mweb",
     version=VERSION,
@@ -29,15 +29,17 @@
         'python-multipart~=0.0',
         'wtforms~=3.0',
         'email_validator~=2.0',
         'multidict~=6.0',
         'psycopg2-yugabytedb~=2.9',
         'PyYAML~=6.0',
         'python-ulid~=1.1',
+        'snowflake-id~=0.0',
         'aiohttp~=3.7',
+        'aioresponses~=0.7',
         # for authentication / crypto
         'bcrypt~=4.0',
         'passlib~=1.7',
         'python-jose[cryptography]~=3.3', # JWT
         # telemetry
         'opentelemetry-api~=1.18',
         'opentelemetry-sdk~=1.18',
```

