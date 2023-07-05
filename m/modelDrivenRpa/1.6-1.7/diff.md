# Comparing `tmp/modelDrivenRpa-1.6.tar.gz` & `tmp/modelDrivenRpa-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelDrivenRpa-1.6.tar", last modified: Wed Jul  5 13:11:23 2023, max compression
+gzip compressed data, was "modelDrivenRpa-1.7.tar", last modified: Wed Jul  5 13:25:01 2023, max compression
```

## Comparing `modelDrivenRpa-1.6.tar` & `modelDrivenRpa-1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:11:23.324209 modelDrivenRpa-1.6/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       56 2023-07-05 13:11:23.324010 modelDrivenRpa-1.6/PKG-INFO
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:11:23.322409 modelDrivenRpa-1.6/modelDrivenRpa/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1006 2023-07-05 13:10:37.000000 modelDrivenRpa-1.6/modelDrivenRpa/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3077 2023-07-03 21:43:37.000000 modelDrivenRpa-1.6/modelDrivenRpa/clickButtonModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      451 2023-07-03 21:43:44.000000 modelDrivenRpa-1.6/modelDrivenRpa/customFunctions.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3121 2023-07-03 21:43:47.000000 modelDrivenRpa-1.6/modelDrivenRpa/inputFieldModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3133 2023-07-03 21:44:12.000000 modelDrivenRpa-1.6/modelDrivenRpa/selectCheckboxModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3194 2023-07-03 21:43:55.000000 modelDrivenRpa-1.6/modelDrivenRpa/selectFromDropdownModel.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:11:23.323600 modelDrivenRpa-1.6/modelDrivenRpa/utils/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:00:07.000000 modelDrivenRpa-1.6/modelDrivenRpa/utils/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1248 2023-06-27 14:36:11.000000 modelDrivenRpa-1.6/modelDrivenRpa/utils/utils.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:11:23.323245 modelDrivenRpa-1.6/modelDrivenRpa.egg-info/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       56 2023-07-05 13:11:23.000000 modelDrivenRpa-1.6/modelDrivenRpa.egg-info/PKG-INFO
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      451 2023-07-05 13:11:23.000000 modelDrivenRpa-1.6/modelDrivenRpa.egg-info/SOURCES.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-05 13:11:23.000000 modelDrivenRpa-1.6/modelDrivenRpa.egg-info/dependency_links.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       15 2023-07-05 13:11:23.000000 modelDrivenRpa-1.6/modelDrivenRpa.egg-info/top_level.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-05 13:11:23.324285 modelDrivenRpa-1.6/setup.cfg
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      197 2023-07-05 13:11:13.000000 modelDrivenRpa-1.6/setup.py
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:25:01.454352 modelDrivenRpa-1.7/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       56 2023-07-05 13:25:01.454209 modelDrivenRpa-1.7/PKG-INFO
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:25:01.452411 modelDrivenRpa-1.7/modelDrivenRpa/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1031 2023-07-05 13:24:07.000000 modelDrivenRpa-1.7/modelDrivenRpa/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3077 2023-07-03 21:43:37.000000 modelDrivenRpa-1.7/modelDrivenRpa/clickButtonModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      451 2023-07-03 21:43:44.000000 modelDrivenRpa-1.7/modelDrivenRpa/customFunctions.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3121 2023-07-03 21:43:47.000000 modelDrivenRpa-1.7/modelDrivenRpa/inputFieldModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3133 2023-07-03 21:44:12.000000 modelDrivenRpa-1.7/modelDrivenRpa/selectCheckboxModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3194 2023-07-03 21:43:55.000000 modelDrivenRpa-1.7/modelDrivenRpa/selectFromDropdownModel.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:25:01.453783 modelDrivenRpa-1.7/modelDrivenRpa/utils/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:00:07.000000 modelDrivenRpa-1.7/modelDrivenRpa/utils/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1248 2023-06-27 14:36:11.000000 modelDrivenRpa-1.7/modelDrivenRpa/utils/utils.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:25:01.453359 modelDrivenRpa-1.7/modelDrivenRpa.egg-info/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       56 2023-07-05 13:25:01.000000 modelDrivenRpa-1.7/modelDrivenRpa.egg-info/PKG-INFO
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      451 2023-07-05 13:25:01.000000 modelDrivenRpa-1.7/modelDrivenRpa.egg-info/SOURCES.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-05 13:25:01.000000 modelDrivenRpa-1.7/modelDrivenRpa.egg-info/dependency_links.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       15 2023-07-05 13:25:01.000000 modelDrivenRpa-1.7/modelDrivenRpa.egg-info/top_level.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-05 13:25:01.454398 modelDrivenRpa-1.7/setup.cfg
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      197 2023-07-05 13:24:52.000000 modelDrivenRpa-1.7/setup.py
```

### Comparing `modelDrivenRpa-1.6/modelDrivenRpa/clickButtonModel.robot` & `modelDrivenRpa-1.7/modelDrivenRpa/clickButtonModel.robot`

 * *Files identical despite different names*

### Comparing `modelDrivenRpa-1.6/modelDrivenRpa/inputFieldModel.robot` & `modelDrivenRpa-1.7/modelDrivenRpa/inputFieldModel.robot`

 * *Files identical despite different names*

### Comparing `modelDrivenRpa-1.6/modelDrivenRpa/selectCheckboxModel.robot` & `modelDrivenRpa-1.7/modelDrivenRpa/selectCheckboxModel.robot`

 * *Files identical despite different names*

### Comparing `modelDrivenRpa-1.6/modelDrivenRpa/selectFromDropdownModel.robot` & `modelDrivenRpa-1.7/modelDrivenRpa/selectFromDropdownModel.robot`

 * *Files identical despite different names*

### Comparing `modelDrivenRpa-1.6/modelDrivenRpa/utils/utils.robot` & `modelDrivenRpa-1.7/modelDrivenRpa/utils/utils.robot`

 * *Files identical despite different names*

