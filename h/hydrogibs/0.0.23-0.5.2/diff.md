# Comparing `tmp/hydrogibs-0.0.23.tar.gz` & `tmp/hydrogibs-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrogibs-0.0.23.tar", last modified: Wed Jul  5 07:33:47 2023, max compression
+gzip compressed data, was "hydrogibs-0.5.2.tar", last modified: Mon Jul  3 15:13:24 2023, max compression
```

## Comparing `hydrogibs-0.0.23.tar` & `hydrogibs-0.5.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-07-05 07:33:47.196751 hydrogibs-0.0.23/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.0.23/LICENSE
--rw-rw-r--   0 axel      (1000) axel      (1000)     1396 2023-07-05 07:33:47.196751 hydrogibs-0.0.23/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)     1008 2023-05-23 16:56:32.000000 hydrogibs-0.0.23/README.md
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-07-05 07:33:47.192751 hydrogibs-0.0.23/hydrogibs/
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-07-05 07:33:47.196751 hydrogibs-0.0.23/hydrogibs/hydrogibs.egg-info/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1396 2023-07-05 07:33:47.000000 hydrogibs-0.0.23/hydrogibs/hydrogibs.egg-info/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)      240 2023-07-05 07:33:47.000000 hydrogibs-0.0.23/hydrogibs/hydrogibs.egg-info/SOURCES.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-07-05 07:33:47.000000 hydrogibs-0.0.23/hydrogibs/hydrogibs.egg-info/dependency_links.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)       12 2023-07-05 07:33:47.000000 hydrogibs-0.0.23/hydrogibs/hydrogibs.egg-info/requires.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-07-05 07:33:47.000000 hydrogibs-0.0.23/hydrogibs/hydrogibs.egg-info/top_level.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-07-05 07:33:47.196751 hydrogibs-0.0.23/setup.cfg
--rw-rw-r--   0 axel      (1000) axel      (1000)      674 2023-07-05 07:33:33.000000 hydrogibs-0.0.23/setup.py
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

### Comparing `hydrogibs-0.0.23/LICENSE` & `hydrogibs-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.0.23/PKG-INFO` & `hydrogibs-0.5.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: hydrogibs
-Version: 0.0.23
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

