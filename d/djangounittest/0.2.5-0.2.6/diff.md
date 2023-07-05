# Comparing `tmp/djangounittest-0.2.5.tar.gz` & `tmp/djangounittest-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangounittest-0.2.5.tar", last modified: Wed Jul  5 03:21:29 2023, max compression
+gzip compressed data, was "djangounittest-0.2.6.tar", last modified: Wed Jul  5 04:45:22 2023, max compression
```

## Comparing `djangounittest-0.2.5.tar` & `djangounittest-0.2.6.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-07-05 03:21:29.768913 djangounittest-0.2.5/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-07-05 03:21:29.768913 djangounittest-0.2.5/PKG-INFO
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       19 2023-06-27 11:26:24.000000 djangounittest-0.2.5/README.md
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-07-05 03:21:29.768913 djangounittest-0.2.5/djangounittest/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       84 2023-07-05 03:16:45.000000 djangounittest-0.2.5/djangounittest/__init__.py
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-07-05 03:21:29.768913 djangounittest-0.2.5/djangounittest.egg-info/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-07-05 03:21:29.000000 djangounittest-0.2.5/djangounittest.egg-info/PKG-INFO
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      197 2023-07-05 03:21:29.000000 djangounittest-0.2.5/djangounittest.egg-info/SOURCES.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        1 2023-07-05 03:21:29.000000 djangounittest-0.2.5/djangounittest.egg-info/dependency_links.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       15 2023-07-05 03:21:29.000000 djangounittest-0.2.5/djangounittest.egg-info/top_level.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       38 2023-07-05 03:21:29.768913 djangounittest-0.2.5/setup.cfg
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1013 2023-07-05 03:21:13.000000 djangounittest-0.2.5/setup.py
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-07-05 04:45:22.960461 djangounittest-0.2.6/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-07-05 04:45:22.960461 djangounittest-0.2.6/PKG-INFO
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       19 2023-06-27 11:26:24.000000 djangounittest-0.2.6/README.md
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-07-05 04:45:22.960461 djangounittest-0.2.6/djangounittest/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       35 2023-07-05 04:44:02.000000 djangounittest-0.2.6/djangounittest/__init__.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      260 2023-07-05 04:43:56.000000 djangounittest-0.2.6/djangounittest/mainunittest.py
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-07-05 04:45:22.960461 djangounittest-0.2.6/djangounittest.egg-info/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-07-05 04:45:22.000000 djangounittest-0.2.6/djangounittest.egg-info/PKG-INFO
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      228 2023-07-05 04:45:22.000000 djangounittest-0.2.6/djangounittest.egg-info/SOURCES.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        1 2023-07-05 04:45:22.000000 djangounittest-0.2.6/djangounittest.egg-info/dependency_links.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       15 2023-07-05 04:45:22.000000 djangounittest-0.2.6/djangounittest.egg-info/top_level.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       38 2023-07-05 04:45:22.960461 djangounittest-0.2.6/setup.cfg
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1056 2023-07-05 04:44:54.000000 djangounittest-0.2.6/setup.py
```

### Comparing `djangounittest-0.2.5/PKG-INFO` & `djangounittest-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangounittest
-Version: 0.2.5
+Version: 0.2.6
 Summary: A django testing framework
 Home-page: UNKNOWN
 Author: NeuralNine (Florian Dedov)
 Author-email: <djangouniittest@gmail.com>
 License: UNKNOWN
 Keywords: python,test,Django
 Platform: UNKNOWN
```

### Comparing `djangounittest-0.2.5/djangounittest.egg-info/PKG-INFO` & `djangounittest-0.2.6/djangounittest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangounittest
-Version: 0.2.5
+Version: 0.2.6
 Summary: A django testing framework
 Home-page: UNKNOWN
 Author: NeuralNine (Florian Dedov)
 Author-email: <djangouniittest@gmail.com>
 License: UNKNOWN
 Keywords: python,test,Django
 Platform: UNKNOWN
```

### Comparing `djangounittest-0.2.5/setup.py` & `djangounittest-0.2.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from setuptools import setup, find_packages
+from distutils.extension import Extension
+
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.5'
+VERSION = '0.2.6'
 DESCRIPTION = 'A django testing framework'
 LONG_DESCRIPTION = 'A package that allows to test your django apps'
 
 # Setting up
 setup(
     name="djangounittest",
     version=VERSION,
```

