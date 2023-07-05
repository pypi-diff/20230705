# Comparing `tmp/mvpoly-0.98.1.tar.gz` & `tmp/mvpoly-0.98.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvpoly-0.98.1.tar", last modified: Wed Mar 22 22:30:35 2023, max compression
+gzip compressed data, was "mvpoly-0.98.2.tar", last modified: Wed Jul  5 14:59:13 2023, max compression
```

## Comparing `mvpoly-0.98.1.tar` & `mvpoly-0.98.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 jjg       (1000) jjg       (1000)        0 2023-03-22 22:30:35.052127 mvpoly-0.98.1/
--rw-rw-r--   0 jjg       (1000) jjg       (1000)       19 2019-01-24 00:17:12.000000 mvpoly-0.98.1/MANIFEST.in
--rw-rw-r--   0 jjg       (1000) jjg       (1000)      987 2023-03-22 22:30:35.052127 mvpoly-0.98.1/PKG-INFO
--rw-r--r--   0 jjg       (1000) jjg       (1000)      106 2013-06-26 22:49:19.000000 mvpoly-0.98.1/README.rst
--rw-rw-r--   0 jjg       (1000) jjg       (1000)       90 2023-03-22 18:50:58.000000 mvpoly-0.98.1/pyproject.toml
--rw-rw-r--   0 jjg       (1000) jjg       (1000)     1273 2023-03-22 22:30:35.056126 mvpoly-0.98.1/setup.cfg
-drwxrwxr-x   0 jjg       (1000) jjg       (1000)        0 2023-03-22 22:30:35.012126 mvpoly-0.98.1/src/
-drwxrwxr-x   0 jjg       (1000) jjg       (1000)        0 2023-03-22 22:30:35.048127 mvpoly-0.98.1/src/mvpoly/
--rw-rw-r--   0 jjg       (1000) jjg       (1000)        0 2023-03-22 18:50:58.000000 mvpoly-0.98.1/src/mvpoly/__init__.py
--rw-rw-r--   0 jjg       (1000) jjg       (1000)    13017 2023-03-22 18:50:58.000000 mvpoly-0.98.1/src/mvpoly/base.py
--rw-rw-r--   0 jjg       (1000) jjg       (1000)    15701 2023-03-22 18:50:58.000000 mvpoly-0.98.1/src/mvpoly/cube.py
--rw-rw-r--   0 jjg       (1000) jjg       (1000)    20899 2023-03-22 18:50:58.000000 mvpoly-0.98.1/src/mvpoly/dict.py
--rw-rw-r--   0 jjg       (1000) jjg       (1000)    16099 2023-03-22 18:50:58.000000 mvpoly-0.98.1/src/mvpoly/rbf.py
-drwxrwxr-x   0 jjg       (1000) jjg       (1000)        0 2023-03-22 22:30:35.052127 mvpoly-0.98.1/src/mvpoly/util/
--rw-rw-r--   0 jjg       (1000) jjg       (1000)        0 2023-03-22 18:50:58.000000 mvpoly-0.98.1/src/mvpoly/util/__init__.py
--rw-rw-r--   0 jjg       (1000) jjg       (1000)      778 2023-03-22 18:50:58.000000 mvpoly-0.98.1/src/mvpoly/util/cached_property.py
--rw-rw-r--   0 jjg       (1000) jjg       (1000)     2354 2023-03-22 18:50:58.000000 mvpoly-0.98.1/src/mvpoly/util/common.py
--rw-rw-r--   0 jjg       (1000) jjg       (1000)     7571 2023-03-22 18:50:58.000000 mvpoly-0.98.1/src/mvpoly/util/cube.py
--rw-rw-r--   0 jjg       (1000) jjg       (1000)     1307 2023-03-22 18:50:58.000000 mvpoly-0.98.1/src/mvpoly/util/dict.py
--rw-rw-r--   0 jjg       (1000) jjg       (1000)      297 2023-03-22 18:50:58.000000 mvpoly-0.98.1/src/mvpoly/util/dtype.py
--rw-rw-r--   0 jjg       (1000) jjg       (1000)      408 2023-03-22 18:50:58.000000 mvpoly-0.98.1/src/mvpoly/util/version.py
+drwxrwxr-x   0 jjg       (1000) jjg       (1000)        0 2023-07-05 14:59:13.434681 mvpoly-0.98.2/
+-rw-rw-r--   0 jjg       (1000) jjg       (1000)       19 2019-01-24 00:17:12.000000 mvpoly-0.98.2/MANIFEST.in
+-rw-rw-r--   0 jjg       (1000) jjg       (1000)     1474 2023-07-05 14:59:13.434681 mvpoly-0.98.2/PKG-INFO
+-rw-r--r--   0 jjg       (1000) jjg       (1000)      593 2023-07-05 12:01:58.000000 mvpoly-0.98.2/README.rst
+-rw-rw-r--   0 jjg       (1000) jjg       (1000)       90 2023-03-22 18:50:58.000000 mvpoly-0.98.2/pyproject.toml
+-rw-rw-r--   0 jjg       (1000) jjg       (1000)     1273 2023-07-05 14:59:13.434681 mvpoly-0.98.2/setup.cfg
+drwxrwxr-x   0 jjg       (1000) jjg       (1000)        0 2023-07-05 14:59:13.422681 mvpoly-0.98.2/src/
+drwxrwxr-x   0 jjg       (1000) jjg       (1000)        0 2023-07-05 14:59:13.426681 mvpoly-0.98.2/src/mvpoly/
+-rw-rw-r--   0 jjg       (1000) jjg       (1000)        0 2023-03-22 18:50:58.000000 mvpoly-0.98.2/src/mvpoly/__init__.py
+-rw-rw-r--   0 jjg       (1000) jjg       (1000)    12992 2023-03-23 00:53:35.000000 mvpoly-0.98.2/src/mvpoly/base.py
+-rw-rw-r--   0 jjg       (1000) jjg       (1000)    15701 2023-03-22 18:50:58.000000 mvpoly-0.98.2/src/mvpoly/cube.py
+-rw-rw-r--   0 jjg       (1000) jjg       (1000)    20875 2023-03-23 00:53:57.000000 mvpoly-0.98.2/src/mvpoly/dict.py
+-rw-rw-r--   0 jjg       (1000) jjg       (1000)    16083 2023-03-23 00:54:29.000000 mvpoly-0.98.2/src/mvpoly/rbf.py
+drwxrwxr-x   0 jjg       (1000) jjg       (1000)        0 2023-07-05 14:59:13.430681 mvpoly-0.98.2/src/mvpoly/util/
+-rw-rw-r--   0 jjg       (1000) jjg       (1000)        0 2023-03-22 18:50:58.000000 mvpoly-0.98.2/src/mvpoly/util/__init__.py
+-rw-rw-r--   0 jjg       (1000) jjg       (1000)      778 2023-03-22 18:50:58.000000 mvpoly-0.98.2/src/mvpoly/util/cached_property.py
+-rw-rw-r--   0 jjg       (1000) jjg       (1000)     2354 2023-03-22 18:50:58.000000 mvpoly-0.98.2/src/mvpoly/util/common.py
+-rw-rw-r--   0 jjg       (1000) jjg       (1000)     7571 2023-03-22 18:50:58.000000 mvpoly-0.98.2/src/mvpoly/util/cube.py
+-rw-rw-r--   0 jjg       (1000) jjg       (1000)     1307 2023-03-22 18:50:58.000000 mvpoly-0.98.2/src/mvpoly/util/dict.py
+-rw-rw-r--   0 jjg       (1000) jjg       (1000)      297 2023-03-22 18:50:58.000000 mvpoly-0.98.2/src/mvpoly/util/dtype.py
+-rw-rw-r--   0 jjg       (1000) jjg       (1000)      408 2023-03-22 18:50:58.000000 mvpoly-0.98.2/src/mvpoly/util/version.py
```

### Comparing `mvpoly-0.98.1/setup.cfg` & `mvpoly-0.98.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mvpoly
-version = 0.98.1
+version = 0.98.2
 url = http://soliton.vm.bytemark.co.uk/pub/jjg/en/code/mvpoly/
 author = J.J. Green
 author_email = j.j.green@gmx.co.uk
 description = A library for multivariate polynomials
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords =
```

### Comparing `mvpoly-0.98.1/src/mvpoly/base.py` & `mvpoly-0.98.2/src/mvpoly/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 import numpy as np
 import mvpoly.util.common
 import mvpoly.util.version
 import scipy.integrate
 import scipy.special
```

### Comparing `mvpoly-0.98.1/src/mvpoly/cube.py` & `mvpoly-0.98.2/src/mvpoly/cube.py`

 * *Files identical despite different names*

### Comparing `mvpoly-0.98.1/src/mvpoly/dict.py` & `mvpoly-0.98.2/src/mvpoly/dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 
 .. class:: MVPolyDict
    :synopsis: Multivariate polynomial class whose
    coefficient representation is a dictionary
 
 .. moduleauthor:: J.J. Green <j.j.green@gmx.co.uk>
```

### Comparing `mvpoly-0.98.1/src/mvpoly/rbf.py` & `mvpoly-0.98.2/src/mvpoly/rbf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding: utf-8
 """
 Hybrid RBF-polynomial interpolation and approximation.
 """
 
 # This code is a derived work from the file of the same name in
 # the SciPy library, based closely on Matlab code by Alex Chirokov
 # and
```

### Comparing `mvpoly-0.98.1/src/mvpoly/util/cached_property.py` & `mvpoly-0.98.2/src/mvpoly/util/cached_property.py`

 * *Files identical despite different names*

### Comparing `mvpoly-0.98.1/src/mvpoly/util/common.py` & `mvpoly-0.98.2/src/mvpoly/util/common.py`

 * *Files identical despite different names*

### Comparing `mvpoly-0.98.1/src/mvpoly/util/cube.py` & `mvpoly-0.98.2/src/mvpoly/util/cube.py`

 * *Files identical despite different names*

### Comparing `mvpoly-0.98.1/src/mvpoly/util/dict.py` & `mvpoly-0.98.2/src/mvpoly/util/dict.py`

 * *Files identical despite different names*

