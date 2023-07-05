# Comparing `tmp/djangounittest-0.2.4.tar.gz` & `tmp/djangounittest-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangounittest-0.2.4.tar", last modified: Wed Jun 28 04:02:52 2023, max compression
+gzip compressed data, was "djangounittest-0.2.5.tar", last modified: Wed Jul  5 03:21:29 2023, max compression
```

## Comparing `djangounittest-0.2.4.tar` & `djangounittest-0.2.5.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-06-28 04:02:52.636455 djangounittest-0.2.4/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-06-28 04:02:52.636455 djangounittest-0.2.4/PKG-INFO
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       19 2023-06-27 11:26:24.000000 djangounittest-0.2.4/README.md
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-06-28 04:02:52.636455 djangounittest-0.2.4/djangounittest/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       84 2023-06-28 04:02:23.000000 djangounittest-0.2.4/djangounittest/__init__.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      239 2023-06-28 04:02:38.000000 djangounittest-0.2.4/djangounittest/mainunittest.py
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-06-28 04:02:52.636455 djangounittest-0.2.4/djangounittest.egg-info/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-06-28 04:02:52.000000 djangounittest-0.2.4/djangounittest.egg-info/PKG-INFO
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      228 2023-06-28 04:02:52.000000 djangounittest-0.2.4/djangounittest.egg-info/SOURCES.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        1 2023-06-28 04:02:52.000000 djangounittest-0.2.4/djangounittest.egg-info/dependency_links.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       15 2023-06-28 04:02:52.000000 djangounittest-0.2.4/djangounittest.egg-info/top_level.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       38 2023-06-28 04:02:52.636455 djangounittest-0.2.4/setup.cfg
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1013 2023-06-28 04:02:45.000000 djangounittest-0.2.4/setup.py
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-07-05 03:21:29.768913 djangounittest-0.2.5/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-07-05 03:21:29.768913 djangounittest-0.2.5/PKG-INFO
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       19 2023-06-27 11:26:24.000000 djangounittest-0.2.5/README.md
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-07-05 03:21:29.768913 djangounittest-0.2.5/djangounittest/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       84 2023-07-05 03:16:45.000000 djangounittest-0.2.5/djangounittest/__init__.py
+drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-07-05 03:21:29.768913 djangounittest-0.2.5/djangounittest.egg-info/
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      595 2023-07-05 03:21:29.000000 djangounittest-0.2.5/djangounittest.egg-info/PKG-INFO
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      197 2023-07-05 03:21:29.000000 djangounittest-0.2.5/djangounittest.egg-info/SOURCES.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        1 2023-07-05 03:21:29.000000 djangounittest-0.2.5/djangounittest.egg-info/dependency_links.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       15 2023-07-05 03:21:29.000000 djangounittest-0.2.5/djangounittest.egg-info/top_level.txt
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       38 2023-07-05 03:21:29.768913 djangounittest-0.2.5/setup.cfg
+-rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1013 2023-07-05 03:21:13.000000 djangounittest-0.2.5/setup.py
```

### Comparing `djangounittest-0.2.4/PKG-INFO` & `djangounittest-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangounittest
-Version: 0.2.4
+Version: 0.2.5
 Summary: A django testing framework
 Home-page: UNKNOWN
 Author: NeuralNine (Florian Dedov)
 Author-email: <djangouniittest@gmail.com>
 License: UNKNOWN
 Keywords: python,test,Django
 Platform: UNKNOWN
```

### Comparing `djangounittest-0.2.4/djangounittest.egg-info/PKG-INFO` & `djangounittest-0.2.5/djangounittest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangounittest
-Version: 0.2.4
+Version: 0.2.5
 Summary: A django testing framework
 Home-page: UNKNOWN
 Author: NeuralNine (Florian Dedov)
 Author-email: <djangouniittest@gmail.com>
 License: UNKNOWN
 Keywords: python,test,Django
 Platform: UNKNOWN
```

### Comparing `djangounittest-0.2.4/setup.py` & `djangounittest-0.2.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.4'
+VERSION = '0.2.5'
 DESCRIPTION = 'A django testing framework'
 LONG_DESCRIPTION = 'A package that allows to test your django apps'
 
 # Setting up
 setup(
     name="djangounittest",
     version=VERSION,
```

