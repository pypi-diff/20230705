# Comparing `tmp/tablepic-0.0.4.tar.gz` & `tmp/tablepic-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablepic-0.0.4.tar", last modified: Wed Jun 21 12:53:23 2023, max compression
+gzip compressed data, was "tablepic-0.0.5.tar", last modified: Wed Jul  5 03:39:18 2023, max compression
```

## Comparing `tablepic-0.0.4.tar` & `tablepic-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-21 12:53:23.078843 tablepic-0.0.4/
--rw-r--r--   0 xinyan     (501) staff       (20)     1066 2023-06-16 07:22:57.000000 tablepic-0.0.4/LICENSE
--rw-r--r--   0 xinyan     (501) staff       (20)     1025 2023-06-21 12:53:23.078691 tablepic-0.0.4/PKG-INFO
--rw-r--r--   0 xinyan     (501) staff       (20)    16193 2023-06-20 15:57:19.000000 tablepic-0.0.4/README.md
--rw-r--r--   0 xinyan     (501) staff       (20)      604 2023-06-21 12:53:16.000000 tablepic-0.0.4/pyproject.toml
--rw-r--r--   0 xinyan     (501) staff       (20)      498 2023-06-16 07:33:42.000000 tablepic-0.0.4/readme_pypi.md
--rw-r--r--   0 xinyan     (501) staff       (20)       38 2023-06-21 12:53:23.078885 tablepic-0.0.4/setup.cfg
-drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-21 12:53:23.077299 tablepic-0.0.4/src/
--rw-r--r--   0 xinyan     (501) staff       (20)     9265 2023-06-20 06:10:03.000000 tablepic-0.0.4/src/demo.py
-drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-21 12:53:23.077701 tablepic-0.0.4/src/tablepic/
--rw-r--r--   0 xinyan     (501) staff       (20)      167 2023-06-14 15:44:10.000000 tablepic-0.0.4/src/tablepic/__init__.py
--rw-r--r--   0 xinyan     (501) staff       (20)    16949 2023-06-20 04:54:03.000000 tablepic-0.0.4/src/tablepic/main.py
-drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-21 12:53:23.078502 tablepic-0.0.4/src/tablepic.egg-info/
--rw-r--r--   0 xinyan     (501) staff       (20)     1025 2023-06-21 12:53:23.000000 tablepic-0.0.4/src/tablepic.egg-info/PKG-INFO
--rw-r--r--   0 xinyan     (501) staff       (20)      249 2023-06-21 12:53:23.000000 tablepic-0.0.4/src/tablepic.egg-info/SOURCES.txt
--rw-r--r--   0 xinyan     (501) staff       (20)        1 2023-06-21 12:53:23.000000 tablepic-0.0.4/src/tablepic.egg-info/dependency_links.txt
--rw-r--r--   0 xinyan     (501) staff       (20)       14 2023-06-21 12:53:23.000000 tablepic-0.0.4/src/tablepic.egg-info/top_level.txt
+drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-07-05 03:39:18.965240 tablepic-0.0.5/
+-rw-r--r--   0 xinyan     (501) staff       (20)     1066 2023-06-16 07:22:57.000000 tablepic-0.0.5/LICENSE
+-rw-r--r--   0 xinyan     (501) staff       (20)     1025 2023-07-05 03:39:18.965068 tablepic-0.0.5/PKG-INFO
+-rw-r--r--   0 xinyan     (501) staff       (20)    16193 2023-06-20 15:57:19.000000 tablepic-0.0.5/README.md
+-rw-r--r--   0 xinyan     (501) staff       (20)      604 2023-07-05 03:38:15.000000 tablepic-0.0.5/pyproject.toml
+-rw-r--r--   0 xinyan     (501) staff       (20)      498 2023-06-16 07:33:42.000000 tablepic-0.0.5/readme_pypi.md
+-rw-r--r--   0 xinyan     (501) staff       (20)       38 2023-07-05 03:39:18.965289 tablepic-0.0.5/setup.cfg
+drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-07-05 03:39:18.962461 tablepic-0.0.5/src/
+-rw-r--r--   0 xinyan     (501) staff       (20)     9265 2023-07-05 03:36:24.000000 tablepic-0.0.5/src/demo.py
+drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-07-05 03:39:18.963687 tablepic-0.0.5/src/tablepic/
+-rw-r--r--   0 xinyan     (501) staff       (20)      167 2023-06-14 15:44:10.000000 tablepic-0.0.5/src/tablepic/__init__.py
+-rw-r--r--   0 xinyan     (501) staff       (20)    17107 2023-07-05 03:35:06.000000 tablepic-0.0.5/src/tablepic/main.py
+drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-07-05 03:39:18.964793 tablepic-0.0.5/src/tablepic.egg-info/
+-rw-r--r--   0 xinyan     (501) staff       (20)     1025 2023-07-05 03:39:18.000000 tablepic-0.0.5/src/tablepic.egg-info/PKG-INFO
+-rw-r--r--   0 xinyan     (501) staff       (20)      249 2023-07-05 03:39:18.000000 tablepic-0.0.5/src/tablepic.egg-info/SOURCES.txt
+-rw-r--r--   0 xinyan     (501) staff       (20)        1 2023-07-05 03:39:18.000000 tablepic-0.0.5/src/tablepic.egg-info/dependency_links.txt
+-rw-r--r--   0 xinyan     (501) staff       (20)       14 2023-07-05 03:39:18.000000 tablepic-0.0.5/src/tablepic.egg-info/top_level.txt
```

### Comparing `tablepic-0.0.4/LICENSE` & `tablepic-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tablepic-0.0.4/PKG-INFO` & `tablepic-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablepic
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package can generate a picture which contains a table.
 Author-email: Xin Yan <slash.xin@gmail.com>
 Project-URL: Homepage, https://github.com/slash-xin/tablepic
 Project-URL: Bug Tracker, https://github.com/slash-xin/tablepic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tablepic-0.0.4/README.md` & `tablepic-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tablepic-0.0.4/pyproject.toml` & `tablepic-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tablepic"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Xin Yan", email="slash.xin@gmail.com" },
 ]
 description = "A package can generate a picture which contains a table."
 readme = "readme_pypi.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `tablepic-0.0.4/src/demo.py` & `tablepic-0.0.5/src/demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: xinyan
 Date: 2023-06-14 23:43:57
 LastEditors: xinyan
-LastEditTime: 2023-06-20 14:10:03
+LastEditTime: 2023-07-05 11:36:19
 Description: file content
 '''
 import tablepic as tp
 
 
 # ---------------------------------
 # Generate a regular table.
```

### Comparing `tablepic-0.0.4/src/tablepic/main.py` & `tablepic-0.0.5/src/tablepic/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: xinyan
 Date: 2023-06-13 17:12:25
 LastEditors: xinyan
-LastEditTime: 2023-06-20 12:54:03
+LastEditTime: 2023-07-05 11:35:06
 Description: file content
 '''
 
 
 import sys
 from PIL import Image, ImageFont, ImageDraw
 
@@ -121,26 +121,27 @@
     elif data_dict[key].get(f'c{j}', None):
         result = data_dict[key].get(f'c{j}')
     else:
         result = v_default
     return result
 
 
-def calculate_cell_width_height(data_dict:dict, font_path:str, cell_width:int, cell_height:int):
+def calculate_cell_width_height(row_num:int, data_dict:dict, font_path:str, cell_width:int, cell_height:int):
     col_width_dict = {}
     row_height_dict = {}
+    header_row = row_num - len(data_dict['content'])
     for i, data_line in enumerate(data_dict['content']):
         for j, data_content in enumerate(data_line):
             data_font = get_font(font_path, get_data_info(data_dict, 'font_size', i, j, 20, int))
             c_w, c_h = 0, 0
             for item in data_content.split('\n'):
                 w, h = data_font.getbbox(item)[2:]
                 c_w = max(c_w, w) + 20
-            c_h = h * len(data_content.split('\n'))
-            row_height_dict[i] = max(row_height_dict.get(i, cell_height), c_h)
+            c_h = h * len(data_content.split('\n')) + 20
+            row_height_dict[i + header_row] = max(row_height_dict.get(i + header_row, cell_height), c_h)
             col_width_dict[j] = max(col_width_dict.get(j, cell_width), c_w)
     return col_width_dict, row_height_dict
 
 
 def generate_table_pic(row_num:int, col_num:int, title_list:list, header_dict:dict, data_dict:dict, img_path:str, footnote_list:list=[],
                        cell_width:int=150, cell_height:int=50,  col_width_dict:dict={}, row_height_dict:dict={}, cell_merge_dict:dict={},
                        table_margin:int=20, pic_bk_color='#FFFFFF', table_line_color='#E8EAED', font_path:str=None):
@@ -195,16 +196,17 @@
         by merging 1 row downward and 0 columns to the right (i.e., not merging columns); the cell at coordinate [0,1] needs to be merged, by merging
         0 rows downward and 1 column to the right.
     :param pic_bk_color: str, optional parameter. Set the background color of the picture, default value is '#FFFFFF'.
     :param table_line_color: str, optional parameter. Set the line color of the table, default value is '#E8EAED'.
     :param font_path: str, optional parameter. Given the font path to set a new font for the text (including title, header, data).
     """
     # Calculate the width for each column and the height for each row
-    if len(row_height_dict) == 0 or len(col_width_dict) == 0:
-        col_width_dict, row_height_dict = calculate_cell_width_height(data_dict, font_path, cell_width, cell_height)
+    default_col_width_dict, default_row_height_dict = calculate_cell_width_height(row_num, data_dict, font_path, cell_width, cell_height)
+    col_width_dict.update(default_col_width_dict)
+    row_height_dict.update(default_row_height_dict)
 
     color_white = '#FFFFFF'
     color_black = '#000000'
     color_default_header_bk = '#CCD6EB'
     title_list = process_title_footnote(title_list, 'title')
     footnote_list = process_title_footnote(footnote_list, 'footnote')
     total_title_height = sum([title['height'] for title in title_list])
```

### Comparing `tablepic-0.0.4/src/tablepic.egg-info/PKG-INFO` & `tablepic-0.0.5/src/tablepic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablepic
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package can generate a picture which contains a table.
 Author-email: Xin Yan <slash.xin@gmail.com>
 Project-URL: Homepage, https://github.com/slash-xin/tablepic
 Project-URL: Bug Tracker, https://github.com/slash-xin/tablepic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

