# Comparing `tmp/micomputing-1.1.33.tar.gz` & `tmp/micomputing-1.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micomputing-1.1.33.tar", last modified: Wed Jul  5 06:46:32 2023, max compression
+gzip compressed data, was "micomputing-1.1.34.tar", last modified: Wed Jul  5 06:57:53 2023, max compression
```

## Comparing `micomputing-1.1.33.tar` & `micomputing-1.1.34.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:32.215663 micomputing-1.1.33/
--rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-05 06:46:32.215525 micomputing-1.1.33/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      766 2023-07-05 06:46:31.000000 micomputing-1.1.33/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:32.214421 micomputing-1.1.33/micomputing/
--rw-r--r--   0 admin      (501) staff       (20)     2336 2023-07-05 06:46:31.000000 micomputing-1.1.33/micomputing/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-05 06:46:31.000000 micomputing-1.1.33/micomputing/data.py
--rw-r--r--   0 admin      (501) staff       (20)    37891 2023-07-05 06:46:31.000000 micomputing-1.1.33/micomputing/funcs.py
--rw-r--r--   0 admin      (501) staff       (20)    54244 2023-07-05 06:46:31.000000 micomputing-1.1.33/micomputing/metrics.py
--rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-05 06:46:31.000000 micomputing-1.1.33/micomputing/network.py
--rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-05 06:46:31.000000 micomputing-1.1.33/micomputing/plot.py
--rw-r--r--   0 admin      (501) staff       (20)    41826 2023-07-05 06:46:31.000000 micomputing-1.1.33/micomputing/stdio.py
--rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-05 06:46:31.000000 micomputing-1.1.33/micomputing/test.py
--rw-r--r--   0 admin      (501) staff       (20)    98769 2023-07-05 06:46:31.000000 micomputing-1.1.33/micomputing/trans.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:32.215287 micomputing-1.1.33/micomputing.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-05 06:46:32.000000 micomputing-1.1.33/micomputing.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      385 2023-07-05 06:46:32.000000 micomputing-1.1.33/micomputing.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-05 06:46:32.000000 micomputing-1.1.33/micomputing.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       72 2023-07-05 06:46:32.000000 micomputing-1.1.33/micomputing.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       12 2023-07-05 06:46:32.000000 micomputing-1.1.33/micomputing.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-05 06:46:32.215714 micomputing-1.1.33/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1482 2023-07-05 06:46:31.000000 micomputing-1.1.33/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:57:53.355531 micomputing-1.1.34/
+-rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-05 06:57:53.355360 micomputing-1.1.34/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      766 2023-07-05 06:57:53.000000 micomputing-1.1.34/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:57:53.354195 micomputing-1.1.34/micomputing/
+-rw-r--r--   0 admin      (501) staff       (20)     2336 2023-07-05 06:57:53.000000 micomputing-1.1.34/micomputing/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-05 06:57:53.000000 micomputing-1.1.34/micomputing/data.py
+-rw-r--r--   0 admin      (501) staff       (20)    37891 2023-07-05 06:57:53.000000 micomputing-1.1.34/micomputing/funcs.py
+-rw-r--r--   0 admin      (501) staff       (20)    54244 2023-07-05 06:57:53.000000 micomputing-1.1.34/micomputing/metrics.py
+-rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-05 06:57:53.000000 micomputing-1.1.34/micomputing/network.py
+-rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-05 06:57:53.000000 micomputing-1.1.34/micomputing/plot.py
+-rw-r--r--   0 admin      (501) staff       (20)    41826 2023-07-05 06:57:53.000000 micomputing-1.1.34/micomputing/stdio.py
+-rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-05 06:57:53.000000 micomputing-1.1.34/micomputing/test.py
+-rw-r--r--   0 admin      (501) staff       (20)    98769 2023-07-05 06:57:53.000000 micomputing-1.1.34/micomputing/trans.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:57:53.355094 micomputing-1.1.34/micomputing.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-05 06:57:53.000000 micomputing-1.1.34/micomputing.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      385 2023-07-05 06:57:53.000000 micomputing-1.1.34/micomputing.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-05 06:57:53.000000 micomputing-1.1.34/micomputing.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       72 2023-07-05 06:57:53.000000 micomputing-1.1.34/micomputing.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       12 2023-07-05 06:57:53.000000 micomputing-1.1.34/micomputing.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-05 06:57:53.355591 micomputing-1.1.34/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1482 2023-07-05 06:57:53.000000 micomputing-1.1.34/setup.py
```

### Comparing `micomputing-1.1.33/PKG-INFO` & `micomputing-1.1.34/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micomputing
-Version: 1.1.33
+Version: 1.1.34
 Summary: 'micomputing' is a package for medical image computing. 
 Home-page: https://github.com/Bertie97/PyZMyc/micomputing
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # MIComputing
```

### Comparing `micomputing-1.1.33/README.md` & `micomputing-1.1.34/README.md`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.33/micomputing/__init__.py` & `micomputing-1.1.34/micomputing/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from pycamia import info_manager
 
 __info__ = info_manager(
     project = 'PyCAMIA',
     package = 'micomputing',
     author = 'Yuncheng Zhou',
     create = '2021-12',
-    version = '1.1.32',
+    version = '1.1.33',
     contact = 'bertiezhou@163.com',
     keywords = ['medical image', 'image registration', 'image similarities'],
     description = "'micomputing' is a package for medical image computing. ",
     requires = ['numpy', 'torch>=1.5.1', 'batorch', 'pycamia', 'pyoverload', 'nibabel', 'pydicom', 'SimpleITK'],
-    update = '2022-07-07 20:09:03'
+    update = '2023-07-05 14:46:31'
 ).check()
 
 from . import plot as plt
 from .stdio import IMG, dcm2nii, nii2dcm #*
 from .data import Info, Subject, ImageObject, Dataset, MedicalDataset #*
 from .network import U_Net, CNN, FCN
 from .funcs import reorient, rescale, reflect, dilate, blur, bending, distance_map, registration, local_prior, center_of_gravity #*
```

### Comparing `micomputing-1.1.33/micomputing/data.py` & `micomputing-1.1.34/micomputing/data.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.33/micomputing/funcs.py` & `micomputing-1.1.34/micomputing/funcs.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.33/micomputing/metrics.py` & `micomputing-1.1.34/micomputing/metrics.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.33/micomputing/network.py` & `micomputing-1.1.34/micomputing/network.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.33/micomputing/plot.py` & `micomputing-1.1.34/micomputing/plot.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.33/micomputing/stdio.py` & `micomputing-1.1.34/micomputing/stdio.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.33/micomputing/test.py` & `micomputing-1.1.34/micomputing/test.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.33/micomputing/trans.py` & `micomputing-1.1.34/micomputing/trans.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.33/micomputing.egg-info/PKG-INFO` & `micomputing-1.1.34/micomputing.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micomputing
-Version: 1.1.33
+Version: 1.1.34
 Summary: 'micomputing' is a package for medical image computing. 
 Home-page: https://github.com/Bertie97/PyZMyc/micomputing
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # MIComputing
```

### Comparing `micomputing-1.1.33/setup.py` & `micomputing-1.1.34/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name = 'micomputing',
-	version = '1.1.33',
+	version = '1.1.34',
 	keywords = ['pip', 'pymyc', 'micomputing', 'medical image', 'image registration', 'image similarities'],
 	description = "'micomputing' is a package for medical image computing. ",
 	long_description = '# MIComputing\n\n## Introduction\n\nPackage [`micomputing`](https://github.com/Bertie97/pycamia/tree/main/micomputing) is the medical image processing package under project [`PyCAMIA`](https://github.com/Bertie97/pycamia). It handles medical image read write, image interpolation, transformation, registration and so on. This package works under `PyCAMIA` and use `batorch.Tensor` as its basic data format. \n\n## Installation\n\nThis package can be installed by `pip install micomputing` or moving the source code to the directory of python libraries (the source code can be downloaded on [github](https://github.com/Bertie97/pycamia) or [PyPI](https://pypi.org/project/micomputing/)). \n\n```shell\npip install micomputing\n```\n\n\n\n## Acknowledgment\n\n@Yuncheng Zhou: Developer\n',
 	long_description_content_type = 'text/markdown',
 	license = 'MIT Licence',
 	url = 'https://github.com/Bertie97/PyZMyc/micomputing',
 	author = 'Yuncheng Zhou',
```

