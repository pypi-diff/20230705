# Comparing `tmp/scblender-0.1.0.tar.gz` & `tmp/scblender-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scblender-0.1.0.tar", last modified: Wed Jul  5 19:15:27 2023, max compression
+gzip compressed data, was "scblender-0.1.1.tar", last modified: Wed Jul  5 19:24:59 2023, max compression
```

## Comparing `scblender-0.1.0.tar` & `scblender-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mackhughes   (501) staff       (20)        0 2023-07-05 19:15:27.113554 scblender-0.1.0/
--rw-r--r--   0 mackhughes   (501) staff       (20)     1072 2023-07-05 19:15:27.113422 scblender-0.1.0/PKG-INFO
--rw-------   0 mackhughes   (501) staff       (20)      497 2022-12-10 22:59:10.000000 scblender-0.1.0/README.md
-drwxr-xr-x   0 mackhughes   (501) staff       (20)        0 2023-07-05 19:15:27.112752 scblender-0.1.0/scblender/
--rw-------   0 mackhughes   (501) staff       (20)      126 2023-07-05 18:47:04.000000 scblender-0.1.0/scblender/__init__.py
--rw-------   0 mackhughes   (501) staff       (20)     1000 2023-01-07 18:53:12.000000 scblender-0.1.0/scblender/curve.py
--rw-------   0 mackhughes   (501) staff       (20)     5899 2023-07-05 19:06:48.000000 scblender-0.1.0/scblender/mesh.py
--rw-------   0 mackhughes   (501) staff       (20)     3818 2023-07-05 19:10:00.000000 scblender-0.1.0/scblender/particle.py
--rw-------   0 mackhughes   (501) staff       (20)     7980 2023-07-05 19:04:38.000000 scblender-0.1.0/scblender/setting.py
-drwxr-xr-x   0 mackhughes   (501) staff       (20)        0 2023-07-05 19:15:27.113219 scblender-0.1.0/scblender.egg-info/
--rw-r--r--   0 mackhughes   (501) staff       (20)     1072 2023-07-05 19:15:27.000000 scblender-0.1.0/scblender.egg-info/PKG-INFO
--rw-r--r--   0 mackhughes   (501) staff       (20)      252 2023-07-05 19:15:27.000000 scblender-0.1.0/scblender.egg-info/SOURCES.txt
--rw-r--r--   0 mackhughes   (501) staff       (20)        1 2023-07-05 19:15:27.000000 scblender-0.1.0/scblender.egg-info/dependency_links.txt
--rw-r--r--   0 mackhughes   (501) staff       (20)       10 2023-07-05 19:15:27.000000 scblender-0.1.0/scblender.egg-info/top_level.txt
--rw-r--r--   0 mackhughes   (501) staff       (20)       38 2023-07-05 19:15:27.113617 scblender-0.1.0/setup.cfg
--rw-------   0 mackhughes   (501) staff       (20)     1033 2023-07-05 19:14:46.000000 scblender-0.1.0/setup.py
+drwxr-xr-x   0 mackhughes   (501) staff       (20)        0 2023-07-05 19:24:59.087692 scblender-0.1.1/
+-rw-r--r--   0 mackhughes   (501) staff       (20)     1072 2023-07-05 19:24:59.087569 scblender-0.1.1/PKG-INFO
+-rw-------   0 mackhughes   (501) staff       (20)      497 2022-12-10 22:59:10.000000 scblender-0.1.1/README.md
+drwxr-xr-x   0 mackhughes   (501) staff       (20)        0 2023-07-05 19:24:59.086629 scblender-0.1.1/scblender/
+-rw-------   0 mackhughes   (501) staff       (20)       98 2023-07-05 19:20:42.000000 scblender-0.1.1/scblender/__init__.py
+-rw-------   0 mackhughes   (501) staff       (20)     1000 2023-01-07 18:53:12.000000 scblender-0.1.1/scblender/curve.py
+-rw-------   0 mackhughes   (501) staff       (20)     5899 2023-07-05 19:06:48.000000 scblender-0.1.1/scblender/mesh.py
+-rw-------   0 mackhughes   (501) staff       (20)     3818 2023-07-05 19:24:14.000000 scblender-0.1.1/scblender/particle.py
+-rw-------   0 mackhughes   (501) staff       (20)     7980 2023-07-05 19:04:38.000000 scblender-0.1.1/scblender/setting.py
+drwxr-xr-x   0 mackhughes   (501) staff       (20)        0 2023-07-05 19:24:59.087334 scblender-0.1.1/scblender.egg-info/
+-rw-r--r--   0 mackhughes   (501) staff       (20)     1072 2023-07-05 19:24:59.000000 scblender-0.1.1/scblender.egg-info/PKG-INFO
+-rw-r--r--   0 mackhughes   (501) staff       (20)      252 2023-07-05 19:24:59.000000 scblender-0.1.1/scblender.egg-info/SOURCES.txt
+-rw-r--r--   0 mackhughes   (501) staff       (20)        1 2023-07-05 19:24:59.000000 scblender-0.1.1/scblender.egg-info/dependency_links.txt
+-rw-r--r--   0 mackhughes   (501) staff       (20)       10 2023-07-05 19:24:59.000000 scblender-0.1.1/scblender.egg-info/top_level.txt
+-rw-r--r--   0 mackhughes   (501) staff       (20)       38 2023-07-05 19:24:59.087746 scblender-0.1.1/setup.cfg
+-rw-------   0 mackhughes   (501) staff       (20)     1033 2023-07-05 19:20:18.000000 scblender-0.1.1/setup.py
```

### Comparing `scblender-0.1.0/PKG-INFO` & `scblender-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scblender
-Version: 0.1.0
+Version: 0.1.1
 Summary: its purpose is to help and facilitate the commands
 Author: Mack Hughes (Allison Eduardo)
 Author-email: <mackhughes251@gmail.com
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scblender-0.1.0/scblender/curve.py` & `scblender-0.1.1/scblender/curve.py`

 * *Files identical despite different names*

### Comparing `scblender-0.1.0/scblender/mesh.py` & `scblender-0.1.1/scblender/mesh.py`

 * *Files identical despite different names*

### Comparing `scblender-0.1.0/scblender/particle.py` & `scblender-0.1.1/scblender/particle.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import numpy
 import bpy
+import numpy
 import setting
 
 class Particle:
     """This class create a particle with the following characteristics:
     Parameters
     ----------
     name : string
```

### Comparing `scblender-0.1.0/scblender/setting.py` & `scblender-0.1.1/scblender/setting.py`

 * *Files identical despite different names*

### Comparing `scblender-0.1.0/scblender.egg-info/PKG-INFO` & `scblender-0.1.1/scblender.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scblender
-Version: 0.1.0
+Version: 0.1.1
 Summary: its purpose is to help and facilitate the commands
 Author: Mack Hughes (Allison Eduardo)
 Author-email: <mackhughes251@gmail.com
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scblender-0.1.0/setup.py` & `scblender-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'its purpose is to help and facilitate the commands'
 
 # Setting up
 setup(
     name="scblender",
     version=VERSION,
     author="Mack Hughes (Allison Eduardo)",
```

