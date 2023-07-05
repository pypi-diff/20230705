# Comparing `tmp/upyog-0.7.2.tar.gz` & `tmp/upyog-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upyog-0.7.2.tar", last modified: Thu May 25 07:50:05 2023, max compression
+gzip compressed data, was "upyog-0.7.3.tar", last modified: Wed Jul  5 17:45:31 2023, max compression
```

## Comparing `upyog-0.7.2.tar` & `upyog-0.7.3.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-25 07:50:05.060754 upyog-0.7.2/
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3488 2023-05-25 07:49:57.000000 upyog-0.7.2/CHANGELOG.md
--rw-r--r--   0 rahulsomani   (501) staff       (20)      133 2022-01-27 18:07:46.000000 upyog-0.7.2/MANIFEST.in
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-05-25 07:50:05.060864 upyog-0.7.2/PKG-INFO
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)      618 2022-01-15 04:03:41.000000 upyog-0.7.2/README.md
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-25 07:50:05.051037 upyog-0.7.2/assets/
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-25 07:50:05.052800 upyog-0.7.2/assets/fonts/
--rw-rwxrwx   0 rahulsomani   (501) staff       (20)    28432 2022-01-27 13:15:35.000000 upyog-0.7.2/assets/fonts/EuroStyleNormal.ttf
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)     1384 2023-05-25 07:50:05.061343 upyog-0.7.2/setup.cfg
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)      251 2022-01-17 09:53:10.000000 upyog-0.7.2/setup.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-25 07:50:05.053967 upyog-0.7.2/upyog/
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)       28 2022-10-28 02:44:32.000000 upyog-0.7.2/upyog/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      644 2023-01-24 04:50:27.000000 upyog-0.7.2/upyog/all.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-25 07:50:05.055839 upyog-0.7.2/upyog/ann/
--rw-r--r--   0 rahulsomani   (501) staff       (20)        0 2022-01-22 05:11:22.000000 upyog-0.7.2/upyog/ann/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     4426 2022-01-22 20:02:13.000000 upyog-0.7.2/upyog/ann/annoy.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3066 2023-04-16 03:50:08.000000 upyog-0.7.2/upyog/cli.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-25 07:50:05.057289 upyog-0.7.2/upyog/image/
--rw-r--r--   0 rahulsomani   (501) staff       (20)      141 2022-09-04 09:39:14.000000 upyog-0.7.2/upyog/image/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3340 2023-04-21 18:57:17.000000 upyog-0.7.2/upyog/image/cli.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     2286 2022-09-01 09:27:43.000000 upyog-0.7.2/upyog/image/composition.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)    17235 2023-05-23 10:33:14.000000 upyog-0.7.2/upyog/image/draw.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1526 2023-04-15 11:13:07.000000 upyog-0.7.2/upyog/image/io.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1442 2023-02-28 09:04:05.000000 upyog-0.7.2/upyog/image/pil_operators.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1518 2023-05-17 11:01:32.000000 upyog-0.7.2/upyog/image/utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     7939 2023-02-28 09:16:20.000000 upyog-0.7.2/upyog/image/visualiser.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1306 2023-05-17 15:42:19.000000 upyog-0.7.2/upyog/imports.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-25 07:50:05.058594 upyog-0.7.2/upyog/ml/
--rw-r--r--   0 rahulsomani   (501) staff       (20)      211 2023-05-17 15:36:44.000000 upyog-0.7.2/upyog/ml/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1419 2023-05-17 11:40:18.000000 upyog-0.7.2/upyog/ml/coreml_utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1803 2023-05-25 07:42:54.000000 upyog-0.7.2/upyog/ml/eval_dataset.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      523 2023-05-25 07:42:28.000000 upyog-0.7.2/upyog/ml/imports.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3662 2023-05-17 16:21:13.000000 upyog-0.7.2/upyog/ml/model_utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1707 2023-05-17 11:41:09.000000 upyog-0.7.2/upyog/ml/preprocessing.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     2066 2023-05-25 07:35:59.000000 upyog-0.7.2/upyog/ml/utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1138 2023-05-17 11:07:07.000000 upyog-0.7.2/upyog/ml/visualise.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1198 2022-06-01 05:03:09.000000 upyog-0.7.2/upyog/nb2script.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-25 07:50:05.059522 upyog-0.7.2/upyog/os/
--rw-r--r--   0 rahulsomani   (501) staff       (20)      137 2022-10-26 00:24:39.000000 upyog-0.7.2/upyog/os/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     6159 2023-04-16 07:09:32.000000 upyog-0.7.2/upyog/os/cli.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-08-03 15:10:12.000000 upyog-0.7.2/upyog/os/patch_pathlib.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     4424 2023-05-25 07:33:09.000000 upyog-0.7.2/upyog/os/read_files.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3459 2023-05-17 10:58:12.000000 upyog-0.7.2/upyog/os/utils.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-25 07:50:05.060570 upyog-0.7.2/upyog/utils/
--rw-r--r--   0 rahulsomani   (501) staff       (20)      118 2022-10-28 03:18:43.000000 upyog-0.7.2/upyog/utils/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-04-05 12:59:08.000000 upyog-0.7.2/upyog/utils/boxes.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)    14495 2023-01-11 07:05:00.000000 upyog-0.7.2/upyog/utils/download.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1324 2023-01-12 17:22:00.000000 upyog-0.7.2/upyog/utils/prettify_df.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     2992 2023-04-16 03:45:58.000000 upyog-0.7.2/upyog/utils/utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      556 2022-08-08 14:04:02.000000 upyog-0.7.2/upyog/utils/zip_utils.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-25 07:50:05.055267 upyog-0.7.2/upyog.egg-info/
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-05-25 07:50:04.000000 upyog-0.7.2/upyog.egg-info/PKG-INFO
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1022 2023-05-25 07:50:05.000000 upyog-0.7.2/upyog.egg-info/SOURCES.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2023-05-25 07:50:04.000000 upyog-0.7.2/upyog.egg-info/dependency_links.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)      454 2023-05-25 07:50:04.000000 upyog-0.7.2/upyog.egg-info/entry_points.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2022-01-17 09:58:14.000000 upyog-0.7.2/upyog.egg-info/not-zip-safe
--rw-r--r--   0 rahulsomani   (501) staff       (20)      179 2023-05-25 07:50:04.000000 upyog-0.7.2/upyog.egg-info/requires.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)       12 2023-05-25 07:50:04.000000 upyog-0.7.2/upyog.egg-info/top_level.txt
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-05 17:45:31.046680 upyog-0.7.3/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3549 2023-07-05 17:45:00.000000 upyog-0.7.3/CHANGELOG.md
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      133 2022-01-27 18:07:46.000000 upyog-0.7.3/MANIFEST.in
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-07-05 17:45:31.046813 upyog-0.7.3/PKG-INFO
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)      618 2022-01-15 04:03:41.000000 upyog-0.7.3/README.md
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-05 17:45:31.036974 upyog-0.7.3/assets/
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-05 17:45:31.038521 upyog-0.7.3/assets/fonts/
+-rw-rwxrwx   0 rahulsomani   (501) staff       (20)    28432 2022-01-27 13:15:35.000000 upyog-0.7.3/assets/fonts/EuroStyleNormal.ttf
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)     1399 2023-07-05 17:45:31.047271 upyog-0.7.3/setup.cfg
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)      251 2022-01-17 09:53:10.000000 upyog-0.7.3/setup.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-05 17:45:31.040025 upyog-0.7.3/upyog/
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)       28 2022-10-28 02:44:32.000000 upyog-0.7.3/upyog/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      644 2023-01-24 04:50:27.000000 upyog-0.7.3/upyog/all.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-05 17:45:31.041749 upyog-0.7.3/upyog/ann/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)        0 2022-01-22 05:11:22.000000 upyog-0.7.3/upyog/ann/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     4426 2022-01-22 20:02:13.000000 upyog-0.7.3/upyog/ann/annoy.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3066 2023-04-16 03:50:08.000000 upyog-0.7.3/upyog/cli.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-05 17:45:31.043133 upyog-0.7.3/upyog/image/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      141 2022-09-04 09:39:14.000000 upyog-0.7.3/upyog/image/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3340 2023-04-21 18:57:17.000000 upyog-0.7.3/upyog/image/cli.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     2286 2022-09-01 09:27:43.000000 upyog-0.7.3/upyog/image/composition.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)    17235 2023-05-23 10:33:14.000000 upyog-0.7.3/upyog/image/draw.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1526 2023-04-15 11:13:07.000000 upyog-0.7.3/upyog/image/io.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1442 2023-02-28 09:04:05.000000 upyog-0.7.3/upyog/image/pil_operators.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1518 2023-05-17 11:01:32.000000 upyog-0.7.3/upyog/image/utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     7939 2023-02-28 09:16:20.000000 upyog-0.7.3/upyog/image/visualiser.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1306 2023-05-17 15:42:19.000000 upyog-0.7.3/upyog/imports.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-05 17:45:31.044598 upyog-0.7.3/upyog/ml/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      211 2023-05-17 15:36:44.000000 upyog-0.7.3/upyog/ml/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     2799 2023-06-21 20:09:18.000000 upyog-0.7.3/upyog/ml/coreml_utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1803 2023-05-25 07:42:54.000000 upyog-0.7.3/upyog/ml/eval_dataset.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      523 2023-05-25 07:42:28.000000 upyog-0.7.3/upyog/ml/imports.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3662 2023-05-17 16:21:13.000000 upyog-0.7.3/upyog/ml/model_utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1707 2023-05-17 11:41:09.000000 upyog-0.7.3/upyog/ml/preprocessing.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     2373 2023-06-25 04:18:02.000000 upyog-0.7.3/upyog/ml/utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     2321 2023-06-25 04:00:34.000000 upyog-0.7.3/upyog/ml/visualise.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1198 2022-06-01 05:03:09.000000 upyog-0.7.3/upyog/nb2script.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-05 17:45:31.045358 upyog-0.7.3/upyog/os/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      137 2022-10-26 00:24:39.000000 upyog-0.7.3/upyog/os/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     6159 2023-04-16 07:09:32.000000 upyog-0.7.3/upyog/os/cli.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-08-03 15:10:12.000000 upyog-0.7.3/upyog/os/patch_pathlib.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     4424 2023-05-25 07:33:09.000000 upyog-0.7.3/upyog/os/read_files.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3459 2023-05-17 10:58:12.000000 upyog-0.7.3/upyog/os/utils.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-05 17:45:31.046498 upyog-0.7.3/upyog/utils/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      144 2023-06-21 15:08:49.000000 upyog-0.7.3/upyog/utils/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-04-05 12:59:08.000000 upyog-0.7.3/upyog/utils/boxes.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1483 2023-06-21 18:28:22.000000 upyog-0.7.3/upyog/utils/date_utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)    14495 2023-01-11 07:05:00.000000 upyog-0.7.3/upyog/utils/download.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1324 2023-01-12 17:22:00.000000 upyog-0.7.3/upyog/utils/prettify_df.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     2636 2023-06-21 15:10:08.000000 upyog-0.7.3/upyog/utils/utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      556 2022-08-08 14:04:02.000000 upyog-0.7.3/upyog/utils/zip_utils.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-05 17:45:31.041447 upyog-0.7.3/upyog.egg-info/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-07-05 17:45:30.000000 upyog-0.7.3/upyog.egg-info/PKG-INFO
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1048 2023-07-05 17:45:31.000000 upyog-0.7.3/upyog.egg-info/SOURCES.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2023-07-05 17:45:30.000000 upyog-0.7.3/upyog.egg-info/dependency_links.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      454 2023-07-05 17:45:30.000000 upyog-0.7.3/upyog.egg-info/entry_points.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2022-01-17 09:58:14.000000 upyog-0.7.3/upyog.egg-info/not-zip-safe
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      192 2023-07-05 17:45:30.000000 upyog-0.7.3/upyog.egg-info/requires.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)       12 2023-07-05 17:45:30.000000 upyog-0.7.3/upyog.egg-info/top_level.txt
```

### Comparing `upyog-0.7.2/CHANGELOG.md` & `upyog-0.7.3/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 0.7.3 -- 5 July 2023
+* Minor changes
+* Update dependency
+
 ## 0.7.2 -- 25 May 2023
 * Font path bugfix...
 * Port over more ML utilities to `upyog.ml`
 
 ## 0.7.1 -- 17 May 2023
 * Rename `InferenceDataset` to `ImageInferenceDataset`
 * Clean up imports
```

### Comparing `upyog-0.7.2/PKG-INFO` & `upyog-0.7.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upyog
-Version: 0.7.2
+Version: 0.7.3
 Summary: Myriad Utilities
 Author: Rahul Somani
 Author-email: rsomani95@gmail.com
 License: MIT
 Keywords: utilities
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
```

### Comparing `upyog-0.7.2/README.md` & `upyog-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/assets/fonts/EuroStyleNormal.ttf` & `upyog-0.7.3/assets/fonts/EuroStyleNormal.ttf`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/setup.cfg` & `upyog-0.7.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = upyog
-version = 0.7.2
+version = 0.7.3
 author = Rahul Somani
 author_email = rsomani95@gmail.com
 description = Myriad Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = utilities
 license = MIT
@@ -28,14 +28,16 @@
 	pyperclip
 	matplotlib
 	loguru
 	aggdraw
 	typing_extensions
 	exif
 	tabulate
+	pytz
+	seaborn
 
 [options.extras_require]
 all = 
 dev = 
 	black >=20.8b1,<21
 	pytest >=6,<7
 	jupyter >=1.0.0,<2
```

### Comparing `upyog-0.7.2/upyog/all.py` & `upyog-0.7.3/upyog/all.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog/ann/annoy.py` & `upyog-0.7.3/upyog/ann/annoy.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog/cli.py` & `upyog-0.7.3/upyog/cli.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog/image/cli.py` & `upyog-0.7.3/upyog/image/cli.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog/image/composition.py` & `upyog-0.7.3/upyog/image/composition.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog/image/draw.py` & `upyog-0.7.3/upyog/image/draw.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog/image/io.py` & `upyog-0.7.3/upyog/image/io.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog/image/pil_operators.py` & `upyog-0.7.3/upyog/image/pil_operators.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog/image/utils.py` & `upyog-0.7.3/upyog/image/utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog/image/visualiser.py` & `upyog-0.7.3/upyog/image/visualiser.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog/imports.py` & `upyog-0.7.3/upyog/imports.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog/ml/eval_dataset.py` & `upyog-0.7.3/upyog/ml/eval_dataset.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog/ml/imports.py` & `upyog-0.7.3/upyog/ml/imports.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog/ml/model_utils.py` & `upyog-0.7.3/upyog/ml/model_utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog/ml/preprocessing.py` & `upyog-0.7.3/upyog/ml/preprocessing.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog/ml/utils.py` & `upyog-0.7.3/upyog/ml/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,17 +13,25 @@
     if gpus == -1:
         return torch.cuda.device_count()
     else:
         assert isinstance(gpus, list)
         return len(gpus)
 
 
-def to_np(tensor: Tensor, dtype=np.float32):
-    if isinstance(tensor, np.ndarray): return tensor
-    return tensor.detach().cpu().numpy().astype(dtype)
+def to_np(
+    data: Union[Tensor, np.ndarray, Collection[Any]],
+    dtype=np.float32
+):
+    "Convert a Tensor / array / collection of numbers to a NP array and optionally change its dtype"
+    if   isinstance(data, np.ndarray): pass
+    elif isinstance(data, Tensor):     data = data.detach().cpu().numpy()
+    else:                              data = np.array(data)
+
+    if dtype is not None: return data.astype(dtype)
+    else:                 return data
 
 
 def to_torch(x) -> Tensor:
     assert isinstance(x, (np.ndarray, torch.Tensor))
     return x.detach() if isinstance(x, torch.Tensor) else torch.from_numpy(x)
```

### Comparing `upyog-0.7.2/upyog/nb2script.py` & `upyog-0.7.3/upyog/nb2script.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog/os/cli.py` & `upyog-0.7.3/upyog/os/cli.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog/os/read_files.py` & `upyog-0.7.3/upyog/os/read_files.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog/os/utils.py` & `upyog-0.7.3/upyog/os/utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog/utils/download.py` & `upyog-0.7.3/upyog/utils/download.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog/utils/prettify_df.py` & `upyog-0.7.3/upyog/utils/prettify_df.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog/utils/utils.py` & `upyog-0.7.3/upyog/utils/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from upyog.imports import *
 from itertools import islice
 
 __all__ = [
-    "flatten", "uniqueify", "get_YYYY_MM_DD", "get_date_YYYY_MM_DD", "get_date_DD_MM_YYYY",
+    "flatten", "uniqueify",
     "chunk", "notnone", "lmap", "allequal", "zipsafe", "convert_size", "convert_to_tuple",
     "convert_to_list",
 ]
 
 
 def flatten(x: Any) -> List[Any]:
     flattened_list = []
@@ -38,26 +38,14 @@
     # fmt: on
 
 
 def uniqueify(x: Collection) -> Collection:
     return sorted(list(set(x)))
 
 
-def get_YYYY_MM_DD(sep="_") -> str:
-    return datetime.now().strftime(f"%Y{sep}%m{sep}%d")
-
-
-def get_date_YYYY_MM_DD(sep="_") -> str:
-    return datetime.now().strftime(f"%Y{sep}%m{sep}%d")
-
-
-def get_date_DD_MM_YYYY(sep="_") -> str:
-    return datetime.now().strftime(f"%d{sep}%m{sep}%Y")
-
-
 def sort_dict_by_keys(x) -> dict:
     return dict(sorted(x.items()))
 
 
 def get_uuid(n=10) -> str:
     return uuid.uuid4().hex[:n].lower()
```

### Comparing `upyog-0.7.2/upyog/utils/zip_utils.py` & `upyog-0.7.3/upyog/utils/zip_utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.2/upyog.egg-info/PKG-INFO` & `upyog-0.7.3/upyog.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upyog
-Version: 0.7.2
+Version: 0.7.3
 Summary: Myriad Utilities
 Author: Rahul Somani
 Author-email: rsomani95@gmail.com
 License: MIT
 Keywords: utilities
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
```

### Comparing `upyog-0.7.2/upyog.egg-info/SOURCES.txt` & `upyog-0.7.3/upyog.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,11 +37,12 @@
 upyog/os/__init__.py
 upyog/os/cli.py
 upyog/os/patch_pathlib.py
 upyog/os/read_files.py
 upyog/os/utils.py
 upyog/utils/__init__.py
 upyog/utils/boxes.py
+upyog/utils/date_utils.py
 upyog/utils/download.py
 upyog/utils/prettify_df.py
 upyog/utils/utils.py
 upyog/utils/zip_utils.py
```

