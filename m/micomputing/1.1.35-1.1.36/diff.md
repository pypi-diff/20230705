# Comparing `tmp/micomputing-1.1.35.tar.gz` & `tmp/micomputing-1.1.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micomputing-1.1.35.tar", last modified: Wed Jul  5 08:20:40 2023, max compression
+gzip compressed data, was "micomputing-1.1.36.tar", last modified: Wed Jul  5 08:28:37 2023, max compression
```

## Comparing `micomputing-1.1.35.tar` & `micomputing-1.1.36.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:20:40.556253 micomputing-1.1.35/
--rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-05 08:20:40.556098 micomputing-1.1.35/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      766 2023-07-05 08:20:40.000000 micomputing-1.1.35/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:20:40.554812 micomputing-1.1.35/micomputing/
--rw-r--r--   0 admin      (501) staff       (20)     2336 2023-07-05 08:20:40.000000 micomputing-1.1.35/micomputing/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-05 08:20:40.000000 micomputing-1.1.35/micomputing/data.py
--rw-r--r--   0 admin      (501) staff       (20)    37891 2023-07-05 08:20:40.000000 micomputing-1.1.35/micomputing/funcs.py
--rw-r--r--   0 admin      (501) staff       (20)    54244 2023-07-05 08:20:40.000000 micomputing-1.1.35/micomputing/metrics.py
--rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-05 08:20:40.000000 micomputing-1.1.35/micomputing/network.py
--rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-05 08:20:40.000000 micomputing-1.1.35/micomputing/plot.py
--rw-r--r--   0 admin      (501) staff       (20)    41826 2023-07-05 08:20:40.000000 micomputing-1.1.35/micomputing/stdio.py
--rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-05 08:20:40.000000 micomputing-1.1.35/micomputing/test.py
--rw-r--r--   0 admin      (501) staff       (20)    98769 2023-07-05 08:20:40.000000 micomputing-1.1.35/micomputing/trans.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:20:40.555837 micomputing-1.1.35/micomputing.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-05 08:20:40.000000 micomputing-1.1.35/micomputing.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      385 2023-07-05 08:20:40.000000 micomputing-1.1.35/micomputing.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-05 08:20:40.000000 micomputing-1.1.35/micomputing.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       72 2023-07-05 08:20:40.000000 micomputing-1.1.35/micomputing.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       12 2023-07-05 08:20:40.000000 micomputing-1.1.35/micomputing.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-05 08:20:40.556307 micomputing-1.1.35/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1883 2023-07-05 08:20:40.000000 micomputing-1.1.35/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:28:37.408757 micomputing-1.1.36/
+-rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-05 08:28:37.408610 micomputing-1.1.36/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      766 2023-07-05 08:28:37.000000 micomputing-1.1.36/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:28:37.407715 micomputing-1.1.36/micomputing/
+-rw-r--r--   0 admin      (501) staff       (20)     2361 2023-07-05 08:28:37.000000 micomputing-1.1.36/micomputing/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-05 08:28:37.000000 micomputing-1.1.36/micomputing/data.py
+-rw-r--r--   0 admin      (501) staff       (20)    37891 2023-07-05 08:28:37.000000 micomputing-1.1.36/micomputing/funcs.py
+-rw-r--r--   0 admin      (501) staff       (20)    54244 2023-07-05 08:28:37.000000 micomputing-1.1.36/micomputing/metrics.py
+-rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-05 08:28:37.000000 micomputing-1.1.36/micomputing/network.py
+-rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-05 08:28:37.000000 micomputing-1.1.36/micomputing/plot.py
+-rw-r--r--   0 admin      (501) staff       (20)    41826 2023-07-05 08:28:37.000000 micomputing-1.1.36/micomputing/stdio.py
+-rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-05 08:28:37.000000 micomputing-1.1.36/micomputing/test.py
+-rw-r--r--   0 admin      (501) staff       (20)    98769 2023-07-05 08:28:37.000000 micomputing-1.1.36/micomputing/trans.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:28:37.408400 micomputing-1.1.36/micomputing.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-05 08:28:37.000000 micomputing-1.1.36/micomputing.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      385 2023-07-05 08:28:37.000000 micomputing-1.1.36/micomputing.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-05 08:28:37.000000 micomputing-1.1.36/micomputing.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       72 2023-07-05 08:28:37.000000 micomputing-1.1.36/micomputing.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       12 2023-07-05 08:28:37.000000 micomputing-1.1.36/micomputing.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-05 08:28:37.408807 micomputing-1.1.36/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1482 2023-07-05 08:28:37.000000 micomputing-1.1.36/setup.py
```

### Comparing `micomputing-1.1.35/PKG-INFO` & `micomputing-1.1.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micomputing
-Version: 1.1.35
+Version: 1.1.36
 Summary: 'micomputing' is a package for medical image computing. 
 Home-page: https://github.com/Bertie97/PyZMyc/micomputing
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # MIComputing
```

### Comparing `micomputing-1.1.35/README.md` & `micomputing-1.1.36/README.md`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.35/micomputing/__init__.py` & `micomputing-1.1.36/micomputing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 from pycamia import info_manager
 
 __info__ = info_manager(
     project = 'PyCAMIA',
     package = 'micomputing',
     author = 'Yuncheng Zhou',
     create = '2021-12',
-    version = '1.1.34',
+    version = '1.1.35',
     contact = 'bertiezhou@163.com',
     keywords = ['medical image', 'image registration', 'image similarities'],
     description = "'micomputing' is a package for medical image computing. ",
     requires = ['numpy', 'torch>=1.5.1', 'batorch', 'pycamia', 'pyoverload', 'nibabel', 'pydicom', 'SimpleITK'],
-    update = '2023-07-05 14:57:53'
+    update = '2023-07-05 16:20:40',
+    package_data = True
 ).check()
 
 from . import plot as plt
 from .stdio import IMG, dcm2nii, nii2dcm #*
 from .data import Info, Subject, ImageObject, Dataset, MedicalDataset #*
 from .network import U_Net, CNN, FCN
 from .funcs import reorient, rescale, reflect, dilate, blur, bending, distance_map, registration, local_prior, center_of_gravity #*
```

### Comparing `micomputing-1.1.35/micomputing/data.py` & `micomputing-1.1.36/micomputing/data.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.35/micomputing/funcs.py` & `micomputing-1.1.36/micomputing/funcs.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.35/micomputing/metrics.py` & `micomputing-1.1.36/micomputing/metrics.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.35/micomputing/network.py` & `micomputing-1.1.36/micomputing/network.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.35/micomputing/plot.py` & `micomputing-1.1.36/micomputing/plot.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.35/micomputing/stdio.py` & `micomputing-1.1.36/micomputing/stdio.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.35/micomputing/test.py` & `micomputing-1.1.36/micomputing/test.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.35/micomputing/trans.py` & `micomputing-1.1.36/micomputing/trans.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.35/micomputing.egg-info/PKG-INFO` & `micomputing-1.1.36/micomputing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micomputing
-Version: 1.1.35
+Version: 1.1.36
 Summary: 'micomputing' is a package for medical image computing. 
 Home-page: https://github.com/Bertie97/PyZMyc/micomputing
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # MIComputing
```

