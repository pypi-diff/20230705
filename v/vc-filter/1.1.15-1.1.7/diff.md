# Comparing `tmp/vc_filter-1.1.15.tar.gz` & `tmp/vc-filter-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vc_filter-1.1.15.tar", max compression
+gzip compressed data, was "vc-filter-1.1.7.tar", last modified: Sun Jun 25 07:57:13 2023, max compression
```

## Comparing `vc_filter-1.1.15.tar` & `vc-filter-1.1.7.tar`

### file list

```diff
@@ -1,6 +1,14 @@
--rw-r--r--   0        0        0     2762 2022-01-30 19:57:29.984822 vc_filter-1.1.15/README.md
--rw-r--r--   0        0        0      448 2023-07-05 11:12:23.294790 vc_filter-1.1.15/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-07-05 11:00:46.490166 vc_filter-1.1.15/vc_filter/.DS_Store
--rw-r--r--   0        0        0        1 2023-07-04 12:52:11.005321 vc_filter-1.1.15/vc_filter/__init__.py
--rw-r--r--   0        0        0     5128 2023-07-04 12:36:37.709170 vc_filter-1.1.15/vc_filter/code.py
--rw-r--r--   0        0        0     3364 1970-01-01 00:00:00.000000 vc_filter-1.1.15/PKG-INFO
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-25 07:57:13.960876 vc-filter-1.1.7/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     3347 2023-06-25 07:57:13.960573 vc-filter-1.1.7/PKG-INFO
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     2762 2022-01-30 19:57:29.000000 vc-filter-1.1.7/README.md
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       38 2023-06-25 07:57:13.960975 vc-filter-1.1.7/setup.cfg
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1120 2023-06-25 07:50:58.000000 vc-filter-1.1.7/setup.py
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-25 07:57:13.958372 vc-filter-1.1.7/vc_filter/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       37 2022-01-02 07:31:26.000000 vc-filter-1.1.7/vc_filter/__init__.py
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     5143 2023-06-25 07:51:49.000000 vc-filter-1.1.7/vc_filter/code.py
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-25 07:57:13.960106 vc-filter-1.1.7/vc_filter.egg-info/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     3347 2023-06-25 07:57:13.000000 vc-filter-1.1.7/vc_filter.egg-info/PKG-INFO
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)      222 2023-06-25 07:57:13.000000 vc-filter-1.1.7/vc_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)        1 2023-06-25 07:57:13.000000 vc-filter-1.1.7/vc_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       29 2023-06-25 07:57:13.000000 vc-filter-1.1.7/vc_filter.egg-info/requires.txt
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       10 2023-06-25 07:57:13.000000 vc-filter-1.1.7/vc_filter.egg-info/top_level.txt
```

### Comparing `vc_filter-1.1.15/README.md` & `vc-filter-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `vc_filter-1.1.15/vc_filter/code.py` & `vc-filter-1.1.7/vc_filter/code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Jul-03-2023
+# Jun-25-2023
 # code.py
 
 import cv2 as cv
 import numpy as np
 
 
 def vc_filter(image):
@@ -166,15 +166,15 @@
 
 
 def dft_rotate(dft, height_dft, width_dft, angle):
 
     re = dft[:, :, 0]
     im = dft[:, :, 1]
 
-    M = cv.getRotationMatrix2D((width_dft / 2, height_dft / 2), angle, 1)
+    matrix = cv.getRotationMatrix2D((width_dft / 2, height_dft / 2), angle, 1)
 
-    re_rot = cv.warpAffine(re, M, (width_dft, height_dft))
-    im_rot = cv.warpAffine(im, M, (width_dft, height_dft))
+    re_rot = cv.warpAffine(re, matrix, (width_dft, height_dft))
+    im_rot = cv.warpAffine(im, matrix, (width_dft, height_dft))
 
     dft_rot = cv.merge([re_rot, im_rot])
 
     return dft_rot
```

### Comparing `vc_filter-1.1.15/PKG-INFO` & `vc-filter-1.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: vc-filter
-Version: 1.1.15
-Summary: VC-filter is a new edge detection algorithm based on the Visual Cortex study
-License: MIT
+Version: 1.1.7
+Summary: VC Filter is a new edge detection algorithm based on the Visual Cortex study
+Home-page: https://boriskravtsov.com/
 Author: Boris Kravtsov
-Author-email: kravtsov.development@gmail.com
-Requires-Python: >=3.9,<4.0
+Author-email: boriskravtsov.contacts@gmail.com
+License: MIT
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: opencv-python-headless (>=4.8.0.74,<5.0.0.0)
+Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 ## VC FILTER
 VC filter is a new high-quality edge detector based on the Visual Cortex study
 
 ### Installation
 ```
@@ -85,8 +85,7 @@
 
 image_edges = vc_filter(image)
 
 image_edges_enh = contrast_enhancement(image_edges, 2.0)
 
 cv.imwrite(path_out, image_edges_enh)
 ```
-
```

