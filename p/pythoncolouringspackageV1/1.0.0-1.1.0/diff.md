# Comparing `tmp/pythoncolouringspackageV1-1.0.0.tar.gz` & `tmp/pythoncolouringspackageV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncolouringspackageV1-1.0.0.tar", last modified: Wed Jul  5 08:48:29 2023, max compression
+gzip compressed data, was "pythoncolouringspackageV1-1.1.0.tar", last modified: Wed Jul  5 08:50:35 2023, max compression
```

## Comparing `pythoncolouringspackageV1-1.0.0.tar` & `pythoncolouringspackageV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:48:29.551977 pythoncolouringspackageV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      358 2023-07-05 08:48:29.551977 pythoncolouringspackageV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:48:29.551977 pythoncolouringspackageV1-1.0.0/pythoncolouringspackageV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-05 08:48:28.000000 pythoncolouringspackageV1-1.0.0/pythoncolouringspackageV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:48:29.551977 pythoncolouringspackageV1-1.0.0/pythoncolouringspackageV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      358 2023-07-05 08:48:29.000000 pythoncolouringspackageV1-1.0.0/pythoncolouringspackageV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2023-07-05 08:48:29.000000 pythoncolouringspackageV1-1.0.0/pythoncolouringspackageV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 08:48:29.000000 pythoncolouringspackageV1-1.0.0/pythoncolouringspackageV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-05 08:48:29.000000 pythoncolouringspackageV1-1.0.0/pythoncolouringspackageV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 08:48:29.555978 pythoncolouringspackageV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      571 2023-07-05 08:48:28.000000 pythoncolouringspackageV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:50:35.071382 pythoncolouringspackageV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      358 2023-07-05 08:50:35.071382 pythoncolouringspackageV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:50:35.071382 pythoncolouringspackageV1-1.1.0/pythoncolouringspackageV1/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-07-05 08:50:34.000000 pythoncolouringspackageV1-1.1.0/pythoncolouringspackageV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:50:35.071382 pythoncolouringspackageV1-1.1.0/pythoncolouringspackageV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      358 2023-07-05 08:50:34.000000 pythoncolouringspackageV1-1.1.0/pythoncolouringspackageV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2023-07-05 08:50:34.000000 pythoncolouringspackageV1-1.1.0/pythoncolouringspackageV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 08:50:34.000000 pythoncolouringspackageV1-1.1.0/pythoncolouringspackageV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-05 08:50:34.000000 pythoncolouringspackageV1-1.1.0/pythoncolouringspackageV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 08:50:35.071382 pythoncolouringspackageV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      571 2023-07-05 08:50:34.000000 pythoncolouringspackageV1-1.1.0/setup.py
```

### Comparing `pythoncolouringspackageV1-1.0.0/setup.py` & `pythoncolouringspackageV1-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pythoncolouringspackageV1",
     version=VERSION,
```

