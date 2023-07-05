# Comparing `tmp/pitop.processing-0.31.0.post4.tar.gz` & `tmp/pitop.processing-0.32.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitop.processing-0.31.0.post4.tar", last modified: Tue Jun 13 18:30:08 2023, max compression
+gzip compressed data, was "dist/pitop.processing-0.32.0.post1.tar", last modified: Wed Jul  5 13:37:08 2023, max compression
```

## Comparing `pitop.processing-0.31.0.post4.tar` & `pitop.processing-0.32.0.post1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      991 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop/processing/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10933 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/ball_detect.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      737 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/core/emotion.py
--rw-r--r--   0 runner    (1001) docker     (122)     3361 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/core/face.py
--rw-r--r--   0 runner    (1001) docker     (122)     7135 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/core/face_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     8777 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/emotion_classifier.py
--rw-r--r--   0 runner    (1001) docker     (122)    10660 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/face_detector.py
--rw-r--r--   0 runner    (1001) docker     (122)     3250 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/line_detect.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop/processing/core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/core/load_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/core/math_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5439 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/core/vision_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop.processing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      991 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop.processing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop.processing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop.processing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      218 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop.processing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop.processing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:08.000000 pitop.processing-0.32.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-05 13:36:52.000000 pitop.processing-0.32.0.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      991 2023-07-05 13:37:08.000000 pitop.processing-0.32.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-07-05 13:36:52.000000 pitop.processing-0.32.0.post1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:08.000000 pitop.processing-0.32.0.post1/pitop/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:08.000000 pitop.processing-0.32.0.post1/pitop/processing/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 13:36:52.000000 pitop.processing-0.32.0.post1/pitop/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:08.000000 pitop.processing-0.32.0.post1/pitop/processing/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-07-05 13:36:52.000000 pitop.processing-0.32.0.post1/pitop/processing/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10933 2023-07-05 13:36:52.000000 pitop.processing-0.32.0.post1/pitop/processing/algorithms/ball_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:08.000000 pitop.processing-0.32.0.post1/pitop/processing/algorithms/faces/
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-07-05 13:36:52.000000 pitop.processing-0.32.0.post1/pitop/processing/algorithms/faces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:08.000000 pitop.processing-0.32.0.post1/pitop/processing/algorithms/faces/core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 13:36:52.000000 pitop.processing-0.32.0.post1/pitop/processing/algorithms/faces/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      737 2023-07-05 13:36:52.000000 pitop.processing-0.32.0.post1/pitop/processing/algorithms/faces/core/emotion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3361 2023-07-05 13:36:52.000000 pitop.processing-0.32.0.post1/pitop/processing/algorithms/faces/core/face.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7135 2023-07-05 13:36:52.000000 pitop.processing-0.32.0.post1/pitop/processing/algorithms/faces/core/face_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8777 2023-07-05 13:36:52.000000 pitop.processing-0.32.0.post1/pitop/processing/algorithms/faces/emotion_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10660 2023-07-05 13:36:52.000000 pitop.processing-0.32.0.post1/pitop/processing/algorithms/faces/face_detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3250 2023-07-05 13:36:52.000000 pitop.processing-0.32.0.post1/pitop/processing/algorithms/line_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:08.000000 pitop.processing-0.32.0.post1/pitop/processing/core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 13:36:52.000000 pitop.processing-0.32.0.post1/pitop/processing/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-07-05 13:36:52.000000 pitop.processing-0.32.0.post1/pitop/processing/core/load_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-07-05 13:36:52.000000 pitop.processing-0.32.0.post1/pitop/processing/core/math_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5439 2023-07-05 13:36:52.000000 pitop.processing-0.32.0.post1/pitop/processing/core/vision_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:37:08.000000 pitop.processing-0.32.0.post1/pitop.processing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      991 2023-07-05 13:37:08.000000 pitop.processing-0.32.0.post1/pitop.processing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-07-05 13:37:08.000000 pitop.processing-0.32.0.post1/pitop.processing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 13:37:08.000000 pitop.processing-0.32.0.post1/pitop.processing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      218 2023-07-05 13:37:08.000000 pitop.processing-0.32.0.post1/pitop.processing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-05 13:37:08.000000 pitop.processing-0.32.0.post1/pitop.processing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-05 13:37:08.000000 pitop.processing-0.32.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-07-05 13:36:52.000000 pitop.processing-0.32.0.post1/setup.py
```

### Comparing `pitop.processing-0.31.0.post4/PKG-INFO` & `pitop.processing-0.32.0.post1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.processing
-Version: 0.31.0.post4
+Version: 0.32.0.post1
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Processing
```

### Comparing `pitop.processing-0.31.0.post4/pitop/processing/algorithms/ball_detect.py` & `pitop.processing-0.32.0.post1/pitop/processing/algorithms/ball_detect.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/core/emotion.py` & `pitop.processing-0.32.0.post1/pitop/processing/algorithms/faces/core/emotion.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/core/face.py` & `pitop.processing-0.32.0.post1/pitop/processing/algorithms/faces/core/face.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/core/face_utils.py` & `pitop.processing-0.32.0.post1/pitop/processing/algorithms/faces/core/face_utils.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/emotion_classifier.py` & `pitop.processing-0.32.0.post1/pitop/processing/algorithms/faces/emotion_classifier.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/face_detector.py` & `pitop.processing-0.32.0.post1/pitop/processing/algorithms/faces/face_detector.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post4/pitop/processing/algorithms/line_detect.py` & `pitop.processing-0.32.0.post1/pitop/processing/algorithms/line_detect.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post4/pitop/processing/core/load_models.py` & `pitop.processing-0.32.0.post1/pitop/processing/core/load_models.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post4/pitop/processing/core/math_functions.py` & `pitop.processing-0.32.0.post1/pitop/processing/core/math_functions.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post4/pitop/processing/core/vision_functions.py` & `pitop.processing-0.32.0.post1/pitop/processing/core/vision_functions.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post4/pitop.processing.egg-info/PKG-INFO` & `pitop.processing-0.32.0.post1/pitop.processing.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.processing
-Version: 0.31.0.post4
+Version: 0.32.0.post1
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Processing
```

### Comparing `pitop.processing-0.31.0.post4/pitop.processing.egg-info/SOURCES.txt` & `pitop.processing-0.32.0.post1/pitop.processing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post4/setup.py` & `pitop.processing-0.32.0.post1/setup.py`

 * *Files identical despite different names*

