# Comparing `tmp/mdrpaLibrary-1.2.tar.gz` & `tmp/mdrpaLibrary-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdrpaLibrary-1.2.tar", last modified: Wed Jul  5 16:08:07 2023, max compression
+gzip compressed data, was "mdrpaLibrary-1.3.tar", last modified: Wed Jul  5 16:19:32 2023, max compression
```

## Comparing `mdrpaLibrary-1.2.tar` & `mdrpaLibrary-1.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:08:07.356603 mdrpaLibrary-1.2/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-05 16:08:07.356478 mdrpaLibrary-1.2/PKG-INFO
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:08:07.354708 mdrpaLibrary-1.2/mdrpaLibrary/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:55:03.000000 mdrpaLibrary-1.2/mdrpaLibrary/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3321 2023-07-05 15:57:25.000000 mdrpaLibrary-1.2/mdrpaLibrary/clickButtonModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      482 2023-07-05 15:57:12.000000 mdrpaLibrary-1.2/mdrpaLibrary/customFunctions.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      491 2023-07-05 15:56:39.000000 mdrpaLibrary-1.2/mdrpaLibrary/getUiModels.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3347 2023-07-05 15:57:04.000000 mdrpaLibrary-1.2/mdrpaLibrary/inputFieldModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1478 2023-07-05 16:07:27.000000 mdrpaLibrary-1.2/mdrpaLibrary/model_driven_rpa.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3360 2023-07-05 15:56:57.000000 mdrpaLibrary-1.2/mdrpaLibrary/selectCheckboxModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3417 2023-07-05 15:56:45.000000 mdrpaLibrary-1.2/mdrpaLibrary/selectFromDropdownModel.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:08:07.356105 mdrpaLibrary-1.2/mdrpaLibrary/utils/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:00:07.000000 mdrpaLibrary-1.2/mdrpaLibrary/utils/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     2955 2023-07-05 15:00:09.000000 mdrpaLibrary-1.2/mdrpaLibrary/utils/utils.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:08:07.355618 mdrpaLibrary-1.2/mdrpaLibrary.egg-info/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-05 16:08:07.000000 mdrpaLibrary-1.2/mdrpaLibrary.egg-info/PKG-INFO
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      491 2023-07-05 16:08:07.000000 mdrpaLibrary-1.2/mdrpaLibrary.egg-info/SOURCES.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-05 16:08:07.000000 mdrpaLibrary-1.2/mdrpaLibrary.egg-info/dependency_links.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       13 2023-07-05 16:08:07.000000 mdrpaLibrary-1.2/mdrpaLibrary.egg-info/top_level.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-05 16:08:07.356647 mdrpaLibrary-1.2/setup.cfg
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      193 2023-07-05 16:06:21.000000 mdrpaLibrary-1.2/setup.py
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:19:32.349184 mdrpaLibrary-1.3/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-05 16:19:32.349060 mdrpaLibrary-1.3/PKG-INFO
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:19:32.347936 mdrpaLibrary-1.3/mdrpaLibrary/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:55:03.000000 mdrpaLibrary-1.3/mdrpaLibrary/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3353 2023-07-05 16:14:44.000000 mdrpaLibrary-1.3/mdrpaLibrary/clickButtonModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      516 2023-07-05 16:14:49.000000 mdrpaLibrary-1.3/mdrpaLibrary/customFunctions.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      524 2023-07-05 16:14:52.000000 mdrpaLibrary-1.3/mdrpaLibrary/getUiModels.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3379 2023-07-05 16:14:55.000000 mdrpaLibrary-1.3/mdrpaLibrary/inputFieldModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1669 2023-07-05 16:18:26.000000 mdrpaLibrary-1.3/mdrpaLibrary/modelDrivenRpa.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3393 2023-07-05 16:14:58.000000 mdrpaLibrary-1.3/mdrpaLibrary/selectCheckboxModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3449 2023-07-05 16:15:00.000000 mdrpaLibrary-1.3/mdrpaLibrary/selectFromDropdownModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      863 2023-07-05 16:13:32.000000 mdrpaLibrary-1.3/mdrpaLibrary/sendReportModel.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:19:32.348780 mdrpaLibrary-1.3/mdrpaLibrary/utils/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:00:07.000000 mdrpaLibrary-1.3/mdrpaLibrary/utils/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     2484 2023-07-05 16:13:57.000000 mdrpaLibrary-1.3/mdrpaLibrary/utils/utils.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 16:19:32.348555 mdrpaLibrary-1.3/mdrpaLibrary.egg-info/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-05 16:19:32.000000 mdrpaLibrary-1.3/mdrpaLibrary.egg-info/PKG-INFO
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      524 2023-07-05 16:19:32.000000 mdrpaLibrary-1.3/mdrpaLibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-05 16:19:32.000000 mdrpaLibrary-1.3/mdrpaLibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       13 2023-07-05 16:19:32.000000 mdrpaLibrary-1.3/mdrpaLibrary.egg-info/top_level.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-05 16:19:32.349224 mdrpaLibrary-1.3/setup.cfg
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      193 2023-07-05 16:19:03.000000 mdrpaLibrary-1.3/setup.py
```

### Comparing `mdrpaLibrary-1.2/mdrpaLibrary/clickButtonModel.robot` & `mdrpaLibrary-1.3/mdrpaLibrary/clickButtonModel.robot`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Library    RPA.HTTP
 Library    OperatingSystem
 Library    BuiltIn
 Library    RPA.JSON
 Library    RPA.Desktop
 Library    Collections
 Resource   ./utils/utils.robot
-
+Resource   sendReportModel.robot
 
 
 
 *** Keywords ***
```

### Comparing `mdrpaLibrary-1.2/mdrpaLibrary/inputFieldModel.robot` & `mdrpaLibrary-1.3/mdrpaLibrary/inputFieldModel.robot`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Library    RPA.HTTP
 Library    OperatingSystem
 Library    BuiltIn
 Library    RPA.JSON
 Library    RPA.Desktop
 Library    Collections
 Resource   ./utils/utils.robot
-
+Resource   sendReportModel.robot
 
 *** Keywords ***
 
 
 Input Field Model
     [Arguments]   ${application}  ${page}   ${ui_element}    ${model}    ${value}
     Set Suite Variable  ${model_name}    ${application}
```

### Comparing `mdrpaLibrary-1.2/mdrpaLibrary/model_driven_rpa.py` & `mdrpaLibrary-1.3/mdrpaLibrary/modelDrivenRpa.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,36 +8,43 @@
         self.builtin = BuiltIn()
         self.resource_files = [
             'clickButtonModel.robot',
             'inputFieldModel.robot',
             'selectCheckboxModel.robot',
             'selectFromDropdownModel.robot',
             'getUiModel.robot'
+            'sendReportModel.robot'
         ]  
 
     def import_resource_file(self, resource_file):
         self.builtin.import_resource(resource_file)
 
     @keyword
-    def click_button_model_keyword(self, *args):
+    def click_button_model(self, *args):
         self.import_resource_file(self.resource_files[0])  
         self.builtin.run_keyword('Click Button Model', *args)
 
     @keyword
-    def input_field_model_keyword(self, *args):
+    def input_field_model(self, *args):
         self.import_resource_file(self.resource_files[1])  
         self.builtin.run_keyword('Input Field Model', *args)
 
     @keyword
-    def select_checkbox_model_keyword(self, *args):
+    def select_checkbox_model(self, *args):
         self.import_resource_file(self.resource_files[2])  
         self.builtin.run_keyword('Select Checkbox Model', *args)
 
     @keyword
-    def select_from_dropdown_model_keyword(self, *args):
+    def select_from_dropdown_model(self, *args):
         self.import_resource_file(self.resource_files[3])  
         self.builtin.run_keyword('Select Value From Dropdown Model', *args)
     
     @keyword
-    def get_ui_models_keyword(self, *args):
+    def get_ui_models(self, *args):
         self.import_resource_file(self.resource_files[4]) 
         self.builtin.run_keyword('Get UiModels', *args)
+    
+    @keyword
+    def send_report_to_UI_Modeler(self, *args):
+        self.import_resource_file(self.resource_files[5]) 
+        self.builtin.run_keyword('Send Report to UI Modeler', *args)
+
```

### Comparing `mdrpaLibrary-1.2/mdrpaLibrary/selectCheckboxModel.robot` & `mdrpaLibrary-1.3/mdrpaLibrary/selectCheckboxModel.robot`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Library    OperatingSystem
 Library    BuiltIn
 Library    RPA.JSON
 Library    RPA.Desktop
 Library    Collections
 
 Resource   ./utils/utils.robot
+Resource   sendReportModel.robot
 
 
 *** Keywords ***
 
 
 Select Checkbox Model
     [Arguments]    ${application}  ${page}   ${ui_element}    ${model}
```

### Comparing `mdrpaLibrary-1.2/mdrpaLibrary/selectFromDropdownModel.robot` & `mdrpaLibrary-1.3/mdrpaLibrary/selectFromDropdownModel.robot`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Library    OperatingSystem
 Library    BuiltIn
 Library    RPA.JSON
 Library    RPA.Desktop
 Library    Collections
 
 Resource   ./utils/utils.robot
-
+Resource   sendReportModel.robot
 
 *** Keywords ***
 
 
 Select Value from Dropdown Model
     [Arguments]   ${application}  ${page}   ${ui_element}    ${model}    ${value}
     Set Suite Variable  ${model_name}    ${application}
```

### Comparing `mdrpaLibrary-1.2/mdrpaLibrary/utils/utils.robot` & `mdrpaLibrary-1.3/mdrpaLibrary/utils/utils.robot`

 * *Files 8% similar despite different names*

```diff
@@ -21,23 +21,15 @@
     FOR    ${attribute}    IN    @{attributes}
         ${name}    Set Variable    ${attribute["name"]}
         ${value}    Set Variable    ${attribute["value"]}
         Run Keyword If    '${name}' == 'id'     Set Suite Variable    ${id}     ${value}
     END
     [Return]    ${id}
 
-Create Error
-    [Arguments]    ${model_name}    ${page_name}    ${element_name}    ${locator}
-    &{element}    Create Dictionary     model_name=${model_name}      page_name=${page_name}    element_name=${element_name}    locator=${locator}
-    Append To List    ${error_list}    ${element}
 
-Send Report to UI Modeler
-    Set Suite Variable   ${report}    ${error_list}
-    ${resp}=    POST    ${HTTP_LOCAL_SERVER}    json=${report}
-    Status Should Be    OK    ${resp}
 
 Set UI Element
     [Arguments]  ${model_name}   ${page_name}    ${element_name}   ${models}
     Set Suite Variable  ${model_name}
     Set Suite Variable  ${page_name}
     Set Suite Variable  ${element_name}
     ${model}=   Get Model From All Models   ${models}
```

