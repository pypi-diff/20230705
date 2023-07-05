# Comparing `tmp/dalec-0.2.0.tar.gz` & `tmp/dalec-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalec-0.2.0.tar", last modified: Thu Jun 29 08:11:21 2023, max compression
+gzip compressed data, was "dalec-0.2.1.tar", last modified: Wed Jul  5 11:32:49 2023, max compression
```

## Comparing `dalec-0.2.0.tar` & `dalec-0.2.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.695129 dalec-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-29 08:11:08.000000 dalec-0.2.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-29 08:11:08.000000 dalec-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-29 08:11:08.000000 dalec-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-06-29 08:11:21.695129 dalec-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-06-29 08:11:08.000000 dalec-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.687129 dalec-0.2.0/dalec/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.683129 dalec-0.2.0/dalec/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.683129 dalec-0.2.0/dalec/locale/dalek/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.687129 dalec-0.2.0/dalec/locale/dalek/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec/locale/dalek/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec/locale/dalek/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.683129 dalec-0.2.0/dalec/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.687129 dalec-0.2.0/dalec/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.683129 dalec-0.2.0/dalec/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.687129 dalec-0.2.0/dalec/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11878 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.683129 dalec-0.2.0/dalec/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.683129 dalec-0.2.0/dalec/static/dalec/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.691129 dalec-0.2.0/dalec/static/dalec/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec/static/dalec/js/main.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.683129 dalec-0.2.0/dalec/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.683129 dalec-0.2.0/dalec/templates/dalec/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.691129 dalec-0.2.0/dalec/templates/dalec/default/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec/templates/dalec/default/item.html
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec/templates/dalec/default/list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.691129 dalec-0.2.0/dalec/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec/templatetags/dalec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec/tests_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.687129 dalec-0.2.0/dalec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-06-29 08:11:21.000000 dalec-0.2.0/dalec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-29 08:11:21.000000 dalec-0.2.0/dalec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:11:21.000000 dalec-0.2.0/dalec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:11:21.000000 dalec-0.2.0/dalec.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-29 08:11:21.000000 dalec-0.2.0/dalec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 08:11:21.000000 dalec-0.2.0/dalec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.691129 dalec-0.2.0/dalec_exemple/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec_exemple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec_exemple/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec_exemple/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.687129 dalec-0.2.0/dalec_exemple/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.687129 dalec-0.2.0/dalec_exemple/templates/dalec/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.691129 dalec-0.2.0/dalec_exemple/templates/dalec/exemple/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec_exemple/templates/dalec/exemple/french_educ-item.html
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec_exemple/templates/dalec/exemple/quarter-item.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.691129 dalec-0.2.0/dalec_prime/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec_prime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec_prime/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.691129 dalec-0.2.0/dalec_prime/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec_prime/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec_prime/migrations/0002_auto_20211109_1546.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec_prime/migrations/0003_auto_20211109_1615.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec_prime/migrations/0004_alter_content_id_alter_fetchhistory_id.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec_prime/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-29 08:11:08.000000 dalec-0.2.0/dalec_prime/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-29 08:11:21.695129 dalec-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-29 08:11:08.000000 dalec-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.691129 dalec-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:08.000000 dalec-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-29 08:11:08.000000 dalec-0.2.0/tests/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-29 08:11:08.000000 dalec-0.2.0/tests/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:21.695129 dalec-0.2.0/tests/proxies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:11:08.000000 dalec-0.2.0/tests/proxies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-29 08:11:08.000000 dalec-0.2.0/tests/proxies/adiposian.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-29 08:11:08.000000 dalec-0.2.0/tests/proxies/bad_wolf.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-29 08:11:08.000000 dalec-0.2.0/tests/proxies/empty_child.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-29 08:11:08.000000 dalec-0.2.0/tests/proxies/nice_dalek.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-29 08:11:08.000000 dalec-0.2.0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    21659 2023-06-29 08:11:08.000000 dalec-0.2.0/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-29 08:11:08.000000 dalec-0.2.0/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.424842 dalec-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-05 11:32:40.000000 dalec-0.2.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-05 11:32:40.000000 dalec-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-05 11:32:40.000000 dalec-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-07-05 11:32:49.424842 dalec-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-07-05 11:32:40.000000 dalec-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.416841 dalec-0.2.1/dalec/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.416841 dalec-0.2.1/dalec/locale/dalek/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec/locale/dalek/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/locale/dalek/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/locale/dalek/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.416841 dalec-0.2.1/dalec/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.416841 dalec-0.2.1/dalec/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.416841 dalec-0.2.1/dalec/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.416841 dalec-0.2.1/dalec/static/dalec/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec/static/dalec/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/static/dalec/js/main.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.416841 dalec-0.2.1/dalec/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.416841 dalec-0.2.1/dalec/templates/dalec/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec/templates/dalec/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/templates/dalec/default/item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/templates/dalec/default/list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/templatetags/dalec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/tests_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-07-05 11:32:49.000000 dalec-0.2.1/dalec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-05 11:32:49.000000 dalec-0.2.1/dalec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 11:32:49.000000 dalec-0.2.1/dalec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 11:32:49.000000 dalec-0.2.1/dalec.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-05 11:32:49.000000 dalec-0.2.1/dalec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 11:32:49.000000 dalec-0.2.1/dalec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec_example/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_example/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_example/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.416841 dalec-0.2.1/dalec_example/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.416841 dalec-0.2.1/dalec_example/templates/dalec/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec_example/templates/dalec/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_example/templates/dalec/example/french_educ-item.html
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_example/templates/dalec/example/quarter-item.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec_prime/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_prime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_prime/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.420841 dalec-0.2.1/dalec_prime/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_prime/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_prime/migrations/0002_auto_20211109_1546.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_prime/migrations/0003_auto_20211109_1615.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_prime/migrations/0004_alter_content_id_alter_fetchhistory_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_prime/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-05 11:32:40.000000 dalec-0.2.1/dalec_prime/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-05 11:32:49.424842 dalec-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 11:32:40.000000 dalec-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.424842 dalec-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:49.424842 dalec-0.2.1/tests/proxies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/proxies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/proxies/adiposian.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/proxies/bad_wolf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/proxies/empty_child.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/proxies/nice_dalek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21659 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-05 11:32:40.000000 dalec-0.2.1/tests/urls.py
```

### Comparing `dalec-0.2.0/LICENSE` & `dalec-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dalec-0.2.0/PKG-INFO` & `dalec-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalec
-Version: 0.2.0
+Version: 0.2.1
 Summary: Extendable app to retrieve external contents from various external sources.
 Home-page: https://github.com/webu/dalec
 Author: Webu
 Author-email: contact@webu.coop
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/webu/dalec
 Project-URL: Tracker, https://github.com/webu/dalec/issues
@@ -32,14 +32,15 @@
 ![](https://img.shields.io/badge/python-3.7%20to%203.11-blue)
 ![](https://img.shields.io/badge/django-2.2%20to%204.2-blue)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![](https://img.shields.io/badge/coverage-100%25-green)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![semver](https://img.shields.io/badge/semver-2.0.0-green)](https://semver.org/)
+[![Documentation Status](https://readthedocs.org/projects/dalec/badge/?version=latest)](https://dalec.readthedocs.io/en/latest/?badge=latest)
 
 Django Aggregator of a Lot of External Contents (DALEC) is a generic app to aggregate contents from various
 external sources. Purposes are to manage (retrieve, clean, display…) those contents in a
 generic way independent of the source.
 
 
 It's designed to be customized / extended to fit your needs.
@@ -67,15 +68,15 @@
 Contents are categorized via :
 
 * `app`: the app which is requested to retrieve contents 
   (eg. `gitlab`)
 * `content_type`: the type of contents we want to retrieve from this app 
   (eg. `issue`, `activity`, `commit`, `merge requests`…)
 * `channel`: some apps can be requested to get a more or less filtered contents. 
-  For exemple, in Gitlab, it's called "scope". You can retrieve issues from:
+  For example, in Gitlab, it's called "scope". You can retrieve issues from:
   * the whole site (`channel=None` and `channel_object=None` for us)
   * a specific group (`channel="group"` and `channel_object="<gitlab_group_id>"`)
   * a specific project (`channel="project"` and `channel_object="<gitlab_project_id>"`)
   * a specific author (`channel="author"` and `channel_object="<gitlab_user_id>"`)
   * a specific assignee (`channel="assignee"` and `channel_object="<gitlab_user_id>"`)
   * etc.
 * `channel_object`: the ID (for the app requested) of the channel's related object
@@ -118,15 +119,15 @@
 
 If you are using Django older than 3.1, the JSONField is provided from 
 [django-jsonfield-backport](https://pypi.org/project/django-jsonfield-backport/). 
 For 3.1+, you **MUST** use a DB supporting the official
 [django's `JSONField`](https://docs.djangoproject.com/fr/3.1/ref/models/fields/#jsonfield).
 
 You **SHOULD NOT** install this app but you **SHOULD** install one (or more) of it's children 
-(see [external sources supported](#External-sources-supported)). eg:
+(see [](#external-sources-supported)). eg:
 
 `pip install dalec-gitlab dalec-nextcloud`
 
 Then, add `dalec`, `dalec_prime` and dalec's children to `INSTALLED_APPS` in `settings.py`:
 
 ```python
 # settings.py
@@ -164,15 +165,15 @@
 template by using the templatetag `dalec`:
 
 ```django
 {% load dalec %}
 
 {% dalec app content_type [channel=None] [channel_object=None] [template=None] [ordered_by=None] %}
 
-real exemples:
+real examples:
 
 Retrieves last gitlab issues for a specific user:
 {% dalec "gitlab" "issue" channel="user" channel_object="doctor-who" %}
 
 Retrieves recent gitlab event for a group:
 {% dalec "gitlab" "event" channel="group" channel_object='42' %}
 
@@ -186,49 +187,49 @@
 {% dalec "gitlab" "issue" channel="project" channel_objects='["42","443"]' %}
 
 Retrieves recent gitlab issues for multiple projects and order them by descending
 issue internal ID (default is `last_update_dt`):
 {% dalec "gitlab" "issue" channel="project" channel_object='42' ordered_by="-iid" %}
 ```
 
-### dalec_exemple
+### dalec_example
 
 An example app is packaged to get a working example which does not require any extra configuration.
 
-* add `dalec_exemple`, `dalec_prime` and `dalec` to `INSTALLED_APPS`
+* add `dalec_example`, `dalec_prime` and `dalec` to `INSTALLED_APPS`
 * run migrations
 * include dalec.urls inside your project's urls
-* add `dalec/main.js` inside your base.html or inside the template where you want to display the example
+* add `dalec/js/main.js` inside your base.html or inside the template where you want to display the example
 * add those fragments of code inside the template where you want to display the example:
 
 ```django
 {% load dalec %}
 <h1>Last quarters (very usefull, isn't it ?)</h1>
-{% dalec "exemple" "quarter" %}
+{% dalec "example" "quarter" %}
 
 <h1>Last updated establishments of french national education</h1>
-{% dalec "exemple" "french_educ" %}
+{% dalec "example" "french_educ" %}
 
 <h1>Last updated establishments of french national education depending of the Academy of Grenoble</h1>
-{% dalec "exemple" "french_educ" channel="academy" channel_object="Grenoble" %}
+{% dalec "example" "french_educ" channel="academy" channel_object="Grenoble" %}
 ```
 
 
 ## Configuration
 
 This app have general settings which can be erased for all of it's children and sometimes by 
 content type.
 
 * General setting format : `DALEC_SOMETHING`
-* override child version (it's app name, like gitlab for exemple): `DALEC_GITLAB_SOMETHING`
-* override content type version (gitlab's issues for exemple): `DALEC_GITLAB_ISSUE_SOMETHING`
+* override child version (it's app name, like gitlab for example): `DALEC_GITLAB_SOMETHING`
+* override content type version (gitlab's issues for example): `DALEC_GITLAB_ISSUE_SOMETHING`
 
 ### DALEC_NB_CONTENTS_KEPT
 
-* * *default*: `10`
+* *default*: `10`
 * per child app setting: yes
 * per child app's content type setting: yes
 
 Set the number of contents to keep by type. Oldest will be purged to keep only the last X contents 
 of each channel and type.
 `0` means "no limit".
```

### Comparing `dalec-0.2.0/README.md` & `dalec-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 ![](https://img.shields.io/badge/python-3.7%20to%203.11-blue)
 ![](https://img.shields.io/badge/django-2.2%20to%204.2-blue)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![](https://img.shields.io/badge/coverage-100%25-green)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![semver](https://img.shields.io/badge/semver-2.0.0-green)](https://semver.org/)
+[![Documentation Status](https://readthedocs.org/projects/dalec/badge/?version=latest)](https://dalec.readthedocs.io/en/latest/?badge=latest)
 
 Django Aggregator of a Lot of External Contents (DALEC) is a generic app to aggregate contents from various
 external sources. Purposes are to manage (retrieve, clean, display…) those contents in a
 generic way independent of the source.
 
 
 It's designed to be customized / extended to fit your needs.
@@ -39,15 +40,15 @@
 Contents are categorized via :
 
 * `app`: the app which is requested to retrieve contents 
   (eg. `gitlab`)
 * `content_type`: the type of contents we want to retrieve from this app 
   (eg. `issue`, `activity`, `commit`, `merge requests`…)
 * `channel`: some apps can be requested to get a more or less filtered contents. 
-  For exemple, in Gitlab, it's called "scope". You can retrieve issues from:
+  For example, in Gitlab, it's called "scope". You can retrieve issues from:
   * the whole site (`channel=None` and `channel_object=None` for us)
   * a specific group (`channel="group"` and `channel_object="<gitlab_group_id>"`)
   * a specific project (`channel="project"` and `channel_object="<gitlab_project_id>"`)
   * a specific author (`channel="author"` and `channel_object="<gitlab_user_id>"`)
   * a specific assignee (`channel="assignee"` and `channel_object="<gitlab_user_id>"`)
   * etc.
 * `channel_object`: the ID (for the app requested) of the channel's related object
@@ -90,15 +91,15 @@
 
 If you are using Django older than 3.1, the JSONField is provided from 
 [django-jsonfield-backport](https://pypi.org/project/django-jsonfield-backport/). 
 For 3.1+, you **MUST** use a DB supporting the official
 [django's `JSONField`](https://docs.djangoproject.com/fr/3.1/ref/models/fields/#jsonfield).
 
 You **SHOULD NOT** install this app but you **SHOULD** install one (or more) of it's children 
-(see [external sources supported](#External-sources-supported)). eg:
+(see [](#external-sources-supported)). eg:
 
 `pip install dalec-gitlab dalec-nextcloud`
 
 Then, add `dalec`, `dalec_prime` and dalec's children to `INSTALLED_APPS` in `settings.py`:
 
 ```python
 # settings.py
@@ -136,15 +137,15 @@
 template by using the templatetag `dalec`:
 
 ```django
 {% load dalec %}
 
 {% dalec app content_type [channel=None] [channel_object=None] [template=None] [ordered_by=None] %}
 
-real exemples:
+real examples:
 
 Retrieves last gitlab issues for a specific user:
 {% dalec "gitlab" "issue" channel="user" channel_object="doctor-who" %}
 
 Retrieves recent gitlab event for a group:
 {% dalec "gitlab" "event" channel="group" channel_object='42' %}
 
@@ -158,49 +159,49 @@
 {% dalec "gitlab" "issue" channel="project" channel_objects='["42","443"]' %}
 
 Retrieves recent gitlab issues for multiple projects and order them by descending
 issue internal ID (default is `last_update_dt`):
 {% dalec "gitlab" "issue" channel="project" channel_object='42' ordered_by="-iid" %}
 ```
 
-### dalec_exemple
+### dalec_example
 
 An example app is packaged to get a working example which does not require any extra configuration.
 
-* add `dalec_exemple`, `dalec_prime` and `dalec` to `INSTALLED_APPS`
+* add `dalec_example`, `dalec_prime` and `dalec` to `INSTALLED_APPS`
 * run migrations
 * include dalec.urls inside your project's urls
-* add `dalec/main.js` inside your base.html or inside the template where you want to display the example
+* add `dalec/js/main.js` inside your base.html or inside the template where you want to display the example
 * add those fragments of code inside the template where you want to display the example:
 
 ```django
 {% load dalec %}
 <h1>Last quarters (very usefull, isn't it ?)</h1>
-{% dalec "exemple" "quarter" %}
+{% dalec "example" "quarter" %}
 
 <h1>Last updated establishments of french national education</h1>
-{% dalec "exemple" "french_educ" %}
+{% dalec "example" "french_educ" %}
 
 <h1>Last updated establishments of french national education depending of the Academy of Grenoble</h1>
-{% dalec "exemple" "french_educ" channel="academy" channel_object="Grenoble" %}
+{% dalec "example" "french_educ" channel="academy" channel_object="Grenoble" %}
 ```
 
 
 ## Configuration
 
 This app have general settings which can be erased for all of it's children and sometimes by 
 content type.
 
 * General setting format : `DALEC_SOMETHING`
-* override child version (it's app name, like gitlab for exemple): `DALEC_GITLAB_SOMETHING`
-* override content type version (gitlab's issues for exemple): `DALEC_GITLAB_ISSUE_SOMETHING`
+* override child version (it's app name, like gitlab for example): `DALEC_GITLAB_SOMETHING`
+* override content type version (gitlab's issues for example): `DALEC_GITLAB_ISSUE_SOMETHING`
 
 ### DALEC_NB_CONTENTS_KEPT
 
-* * *default*: `10`
+* *default*: `10`
 * per child app setting: yes
 * per child app's content type setting: yes
 
 Set the number of contents to keep by type. Oldest will be purged to keep only the last X contents 
 of each channel and type.
 `0` means "no limit".
```

### Comparing `dalec-0.2.0/dalec/locale/dalek/LC_MESSAGES/django.mo` & `dalec-0.2.1/dalec/locale/dalek/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dalec-0.2.0/dalec/locale/dalek/LC_MESSAGES/django.po` & `dalec-0.2.1/dalec/locale/dalek/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dalec-0.2.0/dalec/locale/en/LC_MESSAGES/django.mo` & `dalec-0.2.1/dalec/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dalec-0.2.0/dalec/locale/en/LC_MESSAGES/django.po` & `dalec-0.2.1/dalec/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dalec-0.2.0/dalec/locale/fr/LC_MESSAGES/django.mo` & `dalec-0.2.1/dalec/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dalec-0.2.0/dalec/locale/fr/LC_MESSAGES/django.po` & `dalec-0.2.1/dalec/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dalec-0.2.0/dalec/models.py` & `dalec-0.2.1/dalec/models.py`

 * *Files identical despite different names*

### Comparing `dalec-0.2.0/dalec/proxy.py` & `dalec-0.2.1/dalec/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,18 @@
                         ).format(app=app)
                     ) from e
                 else:
                     return cls.get(app, autoload=False)
             raise ValueError("No proxy registered for app {app}".format(app=app))
         return cls._proxies[app]
 
+    @classmethod
+    def get_registered_apps(cls) -> Tuple[str, ...]:
+        return tuple(cls._proxies.keys())
+
 
 class ProxyMeta(type):
     """
     Meta class to autoregister Proxy class when an app inherit from our Proxy abstact class.
     """
 
     def __new__(
@@ -237,17 +241,18 @@
     def _fetch(
         self, nb: int, content_type: str, channel: str, channel_object: str
     ) -> Dict[str, dict]:
         """
         Fetch updated contents from the source and return it as a dict of dict:
         main dict keys MUST be the app's content id, and value must be the content representation
         with at least three required attrs:
-            id: ID of the content inside the external app
-            last_update_dt: last update datetime inside the external app
-            creation_dt: creation datetime inside the external app
+
+        - `id`: ID of the content inside the external app
+        - `last_update_dt`: last update datetime inside the external app
+        - `creation_dt`: creation datetime inside the external app
         """
         raise NotImplementedError(
             "You MUST implement your own _feth method depending your external source"
         )
 
     def get_contents_queryset(
         self, content_type: str, channel: str, channel_object: str
```

### Comparing `dalec-0.2.0/dalec/settings.py` & `dalec-0.2.1/dalec/settings.py`

 * *Files identical despite different names*

### Comparing `dalec-0.2.0/dalec/static/dalec/js/main.js` & `dalec-0.2.1/dalec/static/dalec/js/main.js`

 * *Files identical despite different names*

### Comparing `dalec-0.2.0/dalec/templates/dalec/default/list.html` & `dalec-0.2.1/dalec/templates/dalec/default/list.html`

 * *Files identical despite different names*

### Comparing `dalec-0.2.0/dalec/templatetags/dalec.py` & `dalec-0.2.1/dalec/templatetags/dalec.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     channel_object: Optional[str] = None,
     channel_objects: Optional[str] = None,
     template: Optional[str] = None,
     ordered_by: Optional[str] = None,
 ) -> str:
     """
     Show last N contents for a specific app+content_type (and optionnaly channel+channel_object)
-    Usage exemple:
+    Usage example:
 
     {% load dalec %}
 
     Retrieves last gitlab issues for a specific user:
     {% dalec "gitlab" "issue" channel="user" channel_object="doctor-who" %}
 
     Retrieves recent gitlab event for a group:
```

### Comparing `dalec-0.2.0/dalec/tests_utils.py` & `dalec-0.2.1/dalec/tests_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from importlib import reload
 
 from django.apps import apps
 
 from dalec import settings as app_settings
+from dalec.proxy import ProxyPool
 
 
 class DalecTestCaseMixin:
     def tearDown(self) -> None:
         """
         reload settings after a test which could have overrided settings
         """
@@ -16,14 +17,21 @@
     def content_model(self) -> app_settings.CONTENT_MODEL:
         return apps.get_model(app_settings.CONTENT_MODEL)
 
     @property
     def fetch_history_model(self) -> app_settings.FETCH_HISTORY_MODEL:
         return apps.get_model(app_settings.FETCH_HISTORY_MODEL)
 
+    def test_invalid_fetch(self) -> None:
+        apps = ProxyPool.get_registered_apps()
+        for app in apps:
+            proxy = ProxyPool.get(app)
+            with self.assertRaises(ValueError):  # type: ignore
+                proxy.refresh(content_type="dr_who_name")
+
     def test_ze_final_test(self) -> None:
         print("\n\033[0;32mNothing destroyed… \033[0;33mAnormal for Daleks!\033[31;5m")
         print("+" + "-" * 61 + "+")
         print("| " + ("Daleks conquer and destroy!!! " * 2) + "|")
         print("+" + "-" * 61 + "+")
         print(
             """                    /\033[0m\033[0;33m
```

### Comparing `dalec-0.2.0/dalec/views.py` & `dalec-0.2.1/dalec/views.py`

 * *Files identical despite different names*

### Comparing `dalec-0.2.0/dalec.egg-info/PKG-INFO` & `dalec-0.2.1/dalec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalec
-Version: 0.2.0
+Version: 0.2.1
 Summary: Extendable app to retrieve external contents from various external sources.
 Home-page: https://github.com/webu/dalec
 Author: Webu
 Author-email: contact@webu.coop
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/webu/dalec
 Project-URL: Tracker, https://github.com/webu/dalec/issues
@@ -32,14 +32,15 @@
 ![](https://img.shields.io/badge/python-3.7%20to%203.11-blue)
 ![](https://img.shields.io/badge/django-2.2%20to%204.2-blue)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![](https://img.shields.io/badge/coverage-100%25-green)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![semver](https://img.shields.io/badge/semver-2.0.0-green)](https://semver.org/)
+[![Documentation Status](https://readthedocs.org/projects/dalec/badge/?version=latest)](https://dalec.readthedocs.io/en/latest/?badge=latest)
 
 Django Aggregator of a Lot of External Contents (DALEC) is a generic app to aggregate contents from various
 external sources. Purposes are to manage (retrieve, clean, display…) those contents in a
 generic way independent of the source.
 
 
 It's designed to be customized / extended to fit your needs.
@@ -67,15 +68,15 @@
 Contents are categorized via :
 
 * `app`: the app which is requested to retrieve contents 
   (eg. `gitlab`)
 * `content_type`: the type of contents we want to retrieve from this app 
   (eg. `issue`, `activity`, `commit`, `merge requests`…)
 * `channel`: some apps can be requested to get a more or less filtered contents. 
-  For exemple, in Gitlab, it's called "scope". You can retrieve issues from:
+  For example, in Gitlab, it's called "scope". You can retrieve issues from:
   * the whole site (`channel=None` and `channel_object=None` for us)
   * a specific group (`channel="group"` and `channel_object="<gitlab_group_id>"`)
   * a specific project (`channel="project"` and `channel_object="<gitlab_project_id>"`)
   * a specific author (`channel="author"` and `channel_object="<gitlab_user_id>"`)
   * a specific assignee (`channel="assignee"` and `channel_object="<gitlab_user_id>"`)
   * etc.
 * `channel_object`: the ID (for the app requested) of the channel's related object
@@ -118,15 +119,15 @@
 
 If you are using Django older than 3.1, the JSONField is provided from 
 [django-jsonfield-backport](https://pypi.org/project/django-jsonfield-backport/). 
 For 3.1+, you **MUST** use a DB supporting the official
 [django's `JSONField`](https://docs.djangoproject.com/fr/3.1/ref/models/fields/#jsonfield).
 
 You **SHOULD NOT** install this app but you **SHOULD** install one (or more) of it's children 
-(see [external sources supported](#External-sources-supported)). eg:
+(see [](#external-sources-supported)). eg:
 
 `pip install dalec-gitlab dalec-nextcloud`
 
 Then, add `dalec`, `dalec_prime` and dalec's children to `INSTALLED_APPS` in `settings.py`:
 
 ```python
 # settings.py
@@ -164,15 +165,15 @@
 template by using the templatetag `dalec`:
 
 ```django
 {% load dalec %}
 
 {% dalec app content_type [channel=None] [channel_object=None] [template=None] [ordered_by=None] %}
 
-real exemples:
+real examples:
 
 Retrieves last gitlab issues for a specific user:
 {% dalec "gitlab" "issue" channel="user" channel_object="doctor-who" %}
 
 Retrieves recent gitlab event for a group:
 {% dalec "gitlab" "event" channel="group" channel_object='42' %}
 
@@ -186,49 +187,49 @@
 {% dalec "gitlab" "issue" channel="project" channel_objects='["42","443"]' %}
 
 Retrieves recent gitlab issues for multiple projects and order them by descending
 issue internal ID (default is `last_update_dt`):
 {% dalec "gitlab" "issue" channel="project" channel_object='42' ordered_by="-iid" %}
 ```
 
-### dalec_exemple
+### dalec_example
 
 An example app is packaged to get a working example which does not require any extra configuration.
 
-* add `dalec_exemple`, `dalec_prime` and `dalec` to `INSTALLED_APPS`
+* add `dalec_example`, `dalec_prime` and `dalec` to `INSTALLED_APPS`
 * run migrations
 * include dalec.urls inside your project's urls
-* add `dalec/main.js` inside your base.html or inside the template where you want to display the example
+* add `dalec/js/main.js` inside your base.html or inside the template where you want to display the example
 * add those fragments of code inside the template where you want to display the example:
 
 ```django
 {% load dalec %}
 <h1>Last quarters (very usefull, isn't it ?)</h1>
-{% dalec "exemple" "quarter" %}
+{% dalec "example" "quarter" %}
 
 <h1>Last updated establishments of french national education</h1>
-{% dalec "exemple" "french_educ" %}
+{% dalec "example" "french_educ" %}
 
 <h1>Last updated establishments of french national education depending of the Academy of Grenoble</h1>
-{% dalec "exemple" "french_educ" channel="academy" channel_object="Grenoble" %}
+{% dalec "example" "french_educ" channel="academy" channel_object="Grenoble" %}
 ```
 
 
 ## Configuration
 
 This app have general settings which can be erased for all of it's children and sometimes by 
 content type.
 
 * General setting format : `DALEC_SOMETHING`
-* override child version (it's app name, like gitlab for exemple): `DALEC_GITLAB_SOMETHING`
-* override content type version (gitlab's issues for exemple): `DALEC_GITLAB_ISSUE_SOMETHING`
+* override child version (it's app name, like gitlab for example): `DALEC_GITLAB_SOMETHING`
+* override content type version (gitlab's issues for example): `DALEC_GITLAB_ISSUE_SOMETHING`
 
 ### DALEC_NB_CONTENTS_KEPT
 
-* * *default*: `10`
+* *default*: `10`
 * per child app setting: yes
 * per child app's content type setting: yes
 
 Set the number of contents to keep by type. Oldest will be purged to keep only the last X contents 
 of each channel and type.
 `0` means "no limit".
```

### Comparing `dalec-0.2.0/dalec.egg-info/SOURCES.txt` & `dalec-0.2.1/dalec.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 dalec/locale/fr/LC_MESSAGES/django.mo
 dalec/locale/fr/LC_MESSAGES/django.po
 dalec/static/dalec/js/main.js
 dalec/templates/dalec/default/item.html
 dalec/templates/dalec/default/list.html
 dalec/templatetags/__init__.py
 dalec/templatetags/dalec.py
-dalec_exemple/__init__.py
-dalec_exemple/apps.py
-dalec_exemple/proxy.py
-dalec_exemple/templates/dalec/exemple/french_educ-item.html
-dalec_exemple/templates/dalec/exemple/quarter-item.html
+dalec_example/__init__.py
+dalec_example/apps.py
+dalec_example/proxy.py
+dalec_example/templates/dalec/example/french_educ-item.html
+dalec_example/templates/dalec/example/quarter-item.html
 dalec_prime/__init__.py
 dalec_prime/apps.py
 dalec_prime/models.py
 dalec_prime/migrations/0001_initial.py
 dalec_prime/migrations/0002_auto_20211109_1546.py
 dalec_prime/migrations/0003_auto_20211109_1615.py
 dalec_prime/migrations/0004_alter_content_id_alter_fetchhistory_id.py
```

### Comparing `dalec-0.2.0/dalec_exemple/proxy.py` & `dalec-0.2.1/dalec_example/proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 
 from django.utils.dateparse import parse_datetime
 from django.utils.timezone import make_aware
 from django.utils.timezone import now
 
 from dalec.proxy import Proxy
 
-__all__ = ["ExempleProxy"]
+__all__ = ["ExampleProxy"]
 
 
-class ExempleProxy(Proxy):
+class ExampleProxy(Proxy):
     """
-    Just a proxy exemple wich just fetch the last :
+    Just a proxy example wich just fetch the last :
     * quarter: quarters or halfs of an hour from "now" or from a specific datetime
     * french_educ: last updated establishments of french national education. Available channels:
         * academy: retrieve for a specific academy name (eg: « Grenoble »)
     """
 
-    app = "exemple"
+    app = "example"
 
     def _fetch(
         self, nb: int, content_type: str, channel: str, channel_object: str
     ) -> Dict[str, dict]:
         if content_type == "hour":
             if not channel or channel not in ("quarter", "half"):
                 raise ValueError(
```

### Comparing `dalec-0.2.0/dalec_exemple/templates/dalec/exemple/french_educ-item.html` & `dalec-0.2.1/dalec_example/templates/dalec/example/french_educ-item.html`

 * *Files identical despite different names*

### Comparing `dalec-0.2.0/dalec_prime/migrations/0001_initial.py` & `dalec-0.2.1/dalec_prime/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dalec-0.2.0/dalec_prime/migrations/0002_auto_20211109_1546.py` & `dalec-0.2.1/dalec_prime/migrations/0002_auto_20211109_1546.py`

 * *Files identical despite different names*

### Comparing `dalec-0.2.0/dalec_prime/migrations/0003_auto_20211109_1615.py` & `dalec-0.2.1/dalec_prime/migrations/0003_auto_20211109_1615.py`

 * *Files identical despite different names*

### Comparing `dalec-0.2.0/dalec_prime/migrations/0004_alter_content_id_alter_fetchhistory_id.py` & `dalec-0.2.1/dalec_prime/migrations/0004_alter_content_id_alter_fetchhistory_id.py`

 * *Files identical despite different names*

### Comparing `dalec-0.2.0/setup.cfg` & `dalec-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dalec-0.2.0/tests/settings.py` & `dalec-0.2.1/tests/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 INSTALLED_APPS = [
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.staticfiles",
     "tests",
-    "dalec_exemple",
+    "dalec_example",
     "dalec_prime",
     "dalec",
 ]
 
 if django.VERSION < (3, 2):
     INSTALLED_APPS.append("django_jsonfield_backport")
```

### Comparing `dalec-0.2.0/tests/tests.py` & `dalec-0.2.1/tests/tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,33 +19,33 @@
 from dalec.views import FetchContentView
 
 __all__ = ["DalecTests"]
 
 
 class DalecTests(DalecTestCaseMixin, TestCase):
     @override_settings(
-        DALEC_EXEMPLE_NB_CONTENTS_KEPT=15,
-        DALEC_EXEMPLE_FRENCH_EDUC_NB_CONTENTS_KEPT=20,
-        DALEC_EXEMPLE_CONTENT_TYPE_NB_CONTENTS_KEPT=30,
+        DALEC_EXAMPLE_NB_CONTENTS_KEPT=15,
+        DALEC_EXAMPLE_FRENCH_EDUC_NB_CONTENTS_KEPT=20,
+        DALEC_EXAMPLE_CONTENT_TYPE_NB_CONTENTS_KEPT=30,
     )
     def test_overrided_settings_app(self):
         """
         Test if settings overrided for a specific app is returned if set
         """
         reload(app_settings)
         self.assertEqual(app_settings.NB_CONTENTS_KEPT, 10)
-        self.assertEqual(app_settings.get_for("NB_CONTENTS_KEPT", "exemple"), 15)
+        self.assertEqual(app_settings.get_for("NB_CONTENTS_KEPT", "example"), 15)
         self.assertEqual(
-            app_settings.get_for("NB_CONTENTS_KEPT", "exemple", "quarter"), 15
+            app_settings.get_for("NB_CONTENTS_KEPT", "example", "quarter"), 15
         )
         self.assertEqual(
-            app_settings.get_for("NB_CONTENTS_KEPT", "exemple", "french_educ"), 20
+            app_settings.get_for("NB_CONTENTS_KEPT", "example", "french_educ"), 20
         )
         self.assertEqual(
-            app_settings.get_for("NB_CONTENTS_KEPT", "exemple", "content-type"), 30
+            app_settings.get_for("NB_CONTENTS_KEPT", "example", "content-type"), 30
         )
 
     @override_settings(
         INSTALLED_APPS=[app for app in settings.INSTALLED_APPS if app != "dalec_prime"]
     )
     def test_missing_dalec_prime_content_model(self):
         with self.assertRaisesRegex(
@@ -76,15 +76,15 @@
 
         content_model = apps.get_model(content_model)
         fetch_history_model = apps.get_model(fetch_history_model)
 
         self.assertEqual(content_model.objects.count(), 0)
         self.assertEqual(fetch_history_model.objects.count(), 0)
 
-        proxy = ProxyPool.get("exemple")
+        proxy = ProxyPool.get("example")
         created, updated, deleted = proxy.refresh("hour", "quarter")
 
         self.assertEqual(content_model.objects.count(), 10)
         self.assertEqual(fetch_history_model.objects.count(), 1)
 
     def test_setting_not_set(self):
         """
@@ -95,15 +95,15 @@
         self.assertIs(app_settings.get_setting("UNDEFINED", False), False)
         with self.assertRaises(ValueError):
             app_settings.get_setting("UNDEFINED", False, raise_if_not_set=True)
 
     @override_settings(DALEC_TTL=1)
     def test_proxy_fetch_and_ttl(self):
         reload(app_settings)
-        proxy = ProxyPool.get("exemple")
+        proxy = ProxyPool.get("example")
         created, updated, deleted = proxy.refresh("hour", "quarter")
         self.assertEqual(created, app_settings.NB_CONTENTS_KEPT)
         self.assertEqual(updated, 0)
         self.assertEqual(deleted, 0)
 
         # still alive
         created, updated, deleted = proxy.refresh("hour", "quarter")
@@ -119,15 +119,15 @@
         self.assertEqual(updated, app_settings.NB_CONTENTS_KEPT - created)
         self.assertEqual(deleted, created)
 
     def test_standard_template_tags_dalec(self):
         template = get_template("dalec_tests/test-quarter.html")
         url = reverse(
             "dalec_fetch_content",
-            kwargs={"app": "exemple", "content_type": "hour", "channel": "quarter"},
+            kwargs={"app": "example", "content_type": "hour", "channel": "quarter"},
         )
         # Check there is nothing returned because nothing has been retrieved yet
         output = template.render()
         soup = BeautifulSoup(output, "html.parser")
         divs = soup.find_all("div")
         self.assertEqual(len(divs), 1)
         self.assertEqual(divs[0].string.strip(), "")
@@ -140,25 +140,25 @@
         output = template.render()
         soup = BeautifulSoup(output, "html.parser")
         divs = soup.find_all("div")
         self.assertEqual(len(divs), 1)
         self.assertEqual(divs[0].string.strip(), "")
 
         # Let's query the external apps to fetch contents
-        proxy = ProxyPool.get("exemple")
+        proxy = ProxyPool.get("example")
         created, updated, deleted = proxy.refresh("hour", "quarter")
         self.assertEqual(created, 10)
         output = template.render()
         soup = BeautifulSoup(output, "html.parser")
         divs = soup.find_all("div")
         self.assertEqual(len(divs), 1 + created)
 
         div_item = divs[1]
         self.assertEqual(div_item.attrs["class"], ["dalec-item"])
-        self.assertEqual(div_item.attrs["data-app"], "exemple")
+        self.assertEqual(div_item.attrs["data-app"], "example")
         self.assertEqual(div_item.attrs["data-content-type"], "hour")
         self.assertEqual(div_item.attrs["data-channel"], "quarter")
         self.assertNotIn("data-channel-object", div_item.attrs)
         last_quarter = self.content_model.objects.latest()
         self.assertEqual(div_item.string.strip(), last_quarter.content_data["id"])
 
     def test_standard_template_tags_to_datetime(self):
@@ -195,34 +195,34 @@
             output = t.render(c)
 
         t = Template("""{% load dalec %}{{ str_now|to_datetime:format }}""")
         with self.assertRaisesRegex(ValueError, "No given format matching"):
             output = t.render(c)
 
     def test_proxy_fetch_with_channel_object(self):
-        proxy = ProxyPool.get("exemple")
+        proxy = ProxyPool.get("example")
         created, updated, deleted = proxy.refresh("hour", "quarter")
         self.assertEqual(created, app_settings.NB_CONTENTS_KEPT)
         self.assertEqual(updated, 0)
         self.assertEqual(deleted, 0)
 
-        proxy = ProxyPool.get("exemple")
+        proxy = ProxyPool.get("example")
         channel_object = "1985-07-02 21:45:00Z"
         created, updated, deleted = proxy.refresh("hour", "quarter", channel_object)
         self.assertEqual(created, app_settings.NB_CONTENTS_KEPT)
         self.assertEqual(updated, 0)
         self.assertEqual(deleted, 0)
 
         all_contents = self.content_model.objects.all()
         self.assertEqual(all_contents.count(), 20)
         self.assertEqual(all_contents.filter(channel_object=None).count(), 10)
         self.assertEqual(all_contents.filter(channel_object=channel_object).count(), 10)
 
     def test_ordering_and_latest(self):
-        proxy = ProxyPool.get("exemple")
+        proxy = ProxyPool.get("example")
         created, updated, deleted = proxy.refresh(
             "hour", "quarter", "1985-07-02 21:45:00Z"
         )
         first_ordered = self.content_model.objects.first()
         latest_chrono = self.content_model.objects.latest()
         self.assertEqual(first_ordered.pk, latest_chrono.pk)
         self.assertEqual(first_ordered.content_data["id"], "21h45")
@@ -241,30 +241,30 @@
         with self.assertRaisesRegex(ValueError, "already registered"):
             ProxyPool.register(AdiposianProxy)
 
         with self.assertRaises(NotImplementedError):
             AdiposianProxy().refresh("adipose")
 
     def test_proxy_pool_autoload(self):
-        proxy = ProxyPool.get("exemple")
-        from dalec_exemple.proxy import ExempleProxy
+        proxy = ProxyPool.get("example")
+        from dalec_example.proxy import ExampleProxy
 
-        self.assertTrue(isinstance(proxy, ExempleProxy))
+        self.assertTrue(isinstance(proxy, ExampleProxy))
 
-        exemple_proxy = ProxyPool.unregister("exemple")
-        self.assertEqual(exemple_proxy, proxy)
+        example_proxy = ProxyPool.unregister("example")
+        self.assertEqual(example_proxy, proxy)
 
         with self.assertRaisesRegex(ValueError, "No proxy registered"):
-            ProxyPool.get("exemple", autoload=False)
+            ProxyPool.get("example", autoload=False)
 
         with self.assertRaisesRegex(ValueError, "No proxy registered"):
-            ProxyPool.get("exemple")
+            ProxyPool.get("example")
 
-        ProxyPool.register(exemple_proxy)
-        self.assertEqual(ProxyPool.get("exemple"), proxy)
+        ProxyPool.register(example_proxy)
+        self.assertEqual(ProxyPool.get("example"), proxy)
 
         with self.assertRaisesRegex(ValueError, "impossible to autoload"):
             proxy = ProxyPool.get("weeping_angel")
 
     def test_proxy_special_case(self):
         from .proxies.nice_dalek import NiceDalek
 
@@ -285,15 +285,15 @@
             "nice": False,
         }
         fake_content_instance = self.content_model(content_data=copy(fake_content))
         res = proxy.update_content(fake_content_instance, fake_content)
         self.assertFalse(res)
 
     def test_view_response_code(self):
-        kwargs = {"app": "exemple", "content_type": "hour", "channel": "quarter"}
+        kwargs = {"app": "example", "content_type": "hour", "channel": "quarter"}
         url = reverse("dalec_fetch_content", kwargs=kwargs)
         client = Client()
         qs = self.content_model.objects.filter(**kwargs)
         self.assertEqual(qs.count(), 0)
 
         response = client.get(url)
         self.assertEqual(response.status_code, 200)
@@ -301,24 +301,24 @@
 
         response = client.get(url)
         self.assertEqual(response.status_code, 204)
         self.assertEqual(response.content, b"")
         self.assertEqual(qs.count(), 10)
 
     def test_view_custom_template(self):
-        kwargs = {"app": "exemple", "content_type": "hour", "channel": "quarter"}
+        kwargs = {"app": "example", "content_type": "hour", "channel": "quarter"}
         url = reverse("dalec_fetch_content", kwargs=kwargs)
         client = Client()
         response = client.get(url + "?template=faceof")
         self.assertEqual(response.status_code, 200)
         self.assertContains(response, "face of Boe")
 
     def test_view_channel_object(self):
         kwargs = {
-            "app": "exemple",
+            "app": "example",
             "content_type": "hour",
             "channel": "quarter",
             "channel_object": "1985-07-02 23:45:00Z",
         }
         url = reverse("dalec_fetch_content", kwargs=kwargs)
         client = Client()
         response = client.get(url)
@@ -327,51 +327,51 @@
         latest = self.content_model.objects.filter(**kwargs).latest()
         earliest = self.content_model.objects.filter(**kwargs).earliest()
         self.assertEqual(latest.content_data["id"], "23h45")
         self.assertEqual(earliest.content_data["id"], "21h30")
 
     def test_channel_object_too_long(self):
         kwargs = {
-            "app": "exemple",
+            "app": "example",
             "content_type": "hour",
             "channel": "quarter",
             "channel_object": "{:256s}".format("2021-12-24 12:00"),
         }
         url = reverse("dalec_fetch_content", kwargs=kwargs)
         client = Client()
         with self.assertRaisesRegex(ValidationError, "channel_object"):
             client.get(url)
 
     def test_multiple_channel_objects_request(self):
-        kwargs = {"app": "exemple", "content_type": "hour", "channel": "quarter"}
+        kwargs = {"app": "example", "content_type": "hour", "channel": "quarter"}
         url = reverse("dalec_fetch_content", kwargs=kwargs)
         client = Client()
         response = client.post(
             url,
             '{"channelObjects": ["2021-12-25 00:00", "2021-12-24 00:00"]}',
             content_type="application/json",
         )
         self.assertEqual(response.status_code, 200)
         qs = self.content_model.objects.filter(
-            app="exemple", content_type="hour", channel="quarter"
+            app="example", content_type="hour", channel="quarter"
         )
         self.assertEqual(qs.filter(channel_object="2021-12-24 00:00").count(), 10)
         self.assertEqual(qs.filter(channel_object="2021-12-25 00:00").count(), 10)
 
     def test_multiple_channel_objects_dalec_templatetags(self):
         template = get_template("dalec_tests/test-multiple-hours.html")
         # Check there is nothing returned because nothing has been retrieved yet
         output = template.render()
         soup = BeautifulSoup(output, "html.parser")
         divs = soup.find_all("div")
         self.assertEqual(len(divs), 1)
         self.assertEqual(divs[0].string.strip(), "")
 
         # Let's query the external apps to fetch contents
-        proxy = ProxyPool.get("exemple")
+        proxy = ProxyPool.get("example")
         created, updated, deleted = proxy.refresh(
             "hour", "half", channel_object="2021-12-24 00:00"
         )
         self.assertEqual(created, 10)
         created, updated, deleted = proxy.refresh(
             "hour", "half", channel_object="2021-12-25 00:00"
         )
@@ -380,78 +380,78 @@
         soup = BeautifulSoup(output, "html.parser")
         divs = soup.find_all("div")
         self.assertEqual(len(divs), 1 + created)
 
     def test_invalid_dalec_templatetags_call(self):
         t = Template(
             """{% load dalec %}
-        {% dalec "exemple" "hour" channel="quarter" channel_object="A" channel_objects='["B"]' %}
+        {% dalec "example" "hour" channel="quarter" channel_object="A" channel_objects='["B"]' %}
         """
         )
         with self.assertRaisesRegexp(ValueError, "channel_objects"):
             t.render(Context({}))
 
     def test_simple_dalec_templatetags_call(self):
         t = Template(
             """{% load dalec %}
-        {% dalec "exemple" "hour" channel="quarter" channel_object="2021-12-24" %}
+        {% dalec "example" "hour" channel="quarter" channel_object="2021-12-24" %}
         """
         )
         output = t.render(Context({}))
         soup = BeautifulSoup(output, "html.parser")
         divs = soup.find_all("div")
         self.assertEqual(divs[0].attrs["data-channel-objects"], '["2021-12-24"]')
         html = (
             "{% load dalec %}"
-            "{% dalec 'exemple' 'hour' "
+            "{% dalec 'example' 'hour' "
             "channel='quarter' channel_objects='[\"2021-12-24\", \"2021-12-25\"]' %}"
         )
         output = Template(html).render(Context({}))
         soup = BeautifulSoup(output, "html.parser")
         divs = soup.find_all("div")
         self.assertEqual(
             divs[0].attrs["data-channel-objects"], '["2021-12-24", "2021-12-25"]'
         )
 
     def test_ordered_by_dalec_templatetags(self):
         # Let's query the external apps to fetch contents
-        proxy = ProxyPool.get("exemple")
+        proxy = ProxyPool.get("example")
         created, updated, deleted = proxy.refresh(
             "hour", "half", channel_object="2021-12-24 12:00"
         )
 
         # Ascending order by ID
         html = (
             "{% load dalec %}"
-            "{% dalec 'exemple' 'hour' channel='half' channel_object='2021-12-24 12:00' "
+            "{% dalec 'example' 'hour' channel='half' channel_object='2021-12-24 12:00' "
             "ordered_by='id' %}"
         )
         t_asc = Template(html)
         output = t_asc.render(Context({}))
         soup = BeautifulSoup(output, "html.parser")
         divs = soup.find_all(class_="dalec-item")
         self.assertIn("07h30", divs[0].string)
         self.assertIn("12h00", divs[-1].string)
 
         # Descending order by ID
         html = (
             "{% load dalec %}"
-            "{% dalec 'exemple' 'hour' channel='half' channel_object='2021-12-24 12:00' "
+            "{% dalec 'example' 'hour' channel='half' channel_object='2021-12-24 12:00' "
             "ordered_by='-id' %}"
         )
         t_desc = Template(html)
         output = t_desc.render(Context({}))
         soup = BeautifulSoup(output, "html.parser")
         divs = soup.find_all(class_="dalec-item")
         self.assertIn("12h00", divs[0].string)
         self.assertIn("07h30", divs[-1].string)
 
     def test_missing_get_for(self):
         with self.assertRaisesRegexp(AttributeError, "MISSING_SETTING"):
-            app_settings.get_for("MISSING_SETTING", "exemple", raise_if_not_set=True)
+            app_settings.get_for("MISSING_SETTING", "example", raise_if_not_set=True)
 
     @override_settings(
         INSTALLED_APPS=[app for app in settings.INSTALLED_APPS if app != "dalec_prime"]
     )
     def test_missing_history_model_and_dalec_prime(self):
         with self.assertRaisesRegexp(
             ValueError, "adding dalec_prime to your INSTALLED_APPS"
@@ -475,58 +475,58 @@
             "dalec/app/content_type-list.html",
             "dalec/app/list.html",
             "dalec/default/list.html",
         ]
         self.assertEqual(template_names, expected)
 
 
-class DalecExempleTests(TestCase):
+class DalecExampleTests(TestCase):
     @property
     def content_model(self):
         return apps.get_model(app_settings.CONTENT_MODEL)
 
     @property
     def fetch_history_model(self):
         return apps.get_model(app_settings.FETCH_HISTORY_MODEL)
 
     def test_proxy_no_channel(self):
-        proxy = ProxyPool.get("exemple")
+        proxy = ProxyPool.get("example")
         created, updated, deleted = proxy.refresh("french_educ")
         self.assertEqual(created, 10)
         self.assertEqual(updated, 0)
         self.assertEqual(deleted, 0)
 
     def test_proxy_channel_object(self):
-        proxy = ProxyPool.get("exemple")
+        proxy = ProxyPool.get("example")
         created, updated, deleted = proxy.refresh("french_educ", "academy", "Grenoble")
         self.assertEqual(created, 10)
         self.assertEqual(updated, 0)
         self.assertEqual(deleted, 0)
         for c in self.content_model.objects.all():
             self.assertEqual(c.content_data["libelle_academie"], "Grenoble")
 
     def test_proxy_channel_object_quoted(self):
-        proxy = ProxyPool.get("exemple")
+        proxy = ProxyPool.get("example")
         created, updated, deleted = proxy.refresh("hour", "quarter", "24/12/2021 12:00")
         self.assertEqual(created, 10)
         self.assertEqual(updated, 0)
         self.assertEqual(deleted, 0)
         for c in self.content_model.objects.all():
             self.assertTrue("/" in c.channel_object)
 
     def test_view_no_channel_object(self):
-        kwargs = {"app": "exemple", "content_type": "french_educ"}
+        kwargs = {"app": "example", "content_type": "french_educ"}
         url = reverse("dalec_fetch_content", kwargs=kwargs)
         client = Client()
         response = client.get(url)
         self.assertEqual(response.status_code, 200)
         self.assertEqual(self.content_model.objects.count(), 10)
 
     def test_invalid_channel_or_ct(self):
-        proxy = ProxyPool.get("exemple")
+        proxy = ProxyPool.get("example")
         with self.assertRaisesRegexp(ValueError, "requires a channel"):
             created, updated, deleted = proxy.refresh("hour")
         with self.assertRaisesRegexp(ValueError, "requires a channel"):
             created, updated, deleted = proxy.refresh("hour", "yolo")
         with self.assertRaisesRegexp(ValueError, "Invalid content_type"):
             created, updated, deleted = proxy.refresh("yolo")
         with self.assertRaisesRegexp(ValueError, "Invalid channel"):
```

