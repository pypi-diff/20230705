# Comparing `tmp/mdrpaLibrary-1.0.tar.gz` & `tmp/mdrpaLibrary-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdrpaLibrary-1.0.tar", last modified: Wed Jul  5 15:50:55 2023, max compression
+gzip compressed data, was "mdrpaLibrary-1.1.tar", last modified: Wed Jul  5 16:00:16 2023, max compression
```

## Comparing `mdrpaLibrary-1.0.tar` & `mdrpaLibrary-1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 15:50:55.968131 mdrpaLibrary-1.0/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-05 15:50:55.967925 mdrpaLibrary-1.0/PKG-INFO
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 15:50:55.966581 mdrpaLibrary-1.0/mdrpaLibrary/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:55:03.000000 mdrpaLibrary-1.0/mdrpaLibrary/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3323 2023-07-05 15:00:09.000000 mdrpaLibrary-1.0/mdrpaLibrary/clickButtonModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      483 2023-07-05 15:00:09.000000 mdrpaLibrary-1.0/mdrpaLibrary/customFunctions.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      492 2023-07-05 15:00:09.000000 mdrpaLibrary-1.0/mdrpaLibrary/getUiModels.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3349 2023-07-05 15:00:09.000000 mdrpaLibrary-1.0/mdrpaLibrary/inputFieldModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1739 2023-07-05 15:47:16.000000 mdrpaLibrary-1.0/mdrpaLibrary/model_driven_rpa.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3361 2023-07-05 15:00:09.000000 mdrpaLibrary-1.0/mdrpaLibrary/selectCheckboxModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3418 2023-07-05 15:00:09.000000 mdrpaLibrary-1.0/mdrpaLibrary/selectFromDropdownModel.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 15:50:55.967623 mdrpaLibrary-1.0/mdrpaLibrary/utils/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:00:07.000000 mdrpaLibrary-1.0/mdrpaLibrary/utils/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     2955 2023-07-05 15:00:09.000000 mdrpaLibrary-1.0/mdrpaLibrary/utils/utils.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 15:50:55.967314 mdrpaLibrary-1.0/mdrpaLibrary.egg-info/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-05 15:50:55.000000 mdrpaLibrary-1.0/mdrpaLibrary.egg-info/PKG-INFO
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      491 2023-07-05 15:50:55.000000 mdrpaLibrary-1.0/mdrpaLibrary.egg-info/SOURCES.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-05 15:50:55.000000 mdrpaLibrary-1.0/mdrpaLibrary.egg-info/dependency_links.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       13 2023-07-05 15:50:55.000000 mdrpaLibrary-1.0/mdrpaLibrary.egg-info/top_level.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-05 15:50:55.968204 mdrpaLibrary-1.0/setup.cfg
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      193 2023-07-05 15:50:48.000000 mdrpaLibrary-1.0/setup.py
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:00:16.908017 mdrpaLibrary-1.1/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-05 16:00:16.907775 mdrpaLibrary-1.1/PKG-INFO
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:00:16.906105 mdrpaLibrary-1.1/mdrpaLibrary/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:55:03.000000 mdrpaLibrary-1.1/mdrpaLibrary/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3321 2023-07-05 15:57:25.000000 mdrpaLibrary-1.1/mdrpaLibrary/clickButtonModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      482 2023-07-05 15:57:12.000000 mdrpaLibrary-1.1/mdrpaLibrary/customFunctions.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      491 2023-07-05 15:56:39.000000 mdrpaLibrary-1.1/mdrpaLibrary/getUiModels.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3347 2023-07-05 15:57:04.000000 mdrpaLibrary-1.1/mdrpaLibrary/inputFieldModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1779 2023-07-05 15:58:45.000000 mdrpaLibrary-1.1/mdrpaLibrary/model_driven_rpa.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3360 2023-07-05 15:56:57.000000 mdrpaLibrary-1.1/mdrpaLibrary/selectCheckboxModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3417 2023-07-05 15:56:45.000000 mdrpaLibrary-1.1/mdrpaLibrary/selectFromDropdownModel.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:00:16.907331 mdrpaLibrary-1.1/mdrpaLibrary/utils/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:00:07.000000 mdrpaLibrary-1.1/mdrpaLibrary/utils/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     2955 2023-07-05 15:00:09.000000 mdrpaLibrary-1.1/mdrpaLibrary/utils/utils.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:00:16.907039 mdrpaLibrary-1.1/mdrpaLibrary.egg-info/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-05 16:00:16.000000 mdrpaLibrary-1.1/mdrpaLibrary.egg-info/PKG-INFO
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      491 2023-07-05 16:00:16.000000 mdrpaLibrary-1.1/mdrpaLibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-05 16:00:16.000000 mdrpaLibrary-1.1/mdrpaLibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       13 2023-07-05 16:00:16.000000 mdrpaLibrary-1.1/mdrpaLibrary.egg-info/top_level.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-05 16:00:16.908068 mdrpaLibrary-1.1/setup.cfg
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      193 2023-07-05 15:59:37.000000 mdrpaLibrary-1.1/setup.py
```

### Comparing `mdrpaLibrary-1.0/mdrpaLibrary/clickButtonModel.robot` & `mdrpaLibrary-1.1/mdrpaLibrary/clickButtonModel.robot`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 Library    RPA.Browser.Selenium  auto_close=${FALSE}
 Library    RPA.HTTP
 Library    OperatingSystem
 Library    BuiltIn
 Library    RPA.JSON
 Library    RPA.Desktop
 Library    Collections
-
-Resource   ../utils/utils.robot
+Resource   ./utils/utils.robot
 
 
 
 
 *** Keywords ***
```

### Comparing `mdrpaLibrary-1.0/mdrpaLibrary/inputFieldModel.robot` & `mdrpaLibrary-1.1/mdrpaLibrary/inputFieldModel.robot`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 Library    RPA.Browser.Selenium  auto_close=${FALSE}
 Library    RPA.HTTP
 Library    OperatingSystem
 Library    BuiltIn
 Library    RPA.JSON
 Library    RPA.Desktop
 Library    Collections
-
-Resource   ../utils/utils.robot
+Resource   ./utils/utils.robot
 
 
 *** Keywords ***
 
 
 Input Field Model
     [Arguments]   ${application}  ${page}   ${ui_element}    ${model}    ${value}
```

### Comparing `mdrpaLibrary-1.0/mdrpaLibrary/model_driven_rpa.py` & `mdrpaLibrary-1.1/mdrpaLibrary/model_driven_rpa.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,30 +15,30 @@
         ]  # Update with the actual resource file names
 
     def import_resource_file(self, resource_file):
         # Use the BuiltIn library's `Import Resource` keyword to import the specified resource file
         self.builtin.import_resource(resource_file)
 
     @keyword
-    def click_button_model(self, *args):
+    def click_button_model_keyword(self, *args):
         self.import_resource_file(self.resource_files[0])  # Import the first resource file
         self.builtin.run_keyword('Click Button Model', *args)
 
     @keyword
-    def input_field_model(self, *args):
+    def input_field_model_keyword(self, *args):
         self.import_resource_file(self.resource_files[1])  # Import the second resource file
         self.builtin.run_keyword('Input Field Model', *args)
 
     @keyword
-    def select_checkbox_model(self, *args):
+    def select_checkbox_model_keyword(self, *args):
         self.import_resource_file(self.resource_files[2])  # Import the third resource file
         self.builtin.run_keyword('Select Checkbox Model', *args)
 
     @keyword
-    def select_from_dropdown_model(self, *args):
+    def select_from_dropdown_model_keyword(self, *args):
         self.import_resource_file(self.resource_files[3])  # Import the fourth resource file
         self.builtin.run_keyword('Select From Dropdown Model', *args)
     
     @keyword
-    def get_ui_models(self, *args):
+    def get_ui_models_keyword(self, *args):
         self.import_resource_file(self.resource_files[4])  # Import the fifth resource file
         self.builtin.run_keyword('Get UiModels', *args)
```

### Comparing `mdrpaLibrary-1.0/mdrpaLibrary/selectCheckboxModel.robot` & `mdrpaLibrary-1.1/mdrpaLibrary/selectCheckboxModel.robot`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Library    RPA.HTTP
 Library    OperatingSystem
 Library    BuiltIn
 Library    RPA.JSON
 Library    RPA.Desktop
 Library    Collections
 
-Resource   ../utils/utils.robot
+Resource   ./utils/utils.robot
 
 
 *** Keywords ***
 
 
 Select Checkbox Model
     [Arguments]    ${application}  ${page}   ${ui_element}    ${model}
```

### Comparing `mdrpaLibrary-1.0/mdrpaLibrary/selectFromDropdownModel.robot` & `mdrpaLibrary-1.1/mdrpaLibrary/selectFromDropdownModel.robot`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Library    RPA.HTTP
 Library    OperatingSystem
 Library    BuiltIn
 Library    RPA.JSON
 Library    RPA.Desktop
 Library    Collections
 
-Resource   ../utils/utils.robot
+Resource   ./utils/utils.robot
 
 
 *** Keywords ***
 
 
 Select Value from Dropdown Model
     [Arguments]   ${application}  ${page}   ${ui_element}    ${model}    ${value}
```

### Comparing `mdrpaLibrary-1.0/mdrpaLibrary/utils/utils.robot` & `mdrpaLibrary-1.1/mdrpaLibrary/utils/utils.robot`

 * *Files identical despite different names*

