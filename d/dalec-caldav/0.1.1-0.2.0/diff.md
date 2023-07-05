# Comparing `tmp/dalec-caldav-0.1.1.tar.gz` & `tmp/dalec-caldav-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalec-caldav-0.1.1.tar", last modified: Wed Jun 28 14:46:27 2023, max compression
+gzip compressed data, was "dalec-caldav-0.2.0.tar", last modified: Wed Jul  5 11:40:59 2023, max compression
```

## Comparing `dalec-caldav-0.1.1.tar` & `dalec-caldav-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:46:27.044160 dalec-caldav-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-28 14:46:15.000000 dalec-caldav-0.1.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-28 14:46:15.000000 dalec-caldav-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-28 14:46:15.000000 dalec-caldav-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-28 14:46:27.044160 dalec-caldav-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-28 14:46:15.000000 dalec-caldav-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:46:27.044160 dalec-caldav-0.1.1/dalec_caldav/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-28 14:46:15.000000 dalec-caldav-0.1.1/dalec_caldav/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-28 14:46:15.000000 dalec-caldav-0.1.1/dalec_caldav/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-28 14:46:15.000000 dalec-caldav-0.1.1/dalec_caldav/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:46:27.044160 dalec-caldav-0.1.1/dalec_caldav.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-28 14:46:27.000000 dalec-caldav-0.1.1/dalec_caldav.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-28 14:46:27.000000 dalec-caldav-0.1.1/dalec_caldav.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 14:46:27.000000 dalec-caldav-0.1.1/dalec_caldav.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 14:46:26.000000 dalec-caldav-0.1.1/dalec_caldav.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-28 14:46:27.000000 dalec-caldav-0.1.1/dalec_caldav.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-28 14:46:27.000000 dalec-caldav-0.1.1/dalec_caldav.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-28 14:46:27.044160 dalec-caldav-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-28 14:46:15.000000 dalec-caldav-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:40:59.933201 dalec-caldav-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-05 11:40:50.000000 dalec-caldav-0.2.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-05 11:40:50.000000 dalec-caldav-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-05 11:40:50.000000 dalec-caldav-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-07-05 11:40:59.933201 dalec-caldav-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-05 11:40:50.000000 dalec-caldav-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:40:59.933201 dalec-caldav-0.2.0/dalec_caldav/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 11:40:50.000000 dalec-caldav-0.2.0/dalec_caldav/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-05 11:40:50.000000 dalec-caldav-0.2.0/dalec_caldav/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-07-05 11:40:50.000000 dalec-caldav-0.2.0/dalec_caldav/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:40:59.933201 dalec-caldav-0.2.0/dalec_caldav.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-07-05 11:40:59.000000 dalec-caldav-0.2.0/dalec_caldav.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-05 11:40:59.000000 dalec-caldav-0.2.0/dalec_caldav.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 11:40:59.000000 dalec-caldav-0.2.0/dalec_caldav.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 11:40:59.000000 dalec-caldav-0.2.0/dalec_caldav.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-05 11:40:59.000000 dalec-caldav-0.2.0/dalec_caldav.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 11:40:59.000000 dalec-caldav-0.2.0/dalec_caldav.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-05 11:40:50.000000 dalec-caldav-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-05 11:40:59.933201 dalec-caldav-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 11:40:50.000000 dalec-caldav-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:40:59.933201 dalec-caldav-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:40:50.000000 dalec-caldav-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-05 11:40:50.000000 dalec-caldav-0.2.0/tests/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-05 11:40:50.000000 dalec-caldav-0.2.0/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-05 11:40:50.000000 dalec-caldav-0.2.0/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-07-05 11:40:50.000000 dalec-caldav-0.2.0/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-05 11:40:50.000000 dalec-caldav-0.2.0/tests/urls.py
```

### Comparing `dalec-caldav-0.1.1/LICENSE` & `dalec-caldav-0.2.0/LICENSE`

 * *Files identical despite different names*

