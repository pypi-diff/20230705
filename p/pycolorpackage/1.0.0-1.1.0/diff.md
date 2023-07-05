# Comparing `tmp/pycolorpackage-1.0.0.tar.gz` & `tmp/pycolorpackage-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycolorpackage-1.0.0.tar", last modified: Wed Jul  5 10:29:57 2023, max compression
+gzip compressed data, was "pycolorpackage-1.1.0.tar", last modified: Wed Jul  5 10:32:06 2023, max compression
```

## Comparing `pycolorpackage-1.0.0.tar` & `pycolorpackage-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:29:57.686306 pycolorpackage-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      347 2023-07-05 10:29:57.686306 pycolorpackage-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:29:57.682306 pycolorpackage-1.0.0/pycolorpackage/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-05 10:29:57.000000 pycolorpackage-1.0.0/pycolorpackage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:29:57.686306 pycolorpackage-1.0.0/pycolorpackage.egg-info/
--rw-r--r--   0 root         (0) root         (0)      347 2023-07-05 10:29:57.000000 pycolorpackage-1.0.0/pycolorpackage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      187 2023-07-05 10:29:57.000000 pycolorpackage-1.0.0/pycolorpackage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 10:29:57.000000 pycolorpackage-1.0.0/pycolorpackage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-05 10:29:57.000000 pycolorpackage-1.0.0/pycolorpackage.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 10:29:57.686306 pycolorpackage-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      560 2023-07-05 10:29:57.000000 pycolorpackage-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:32:06.765940 pycolorpackage-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-05 10:32:06.765940 pycolorpackage-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:32:06.761940 pycolorpackage-1.1.0/pycolorpackage/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-07-05 10:32:06.000000 pycolorpackage-1.1.0/pycolorpackage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:32:06.765940 pycolorpackage-1.1.0/pycolorpackage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-05 10:32:06.000000 pycolorpackage-1.1.0/pycolorpackage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      187 2023-07-05 10:32:06.000000 pycolorpackage-1.1.0/pycolorpackage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 10:32:06.000000 pycolorpackage-1.1.0/pycolorpackage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-05 10:32:06.000000 pycolorpackage-1.1.0/pycolorpackage.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 10:32:06.765940 pycolorpackage-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      560 2023-07-05 10:32:06.000000 pycolorpackage-1.1.0/setup.py
```

### Comparing `pycolorpackage-1.0.0/setup.py` & `pycolorpackage-1.1.0/setup.py`

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
     name="pycolorpackage",
     version=VERSION,
```

