# Comparing `tmp/djangounittest-0.2.8.tar.gz` & `tmp/djangounittest-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangounittest-0.2.8.tar", last modified: Wed Jul  5 05:45:57 2023, max compression
+gzip compressed data, was "djangounittest-0.2.9.tar", last modified: Wed Jul  5 06:20:43 2023, max compression
```

## Comparing `djangounittest-0.2.8.tar` & `djangounittest-0.2.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-07-05 05:45:57.982394 djangounittest-0.2.8/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-07-05 05:45:57.982394 djangounittest-0.2.8/PKG-INFO
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       19 2023-06-27 11:26:24.000000 djangounittest-0.2.8/README.md
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-07-05 05:45:57.982394 djangounittest-0.2.8/djangounittest/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       35 2023-07-05 04:44:02.000000 djangounittest-0.2.8/djangounittest/__init__.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    39154 2023-07-05 05:44:55.000000 djangounittest-0.2.8/djangounittest/mainunittest.py
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-07-05 05:45:57.982394 djangounittest-0.2.8/djangounittest.egg-info/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-07-05 05:45:57.000000 djangounittest-0.2.8/djangounittest.egg-info/PKG-INFO
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      228 2023-07-05 05:45:57.000000 djangounittest-0.2.8/djangounittest.egg-info/SOURCES.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        1 2023-07-05 05:45:57.000000 djangounittest-0.2.8/djangounittest.egg-info/dependency_links.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       15 2023-07-05 05:45:57.000000 djangounittest-0.2.8/djangounittest.egg-info/top_level.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       38 2023-07-05 05:45:57.982394 djangounittest-0.2.8/setup.cfg
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1056 2023-07-05 05:44:35.000000 djangounittest-0.2.8/setup.py
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-07-05 06:20:43.974526 djangounittest-0.2.9/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-07-05 06:20:43.974526 djangounittest-0.2.9/PKG-INFO
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       19 2023-06-27 11:26:24.000000 djangounittest-0.2.9/README.md
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-07-05 06:20:43.974526 djangounittest-0.2.9/djangounittest/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       35 2023-07-05 04:44:02.000000 djangounittest-0.2.9/djangounittest/__init__.py
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    15329 2023-07-05 06:19:50.000000 djangounittest-0.2.9/djangounittest/mainunittest.py
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-07-05 06:20:43.974526 djangounittest-0.2.9/djangounittest.egg-info/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-07-05 06:20:43.000000 djangounittest-0.2.9/djangounittest.egg-info/PKG-INFO
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      228 2023-07-05 06:20:43.000000 djangounittest-0.2.9/djangounittest.egg-info/SOURCES.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        1 2023-07-05 06:20:43.000000 djangounittest-0.2.9/djangounittest.egg-info/dependency_links.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       15 2023-07-05 06:20:43.000000 djangounittest-0.2.9/djangounittest.egg-info/top_level.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       38 2023-07-05 06:20:43.974526 djangounittest-0.2.9/setup.cfg
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1056 2023-07-05 06:20:28.000000 djangounittest-0.2.9/setup.py
```

### Comparing `djangounittest-0.2.8/PKG-INFO` & `djangounittest-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangounittest
-Version: 0.2.8
+Version: 0.2.9
 Summary: A django testing framework
 Home-page: UNKNOWN
 Author: NeuralNine (Florian Dedov)
 Author-email: <djangouniittest@gmail.com>
 License: UNKNOWN
 Keywords: python,test,Django
 Platform: UNKNOWN
```

### Comparing `djangounittest-0.2.8/djangounittest.egg-info/PKG-INFO` & `djangounittest-0.2.9/djangounittest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangounittest
-Version: 0.2.8
+Version: 0.2.9
 Summary: A django testing framework
 Home-page: UNKNOWN
 Author: NeuralNine (Florian Dedov)
 Author-email: <djangouniittest@gmail.com>
 License: UNKNOWN
 Keywords: python,test,Django
 Platform: UNKNOWN
```

### Comparing `djangounittest-0.2.8/setup.py` & `djangounittest-0.2.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.8'
+VERSION = '0.2.9'
 DESCRIPTION = 'A django testing framework'
 LONG_DESCRIPTION = 'A package that allows to test your django apps'
 
 # Setting up
 setup(
     name="djangounittest",
     version=VERSION,
```

