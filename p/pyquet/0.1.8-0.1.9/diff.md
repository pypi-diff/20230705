# Comparing `tmp/pyquet-0.1.8.tar.gz` & `tmp/pyquet-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquet-0.1.8.tar", last modified: Tue Jun 13 16:39:17 2023, max compression
+gzip compressed data, was "pyquet-0.1.9.tar", last modified: Wed Jul  5 12:52:43 2023, max compression
```

## Comparing `pyquet-0.1.8.tar` & `pyquet-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 16:39:16.997105 pyquet-0.1.8/
--rw-rw-rw-   0        0        0     1086 2023-05-26 12:18:55.000000 pyquet-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      546 2023-06-13 16:39:16.997105 pyquet-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       51 2023-05-26 12:18:55.000000 pyquet-0.1.8/README.md
--rw-rw-rw-   0        0        0      104 2023-06-11 07:58:49.000000 pyquet-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0      797 2023-06-13 16:39:16.999101 pyquet-0.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 16:39:16.954220 pyquet-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 16:39:16.975164 pyquet-0.1.8/src/pyquet/
--rw-rw-rw-   0        0        0        0 2023-05-26 10:40:59.000000 pyquet-0.1.8/src/pyquet/__init__.py
--rw-rw-rw-   0        0        0      628 2023-06-12 19:39:16.000000 pyquet-0.1.8/src/pyquet/common.py
--rw-rw-rw-   0        0        0     1867 2023-06-11 09:50:23.000000 pyquet-0.1.8/src/pyquet/editor.py
--rw-rw-rw-   0        0        0     3038 2023-06-13 16:38:33.000000 pyquet-0.1.8/src/pyquet/editor_ui.py
--rw-rw-rw-   0        0        0     6685 2023-06-13 15:56:49.000000 pyquet-0.1.8/src/pyquet/generator.py
--rw-rw-rw-   0        0        0     2176 2023-05-27 09:33:39.000000 pyquet-0.1.8/src/pyquet/schemas.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:39:16.992118 pyquet-0.1.8/src/pyquet.egg-info/
--rw-rw-rw-   0        0        0      546 2023-06-13 16:39:16.000000 pyquet-0.1.8/src/pyquet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      404 2023-06-13 16:39:16.000000 pyquet-0.1.8/src/pyquet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 16:39:16.000000 pyquet-0.1.8/src/pyquet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-13 16:39:16.000000 pyquet-0.1.8/src/pyquet.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2023-06-13 16:39:16.000000 pyquet-0.1.8/src/pyquet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-13 16:39:16.000000 pyquet-0.1.8/src/pyquet.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 16:39:16.997105 pyquet-0.1.8/tests/
--rw-rw-rw-   0        0        0     2078 2023-05-27 09:31:42.000000 pyquet-0.1.8/tests/test_reader.py
+drwxrwxrwx   0        0        0        0 2023-07-05 12:52:43.827235 pyquet-0.1.9/
+-rw-rw-rw-   0        0        0     1086 2023-05-26 12:18:55.000000 pyquet-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      546 2023-07-05 12:52:43.828244 pyquet-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2023-05-26 12:18:55.000000 pyquet-0.1.9/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-11 07:58:49.000000 pyquet-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      797 2023-07-05 12:52:43.829229 pyquet-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 12:52:43.770386 pyquet-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-05 12:52:43.804297 pyquet-0.1.9/src/pyquet/
+-rw-rw-rw-   0        0        0        0 2023-05-26 10:40:59.000000 pyquet-0.1.9/src/pyquet/__init__.py
+-rw-rw-rw-   0        0        0      628 2023-06-12 19:39:16.000000 pyquet-0.1.9/src/pyquet/common.py
+-rw-rw-rw-   0        0        0     1867 2023-07-05 12:50:11.000000 pyquet-0.1.9/src/pyquet/editor.py
+-rw-rw-rw-   0        0        0     3038 2023-06-13 16:38:33.000000 pyquet-0.1.9/src/pyquet/editor_ui.py
+-rw-rw-rw-   0        0        0     6795 2023-07-05 12:50:11.000000 pyquet-0.1.9/src/pyquet/generator.py
+-rw-rw-rw-   0        0        0     2176 2023-05-27 09:33:39.000000 pyquet-0.1.9/src/pyquet/schemas.py
+drwxrwxrwx   0        0        0        0 2023-07-05 12:52:43.822248 pyquet-0.1.9/src/pyquet.egg-info/
+-rw-rw-rw-   0        0        0      546 2023-07-05 12:52:43.000000 pyquet-0.1.9/src/pyquet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      404 2023-07-05 12:52:43.000000 pyquet-0.1.9/src/pyquet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 12:52:43.000000 pyquet-0.1.9/src/pyquet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-05 12:52:43.000000 pyquet-0.1.9/src/pyquet.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2023-07-05 12:52:43.000000 pyquet-0.1.9/src/pyquet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-05 12:52:43.000000 pyquet-0.1.9/src/pyquet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 12:52:43.827235 pyquet-0.1.9/tests/
+-rw-rw-rw-   0        0        0     2078 2023-05-27 09:31:42.000000 pyquet-0.1.9/tests/test_reader.py
```

### Comparing `pyquet-0.1.8/LICENSE` & `pyquet-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyquet-0.1.8/PKG-INFO` & `pyquet-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquet
-Version: 0.1.8
+Version: 0.1.9
 Summary: Text comparator UI
 Home-page: https://github.com/rmugicag/pyquet
 Author: Ricardo Mugica
 Author-email: rmugicag@gmail.com
 Project-URL: Bug Tracker, https://github.com/rmugicag/pyquet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyquet-0.1.8/setup.cfg` & `pyquet-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7971 7565 740d 0a76 6572 7369   = pyquet..versi
-00000020: 6f6e 203d 2030 2e31 2e38 0d0a 6175 7468  on = 0.1.8..auth
+00000020: 6f6e 203d 2030 2e31 2e39 0d0a 6175 7468  on = 0.1.9..auth
 00000030: 6f72 203d 2052 6963 6172 646f 204d 7567  or = Ricardo Mug
 00000040: 6963 610d 0a61 7574 686f 725f 656d 6169  ica..author_emai
 00000050: 6c20 3d20 726d 7567 6963 6167 4067 6d61  l = rmugicag@gma
 00000060: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
 00000070: 696f 6e20 3d20 5465 7874 2063 6f6d 7061  ion = Text compa
 00000080: 7261 746f 7220 5549 0d0a 6c6f 6e67 5f64  rator UI..long_d
 00000090: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
```

### Comparing `pyquet-0.1.8/src/pyquet/common.py` & `pyquet-0.1.9/src/pyquet/common.py`

 * *Files identical despite different names*

### Comparing `pyquet-0.1.8/src/pyquet/editor.py` & `pyquet-0.1.9/src/pyquet/editor.py`

 * *Files identical despite different names*

### Comparing `pyquet-0.1.8/src/pyquet/editor_ui.py` & `pyquet-0.1.9/src/pyquet/editor_ui.py`

 * *Files identical despite different names*

### Comparing `pyquet-0.1.8/src/pyquet/generator.py` & `pyquet-0.1.9/src/pyquet/generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,24 @@
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 from . import common
 
 
 class DataGenerator:
-    def __init__(self, catalog_path=None, num_rows=10):
+    def __init__(self, catalog_path=None, num_rows=10, limit_rows=True):
         if catalog_path:
             self.catalog = common.read_json(catalog_path)
-            self.min_rows = len(max(self.catalog.values(), key=lambda x: len(x)))
+            if limit_rows:
+                self.num_rows = len(max(self.catalog.values(), key=lambda x: len(x)))
+            else:
+                self.num_rows = num_rows
         else:
             self.catalog = {}
-            self.min_rows = num_rows
+            self.num_rows = num_rows
 
     def generate_data(self, schema_path, partitions=None, destination_dir="."):
         data = {}
         field_format = []
         schema = common.read_json(schema_path)
         schema_physical_path = os.path.normpath(schema["physicalPath"])
         for field in schema["fields"]:
@@ -68,72 +71,72 @@
             pq.write_to_dataset(table, destination_path, partition_cols=partitions)
         else:
             pq.write_to_dataset(table, destination_path)
         return destination_path
 
     def generate_alphanumeric(self, name, size=1):
         alphanumeric_list = []
-        for counter in range(self.min_rows):
+        for counter in range(self.num_rows):
             if name in self.catalog:
                 value = self.catalog[name][counter % len(self.catalog[name])]
             else:
                 value = "".join(random.choices(string.ascii_letters + string.digits, k=size))
             alphanumeric_list.append(value)
         return alphanumeric_list
 
     def generate_int(self, name, size=1000):
         int_list = []
-        for counter in range(self.min_rows):
+        for counter in range(self.num_rows):
             if name in self.catalog:
                 value = self.catalog[name][counter % len(self.catalog[name])]
             else:
                 value = random.randint(0, size)
             int_list.append(value)
         return int_list
 
     def generate_decimal(self, name, decimal_precision=12, decimal_scale=6):
         decimal_list = []
-        for counter in range(self.min_rows):
+        for counter in range(self.num_rows):
             if name in self.catalog:
                 value = self.catalog[name][counter % len(self.catalog[name])]
             else:
                 value = Decimal(random.randrange(10 ** decimal_precision)) / (10 ** decimal_scale)
             decimal_list.append(value)
         return decimal_list
 
     def generate_date(self, name, date_format='%Y-%m-%d'):
         date_list = []
-        for counter in range(self.min_rows):
+        for counter in range(self.num_rows):
             if name in self.catalog:
                 date = self.catalog[name][counter % len(self.catalog[name])]
             else:
                 date = datetime.today() - timedelta(days=random.randint(0, 365 * 5))
                 date = date.strftime(date_format)
             date_list.append(date)
         date_list = pd.Series(date_list).apply(lambda x: datetime.strptime(x, date_format))
         return date_list
 
     def generate_timestamp(self, name, date_format='%Y-%m-%d %H:%M:%S'):
         timestamp_list = []
-        for counter in range(self.min_rows):
+        for counter in range(self.num_rows):
             if name in self.catalog:
                 date = self.catalog[name][counter % len(self.catalog[name])]
             else:
                 date = datetime.today() - timedelta(days=random.randint(0, 365 * 5),
                                                     hours=random.randint(0, 24),
                                                     minutes=random.randint(0, 60),
                                                     seconds=random.randint(0, 60))
                 date = date.strftime(date_format)
             timestamp_list.append(date)
         timestamp_list = pd.Series(timestamp_list).apply(lambda x: datetime.strptime(x, date_format))
         return timestamp_list
 
     def generate_time(self, name, date_format='%H:%M:%S'):
         time_list = []
-        for counter in range(self.min_rows):
+        for counter in range(self.num_rows):
             if name in self.catalog:
                 date = self.catalog[name][counter % len(self.catalog[name])]
             else:
                 date = datetime.today() - timedelta(hours=random.randint(0, 24),
                                                     minutes=random.randint(0, 60),
                                                     seconds=random.randint(0, 60))
                 date = date.strftime(date_format)
```

### Comparing `pyquet-0.1.8/src/pyquet/schemas.py` & `pyquet-0.1.9/src/pyquet/schemas.py`

 * *Files identical despite different names*

### Comparing `pyquet-0.1.8/src/pyquet.egg-info/PKG-INFO` & `pyquet-0.1.9/src/pyquet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquet
-Version: 0.1.8
+Version: 0.1.9
 Summary: Text comparator UI
 Home-page: https://github.com/rmugicag/pyquet
 Author: Ricardo Mugica
 Author-email: rmugicag@gmail.com
 Project-URL: Bug Tracker, https://github.com/rmugicag/pyquet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyquet-0.1.8/tests/test_reader.py` & `pyquet-0.1.9/tests/test_reader.py`

 * *Files identical despite different names*

