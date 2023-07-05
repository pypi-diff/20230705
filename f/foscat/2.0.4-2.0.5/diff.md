# Comparing `tmp/foscat-2.0.4.tar.gz` & `tmp/foscat-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/export/home/jmdeloui/FOSCAT/dist/.tmp-32znl1a1/foscat-2.0.4.tar", last modified: Wed Jul  5 08:43:24 2023, max compression
+gzip compressed data, was "/export/home/jmdeloui/FOSCAT/dist/.tmp-js6yoa5p/foscat-2.0.5.tar", last modified: Wed Jul  5 10:04:06 2023, max compression
```

## Comparing `foscat-2.0.4.tar` & `foscat-2.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-05 08:43:24.000000 foscat-2.0.4/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-05 08:43:24.000000 foscat-2.0.4/PKG-INFO
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     2160 2022-12-13 16:07:53.000000 foscat-2.0.4/README.md
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      107 2023-07-05 08:43:24.000000 foscat-2.0.4/setup.cfg
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1097 2023-07-05 08:42:27.000000 foscat-2.0.4/setup.py
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-05 08:43:24.000000 foscat-2.0.4/src/
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-05 08:43:24.000000 foscat-2.0.4/src/foscat/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    57132 2023-06-10 06:53:35.000000 foscat-2.0.4/src/foscat/FoCUS.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      731 2023-01-27 14:00:55.000000 foscat-2.0.4/src/foscat/GetGPUinfo.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     3594 2023-06-23 10:27:41.000000 foscat-2.0.4/src/foscat/Rformat.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    16208 2023-06-10 06:53:35.000000 foscat-2.0.4/src/foscat/Synthesis.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2022-12-13 16:07:53.000000 foscat-2.0.4/src/foscat/__init__.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    13733 2023-06-10 06:53:35.000000 foscat-2.0.4/src/foscat/backend.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    53863 2023-03-28 12:51:05.000000 foscat-2.0.4/src/foscat/build_demo.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2023-03-04 09:58:28.000000 foscat-2.0.4/src/foscat/demo2d.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    29024 2023-07-05 08:23:52.000000 foscat-2.0.4/src/foscat/scat.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    41808 2023-03-24 11:01:28.000000 foscat-2.0.4/src/foscat/scat_cov.old.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    48336 2023-07-05 08:21:43.000000 foscat-2.0.4/src/foscat/scat_cov.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    27568 2023-02-08 17:11:11.000000 foscat-2.0.4/src/foscat/scat_cov_new.py
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-05 08:43:24.000000 foscat-2.0.4/src/foscat.egg-info/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-05 08:43:24.000000 foscat-2.0.4/src/foscat.egg-info/PKG-INFO
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      475 2023-07-05 08:43:24.000000 foscat-2.0.4/src/foscat.egg-info/SOURCES.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        1 2023-07-05 08:43:24.000000 foscat-2.0.4/src/foscat.egg-info/dependency_links.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)       55 2023-07-05 08:43:24.000000 foscat-2.0.4/src/foscat.egg-info/requires.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        7 2023-07-05 08:43:24.000000 foscat-2.0.4/src/foscat.egg-info/top_level.txt
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-05 10:04:06.000000 foscat-2.0.5/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-05 10:04:06.000000 foscat-2.0.5/PKG-INFO
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     2160 2022-12-13 16:07:53.000000 foscat-2.0.5/README.md
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      107 2023-07-05 10:04:06.000000 foscat-2.0.5/setup.cfg
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1097 2023-07-05 10:02:36.000000 foscat-2.0.5/setup.py
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-05 10:04:06.000000 foscat-2.0.5/src/
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-05 10:04:06.000000 foscat-2.0.5/src/foscat/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    57132 2023-06-10 06:53:35.000000 foscat-2.0.5/src/foscat/FoCUS.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      731 2023-01-27 14:00:55.000000 foscat-2.0.5/src/foscat/GetGPUinfo.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     3594 2023-06-23 10:27:41.000000 foscat-2.0.5/src/foscat/Rformat.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    16207 2023-07-05 10:03:34.000000 foscat-2.0.5/src/foscat/Synthesis.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2022-12-13 16:07:53.000000 foscat-2.0.5/src/foscat/__init__.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    13733 2023-06-10 06:53:35.000000 foscat-2.0.5/src/foscat/backend.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    53863 2023-03-28 12:51:05.000000 foscat-2.0.5/src/foscat/build_demo.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2023-03-04 09:58:28.000000 foscat-2.0.5/src/foscat/demo2d.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    29024 2023-07-05 08:23:52.000000 foscat-2.0.5/src/foscat/scat.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    41808 2023-03-24 11:01:28.000000 foscat-2.0.5/src/foscat/scat_cov.old.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    48336 2023-07-05 08:21:43.000000 foscat-2.0.5/src/foscat/scat_cov.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    27568 2023-02-08 17:11:11.000000 foscat-2.0.5/src/foscat/scat_cov_new.py
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-05 10:04:06.000000 foscat-2.0.5/src/foscat.egg-info/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-05 10:04:06.000000 foscat-2.0.5/src/foscat.egg-info/PKG-INFO
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      475 2023-07-05 10:04:06.000000 foscat-2.0.5/src/foscat.egg-info/SOURCES.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        1 2023-07-05 10:04:06.000000 foscat-2.0.5/src/foscat.egg-info/dependency_links.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)       55 2023-07-05 10:04:06.000000 foscat-2.0.5/src/foscat.egg-info/requires.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        7 2023-07-05 10:04:06.000000 foscat-2.0.5/src/foscat.egg-info/top_level.txt
```

### Comparing `foscat-2.0.4/PKG-INFO` & `foscat-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foscat
-Version: 2.0.4
+Version: 2.0.5
 Summary: Generate synthetic Healpix or 2D data using Cross Scattering Transform
 Home-page: https://github.com/jmdelouis/FOSCAT
 Author: Jean-Marc DELOUIS
 Author-email: jean.marc.delouis@ifremer.fr
 Maintainer: Theo Foulquier
 Maintainer-email: theo.foulquier@ifremer.fr
 License: MIT
```

### Comparing `foscat-2.0.4/README.md` & `foscat-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `foscat-2.0.4/setup.py` & `foscat-2.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='foscat',
-    version='2.0.4',
+    version='2.0.5',
     description='Generate synthetic Healpix or 2D data using Cross Scattering Transform' ,
     long_description='Utilize the Cross Scattering Transform (described in https://arxiv.org/abs/2207.12527) to synthesize Healpix or 2D data that is suitable for component separation purposes, such as denoising. \n A demo package for this process can be found at https://github.com/jmdelouis/FOSCAT_DEMO. \n\n List of developers : J.-M. Delouis, T. Foulquier, L. Mousset, E. Allys ' ,
     license='MIT',
     author='Jean-Marc DELOUIS',
     author_email='jean.marc.delouis@ifremer.fr',
     maintainer='Theo Foulquier',
     maintainer_email='theo.foulquier@ifremer.fr',
```

### Comparing `foscat-2.0.4/src/foscat/FoCUS.py` & `foscat-2.0.5/src/foscat/FoCUS.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.4/src/foscat/GetGPUinfo.py` & `foscat-2.0.5/src/foscat/GetGPUinfo.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.4/src/foscat/Rformat.py` & `foscat-2.0.5/src/foscat/Rformat.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.4/src/foscat/Synthesis.py` & `foscat-2.0.5/src/foscat/Synthesis.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,15 @@
             LEARNING_RATE = 0.03,
             EPSILON = 1E-7,
             grd_mask=None,
             SHOWGPU=False,
             MESSAGE='',
             batchsz=1,
             totalsz=1,
-            do_lbfgs=False,
+            do_lbfgs=True,
             axis=0):
         
         self.eta=LEARNING_RATE
         self.epsilon=EPSILON
         self.decay_rate = DECAY_RATE
         self.nlog=0
         self.itt2=0
```

### Comparing `foscat-2.0.4/src/foscat/backend.py` & `foscat-2.0.5/src/foscat/backend.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.4/src/foscat/build_demo.py` & `foscat-2.0.5/src/foscat/build_demo.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.4/src/foscat/scat.py` & `foscat-2.0.5/src/foscat/scat.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.4/src/foscat/scat_cov.old.py` & `foscat-2.0.5/src/foscat/scat_cov.old.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.4/src/foscat/scat_cov.py` & `foscat-2.0.5/src/foscat/scat_cov.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.4/src/foscat/scat_cov_new.py` & `foscat-2.0.5/src/foscat/scat_cov_new.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.4/src/foscat.egg-info/PKG-INFO` & `foscat-2.0.5/src/foscat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foscat
-Version: 2.0.4
+Version: 2.0.5
 Summary: Generate synthetic Healpix or 2D data using Cross Scattering Transform
 Home-page: https://github.com/jmdelouis/FOSCAT
 Author: Jean-Marc DELOUIS
 Author-email: jean.marc.delouis@ifremer.fr
 Maintainer: Theo Foulquier
 Maintainer-email: theo.foulquier@ifremer.fr
 License: MIT
```

