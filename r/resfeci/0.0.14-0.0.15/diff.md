# Comparing `tmp/resfeci-0.0.14.tar.gz` & `tmp/resfeci-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\jason\Desktop\Split_Excel\dist\.tmp-wknm7rkc\resfeci-0.0.14.tar", last modified: Tue Jul  4 23:36:20 2023, max compression
+gzip compressed data, was "C:\Users\jason\Desktop\Split_Excel\dist\.tmp-phf2qyza\resfeci-0.0.15.tar", last modified: Tue Jul  4 23:51:07 2023, max compression
```

## Comparing `resfeci-0.0.14.tar` & `resfeci-0.0.15.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 23:36:20.473399 resfeci-0.0.14/
--rw-rw-rw-   0        0        0     1069 2023-07-03 03:18:05.000000 resfeci-0.0.14/LICENSE
--rw-rw-rw-   0        0        0     2099 2023-07-04 23:36:20.472387 resfeci-0.0.14/PKG-INFO
--rw-rw-rw-   0        0        0     1494 2023-07-04 08:28:43.000000 resfeci-0.0.14/README.md
--rw-rw-rw-   0        0        0      809 2023-07-04 23:34:46.000000 resfeci-0.0.14/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-04 23:36:20.473399 resfeci-0.0.14/setup.cfg
--rw-rw-rw-   0        0        0       76 2023-07-04 06:55:59.000000 resfeci-0.0.14/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 23:36:20.438921 resfeci-0.0.14/src/
-drwxrwxrwx   0        0        0        0 2023-07-04 23:36:20.457060 resfeci-0.0.14/src/resfeci/
--rw-rw-rw-   0        0        0        0 2023-07-03 03:20:14.000000 resfeci-0.0.14/src/resfeci/__init__.py
--rw-rw-rw-   0        0        0     4919 2023-07-04 23:34:46.000000 resfeci-0.0.14/src/resfeci/excel_split.py
-drwxrwxrwx   0        0        0        0 2023-07-04 23:36:20.471372 resfeci-0.0.14/src/resfeci.egg-info/
--rw-rw-rw-   0        0        0     2099 2023-07-04 23:36:20.000000 resfeci-0.0.14/src/resfeci.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-07-04 23:36:20.000000 resfeci-0.0.14/src/resfeci.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 23:36:20.000000 resfeci-0.0.14/src/resfeci.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-04 23:36:20.000000 resfeci-0.0.14/src/resfeci.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 23:51:07.856731 resfeci-0.0.15/
+-rw-rw-rw-   0        0        0     1069 2023-07-03 03:18:05.000000 resfeci-0.0.15/LICENSE
+-rw-rw-rw-   0        0        0     2023 2023-07-04 23:51:07.855716 resfeci-0.0.15/PKG-INFO
+-rw-rw-rw-   0        0        0     1418 2023-07-04 23:50:12.000000 resfeci-0.0.15/README.md
+-rw-rw-rw-   0        0        0      809 2023-07-04 23:50:12.000000 resfeci-0.0.15/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-04 23:51:07.856731 resfeci-0.0.15/setup.cfg
+-rw-rw-rw-   0        0        0       76 2023-07-04 06:55:59.000000 resfeci-0.0.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:51:07.828587 resfeci-0.0.15/src/
+drwxrwxrwx   0        0        0        0 2023-07-04 23:51:07.840779 resfeci-0.0.15/src/resfeci/
+-rw-rw-rw-   0        0        0        0 2023-07-03 03:20:14.000000 resfeci-0.0.15/src/resfeci/__init__.py
+-rw-rw-rw-   0        0        0     9068 2023-07-04 23:47:46.000000 resfeci-0.0.15/src/resfeci/excel_split.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:51:07.854700 resfeci-0.0.15/src/resfeci.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-07-04 23:51:07.000000 resfeci-0.0.15/src/resfeci.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-07-04 23:51:07.000000 resfeci-0.0.15/src/resfeci.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 23:51:07.000000 resfeci-0.0.15/src/resfeci.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-04 23:51:07.000000 resfeci-0.0.15/src/resfeci.egg-info/top_level.txt
```

### Comparing `resfeci-0.0.14/LICENSE` & `resfeci-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `resfeci-0.0.14/PKG-INFO` & `resfeci-0.0.15/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 Metadata-Version: 2.1
 Name: resfeci
-Version: 0.0.14
+Version: 0.0.15
 Summary: Currently allows you to quickly split an Excel report into multiple sheets or multiple reports based on unique column values.
 Author-email: Jason Yearry <jasonyearry@gmail.com>
 Project-URL: Homepage, https://github.com/Guitarman-Waiting-In-The-Sky/excel_splitter
 Keywords: Excel,Split,opensource
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ResFeci for Excel
 
-In it's current state, this package will allow you to quickly split a single Excel sheet into either separate tabs within the same report or into different Excel reports.  For example, if Column 'B' of your Excel report contains "Names" and "Jack" appears in 3 rows and "Jill" appears in 2, then, this will split the report into 2 separate reports (one for only Jack's rows and another for only Jill's)---or, this will create a new report tabs entitled "Jack" and "Jill".
+In it's current state, this package will allow you to quickly split a single Excel sheet into either separate tabs within the same report or into different Excel reports.  For example, if Column 'B' of your Excel report contains "Names" and "Jack" appears in 3 rows and "Jill" appears in 2, then, this will split the report into 2 separate reports (one for only Jack's rows and another for only Jill's)---or, this will create a new report with tabs entitled "Jack" and "Jill".
 
 **IMPORTANT: Your sheet must contain a header row to function properly!**
 
 
 ## EXAMPLE OF SPLITTING AN EXCEL SHEET BY UNIQUE VALUES IN COLUMN B INTO DIFFERENT REPORTS
 
 from resfeci import excel_split
 
-excel_split.split_sheet(split_type= 'separate_files' , input_report_path= 'PATH_TO_REPORT.xlsx' , column_number_to_split_by=2)
+excel_split.split_into_separate_reports(input_report_path= 'PATH_TO_REPORT.xlsx' , column_number_to_split_by=2)
 
 
 ## EXAMPLE OF SPLITTING AN EXCEL SHEET BY UNIQUE VALUES IN COLUMN B INTO DIFFERENT TABS OF THE SAME REPORT
 
 from resfeci import excel_split
 
-excel_split.split_sheet(split_type= 'split_tabs' , input_report_path= 'PATH_TO_REPORT.xlsx' , column_number_to_split_by=2)
+excel_split.split_into_new_tabs_of_single_report(input_report_path= 'PATH_TO_REPORT.xlsx' , column_number_to_split_by=2)
 
 
 **PARAMETER DESCRIPTIONS**
 
-split_type = must be either "separate_files" or "split_tabs"
-
 input_report_path = the path to the report to be split
 
 column_number_to_split_by = the NUMBER of the Excel column to split by (A = 1, B = 2, C =3, etc.)
 
 **DEPENDENCIES**
-Openpyxl
-Pandas
+Openpyxl, Pandas
 
 **KNOWN ISSUE** 
 The current version of this script does not support transfer of formulas!!
```

### Comparing `resfeci-0.0.14/README.md` & `resfeci-0.0.15/src/resfeci.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,46 @@
+Metadata-Version: 2.1
+Name: resfeci
+Version: 0.0.15
+Summary: Currently allows you to quickly split an Excel report into multiple sheets or multiple reports based on unique column values.
+Author-email: Jason Yearry <jasonyearry@gmail.com>
+Project-URL: Homepage, https://github.com/Guitarman-Waiting-In-The-Sky/excel_splitter
+Keywords: Excel,Split,opensource
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ResFeci for Excel
 
-In it's current state, this package will allow you to quickly split a single Excel sheet into either separate tabs within the same report or into different Excel reports.  For example, if Column 'B' of your Excel report contains "Names" and "Jack" appears in 3 rows and "Jill" appears in 2, then, this will split the report into 2 separate reports (one for only Jack's rows and another for only Jill's)---or, this will create a new report tabs entitled "Jack" and "Jill".
+In it's current state, this package will allow you to quickly split a single Excel sheet into either separate tabs within the same report or into different Excel reports.  For example, if Column 'B' of your Excel report contains "Names" and "Jack" appears in 3 rows and "Jill" appears in 2, then, this will split the report into 2 separate reports (one for only Jack's rows and another for only Jill's)---or, this will create a new report with tabs entitled "Jack" and "Jill".
 
 **IMPORTANT: Your sheet must contain a header row to function properly!**
 
 
 ## EXAMPLE OF SPLITTING AN EXCEL SHEET BY UNIQUE VALUES IN COLUMN B INTO DIFFERENT REPORTS
 
 from resfeci import excel_split
 
-excel_split.split_sheet(split_type= 'separate_files' , input_report_path= 'PATH_TO_REPORT.xlsx' , column_number_to_split_by=2)
+excel_split.split_into_separate_reports(input_report_path= 'PATH_TO_REPORT.xlsx' , column_number_to_split_by=2)
 
 
 ## EXAMPLE OF SPLITTING AN EXCEL SHEET BY UNIQUE VALUES IN COLUMN B INTO DIFFERENT TABS OF THE SAME REPORT
 
 from resfeci import excel_split
 
-excel_split.split_sheet(split_type= 'split_tabs' , input_report_path= 'PATH_TO_REPORT.xlsx' , column_number_to_split_by=2)
+excel_split.split_into_new_tabs_of_single_report(input_report_path= 'PATH_TO_REPORT.xlsx' , column_number_to_split_by=2)
 
 
 **PARAMETER DESCRIPTIONS**
 
-split_type = must be either "separate_files" or "split_tabs"
-
 input_report_path = the path to the report to be split
 
 column_number_to_split_by = the NUMBER of the Excel column to split by (A = 1, B = 2, C =3, etc.)
 
 **DEPENDENCIES**
-Openpyxl
-Pandas
+Openpyxl, Pandas
 
 **KNOWN ISSUE** 
-The current version of this script does not support transfer of formulas!!
+The current version of this script does not support transfer of formulas!!
```

### Comparing `resfeci-0.0.14/pyproject.toml` & `resfeci-0.0.15/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools", "wheel", "openpyxl>=3.0.10", "pandas>=1.2.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "resfeci"
-version = "0.0.14"
+version = "0.0.15"
 authors = [
   { name="Jason Yearry", email="jasonyearry@gmail.com" },
 ]
 
 
 description = "Currently allows you to quickly split an Excel report into multiple sheets or multiple reports based on unique column values."
 readme = "README.md"
```

