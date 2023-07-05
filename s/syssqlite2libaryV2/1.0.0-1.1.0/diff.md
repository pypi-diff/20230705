# Comparing `tmp/syssqlite2libaryV2-1.0.0.tar.gz` & `tmp/syssqlite2libaryV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syssqlite2libaryV2-1.0.0.tar", last modified: Wed Jul  5 10:31:01 2023, max compression
+gzip compressed data, was "syssqlite2libaryV2-1.1.0.tar", last modified: Wed Jul  5 10:33:07 2023, max compression
```

## Comparing `syssqlite2libaryV2-1.0.0.tar` & `syssqlite2libaryV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:31:01.718124 syssqlite2libaryV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      351 2023-07-05 10:31:01.718124 syssqlite2libaryV2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 10:31:01.718124 syssqlite2libaryV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      564 2023-07-05 10:31:01.000000 syssqlite2libaryV2-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:31:01.718124 syssqlite2libaryV2-1.0.0/syssqlite2libaryV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-05 10:31:01.000000 syssqlite2libaryV2-1.0.0/syssqlite2libaryV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:31:01.718124 syssqlite2libaryV2-1.0.0/syssqlite2libaryV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      351 2023-07-05 10:31:01.000000 syssqlite2libaryV2-1.0.0/syssqlite2libaryV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      207 2023-07-05 10:31:01.000000 syssqlite2libaryV2-1.0.0/syssqlite2libaryV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 10:31:01.000000 syssqlite2libaryV2-1.0.0/syssqlite2libaryV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-05 10:31:01.000000 syssqlite2libaryV2-1.0.0/syssqlite2libaryV2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:33:07.761767 syssqlite2libaryV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-07-05 10:33:07.757767 syssqlite2libaryV2-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 10:33:07.761767 syssqlite2libaryV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      564 2023-07-05 10:33:06.000000 syssqlite2libaryV2-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:33:07.749767 syssqlite2libaryV2-1.1.0/syssqlite2libaryV2/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-07-05 10:33:06.000000 syssqlite2libaryV2-1.1.0/syssqlite2libaryV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:33:07.753767 syssqlite2libaryV2-1.1.0/syssqlite2libaryV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-07-05 10:33:07.000000 syssqlite2libaryV2-1.1.0/syssqlite2libaryV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      207 2023-07-05 10:33:07.000000 syssqlite2libaryV2-1.1.0/syssqlite2libaryV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 10:33:07.000000 syssqlite2libaryV2-1.1.0/syssqlite2libaryV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-05 10:33:07.000000 syssqlite2libaryV2-1.1.0/syssqlite2libaryV2.egg-info/top_level.txt
```

### Comparing `syssqlite2libaryV2-1.0.0/setup.py` & `syssqlite2libaryV2-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="syssqlite2libaryV2",
     version=VERSION,
```

