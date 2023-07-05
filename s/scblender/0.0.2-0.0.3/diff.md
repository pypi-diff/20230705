# Comparing `tmp/scblender-0.0.2.tar.gz` & `tmp/scblender-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scblender-0.0.2.tar", last modified: Wed Jul  5 17:49:07 2023, max compression
+gzip compressed data, was "scblender-0.0.3.tar", last modified: Wed Jul  5 18:27:30 2023, max compression
```

## Comparing `scblender-0.0.2.tar` & `scblender-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mackhughes   (501) staff       (20)        0 2023-07-05 17:49:07.746243 scblender-0.0.2/
--rw-r--r--   0 mackhughes   (501) staff       (20)     1072 2023-07-05 17:49:07.746100 scblender-0.0.2/PKG-INFO
--rw-------   0 mackhughes   (501) staff       (20)      497 2022-12-10 22:59:10.000000 scblender-0.0.2/README.md
-drwxr-xr-x   0 mackhughes   (501) staff       (20)        0 2023-07-05 17:49:07.745269 scblender-0.0.2/scblender/
--rw-------   0 mackhughes   (501) staff       (20)       82 2023-01-19 00:51:40.000000 scblender-0.0.2/scblender/__init__.py
--rw-------   0 mackhughes   (501) staff       (20)     1000 2023-01-07 18:53:12.000000 scblender-0.0.2/scblender/curve.py
--rw-------   0 mackhughes   (501) staff       (20)      779 2023-01-06 17:32:10.000000 scblender-0.0.2/scblender/frame.py
--rw-------   0 mackhughes   (501) staff       (20)     5922 2023-07-04 19:44:41.000000 scblender-0.0.2/scblender/mesh.py
--rw-------   0 mackhughes   (501) staff       (20)     3868 2023-06-04 00:21:26.000000 scblender-0.0.2/scblender/particle.py
--rw-------   0 mackhughes   (501) staff       (20)     7798 2023-01-18 23:59:56.000000 scblender-0.0.2/scblender/setting.py
-drwxr-xr-x   0 mackhughes   (501) staff       (20)        0 2023-07-05 17:49:07.745875 scblender-0.0.2/scblender.egg-info/
--rw-r--r--   0 mackhughes   (501) staff       (20)     1072 2023-07-05 17:49:07.000000 scblender-0.0.2/scblender.egg-info/PKG-INFO
--rw-r--r--   0 mackhughes   (501) staff       (20)      271 2023-07-05 17:49:07.000000 scblender-0.0.2/scblender.egg-info/SOURCES.txt
--rw-r--r--   0 mackhughes   (501) staff       (20)        1 2023-07-05 17:49:07.000000 scblender-0.0.2/scblender.egg-info/dependency_links.txt
--rw-r--r--   0 mackhughes   (501) staff       (20)       10 2023-07-05 17:49:07.000000 scblender-0.0.2/scblender.egg-info/top_level.txt
--rw-r--r--   0 mackhughes   (501) staff       (20)       38 2023-07-05 17:49:07.746293 scblender-0.0.2/setup.cfg
--rw-------   0 mackhughes   (501) staff       (20)     1033 2023-07-05 17:47:18.000000 scblender-0.0.2/setup.py
+drwxr-xr-x   0 mackhughes   (501) staff       (20)        0 2023-07-05 18:27:30.218264 scblender-0.0.3/
+-rw-r--r--   0 mackhughes   (501) staff       (20)     1072 2023-07-05 18:27:30.218138 scblender-0.0.3/PKG-INFO
+-rw-------   0 mackhughes   (501) staff       (20)      497 2022-12-10 22:59:10.000000 scblender-0.0.3/README.md
+drwxr-xr-x   0 mackhughes   (501) staff       (20)        0 2023-07-05 18:27:30.217495 scblender-0.0.3/scblender/
+-rw-------   0 mackhughes   (501) staff       (20)      126 2023-07-05 18:23:43.000000 scblender-0.0.3/scblender/__init__.py
+-rw-------   0 mackhughes   (501) staff       (20)     1000 2023-01-07 18:53:12.000000 scblender-0.0.3/scblender/curve.py
+-rw-------   0 mackhughes   (501) staff       (20)      779 2023-07-05 18:18:41.000000 scblender-0.0.3/scblender/frame.py
+-rw-------   0 mackhughes   (501) staff       (20)     5922 2023-07-05 18:12:53.000000 scblender-0.0.3/scblender/mesh.py
+-rw-------   0 mackhughes   (501) staff       (20)     3868 2023-06-04 00:21:26.000000 scblender-0.0.3/scblender/particle.py
+-rw-------   0 mackhughes   (501) staff       (20)     7798 2023-01-18 23:59:56.000000 scblender-0.0.3/scblender/setting.py
+drwxr-xr-x   0 mackhughes   (501) staff       (20)        0 2023-07-05 18:27:30.217939 scblender-0.0.3/scblender.egg-info/
+-rw-r--r--   0 mackhughes   (501) staff       (20)     1072 2023-07-05 18:27:30.000000 scblender-0.0.3/scblender.egg-info/PKG-INFO
+-rw-r--r--   0 mackhughes   (501) staff       (20)      271 2023-07-05 18:27:30.000000 scblender-0.0.3/scblender.egg-info/SOURCES.txt
+-rw-r--r--   0 mackhughes   (501) staff       (20)        1 2023-07-05 18:27:30.000000 scblender-0.0.3/scblender.egg-info/dependency_links.txt
+-rw-r--r--   0 mackhughes   (501) staff       (20)       10 2023-07-05 18:27:30.000000 scblender-0.0.3/scblender.egg-info/top_level.txt
+-rw-r--r--   0 mackhughes   (501) staff       (20)       38 2023-07-05 18:27:30.218307 scblender-0.0.3/setup.cfg
+-rw-------   0 mackhughes   (501) staff       (20)     1033 2023-07-05 18:27:14.000000 scblender-0.0.3/setup.py
```

### Comparing `scblender-0.0.2/PKG-INFO` & `scblender-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scblender
-Version: 0.0.2
+Version: 0.0.3
 Summary: its purpose is to help and facilitate the commands
 Author: Mack Hughes (Allison Eduardo)
 Author-email: <mackhughes251@gmail.com
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scblender-0.0.2/scblender/curve.py` & `scblender-0.0.3/scblender/curve.py`

 * *Files identical despite different names*

### Comparing `scblender-0.0.2/scblender/frame.py` & `scblender-0.0.3/scblender/frame.py`

 * *Files identical despite different names*

### Comparing `scblender-0.0.2/scblender/mesh.py` & `scblender-0.0.3/scblender/mesh.py`

 * *Files identical despite different names*

### Comparing `scblender-0.0.2/scblender/particle.py` & `scblender-0.0.3/scblender/particle.py`

 * *Files identical despite different names*

### Comparing `scblender-0.0.2/scblender/setting.py` & `scblender-0.0.3/scblender/setting.py`

 * *Files identical despite different names*

### Comparing `scblender-0.0.2/scblender.egg-info/PKG-INFO` & `scblender-0.0.3/scblender.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scblender
-Version: 0.0.2
+Version: 0.0.3
 Summary: its purpose is to help and facilitate the commands
 Author: Mack Hughes (Allison Eduardo)
 Author-email: <mackhughes251@gmail.com
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scblender-0.0.2/setup.py` & `scblender-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'its purpose is to help and facilitate the commands'
 
 # Setting up
 setup(
     name="scblender",
     version=VERSION,
     author="Mack Hughes (Allison Eduardo)",
```

