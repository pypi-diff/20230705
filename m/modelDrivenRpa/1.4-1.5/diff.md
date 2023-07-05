# Comparing `tmp/modelDrivenRpa-1.4.tar.gz` & `tmp/modelDrivenRpa-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelDrivenRpa-1.4.tar", last modified: Wed Jul  5 12:51:47 2023, max compression
+gzip compressed data, was "modelDrivenRpa-1.5.tar", last modified: Wed Jul  5 13:01:45 2023, max compression
```

## Comparing `modelDrivenRpa-1.4.tar` & `modelDrivenRpa-1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 12:51:47.400838 modelDrivenRpa-1.4/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       56 2023-07-05 12:51:47.400715 modelDrivenRpa-1.4/PKG-INFO
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 12:51:47.399582 modelDrivenRpa-1.4/modelDrivenRpa/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1106 2023-07-05 12:49:32.000000 modelDrivenRpa-1.4/modelDrivenRpa/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3077 2023-07-03 21:43:37.000000 modelDrivenRpa-1.4/modelDrivenRpa/clickButtonModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      451 2023-07-03 21:43:44.000000 modelDrivenRpa-1.4/modelDrivenRpa/customFunctions.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3121 2023-07-03 21:43:47.000000 modelDrivenRpa-1.4/modelDrivenRpa/inputFieldModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3133 2023-07-03 21:44:12.000000 modelDrivenRpa-1.4/modelDrivenRpa/selectCheckboxModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3194 2023-07-03 21:43:55.000000 modelDrivenRpa-1.4/modelDrivenRpa/selectFromDropdownModel.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 12:51:47.400532 modelDrivenRpa-1.4/modelDrivenRpa/utils/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      288 2023-07-05 12:50:43.000000 modelDrivenRpa-1.4/modelDrivenRpa/utils/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1248 2023-06-27 14:36:11.000000 modelDrivenRpa-1.4/modelDrivenRpa/utils/utils.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 12:51:47.400215 modelDrivenRpa-1.4/modelDrivenRpa.egg-info/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       56 2023-07-05 12:51:47.000000 modelDrivenRpa-1.4/modelDrivenRpa.egg-info/PKG-INFO
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      451 2023-07-05 12:51:47.000000 modelDrivenRpa-1.4/modelDrivenRpa.egg-info/SOURCES.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-05 12:51:47.000000 modelDrivenRpa-1.4/modelDrivenRpa.egg-info/dependency_links.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       15 2023-07-05 12:51:47.000000 modelDrivenRpa-1.4/modelDrivenRpa.egg-info/top_level.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-05 12:51:47.400879 modelDrivenRpa-1.4/setup.cfg
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      197 2023-07-05 12:50:49.000000 modelDrivenRpa-1.4/setup.py
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:01:45.153981 modelDrivenRpa-1.5/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       56 2023-07-05 13:01:45.153761 modelDrivenRpa-1.5/PKG-INFO
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:01:45.151828 modelDrivenRpa-1.5/modelDrivenRpa/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1093 2023-07-05 13:00:20.000000 modelDrivenRpa-1.5/modelDrivenRpa/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3077 2023-07-03 21:43:37.000000 modelDrivenRpa-1.5/modelDrivenRpa/clickButtonModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      451 2023-07-03 21:43:44.000000 modelDrivenRpa-1.5/modelDrivenRpa/customFunctions.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3121 2023-07-03 21:43:47.000000 modelDrivenRpa-1.5/modelDrivenRpa/inputFieldModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3133 2023-07-03 21:44:12.000000 modelDrivenRpa-1.5/modelDrivenRpa/selectCheckboxModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3194 2023-07-03 21:43:55.000000 modelDrivenRpa-1.5/modelDrivenRpa/selectFromDropdownModel.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:01:45.153184 modelDrivenRpa-1.5/modelDrivenRpa/utils/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:00:07.000000 modelDrivenRpa-1.5/modelDrivenRpa/utils/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1248 2023-06-27 14:36:11.000000 modelDrivenRpa-1.5/modelDrivenRpa/utils/utils.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:01:45.152800 modelDrivenRpa-1.5/modelDrivenRpa.egg-info/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       56 2023-07-05 13:01:45.000000 modelDrivenRpa-1.5/modelDrivenRpa.egg-info/PKG-INFO
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      451 2023-07-05 13:01:45.000000 modelDrivenRpa-1.5/modelDrivenRpa.egg-info/SOURCES.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-05 13:01:45.000000 modelDrivenRpa-1.5/modelDrivenRpa.egg-info/dependency_links.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       15 2023-07-05 13:01:45.000000 modelDrivenRpa-1.5/modelDrivenRpa.egg-info/top_level.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-05 13:01:45.154036 modelDrivenRpa-1.5/setup.cfg
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      197 2023-07-05 13:00:48.000000 modelDrivenRpa-1.5/setup.py
```

### Comparing `modelDrivenRpa-1.4/modelDrivenRpa/__init__.py` & `modelDrivenRpa-1.5/modelDrivenRpa/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-from robot.api import get_keyword_names
+from robot.parsing.model import TestData
 from robot.libraries import LibraryComponent
-from robot.parsing.model import TestDataDirectory
-import os
 
-class modelDrivenRpa(LibraryComponent):
+class ModelDrivenRpa(LibraryComponent):
     ROBOT_LIBRARY_SCOPE = 'GLOBAL'
 
     def __init__(self):
         self.keywords = []
+        self.import_keywords_from_files()
 
-        # Get the current directory
-        current_directory = os.path.dirname(os.path.abspath(__file__))
-
-        # Import all .robot files in the modelDrivenRpa package
-        for filename in os.listdir(current_directory):
-            if filename.endswith('.robot'):
-                path = os.path.join(current_directory, filename)
-                self.import_keywords_from_file(path)
+    def import_keywords_from_files(self):
+        # Get the directory path of the modelDrivenRpa package
+        package_dir = __file__.rsplit("/", 1)[0]
+
+        # Import keywords from .robot files
+        for filename in ["clickButtonModel.robot", "inputFieldModel.robot", "selectCheckboxModel.robot", "selectFromDropdownModel.robot"]:
+            file_path = f"{package_dir}/{filename}"
+            self.import_keywords_from_file(file_path)
 
     def import_keywords_from_file(self, file_path):
-        # Create a TestDataDirectory instance for the .robot file
-        test_data = TestDataDirectory(source=file_path)
+        test_data = TestData(parent=None, source=file_path)
 
         # Get the keywords from the .robot file
-        for keyword_table in test_data.keyword_table:
+        for keyword_table in test_data.keyword_table_set.tables:
             for keyword in keyword_table.keywords:
                 self.keywords.append(keyword.name)
 
     def get_keyword_names(self):
         return self.keywords
```

### Comparing `modelDrivenRpa-1.4/modelDrivenRpa/clickButtonModel.robot` & `modelDrivenRpa-1.5/modelDrivenRpa/clickButtonModel.robot`

 * *Files identical despite different names*

### Comparing `modelDrivenRpa-1.4/modelDrivenRpa/inputFieldModel.robot` & `modelDrivenRpa-1.5/modelDrivenRpa/inputFieldModel.robot`

 * *Files identical despite different names*

### Comparing `modelDrivenRpa-1.4/modelDrivenRpa/selectCheckboxModel.robot` & `modelDrivenRpa-1.5/modelDrivenRpa/selectCheckboxModel.robot`

 * *Files identical despite different names*

### Comparing `modelDrivenRpa-1.4/modelDrivenRpa/selectFromDropdownModel.robot` & `modelDrivenRpa-1.5/modelDrivenRpa/selectFromDropdownModel.robot`

 * *Files identical despite different names*

### Comparing `modelDrivenRpa-1.4/modelDrivenRpa/utils/utils.robot` & `modelDrivenRpa-1.5/modelDrivenRpa/utils/utils.robot`

 * *Files identical despite different names*

