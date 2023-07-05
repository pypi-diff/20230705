# Comparing `tmp/djangounittest-0.2.6.tar.gz` & `tmp/djangounittest-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangounittest-0.2.6.tar", last modified: Wed Jul  5 04:45:22 2023, max compression
+gzip compressed data, was "djangounittest-0.2.7.tar", last modified: Wed Jul  5 04:54:42 2023, max compression
```

## Comparing `djangounittest-0.2.6.tar` & `djangounittest-0.2.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-07-05 04:45:22.960461 djangounittest-0.2.6/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-07-05 04:45:22.960461 djangounittest-0.2.6/PKG-INFO
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       19 2023-06-27 11:26:24.000000 djangounittest-0.2.6/README.md
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-07-05 04:45:22.960461 djangounittest-0.2.6/djangounittest/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       35 2023-07-05 04:44:02.000000 djangounittest-0.2.6/djangounittest/__init__.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      260 2023-07-05 04:43:56.000000 djangounittest-0.2.6/djangounittest/mainunittest.py
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-07-05 04:45:22.960461 djangounittest-0.2.6/djangounittest.egg-info/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-07-05 04:45:22.000000 djangounittest-0.2.6/djangounittest.egg-info/PKG-INFO
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      228 2023-07-05 04:45:22.000000 djangounittest-0.2.6/djangounittest.egg-info/SOURCES.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        1 2023-07-05 04:45:22.000000 djangounittest-0.2.6/djangounittest.egg-info/dependency_links.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       15 2023-07-05 04:45:22.000000 djangounittest-0.2.6/djangounittest.egg-info/top_level.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       38 2023-07-05 04:45:22.960461 djangounittest-0.2.6/setup.cfg
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1056 2023-07-05 04:44:54.000000 djangounittest-0.2.6/setup.py
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-07-05 04:54:42.613680 djangounittest-0.2.7/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-07-05 04:54:42.613680 djangounittest-0.2.7/PKG-INFO
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       19 2023-06-27 11:26:24.000000 djangounittest-0.2.7/README.md
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-07-05 04:54:42.613680 djangounittest-0.2.7/djangounittest/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       35 2023-07-05 04:44:02.000000 djangounittest-0.2.7/djangounittest/__init__.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    28472 2023-07-05 04:52:57.000000 djangounittest-0.2.7/djangounittest/mainunittest.py
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-07-05 04:54:42.613680 djangounittest-0.2.7/djangounittest.egg-info/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-07-05 04:54:42.000000 djangounittest-0.2.7/djangounittest.egg-info/PKG-INFO
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      228 2023-07-05 04:54:42.000000 djangounittest-0.2.7/djangounittest.egg-info/SOURCES.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        1 2023-07-05 04:54:42.000000 djangounittest-0.2.7/djangounittest.egg-info/dependency_links.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       15 2023-07-05 04:54:42.000000 djangounittest-0.2.7/djangounittest.egg-info/top_level.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       38 2023-07-05 04:54:42.613680 djangounittest-0.2.7/setup.cfg
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1056 2023-07-05 04:54:25.000000 djangounittest-0.2.7/setup.py
```

### Comparing `djangounittest-0.2.6/PKG-INFO` & `djangounittest-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangounittest
-Version: 0.2.6
+Version: 0.2.7
 Summary: A django testing framework
 Home-page: UNKNOWN
 Author: NeuralNine (Florian Dedov)
 Author-email: <djangouniittest@gmail.com>
 License: UNKNOWN
 Keywords: python,test,Django
 Platform: UNKNOWN
```

### Comparing `djangounittest-0.2.6/djangounittest.egg-info/PKG-INFO` & `djangounittest-0.2.7/djangounittest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangounittest
-Version: 0.2.6
+Version: 0.2.7
 Summary: A django testing framework
 Home-page: UNKNOWN
 Author: NeuralNine (Florian Dedov)
 Author-email: <djangouniittest@gmail.com>
 License: UNKNOWN
 Keywords: python,test,Django
 Platform: UNKNOWN
```

### Comparing `djangounittest-0.2.6/setup.py` & `djangounittest-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.6'
+VERSION = '0.2.7'
 DESCRIPTION = 'A django testing framework'
 LONG_DESCRIPTION = 'A package that allows to test your django apps'
 
 # Setting up
 setup(
     name="djangounittest",
     version=VERSION,
```

