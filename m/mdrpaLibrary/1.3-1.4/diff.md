# Comparing `tmp/mdrpaLibrary-1.3.tar.gz` & `tmp/mdrpaLibrary-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdrpaLibrary-1.3.tar", last modified: Wed Jul  5 16:19:32 2023, max compression
+gzip compressed data, was "mdrpaLibrary-1.4.tar", last modified: Wed Jul  5 16:33:25 2023, max compression
```

## Comparing `mdrpaLibrary-1.3.tar` & `mdrpaLibrary-1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:19:32.349184 mdrpaLibrary-1.3/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-05 16:19:32.349060 mdrpaLibrary-1.3/PKG-INFO
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:19:32.347936 mdrpaLibrary-1.3/mdrpaLibrary/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:55:03.000000 mdrpaLibrary-1.3/mdrpaLibrary/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3353 2023-07-05 16:14:44.000000 mdrpaLibrary-1.3/mdrpaLibrary/clickButtonModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      516 2023-07-05 16:14:49.000000 mdrpaLibrary-1.3/mdrpaLibrary/customFunctions.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      524 2023-07-05 16:14:52.000000 mdrpaLibrary-1.3/mdrpaLibrary/getUiModels.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3379 2023-07-05 16:14:55.000000 mdrpaLibrary-1.3/mdrpaLibrary/inputFieldModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1669 2023-07-05 16:18:26.000000 mdrpaLibrary-1.3/mdrpaLibrary/modelDrivenRpa.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3393 2023-07-05 16:14:58.000000 mdrpaLibrary-1.3/mdrpaLibrary/selectCheckboxModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3449 2023-07-05 16:15:00.000000 mdrpaLibrary-1.3/mdrpaLibrary/selectFromDropdownModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      863 2023-07-05 16:13:32.000000 mdrpaLibrary-1.3/mdrpaLibrary/sendReportModel.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:19:32.348780 mdrpaLibrary-1.3/mdrpaLibrary/utils/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:00:07.000000 mdrpaLibrary-1.3/mdrpaLibrary/utils/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     2484 2023-07-05 16:13:57.000000 mdrpaLibrary-1.3/mdrpaLibrary/utils/utils.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:19:32.348555 mdrpaLibrary-1.3/mdrpaLibrary.egg-info/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-05 16:19:32.000000 mdrpaLibrary-1.3/mdrpaLibrary.egg-info/PKG-INFO
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      524 2023-07-05 16:19:32.000000 mdrpaLibrary-1.3/mdrpaLibrary.egg-info/SOURCES.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-05 16:19:32.000000 mdrpaLibrary-1.3/mdrpaLibrary.egg-info/dependency_links.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       13 2023-07-05 16:19:32.000000 mdrpaLibrary-1.3/mdrpaLibrary.egg-info/top_level.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-05 16:19:32.349224 mdrpaLibrary-1.3/setup.cfg
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      193 2023-07-05 16:19:03.000000 mdrpaLibrary-1.3/setup.py
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:33:25.717791 mdrpaLibrary-1.4/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-05 16:33:25.717663 mdrpaLibrary-1.4/PKG-INFO
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:33:25.716230 mdrpaLibrary-1.4/mdrpaLibrary/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:55:03.000000 mdrpaLibrary-1.4/mdrpaLibrary/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3353 2023-07-05 16:14:44.000000 mdrpaLibrary-1.4/mdrpaLibrary/clickButtonModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      516 2023-07-05 16:14:49.000000 mdrpaLibrary-1.4/mdrpaLibrary/customFunctions.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      524 2023-07-05 16:14:52.000000 mdrpaLibrary-1.4/mdrpaLibrary/getUiModels.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3379 2023-07-05 16:14:55.000000 mdrpaLibrary-1.4/mdrpaLibrary/inputFieldModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1670 2023-07-05 16:32:40.000000 mdrpaLibrary-1.4/mdrpaLibrary/modelDrivenRpa.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3393 2023-07-05 16:14:58.000000 mdrpaLibrary-1.4/mdrpaLibrary/selectCheckboxModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3449 2023-07-05 16:15:00.000000 mdrpaLibrary-1.4/mdrpaLibrary/selectFromDropdownModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      863 2023-07-05 16:13:32.000000 mdrpaLibrary-1.4/mdrpaLibrary/sendReportModel.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:33:25.717339 mdrpaLibrary-1.4/mdrpaLibrary/utils/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:00:07.000000 mdrpaLibrary-1.4/mdrpaLibrary/utils/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     2484 2023-07-05 16:13:57.000000 mdrpaLibrary-1.4/mdrpaLibrary/utils/utils.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:33:25.717072 mdrpaLibrary-1.4/mdrpaLibrary.egg-info/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-05 16:33:25.000000 mdrpaLibrary-1.4/mdrpaLibrary.egg-info/PKG-INFO
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      524 2023-07-05 16:33:25.000000 mdrpaLibrary-1.4/mdrpaLibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-05 16:33:25.000000 mdrpaLibrary-1.4/mdrpaLibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       13 2023-07-05 16:33:25.000000 mdrpaLibrary-1.4/mdrpaLibrary.egg-info/top_level.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-05 16:33:25.717839 mdrpaLibrary-1.4/setup.cfg
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      193 2023-07-05 16:32:58.000000 mdrpaLibrary-1.4/setup.py
```

### Comparing `mdrpaLibrary-1.3/mdrpaLibrary/clickButtonModel.robot` & `mdrpaLibrary-1.4/mdrpaLibrary/clickButtonModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-1.3/mdrpaLibrary/customFunctions.robot` & `mdrpaLibrary-1.4/mdrpaLibrary/customFunctions.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-1.3/mdrpaLibrary/getUiModels.robot` & `mdrpaLibrary-1.4/mdrpaLibrary/getUiModels.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-1.3/mdrpaLibrary/inputFieldModel.robot` & `mdrpaLibrary-1.4/mdrpaLibrary/inputFieldModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-1.3/mdrpaLibrary/modelDrivenRpa.py` & `mdrpaLibrary-1.4/mdrpaLibrary/modelDrivenRpa.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     def __init__(self):
         self.builtin = BuiltIn()
         self.resource_files = [
             'clickButtonModel.robot',
             'inputFieldModel.robot',
             'selectCheckboxModel.robot',
             'selectFromDropdownModel.robot',
-            'getUiModel.robot'
+            'getUiModels.robot'
             'sendReportModel.robot'
         ]  
 
     def import_resource_file(self, resource_file):
         self.builtin.import_resource(resource_file)
 
     @keyword
```

### Comparing `mdrpaLibrary-1.3/mdrpaLibrary/selectCheckboxModel.robot` & `mdrpaLibrary-1.4/mdrpaLibrary/selectCheckboxModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-1.3/mdrpaLibrary/selectFromDropdownModel.robot` & `mdrpaLibrary-1.4/mdrpaLibrary/selectFromDropdownModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-1.3/mdrpaLibrary/sendReportModel.robot` & `mdrpaLibrary-1.4/mdrpaLibrary/sendReportModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-1.3/mdrpaLibrary/utils/utils.robot` & `mdrpaLibrary-1.4/mdrpaLibrary/utils/utils.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-1.3/mdrpaLibrary.egg-info/SOURCES.txt` & `mdrpaLibrary-1.4/mdrpaLibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

