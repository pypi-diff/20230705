# Comparing `tmp/syscolouringsaddon-1.0.0.tar.gz` & `tmp/syscolouringsaddon-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syscolouringsaddon-1.0.0.tar", last modified: Wed Jul  5 08:47:24 2023, max compression
+gzip compressed data, was "syscolouringsaddon-1.1.0.tar", last modified: Wed Jul  5 08:49:30 2023, max compression
```

## Comparing `syscolouringsaddon-1.0.0.tar` & `syscolouringsaddon-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:47:24.916305 syscolouringsaddon-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      351 2023-07-05 08:47:24.916305 syscolouringsaddon-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 08:47:24.916305 syscolouringsaddon-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      564 2023-07-05 08:47:24.000000 syscolouringsaddon-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:47:24.912305 syscolouringsaddon-1.0.0/syscolouringsaddon/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-05 08:47:24.000000 syscolouringsaddon-1.0.0/syscolouringsaddon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:47:24.916305 syscolouringsaddon-1.0.0/syscolouringsaddon.egg-info/
--rw-r--r--   0 root         (0) root         (0)      351 2023-07-05 08:47:24.000000 syscolouringsaddon-1.0.0/syscolouringsaddon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      207 2023-07-05 08:47:24.000000 syscolouringsaddon-1.0.0/syscolouringsaddon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 08:47:24.000000 syscolouringsaddon-1.0.0/syscolouringsaddon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-05 08:47:24.000000 syscolouringsaddon-1.0.0/syscolouringsaddon.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:49:30.603682 syscolouringsaddon-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-07-05 08:49:30.603682 syscolouringsaddon-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 08:49:30.603682 syscolouringsaddon-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      564 2023-07-05 08:49:30.000000 syscolouringsaddon-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:49:30.603682 syscolouringsaddon-1.1.0/syscolouringsaddon/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-07-05 08:49:30.000000 syscolouringsaddon-1.1.0/syscolouringsaddon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:49:30.603682 syscolouringsaddon-1.1.0/syscolouringsaddon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-07-05 08:49:30.000000 syscolouringsaddon-1.1.0/syscolouringsaddon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      207 2023-07-05 08:49:30.000000 syscolouringsaddon-1.1.0/syscolouringsaddon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 08:49:30.000000 syscolouringsaddon-1.1.0/syscolouringsaddon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-05 08:49:30.000000 syscolouringsaddon-1.1.0/syscolouringsaddon.egg-info/top_level.txt
```

### Comparing `syscolouringsaddon-1.0.0/setup.py` & `syscolouringsaddon-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="syscolouringsaddon",
     version=VERSION,
```

