# Comparing `tmp/resfeci-0.0.16.tar.gz` & `tmp/resfeci-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\jason\Desktop\Split_Excel\dist\.tmp-cgmn0ktx\resfeci-0.0.16.tar", last modified: Wed Jul  5 02:45:16 2023, max compression
+gzip compressed data, was "C:\Users\jason\Desktop\Split_Excel\dist\.tmp-7tvffme4\resfeci-0.0.17.tar", last modified: Wed Jul  5 02:49:44 2023, max compression
```

## Comparing `resfeci-0.0.16.tar` & `resfeci-0.0.17.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 02:45:16.147997 resfeci-0.0.16/
--rw-rw-rw-   0        0        0     1069 2023-07-03 03:18:05.000000 resfeci-0.0.16/LICENSE
--rw-rw-rw-   0        0        0     2651 2023-07-05 02:45:16.147488 resfeci-0.0.16/PKG-INFO
--rw-rw-rw-   0        0        0     2046 2023-07-05 02:43:13.000000 resfeci-0.0.16/README.md
--rw-rw-rw-   0        0        0      809 2023-07-05 02:42:33.000000 resfeci-0.0.16/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-05 02:45:16.147997 resfeci-0.0.16/setup.cfg
--rw-rw-rw-   0        0        0       76 2023-07-04 06:55:59.000000 resfeci-0.0.16/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 02:45:16.128167 resfeci-0.0.16/src/
-drwxrwxrwx   0        0        0        0 2023-07-05 02:45:16.134797 resfeci-0.0.16/src/resfeci/
--rw-rw-rw-   0        0        0        0 2023-07-03 03:20:14.000000 resfeci-0.0.16/src/resfeci/__init__.py
--rw-rw-rw-   0        0        0     5463 2023-07-05 02:36:56.000000 resfeci-0.0.16/src/resfeci/excel_split.py
-drwxrwxrwx   0        0        0        0 2023-07-05 02:45:16.146476 resfeci-0.0.16/src/resfeci.egg-info/
--rw-rw-rw-   0        0        0     2651 2023-07-05 02:45:16.000000 resfeci-0.0.16/src/resfeci.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-07-05 02:45:16.000000 resfeci-0.0.16/src/resfeci.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 02:45:16.000000 resfeci-0.0.16/src/resfeci.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-05 02:45:16.000000 resfeci-0.0.16/src/resfeci.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 02:49:44.921710 resfeci-0.0.17/
+-rw-rw-rw-   0        0        0     1069 2023-07-03 03:18:05.000000 resfeci-0.0.17/LICENSE
+-rw-rw-rw-   0        0        0     2651 2023-07-05 02:49:44.921204 resfeci-0.0.17/PKG-INFO
+-rw-rw-rw-   0        0        0     2046 2023-07-05 02:43:13.000000 resfeci-0.0.17/README.md
+-rw-rw-rw-   0        0        0      809 2023-07-05 02:47:45.000000 resfeci-0.0.17/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-05 02:49:44.922217 resfeci-0.0.17/setup.cfg
+-rw-rw-rw-   0        0        0       76 2023-07-04 06:55:59.000000 resfeci-0.0.17/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 02:49:44.892594 resfeci-0.0.17/src/
+drwxrwxrwx   0        0        0        0 2023-07-05 02:49:44.910489 resfeci-0.0.17/src/resfeci/
+-rw-rw-rw-   0        0        0        0 2023-07-03 03:20:14.000000 resfeci-0.0.17/src/resfeci/__init__.py
+-rw-rw-rw-   0        0        0     5291 2023-07-05 02:48:56.000000 resfeci-0.0.17/src/resfeci/excel_split.py
+drwxrwxrwx   0        0        0        0 2023-07-05 02:49:44.919679 resfeci-0.0.17/src/resfeci.egg-info/
+-rw-rw-rw-   0        0        0     2651 2023-07-05 02:49:44.000000 resfeci-0.0.17/src/resfeci.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-07-05 02:49:44.000000 resfeci-0.0.17/src/resfeci.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 02:49:44.000000 resfeci-0.0.17/src/resfeci.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-05 02:49:44.000000 resfeci-0.0.17/src/resfeci.egg-info/top_level.txt
```

### Comparing `resfeci-0.0.16/LICENSE` & `resfeci-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `resfeci-0.0.16/PKG-INFO` & `resfeci-0.0.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resfeci
-Version: 0.0.16
+Version: 0.0.17
 Summary: Currently allows you to quickly split an Excel report into multiple sheets or multiple reports based on unique column values.
 Author-email: Jason Yearry <jasonyearry@gmail.com>
 Project-URL: Homepage, https://github.com/Guitarman-Waiting-In-The-Sky/excel_splitter
 Keywords: Excel,Split,opensource
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `resfeci-0.0.16/README.md` & `resfeci-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `resfeci-0.0.16/pyproject.toml` & `resfeci-0.0.17/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools", "wheel", "openpyxl>=3.0.10", "pandas>=1.2.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "resfeci"
-version = "0.0.16"
+version = "0.0.17"
 authors = [
   { name="Jason Yearry", email="jasonyearry@gmail.com" },
 ]
 
 
 description = "Currently allows you to quickly split an Excel report into multiple sheets or multiple reports based on unique column values."
 readme = "README.md"
```

### Comparing `resfeci-0.0.16/src/resfeci/excel_split.py` & `resfeci-0.0.17/src/resfeci/excel_split.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,10 +119,7 @@
                 row_counter=row_counter+1
 
 
             unique_items=remove_illegal_characters(str(unique_items))
 
             final_destination_wb.save(f'{str(unique_items)}.xlsx')
             final_destination_wb.close()
-
-if __name__=='__main__':
-    split_into_new_tabs_of_single_report(input_report_path="C:\\Users\\jason\\Desktop\\Songs.xlsx", column_number_to_split_by=2, sheet='Movies')
```

### Comparing `resfeci-0.0.16/src/resfeci.egg-info/PKG-INFO` & `resfeci-0.0.17/src/resfeci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resfeci
-Version: 0.0.16
+Version: 0.0.17
 Summary: Currently allows you to quickly split an Excel report into multiple sheets or multiple reports based on unique column values.
 Author-email: Jason Yearry <jasonyearry@gmail.com>
 Project-URL: Homepage, https://github.com/Guitarman-Waiting-In-The-Sky/excel_splitter
 Keywords: Excel,Split,opensource
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

