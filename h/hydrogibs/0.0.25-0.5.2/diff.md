# Comparing `tmp/hydrogibs-0.0.25.tar.gz` & `tmp/hydrogibs-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrogibs-0.0.25.tar", last modified: Wed Jul  5 07:44:01 2023, max compression
+gzip compressed data, was "hydrogibs-0.5.2.tar", last modified: Mon Jul  3 15:13:24 2023, max compression
```

## Comparing `hydrogibs-0.0.25.tar` & `hydrogibs-0.5.2.tar`

### file list

```diff
@@ -1,31 +1,12 @@
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-07-05 07:44:01.742144 hydrogibs-0.0.25/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.0.25/LICENSE
--rw-rw-r--   0 axel      (1000) axel      (1000)     1396 2023-07-05 07:44:01.742144 hydrogibs-0.0.25/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)     1008 2023-05-23 16:56:32.000000 hydrogibs-0.0.25/README.md
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-07-05 07:44:01.738144 hydrogibs-0.0.25/hydrogibs/
--rw-rw-r--   0 axel      (1000) axel      (1000)      208 2023-07-05 07:18:42.000000 hydrogibs-0.0.25/hydrogibs/__init__.py
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-07-05 07:44:01.738144 hydrogibs-0.0.25/hydrogibs/floods/
--rwxrwxr-x   0 axel      (1000) axel      (1000)    13227 2023-07-03 21:17:05.000000 hydrogibs-0.0.25/hydrogibs/floods/GR4.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     5249 2023-07-03 21:15:05.000000 hydrogibs-0.0.25/hydrogibs/floods/ModelApp.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     1943 2023-06-21 12:15:20.000000 hydrogibs-0.0.25/hydrogibs/floods/ModelTemplate.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     7452 2023-07-03 21:25:21.000000 hydrogibs-0.0.25/hydrogibs/floods/QDF.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     1022 2023-05-14 09:41:57.000000 hydrogibs-0.0.25/hydrogibs/floods/RationalMethod.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     2228 2023-06-12 15:14:30.000000 hydrogibs-0.0.25/hydrogibs/floods/Riemann.py
--rw-rw-r--   0 axel      (1000) axel      (1000)      874 2023-05-24 13:52:28.000000 hydrogibs-0.0.25/hydrogibs/floods/SoCoSe.py
--rw-rw-r--   0 axel      (1000) axel      (1000)        0 2023-07-03 21:27:16.000000 hydrogibs-0.0.25/hydrogibs/floods/__init__.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     1891 2023-06-04 08:00:38.000000 hydrogibs-0.0.25/hydrogibs/floods/constants.py
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-07-05 07:44:01.742144 hydrogibs-0.0.25/hydrogibs/misc/
--rw-rw-r--   0 axel      (1000) axel      (1000)        0 2023-07-03 21:25:16.000000 hydrogibs-0.0.25/hydrogibs/misc/__init__.py
--rw-rw-r--   0 axel      (1000) axel      (1000)    10957 2023-06-22 16:01:53.000000 hydrogibs-0.0.25/hydrogibs/misc/misc.py
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-07-05 07:44:01.742144 hydrogibs-0.0.25/hydrogibs/test/
--rw-rw-r--   0 axel      (1000) axel      (1000)        0 2023-07-03 20:51:52.000000 hydrogibs-0.0.25/hydrogibs/test/__init__.py
--rw-rw-r--   0 axel      (1000) axel      (1000)        0 2023-07-03 20:52:06.000000 hydrogibs-0.0.25/hydrogibs/test/test_GR4.py
--rw-rw-r--   0 axel      (1000) axel      (1000)        0 2023-07-05 07:11:57.000000 hydrogibs-0.0.25/hydrogibs/test.csv
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-07-05 07:44:01.738144 hydrogibs-0.0.25/hydrogibs.egg-info/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1396 2023-07-05 07:44:01.000000 hydrogibs-0.0.25/hydrogibs.egg-info/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)      595 2023-07-05 07:44:01.000000 hydrogibs-0.0.25/hydrogibs.egg-info/SOURCES.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-07-05 07:44:01.000000 hydrogibs-0.0.25/hydrogibs.egg-info/dependency_links.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)       12 2023-07-05 07:44:01.000000 hydrogibs-0.0.25/hydrogibs.egg-info/requires.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-07-05 07:44:01.000000 hydrogibs-0.0.25/hydrogibs.egg-info/top_level.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-07-05 07:44:01.742144 hydrogibs-0.0.25/setup.cfg
--rw-rw-r--   0 axel      (1000) axel      (1000)      707 2023-07-05 07:42:42.000000 hydrogibs-0.0.25/setup.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-07-03 15:13:24.228182 hydrogibs-0.5.2/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.5.2/LICENSE
+-rw-rw-r--   0 axel      (1000) axel      (1000)      286 2023-07-03 15:13:24.228182 hydrogibs-0.5.2/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1008 2023-05-23 16:56:32.000000 hydrogibs-0.5.2/README.md
+-rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-07-03 15:13:24.228182 hydrogibs-0.5.2/setup.cfg
+-rw-rw-r--   0 axel      (1000) axel      (1000)      334 2023-07-03 15:10:21.000000 hydrogibs-0.5.2/setup.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-07-03 15:13:24.224182 hydrogibs-0.5.2/src/
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-07-03 15:13:24.228182 hydrogibs-0.5.2/src/hydrogibs.egg-info/
+-rw-rw-r--   0 axel      (1000) axel      (1000)      286 2023-07-03 15:13:24.000000 hydrogibs-0.5.2/src/hydrogibs.egg-info/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)      174 2023-07-03 15:13:24.000000 hydrogibs-0.5.2/src/hydrogibs.egg-info/SOURCES.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-07-03 15:13:24.000000 hydrogibs-0.5.2/src/hydrogibs.egg-info/dependency_links.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)       18 2023-07-03 15:13:24.000000 hydrogibs-0.5.2/src/hydrogibs.egg-info/top_level.txt
```

### Comparing `hydrogibs-0.0.25/LICENSE` & `hydrogibs-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.0.25/PKG-INFO` & `hydrogibs-0.5.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: hydrogibs
-Version: 0.0.25
-Summary: A personal hydrology and hydraulics package based on Christophe Ancey's teaching: http://fr.ancey.ch/cours/masterGC/cours-hydraulique.pdf
-Home-page: UNKNOWN
-Author: giboul
-Author-email: axel.giboulot@epfl.ch
-License: MIT
-Platform: UNKNOWN
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # hydrogibs
 
 Small hydrology package created for the sake of a class project with [Christophe Ancey](https://fr.ancey.ch/ "fr.ancey.ch").
 
 The only module that's currently usable is the GR4 model containing:
 
 
@@ -51,9 +38,7 @@
 ## An app to goof around with all parameters
 
  `App(catchment, rain)`
 
 # Example file
 
 `example.ipynb` might help you get the hang of this package
-
-
```

