# Comparing `tmp/mdrpaLibrary-1.6.tar.gz` & `tmp/mdrpaLibrary-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdrpaLibrary-1.6.tar", last modified: Wed Jul  5 16:47:28 2023, max compression
+gzip compressed data, was "mdrpaLibrary-1.7.tar", last modified: Wed Jul  5 17:08:02 2023, max compression
```

## Comparing `mdrpaLibrary-1.6.tar` & `mdrpaLibrary-1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:47:28.195522 mdrpaLibrary-1.6/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-05 16:47:28.195165 mdrpaLibrary-1.6/PKG-INFO
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:47:28.192544 mdrpaLibrary-1.6/mdrpaLibrary/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:55:03.000000 mdrpaLibrary-1.6/mdrpaLibrary/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3353 2023-07-05 16:14:44.000000 mdrpaLibrary-1.6/mdrpaLibrary/clickButtonModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      491 2023-07-05 16:40:30.000000 mdrpaLibrary-1.6/mdrpaLibrary/getUiModels.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3379 2023-07-05 16:14:55.000000 mdrpaLibrary-1.6/mdrpaLibrary/inputFieldModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1671 2023-07-05 16:46:58.000000 mdrpaLibrary-1.6/mdrpaLibrary/modelDrivenRpa.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3393 2023-07-05 16:14:58.000000 mdrpaLibrary-1.6/mdrpaLibrary/selectCheckboxModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3449 2023-07-05 16:15:00.000000 mdrpaLibrary-1.6/mdrpaLibrary/selectFromDropdownModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      863 2023-07-05 16:13:32.000000 mdrpaLibrary-1.6/mdrpaLibrary/sendReportModel.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:47:28.194632 mdrpaLibrary-1.6/mdrpaLibrary/utils/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:00:07.000000 mdrpaLibrary-1.6/mdrpaLibrary/utils/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     2484 2023-07-05 16:13:57.000000 mdrpaLibrary-1.6/mdrpaLibrary/utils/utils.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:47:28.193908 mdrpaLibrary-1.6/mdrpaLibrary.egg-info/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-05 16:47:28.000000 mdrpaLibrary-1.6/mdrpaLibrary.egg-info/PKG-INFO
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      489 2023-07-05 16:47:28.000000 mdrpaLibrary-1.6/mdrpaLibrary.egg-info/SOURCES.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-05 16:47:28.000000 mdrpaLibrary-1.6/mdrpaLibrary.egg-info/dependency_links.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       13 2023-07-05 16:47:28.000000 mdrpaLibrary-1.6/mdrpaLibrary.egg-info/top_level.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-05 16:47:28.195613 mdrpaLibrary-1.6/setup.cfg
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      193 2023-07-05 16:47:03.000000 mdrpaLibrary-1.6/setup.py
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 17:08:02.348634 mdrpaLibrary-1.7/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-05 17:08:02.348499 mdrpaLibrary-1.7/PKG-INFO
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 17:08:02.347000 mdrpaLibrary-1.7/mdrpaLibrary/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:55:03.000000 mdrpaLibrary-1.7/mdrpaLibrary/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3353 2023-07-05 16:14:44.000000 mdrpaLibrary-1.7/mdrpaLibrary/clickButtonModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      491 2023-07-05 16:40:30.000000 mdrpaLibrary-1.7/mdrpaLibrary/getUiModels.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3379 2023-07-05 16:14:55.000000 mdrpaLibrary-1.7/mdrpaLibrary/inputFieldModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1817 2023-07-05 17:07:20.000000 mdrpaLibrary-1.7/mdrpaLibrary/modelDrivenRpa.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3393 2023-07-05 16:14:58.000000 mdrpaLibrary-1.7/mdrpaLibrary/selectCheckboxModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3449 2023-07-05 16:15:00.000000 mdrpaLibrary-1.7/mdrpaLibrary/selectFromDropdownModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      863 2023-07-05 16:13:32.000000 mdrpaLibrary-1.7/mdrpaLibrary/sendReportModel.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 17:08:02.348043 mdrpaLibrary-1.7/mdrpaLibrary/utils/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:00:07.000000 mdrpaLibrary-1.7/mdrpaLibrary/utils/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     2484 2023-07-05 16:13:57.000000 mdrpaLibrary-1.7/mdrpaLibrary/utils/utils.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 17:08:02.347802 mdrpaLibrary-1.7/mdrpaLibrary.egg-info/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-05 17:08:02.000000 mdrpaLibrary-1.7/mdrpaLibrary.egg-info/PKG-INFO
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      489 2023-07-05 17:08:02.000000 mdrpaLibrary-1.7/mdrpaLibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-05 17:08:02.000000 mdrpaLibrary-1.7/mdrpaLibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       13 2023-07-05 17:08:02.000000 mdrpaLibrary-1.7/mdrpaLibrary.egg-info/top_level.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-05 17:08:02.348681 mdrpaLibrary-1.7/setup.cfg
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      193 2023-07-05 17:07:51.000000 mdrpaLibrary-1.7/setup.py
```

### Comparing `mdrpaLibrary-1.6/mdrpaLibrary/clickButtonModel.robot` & `mdrpaLibrary-1.7/mdrpaLibrary/clickButtonModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-1.6/mdrpaLibrary/inputFieldModel.robot` & `mdrpaLibrary-1.7/mdrpaLibrary/inputFieldModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-1.6/mdrpaLibrary/modelDrivenRpa.py` & `mdrpaLibrary-1.7/mdrpaLibrary/modelDrivenRpa.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,31 @@
+import os
 from robot.api.deco import keyword
 from robot.libraries.BuiltIn import BuiltIn
 
 class ModelDrivenRpa:
     ROBOT_LIBRARY_SCOPE = 'GLOBAL'
 
     def __init__(self):
         self.builtin = BuiltIn()
+        self.resource_dir = os.path.dirname(os.path.abspath(__file__))
         self.resource_files = [
             'clickButtonModel.robot',
             'inputFieldModel.robot',
             'selectCheckboxModel.robot',
             'selectFromDropdownModel.robot',
             'getUiModels.robot',
             'sendReportModel.robot'
         ]  
 
     def import_resource_file(self, resource_file):
-        self.builtin.import_resource(resource_file)
+        file_path = os.path.join(self.resource_dir, resource_file)
+        self.builtin.import_resource(file_path)
+
+
 
     @keyword
     def click_button_model(self, *args):
         self.import_resource_file(self.resource_files[0])  
         self.builtin.run_keyword('Click Button Model', *args)
 
     @keyword
```

### Comparing `mdrpaLibrary-1.6/mdrpaLibrary/selectCheckboxModel.robot` & `mdrpaLibrary-1.7/mdrpaLibrary/selectCheckboxModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-1.6/mdrpaLibrary/selectFromDropdownModel.robot` & `mdrpaLibrary-1.7/mdrpaLibrary/selectFromDropdownModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-1.6/mdrpaLibrary/sendReportModel.robot` & `mdrpaLibrary-1.7/mdrpaLibrary/sendReportModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-1.6/mdrpaLibrary/utils/utils.robot` & `mdrpaLibrary-1.7/mdrpaLibrary/utils/utils.robot`

 * *Files identical despite different names*

