# Comparing `tmp/codon-jit-0.1.5.tar.gz` & `tmp/codon-jit-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codon-jit-0.1.5.tar", last modified: Tue May 23 23:48:27 2023, max compression
+gzip compressed data, was "codon-jit-0.1.6.tar", last modified: Wed Jul  5 16:25:59 2023, max compression
```

## Comparing `codon-jit-0.1.5.tar` & `codon-jit-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:48:27.295497 codon-jit-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:31:40.000000 codon-jit-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-23 23:48:27.295497 codon-jit-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-23 23:31:40.000000 codon-jit-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:48:27.291497 codon-jit-0.1.5/codon/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-23 23:31:40.000000 codon-jit-0.1.5/codon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-05-23 23:31:40.000000 codon-jit-0.1.5/codon/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-23 23:31:40.000000 codon-jit-0.1.5/codon/jit.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-23 23:31:40.000000 codon-jit-0.1.5/codon/jit.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-23 23:32:11.000000 codon-jit-0.1.5/codon/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:48:27.295497 codon-jit-0.1.5/codon_jit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-23 23:48:27.000000 codon-jit-0.1.5/codon_jit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-23 23:48:27.000000 codon-jit-0.1.5/codon_jit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:48:27.000000 codon-jit-0.1.5/codon_jit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 23:48:27.000000 codon-jit-0.1.5/codon_jit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 23:48:27.000000 codon-jit-0.1.5/codon_jit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-23 23:31:40.000000 codon-jit-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 23:48:27.295497 codon-jit-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-23 23:31:40.000000 codon-jit-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:25:59.617308 codon-jit-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:05:55.000000 codon-jit-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-05 16:25:59.617308 codon-jit-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-05 16:05:55.000000 codon-jit-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:25:59.617308 codon-jit-0.1.6/codon/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-05 16:05:55.000000 codon-jit-0.1.6/codon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-05 16:05:55.000000 codon-jit-0.1.6/codon/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-05 16:05:55.000000 codon-jit-0.1.6/codon/jit.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-05 16:05:55.000000 codon-jit-0.1.6/codon/jit.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-05 16:06:36.000000 codon-jit-0.1.6/codon/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:25:59.617308 codon-jit-0.1.6/codon_jit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-05 16:25:59.000000 codon-jit-0.1.6/codon_jit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-05 16:25:59.000000 codon-jit-0.1.6/codon_jit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:25:59.000000 codon-jit-0.1.6/codon_jit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 16:25:59.000000 codon-jit-0.1.6/codon_jit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 16:25:59.000000 codon-jit-0.1.6/codon_jit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-05 16:05:55.000000 codon-jit-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 16:25:59.617308 codon-jit-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-05 16:05:55.000000 codon-jit-0.1.6/setup.py
```

### Comparing `codon-jit-0.1.5/codon/decorator.py` & `codon-jit-0.1.6/codon/decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import ctypes
 import inspect
 import sys
 import os
 import functools
 import itertools
 import ast
-import shutil
 import astunparse
 from pathlib import Path
 
 sys.setdlopenflags(sys.getdlopenflags() | ctypes.RTLD_GLOBAL)
 
 from .codon_jit import JITWrapper, JITError, codon_library
 
@@ -126,17 +125,21 @@
         lines = inspect.getsourcelines(obj)[0]
         extra_spaces = lines[0].find("class")
         obj_str = "".join(l[extra_spaces:] for l in lines)
     elif callable(obj):
         lines = inspect.getsourcelines(obj)[0]
         extra_spaces = lines[0].find("@")
         obj_str = "".join(l[extra_spaces:] for l in lines[1:])
-        if kwargs.get("pyvars", None):
+        pyvars = kwargs.get("pyvars", None)
+        if pyvars:
+            for i in pyvars:
+                if not isinstance(i, str):
+                    raise ValueError("pyvars only takes string literals")
             node = ast.fix_missing_locations(
-                RewriteFunctionArgs(kwargs["pyvars"]).visit(ast.parse(obj_str))
+                RewriteFunctionArgs(pyvars).visit(ast.parse(obj_str))
             )
             obj_str = astunparse.unparse(node)
     else:
         raise TypeError("Function or class expected, got " + type(obj).__name__)
     return obj_str.replace("_@par", "@par")
```

### Comparing `codon-jit-0.1.5/codon/jit.pxd` & `codon-jit-0.1.6/codon/jit.pxd`

 * *Files identical despite different names*

### Comparing `codon-jit-0.1.5/codon/jit.pyx` & `codon-jit-0.1.6/codon/jit.pyx`

 * *Files identical despite different names*

### Comparing `codon-jit-0.1.5/setup.py` & `codon-jit-0.1.6/setup.py`

 * *Files identical despite different names*

