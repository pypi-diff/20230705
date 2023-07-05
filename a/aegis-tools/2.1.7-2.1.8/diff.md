# Comparing `tmp/aegis-tools-2.1.7.tar.gz` & `tmp/aegis-tools-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aegis-tools-2.1.7.tar", last modified: Fri Jun 30 00:03:16 2023, max compression
+gzip compressed data, was "aegis-tools-2.1.8.tar", last modified: Wed Jul  5 19:07:39 2023, max compression
```

## Comparing `aegis-tools-2.1.7.tar` & `aegis-tools-2.1.8.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-06-30 00:03:16.412596 aegis-tools-2.1.7/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/LICENSE
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/MANIFEST.in
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-06-30 00:03:16.412596 aegis-tools-2.1.7/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/README.md
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-06-30 00:03:16.396596 aegis-tools-2.1.7/aegis/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/aegis/__init__.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    17334 2022-11-21 05:05:18.000000 aegis-tools-2.1.7/aegis/aegis_.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    18804 2023-05-12 16:02:53.000000 aegis-tools-2.1.7/aegis/build.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2380 2023-01-12 20:56:01.000000 aegis-tools-2.1.7/aegis/config.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    25757 2023-04-02 20:38:42.000000 aegis-tools-2.1.7/aegis/database.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    25692 2023-05-24 02:49:53.000000 aegis-tools-2.1.7/aegis/hydra.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7559 2023-05-24 02:47:45.000000 aegis-tools-2.1.7/aegis/mailer.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    43046 2023-05-24 02:50:29.000000 aegis-tools-2.1.7/aegis/model.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-06-30 00:03:16.404596 aegis-tools-2.1.7/aegis/sql/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.1.7/aegis/sql/auditing-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4271 2023-02-05 03:12:16.000000 aegis-tools-2.1.7/aegis/sql/auditing-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/aegis/sql/build-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.1.7/aegis/sql/build-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/aegis/sql/cache_system.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.1.7/aegis/sql/email_system-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-05-22 20:40:27.000000 aegis-tools-2.1.7/aegis/sql/google_signin.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/aegis/sql/hydra-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/aegis/sql/hydra-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/aegis/sql/member_auth.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/aegis/sql/monitor-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/aegis/sql/reports.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    31598 2023-06-30 00:02:27.000000 aegis-tools-2.1.7/aegis/stdlib.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-06-30 00:03:16.412596 aegis-tools-2.1.7/aegis/templates/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3083 2023-03-11 00:56:38.000000 aegis-tools-2.1.7/aegis/templates/build.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.1.7/aegis/templates/build_confirm.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.1.7/aegis/templates/build_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.1.7/aegis/templates/build_view.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/aegis/templates/error_message.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3297 2023-04-27 02:34:36.000000 aegis-tools-2.1.7/aegis/templates/frame.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2107 2023-03-11 00:53:08.000000 aegis-tools-2.1.7/aegis/templates/hydra.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.1.7/aegis/templates/hydra_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1660 2023-03-11 00:55:55.000000 aegis-tools-2.1.7/aegis/templates/hydra_queue.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.1.7/aegis/templates/index.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.1.7/aegis/templates/report.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.1.7/aegis/templates/report_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.1.7/aegis/templates/reports.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.1.7/aegis/templates/w3.css
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/aegis/threadpool.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    73800 2023-05-24 02:36:08.000000 aegis-tools-2.1.7/aegis/webapp.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-06-30 00:03:16.412596 aegis-tools-2.1.7/aegis_tools.egg-info/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-06-30 00:03:16.000000 aegis-tools-2.1.7/aegis_tools.egg-info/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2023-06-30 00:03:16.000000 aegis-tools-2.1.7/aegis_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2023-06-30 00:03:16.000000 aegis-tools-2.1.7/aegis_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2023-06-30 00:03:16.000000 aegis-tools-2.1.7/aegis_tools.egg-info/entry_points.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2023-06-30 00:03:16.000000 aegis-tools-2.1.7/aegis_tools.egg-info/requires.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2023-06-30 00:03:16.000000 aegis-tools-2.1.7/aegis_tools.egg-info/top_level.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2023-06-30 00:03:16.412596 aegis-tools-2.1.7/setup.cfg
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1676 2023-06-30 00:02:53.000000 aegis-tools-2.1.7/setup.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-07-05 19:07:39.679728 aegis-tools-2.1.8/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.1.8/LICENSE
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.1.8/MANIFEST.in
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-07-05 19:07:39.679728 aegis-tools-2.1.8/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.1.8/README.md
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-07-05 19:07:39.659728 aegis-tools-2.1.8/aegis/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.1.8/aegis/__init__.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    17334 2022-11-21 05:05:18.000000 aegis-tools-2.1.8/aegis/aegis_.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    18804 2023-05-12 16:02:53.000000 aegis-tools-2.1.8/aegis/build.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2380 2023-01-12 20:56:01.000000 aegis-tools-2.1.8/aegis/config.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    25757 2023-04-02 20:38:42.000000 aegis-tools-2.1.8/aegis/database.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    25692 2023-05-24 02:49:53.000000 aegis-tools-2.1.8/aegis/hydra.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7559 2023-05-24 02:47:45.000000 aegis-tools-2.1.8/aegis/mailer.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    43046 2023-05-24 02:50:29.000000 aegis-tools-2.1.8/aegis/model.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-07-05 19:07:39.667728 aegis-tools-2.1.8/aegis/sql/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.1.8/aegis/sql/auditing-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4271 2023-02-05 03:12:16.000000 aegis-tools-2.1.8/aegis/sql/auditing-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.1.8/aegis/sql/build-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.1.8/aegis/sql/build-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.1.8/aegis/sql/cache_system.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.1.8/aegis/sql/email_system-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-05-22 20:40:27.000000 aegis-tools-2.1.8/aegis/sql/google_signin.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.1.8/aegis/sql/hydra-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.1.8/aegis/sql/hydra-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.1.8/aegis/sql/member_auth.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.1.8/aegis/sql/monitor-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.1.8/aegis/sql/reports.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    31598 2023-06-30 00:02:27.000000 aegis-tools-2.1.8/aegis/stdlib.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-07-05 19:07:39.671728 aegis-tools-2.1.8/aegis/templates/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3083 2023-03-11 00:56:38.000000 aegis-tools-2.1.8/aegis/templates/build.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.1.8/aegis/templates/build_confirm.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.1.8/aegis/templates/build_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.1.8/aegis/templates/build_view.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.1.8/aegis/templates/error_message.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3297 2023-04-27 02:34:36.000000 aegis-tools-2.1.8/aegis/templates/frame.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2107 2023-03-11 00:53:08.000000 aegis-tools-2.1.8/aegis/templates/hydra.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.1.8/aegis/templates/hydra_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1660 2023-03-11 00:55:55.000000 aegis-tools-2.1.8/aegis/templates/hydra_queue.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.1.8/aegis/templates/index.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.1.8/aegis/templates/report.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.1.8/aegis/templates/report_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.1.8/aegis/templates/reports.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.1.8/aegis/templates/w3.css
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.1.8/aegis/threadpool.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    73871 2023-07-05 19:06:45.000000 aegis-tools-2.1.8/aegis/webapp.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-07-05 19:07:39.679728 aegis-tools-2.1.8/aegis_tools.egg-info/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-07-05 19:07:39.000000 aegis-tools-2.1.8/aegis_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2023-07-05 19:07:39.000000 aegis-tools-2.1.8/aegis_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2023-07-05 19:07:39.000000 aegis-tools-2.1.8/aegis_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2023-07-05 19:07:39.000000 aegis-tools-2.1.8/aegis_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2023-07-05 19:07:39.000000 aegis-tools-2.1.8/aegis_tools.egg-info/requires.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2023-07-05 19:07:39.000000 aegis-tools-2.1.8/aegis_tools.egg-info/top_level.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2023-07-05 19:07:39.679728 aegis-tools-2.1.8/setup.cfg
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1676 2023-07-05 19:07:14.000000 aegis-tools-2.1.8/setup.py
```

### Comparing `aegis-tools-2.1.7/LICENSE` & `aegis-tools-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/PKG-INFO` & `aegis-tools-2.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.1.7
+Version: 2.1.8
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.1.7/README.md` & `aegis-tools-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/aegis_.py` & `aegis-tools-2.1.8/aegis/aegis_.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/build.py` & `aegis-tools-2.1.8/aegis/build.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/config.py` & `aegis-tools-2.1.8/aegis/config.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/database.py` & `aegis-tools-2.1.8/aegis/database.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/hydra.py` & `aegis-tools-2.1.8/aegis/hydra.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/mailer.py` & `aegis-tools-2.1.8/aegis/mailer.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/model.py` & `aegis-tools-2.1.8/aegis/model.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/sql/auditing-mysql.sql` & `aegis-tools-2.1.8/aegis/sql/auditing-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/sql/auditing-pgsql.sql` & `aegis-tools-2.1.8/aegis/sql/auditing-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/sql/build-mysql.sql` & `aegis-tools-2.1.8/aegis/sql/build-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/sql/build-pgsql.sql` & `aegis-tools-2.1.8/aegis/sql/build-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/sql/email_system-pgsql.sql` & `aegis-tools-2.1.8/aegis/sql/email_system-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/sql/google_signin.sql` & `aegis-tools-2.1.8/aegis/sql/google_signin.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/sql/hydra-mysql.sql` & `aegis-tools-2.1.8/aegis/sql/hydra-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/sql/hydra-pgsql.sql` & `aegis-tools-2.1.8/aegis/sql/hydra-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/sql/member_auth.sql` & `aegis-tools-2.1.8/aegis/sql/member_auth.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/sql/monitor-mysql.sql` & `aegis-tools-2.1.8/aegis/sql/monitor-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/sql/reports.sql` & `aegis-tools-2.1.8/aegis/sql/reports.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/stdlib.py` & `aegis-tools-2.1.8/aegis/stdlib.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/templates/build.html` & `aegis-tools-2.1.8/aegis/templates/build.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/templates/build_confirm.html` & `aegis-tools-2.1.8/aegis/templates/build_confirm.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/templates/build_form.html` & `aegis-tools-2.1.8/aegis/templates/build_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/templates/build_view.html` & `aegis-tools-2.1.8/aegis/templates/build_view.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/templates/frame.html` & `aegis-tools-2.1.8/aegis/templates/frame.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/templates/hydra.html` & `aegis-tools-2.1.8/aegis/templates/hydra.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/templates/hydra_form.html` & `aegis-tools-2.1.8/aegis/templates/hydra_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/templates/hydra_queue.html` & `aegis-tools-2.1.8/aegis/templates/hydra_queue.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/templates/report.html` & `aegis-tools-2.1.8/aegis/templates/report.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/templates/report_form.html` & `aegis-tools-2.1.8/aegis/templates/report_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/templates/reports.html` & `aegis-tools-2.1.8/aegis/templates/reports.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/templates/w3.css` & `aegis-tools-2.1.8/aegis/templates/w3.css`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/threadpool.py` & `aegis-tools-2.1.8/aegis/threadpool.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/aegis/webapp.py` & `aegis-tools-2.1.8/aegis/webapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,14 +242,15 @@
         return bool(self.tmpl['user_agent_obj'].is_bot or aegis.stdlib.is_robot(self.tmpl['user_agent']))
 
     def get_template_path(self):
         return options.template_path
 
     def render(self, template_name, **kwargs):
         aegis.stdlib.timer_start(self.timer_obj, 'render')
+        # XXX template_path seems unused...
         template_path = self.tmpl['host_config'].get('template_path') or options.template_path
         template_path = os.path.join(template_path, template_name)
         # Override parent class render to remove the embeds and instrument a timer here. Copied in from tornado/web.py render()
         if self._finished:
             raise RuntimeError("Cannot render() after finish()")
         html = self.render_string(template_name, **kwargs)
         aegis.stdlib.timer_stop(self.timer_obj, 'render')
@@ -274,27 +275,27 @@
         if self.request.headers.get('Cookie'):
             del self.request.headers['Cookie']
         # Don't post boring pseudo-errors to channels
         if isinstance(ex, tornado.web.HTTPError) and ex.status_code == 400 and 'No CSRF token in Cookie' in ex.log_message:
             #logging.warning("Prevent CSRF token errors from POSTing to Chat")
             super(AegisHandler, self)._handle_request_exception(ex)
             return
-        if isinstance(ex, tornado.web.HTTPError) and ex.status_code in [401, 403, 404, 405]:
+        if isinstance(ex, tornado.web.HTTPError) and ex.status_code in [401, 403, 404, 405, 410]:
             logging.warning("Prevent annoying errors from POSTing to Chat")
             super(AegisHandler, self)._handle_request_exception(ex)
             return
 
         # Send errors to chat hooks, based on them being configured for the environment
         header = "`[%s ENV   %s   %s   uid: %s   mid: %s]`" % (config.get_env().upper(), self.request.uri, self.tmpl['request_name'], self.get_user_id() or '-', self.get_member_id() or '-')
         template_opts = {'handler': self, 'traceback': traceback.format_exc(), 'kwargs': {}, 'header': header}
         template_opts['kwargs']['user_agent'] = self.tmpl['user_agent']
         template_opts['kwargs']['remote_ip'] = self.request.remote_ip
         if hasattr(self, 'audit_request'):
-            template_opts['kwargs']['country_cd'] = self.audit_request['country_cd']
-            template_opts['kwargs']['region_cd'] = self.audit_request['region_cd']
+            template_opts['kwargs']['country_cd'] = self.audit_request.get('country_cd', 'N/A')
+            template_opts['kwargs']['region_cd'] = self.audit_request.get('region_cd', 'N/A')
         if hasattr(self, 'audit_session'):
             template_opts['kwargs']['audit_session_id'] = self.audit_session.get('audit_session_id')
         template_opts['kwargs']['robot'] = self.user_is_robot()
         template_opts['kwargs']['Python UTC Now'] = self.tmpl['utcnow'].strftime('%Y-%m-%dT%H:%M:%S')
         error_message = self.render_string("error_message.txt", **template_opts).decode('utf-8')
         if config.get_env() == 'prod':
             hooks = ['alerts_chat_hook']
```

### Comparing `aegis-tools-2.1.7/aegis_tools.egg-info/PKG-INFO` & `aegis-tools-2.1.8/aegis_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.1.7
+Version: 2.1.8
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.1.7/aegis_tools.egg-info/SOURCES.txt` & `aegis-tools-2.1.8/aegis_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.7/setup.py` & `aegis-tools-2.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 
 import os
 import setuptools
 
 setuptools.setup (
     name = 'aegis-tools',
-    version = '2.1.7',
+    version = '2.1.8',
     description = 'Aegis is a set of battle-tested tools and tricks to help everyone make better software',
     long_description = 'A combination of tools and framework, Aegis has multiple different uses. You can import it and use the thoroughly made and tested functions. You can use it as a natural extension for the tornado web framework. And you can use it to quickly create a new web application with the structure already built-in, and follow along.',
     author = "Michael D'Agosta",
     author_email = 'mdagosta@codebug.com',
     url = 'https://github.com/mdagosta/aegis',
     python_requires='>=3.6',
     packages = ['aegis'],
```

