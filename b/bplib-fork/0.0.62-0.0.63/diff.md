# Comparing `tmp/bplib_fork-0.0.62.tar.gz` & `tmp/bplib_fork-0.0.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bplib_fork-0.0.62.tar", last modified: Wed Jul  5 01:30:06 2023, max compression
+gzip compressed data, was "dist/bplib_fork-0.0.63.tar", last modified: Wed Jul  5 10:17:12 2023, max compression
```

## Comparing `bplib_fork-0.0.62.tar` & `bplib_fork-0.0.63.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-05 01:30:06.000000 bplib_fork-0.0.62/
--rw-r--r--   0 benjaminK   (501) staff       (20)       41 2023-07-05 01:13:50.000000 bplib_fork-0.0.62/MANIFEST.in
--rw-r--r--   0 benjaminK   (501) staff       (20)     1475 2023-07-05 01:30:06.000000 bplib_fork-0.0.62/PKG-INFO
--rw-r--r--   0 benjaminK   (501) staff       (20)      229 2023-07-05 01:13:50.000000 bplib_fork-0.0.62/README.md
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-05 01:30:06.000000 bplib_fork-0.0.62/bplib/
--rw-r--r--   0 benjaminK   (501) staff       (20)     1357 2023-07-05 01:30:03.000000 bplib_fork-0.0.62/bplib/__init__.py
--rw-r--r--   0 benjaminK   (501) staff       (20)      297 2023-07-05 01:13:50.000000 bplib_fork-0.0.62/bplib/bindings.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    19407 2023-07-05 01:13:50.000000 bplib_fork-0.0.62/bplib/bp.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    10817 2023-07-05 01:13:50.000000 bplib_fork-0.0.62/bplib/compile.py
--rw-r--r--   0 benjaminK   (501) staff       (20)     1713 2023-07-05 01:13:50.000000 bplib_fork-0.0.62/bplib/pack.py
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-05 01:30:06.000000 bplib_fork-0.0.62/bplib/src/
--rw-r--r--   0 benjaminK   (501) staff       (20)    22467 2023-07-05 01:13:50.000000 bplib_fork-0.0.62/bplib/src/bp_fp12.c
--rw-r--r--   0 benjaminK   (501) staff       (20)    14124 2023-07-05 01:13:50.000000 bplib_fork-0.0.62/bplib/src/bp_fp2.c
--rw-r--r--   0 benjaminK   (501) staff       (20)    14506 2023-07-05 01:13:50.000000 bplib_fork-0.0.62/bplib/src/bp_fp6.c
--rw-r--r--   0 benjaminK   (501) staff       (20)     8535 2023-07-05 01:13:50.000000 bplib_fork-0.0.62/bplib/src/bp_g1.c
--rw-r--r--   0 benjaminK   (501) staff       (20)    30707 2023-07-05 01:13:50.000000 bplib_fork-0.0.62/bplib/src/bp_g2.c
--rw-r--r--   0 benjaminK   (501) staff       (20)    27964 2023-07-05 01:13:50.000000 bplib_fork-0.0.62/bplib/src/bp_g2_mult.c
--rw-r--r--   0 benjaminK   (501) staff       (20)    16353 2023-07-05 01:13:50.000000 bplib_fork-0.0.62/bplib/src/bp_group.c
--rw-r--r--   0 benjaminK   (501) staff       (20)     8691 2023-07-05 01:13:50.000000 bplib_fork-0.0.62/bplib/src/bp_gt.c
--rw-r--r--   0 benjaminK   (501) staff       (20)    19235 2023-07-05 01:13:50.000000 bplib_fork-0.0.62/bplib/src/bp_map.c
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-05 01:30:06.000000 bplib_fork-0.0.62/bplib_fork.egg-info/
--rw-r--r--   0 benjaminK   (501) staff       (20)     1475 2023-07-05 01:30:06.000000 bplib_fork-0.0.62/bplib_fork.egg-info/PKG-INFO
--rw-r--r--   0 benjaminK   (501) staff       (20)      565 2023-07-05 01:30:06.000000 bplib_fork-0.0.62/bplib_fork.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)        1 2023-07-05 01:30:06.000000 bplib_fork-0.0.62/bplib_fork.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)        1 2023-07-05 01:15:36.000000 bplib_fork-0.0.62/bplib_fork.egg-info/not-zip-safe
--rw-r--r--   0 benjaminK   (501) staff       (20)      112 2023-07-05 01:30:06.000000 bplib_fork-0.0.62/bplib_fork.egg-info/requires.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)        6 2023-07-05 01:30:06.000000 bplib_fork-0.0.62/bplib_fork.egg-info/top_level.txt
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-05 01:30:06.000000 bplib_fork-0.0.62/examples/
--rw-r--r--   0 benjaminK   (501) staff       (20)     1383 2023-07-05 01:13:50.000000 bplib_fork-0.0.62/examples/PSH16mp3.py
--rw-r--r--   0 benjaminK   (501) staff       (20)     2023 2023-07-05 01:13:50.000000 bplib_fork-0.0.62/examples/PSSig.py
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-05 01:30:06.000000 bplib_fork-0.0.62/include/
--rw-r--r--   0 benjaminK   (501) staff       (20)    36468 2023-07-05 01:13:50.000000 bplib_fork-0.0.62/include/bp.h
--rw-r--r--   0 benjaminK   (501) staff       (20)    11641 2023-07-05 01:13:50.000000 bplib_fork-0.0.62/include/bp_lcl.h
--rw-r--r--   0 benjaminK   (501) staff       (20)      237 2023-07-05 01:30:06.000000 bplib_fork-0.0.62/setup.cfg
--rw-r--r--   0 benjaminK   (501) staff       (20)     1145 2023-07-05 01:26:18.000000 bplib_fork-0.0.62/setup.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-05 10:17:12.000000 bplib_fork-0.0.63/
+-rw-r--r--   0 benjaminK   (501) staff       (20)       41 2023-07-05 01:13:50.000000 bplib_fork-0.0.63/MANIFEST.in
+-rw-r--r--   0 benjaminK   (501) staff       (20)     1475 2023-07-05 10:17:12.000000 bplib_fork-0.0.63/PKG-INFO
+-rw-r--r--   0 benjaminK   (501) staff       (20)      229 2023-07-05 01:13:50.000000 bplib_fork-0.0.63/README.md
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-05 10:17:12.000000 bplib_fork-0.0.63/bplib/
+-rw-r--r--   0 benjaminK   (501) staff       (20)     1357 2023-07-05 10:16:49.000000 bplib_fork-0.0.63/bplib/__init__.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)      297 2023-07-05 01:13:50.000000 bplib_fork-0.0.63/bplib/bindings.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    19407 2023-07-05 01:13:50.000000 bplib_fork-0.0.63/bplib/bp.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    10817 2023-07-05 01:13:50.000000 bplib_fork-0.0.63/bplib/compile.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)     1713 2023-07-05 01:13:50.000000 bplib_fork-0.0.63/bplib/pack.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-05 10:17:12.000000 bplib_fork-0.0.63/bplib/src/
+-rw-r--r--   0 benjaminK   (501) staff       (20)    22467 2023-07-05 01:13:50.000000 bplib_fork-0.0.63/bplib/src/bp_fp12.c
+-rw-r--r--   0 benjaminK   (501) staff       (20)    14124 2023-07-05 01:13:50.000000 bplib_fork-0.0.63/bplib/src/bp_fp2.c
+-rw-r--r--   0 benjaminK   (501) staff       (20)    14506 2023-07-05 01:13:50.000000 bplib_fork-0.0.63/bplib/src/bp_fp6.c
+-rw-r--r--   0 benjaminK   (501) staff       (20)     8535 2023-07-05 01:13:50.000000 bplib_fork-0.0.63/bplib/src/bp_g1.c
+-rw-r--r--   0 benjaminK   (501) staff       (20)    30707 2023-07-05 01:13:50.000000 bplib_fork-0.0.63/bplib/src/bp_g2.c
+-rw-r--r--   0 benjaminK   (501) staff       (20)    27964 2023-07-05 01:13:50.000000 bplib_fork-0.0.63/bplib/src/bp_g2_mult.c
+-rw-r--r--   0 benjaminK   (501) staff       (20)    16353 2023-07-05 01:13:50.000000 bplib_fork-0.0.63/bplib/src/bp_group.c
+-rw-r--r--   0 benjaminK   (501) staff       (20)     8691 2023-07-05 01:13:50.000000 bplib_fork-0.0.63/bplib/src/bp_gt.c
+-rw-r--r--   0 benjaminK   (501) staff       (20)    19235 2023-07-05 01:13:50.000000 bplib_fork-0.0.63/bplib/src/bp_map.c
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-05 10:17:12.000000 bplib_fork-0.0.63/bplib_fork.egg-info/
+-rw-r--r--   0 benjaminK   (501) staff       (20)     1475 2023-07-05 10:17:12.000000 bplib_fork-0.0.63/bplib_fork.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminK   (501) staff       (20)      565 2023-07-05 10:17:12.000000 bplib_fork-0.0.63/bplib_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)        1 2023-07-05 10:17:12.000000 bplib_fork-0.0.63/bplib_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)        1 2023-07-05 01:15:36.000000 bplib_fork-0.0.63/bplib_fork.egg-info/not-zip-safe
+-rw-r--r--   0 benjaminK   (501) staff       (20)      117 2023-07-05 10:17:12.000000 bplib_fork-0.0.63/bplib_fork.egg-info/requires.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)        6 2023-07-05 10:17:12.000000 bplib_fork-0.0.63/bplib_fork.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-05 10:17:12.000000 bplib_fork-0.0.63/examples/
+-rw-r--r--   0 benjaminK   (501) staff       (20)     1383 2023-07-05 01:13:50.000000 bplib_fork-0.0.63/examples/PSH16mp3.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)     2023 2023-07-05 01:13:50.000000 bplib_fork-0.0.63/examples/PSSig.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-05 10:17:12.000000 bplib_fork-0.0.63/include/
+-rw-r--r--   0 benjaminK   (501) staff       (20)    36468 2023-07-05 01:13:50.000000 bplib_fork-0.0.63/include/bp.h
+-rw-r--r--   0 benjaminK   (501) staff       (20)    11641 2023-07-05 01:13:50.000000 bplib_fork-0.0.63/include/bp_lcl.h
+-rw-r--r--   0 benjaminK   (501) staff       (20)      237 2023-07-05 10:17:12.000000 bplib_fork-0.0.63/setup.cfg
+-rw-r--r--   0 benjaminK   (501) staff       (20)     1160 2023-07-05 10:15:53.000000 bplib_fork-0.0.63/setup.py
```

### Comparing `bplib_fork-0.0.62/PKG-INFO` & `bplib_fork-0.0.63/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bplib_fork
-Version: 0.0.62
+Version: 0.0.63
 Summary: A bilinear pairing library for petlib.
 Home-page: https://pypi.python.org/pypi/bplib/
 Author: George Danezis
 Author-email: g.danezis@ucl.ac.uk
 License: LGPL
 
 The ``bplib`` is a library implementing support for computations on groups supporting
```

### Comparing `bplib_fork-0.0.62/bplib/__init__.py` & `bplib_fork-0.0.63/bplib/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,8 +38,8 @@
     >>> G.pair(6*g1, g2) == gt6
     True
     >>> G.pair(2*g1, 3*g2) == gt6
     True
 
 """
 
-VERSION = "0.0.62"
+VERSION = "0.0.63"
```

### Comparing `bplib_fork-0.0.62/bplib/bp.py` & `bplib_fork-0.0.63/bplib/bp.py`

 * *Files identical despite different names*

### Comparing `bplib_fork-0.0.62/bplib/compile.py` & `bplib_fork-0.0.63/bplib/compile.py`

 * *Files identical despite different names*

### Comparing `bplib_fork-0.0.62/bplib/pack.py` & `bplib_fork-0.0.63/bplib/pack.py`

 * *Files identical despite different names*

### Comparing `bplib_fork-0.0.62/bplib/src/bp_fp12.c` & `bplib_fork-0.0.63/bplib/src/bp_fp12.c`

 * *Files identical despite different names*

### Comparing `bplib_fork-0.0.62/bplib/src/bp_fp2.c` & `bplib_fork-0.0.63/bplib/src/bp_fp2.c`

 * *Files identical despite different names*

### Comparing `bplib_fork-0.0.62/bplib/src/bp_fp6.c` & `bplib_fork-0.0.63/bplib/src/bp_fp6.c`

 * *Files identical despite different names*

### Comparing `bplib_fork-0.0.62/bplib/src/bp_g1.c` & `bplib_fork-0.0.63/bplib/src/bp_g1.c`

 * *Files identical despite different names*

### Comparing `bplib_fork-0.0.62/bplib/src/bp_g2.c` & `bplib_fork-0.0.63/bplib/src/bp_g2.c`

 * *Files identical despite different names*

### Comparing `bplib_fork-0.0.62/bplib/src/bp_g2_mult.c` & `bplib_fork-0.0.63/bplib/src/bp_g2_mult.c`

 * *Files identical despite different names*

### Comparing `bplib_fork-0.0.62/bplib/src/bp_group.c` & `bplib_fork-0.0.63/bplib/src/bp_group.c`

 * *Files identical despite different names*

### Comparing `bplib_fork-0.0.62/bplib/src/bp_gt.c` & `bplib_fork-0.0.63/bplib/src/bp_gt.c`

 * *Files identical despite different names*

### Comparing `bplib_fork-0.0.62/bplib/src/bp_map.c` & `bplib_fork-0.0.63/bplib/src/bp_map.c`

 * *Files identical despite different names*

### Comparing `bplib_fork-0.0.62/bplib_fork.egg-info/PKG-INFO` & `bplib_fork-0.0.63/bplib_fork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bplib-fork
-Version: 0.0.62
+Version: 0.0.63
 Summary: A bilinear pairing library for petlib.
 Home-page: https://pypi.python.org/pypi/bplib/
 Author: George Danezis
 Author-email: g.danezis@ucl.ac.uk
 License: LGPL
 
 The ``bplib`` is a library implementing support for computations on groups supporting
```

### Comparing `bplib_fork-0.0.62/bplib_fork.egg-info/SOURCES.txt` & `bplib_fork-0.0.63/bplib_fork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bplib_fork-0.0.62/examples/PSH16mp3.py` & `bplib_fork-0.0.63/examples/PSH16mp3.py`

 * *Files identical despite different names*

### Comparing `bplib_fork-0.0.62/examples/PSSig.py` & `bplib_fork-0.0.63/examples/PSSig.py`

 * *Files identical despite different names*

### Comparing `bplib_fork-0.0.62/include/bp.h` & `bplib_fork-0.0.63/include/bp.h`

 * *Files identical despite different names*

### Comparing `bplib_fork-0.0.62/include/bp_lcl.h` & `bplib_fork-0.0.63/include/bp_lcl.h`

 * *Files identical despite different names*

### Comparing `bplib_fork-0.0.62/setup.py` & `bplib_fork-0.0.63/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,31 +12,31 @@
       url=r'https://pypi.python.org/pypi/bplib/',
       packages=['bplib'],
       license="LGPL",
       long_description=bplib.__doc__,
 
       setup_requires=["cffi>=1.0.0",
                       "pytest >= 2.6.4",
-                      "petlib >= 0.0.45"],
+                      "petlib_fork >= 0.0.45"],
       package_data={
           "bplib": ["include/*.h"]},
       include_package_data=True,
       tests_require=[
           "cffi >= 1.0.0",
           "pycparser >= 2.10",
           "future >= 0.14.3",
           "pytest >= 2.5.0",
           "pytest-cov >= 1.8.1",
-          "petlib >= 0.0.43"
+          "petlib_fork >= 0.0.43"
       ],
       cffi_modules=["bplib/compile.py:ffibuilder"],
       install_requires=[
           "cffi >= 1.0.0",
           "pycparser >= 2.10",
           "future >= 0.14.3",
           "pytest >= 2.5.0",
           "pytest-cov >= 1.8.1",
           "msgpack-python >= 0.4.6",
-          "petlib >= 0.0.43"
+          "petlib_fork >= 0.0.43"
       ],
       zip_safe=False,
       )
```

