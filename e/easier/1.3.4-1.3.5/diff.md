# Comparing `tmp/easier-1.3.4.tar.gz` & `tmp/easier-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easier-1.3.4.tar", last modified: Mon Jul  3 14:17:21 2023, max compression
+gzip compressed data, was "easier-1.3.5.tar", last modified: Wed Jul  5 18:37:37 2023, max compression
```

## Comparing `easier-1.3.4.tar` & `easier-1.3.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-07-03 14:17:21.675921 easier-1.3.4/
--rw-rw-r--   0 rob        (501) staff       (20)       39 2017-12-14 15:28:52.000000 easier-1.3.4/CONTRIBUTORS.txt
--rw-rw-r--   0 rob        (501) staff       (20)     1081 2017-12-14 15:28:52.000000 easier-1.3.4/LICENSE
--rw-rw-r--   0 rob        (501) staff       (20)       73 2017-12-14 15:28:52.000000 easier-1.3.4/MANIFEST.in
--rw-rw-r--   0 rob        (501) staff       (20)      448 2023-07-03 14:17:21.675978 easier-1.3.4/PKG-INFO
--rw-rw-r--   0 rob        (501) staff       (20)    12815 2019-12-20 21:04:42.000000 easier-1.3.4/README.md
-drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-07-03 14:17:21.674384 easier-1.3.4/easier/
--rw-rw-r--   0 rob        (501) staff       (20)      685 2022-08-17 21:35:50.000000 easier-1.3.4/easier/__init__.py
--rw-rw-r--   0 rob        (501) staff       (20)     5869 2023-07-03 14:15:05.000000 easier-1.3.4/easier/api.py
--rw-rw-r--   0 rob        (501) staff       (20)    10490 2022-09-21 18:47:14.000000 easier-1.3.4/easier/bernstein.py
--rw-rw-r--   0 rob        (501) staff       (20)    15283 2021-08-04 15:44:52.000000 easier-1.3.4/easier/bigquery.py
--rw-rw-r--   0 rob        (501) staff       (20)     1449 2021-01-14 22:38:24.000000 easier-1.3.4/easier/cli.py
--rw-rw-r--   0 rob        (501) staff       (20)     4453 2019-12-12 19:11:35.000000 easier-1.3.4/easier/clock.py
--rw-rw-r--   0 rob        (501) staff       (20)     2118 2020-05-29 19:14:34.000000 easier-1.3.4/easier/crypt.py
--rw-rw-r--   0 rob        (501) staff       (20)    11273 2023-07-03 14:16:23.000000 easier-1.3.4/easier/dataframe_tools.py
--rw-rw-r--   0 rob        (501) staff       (20)     4416 2021-10-25 19:35:54.000000 easier-1.3.4/easier/distributions.py
--rw-rw-r--   0 rob        (501) staff       (20)     3729 2022-11-06 22:52:50.000000 easier-1.3.4/easier/duck.py
--rw-rw-r--   0 rob        (501) staff       (20)     6934 2023-01-04 21:20:27.000000 easier-1.3.4/easier/duck_model.py
--rw-rw-r--   0 rob        (501) staff       (20)     1312 2022-12-27 18:28:43.000000 easier-1.3.4/easier/ecdf_lib.py
-drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-07-03 14:17:21.675814 easier-1.3.4/easier/filtering/
--rw-rw-r--   0 rob        (501) staff       (20)       89 2021-09-24 01:20:15.000000 easier-1.3.4/easier/filtering/__init__.py
--rw-rw-r--   0 rob        (501) staff       (20)     5693 2021-09-24 01:20:25.000000 easier-1.3.4/easier/filtering/elliptic_filter.py
--rw-rw-r--   0 rob        (501) staff       (20)     2106 2021-11-24 17:03:48.000000 easier-1.3.4/easier/filtering/tvd.py
--rw-rw-r--   0 rob        (501) staff       (20)    14061 2022-08-17 21:35:50.000000 easier-1.3.4/easier/fit_lib.py
--rw-rw-r--   0 rob        (501) staff       (20)     8505 2021-01-14 20:54:34.000000 easier-1.3.4/easier/gsheet.py
--rw-rw-r--   0 rob        (501) staff       (20)     7770 2022-08-16 22:01:30.000000 easier-1.3.4/easier/hvtools.py
--rw-rw-r--   0 rob        (501) staff       (20)     3749 2023-07-01 21:46:38.000000 easier-1.3.4/easier/ibis_tools.py
--rw-rw-r--   0 rob        (501) staff       (20)     1794 2020-03-27 15:13:42.000000 easier-1.3.4/easier/item.py
--rw-rw-r--   0 rob        (501) staff       (20)     2136 2020-05-29 19:14:34.000000 easier-1.3.4/easier/iterify.py
--rw-rw-r--   0 rob        (501) staff       (20)      208 2020-05-29 19:14:34.000000 easier-1.3.4/easier/memory.py
--rw-rw-r--   0 rob        (501) staff       (20)    11444 2022-11-07 18:39:22.000000 easier-1.3.4/easier/minimodel.py
--rw-rw-r--   0 rob        (501) staff       (20)     8148 2022-08-11 18:33:31.000000 easier-1.3.4/easier/minimodel_orig.py
--rw-rw-r--   0 rob        (501) staff       (20)     4950 2021-12-08 22:15:51.000000 easier-1.3.4/easier/nice_dates.py
--rw-rw-r--   0 rob        (501) staff       (20)     2087 2020-05-29 19:14:34.000000 easier-1.3.4/easier/outlier_tools.py
--rw-rw-r--   0 rob        (501) staff       (20)     3186 2022-08-17 21:35:50.000000 easier-1.3.4/easier/parallel.py
--rw-rw-r--   0 rob        (501) staff       (20)     7743 2019-12-12 19:22:12.000000 easier-1.3.4/easier/param_state.py
--rw-rw-r--   0 rob        (501) staff       (20)     1195 2022-08-17 21:35:50.000000 easier-1.3.4/easier/plotting.py
--rw-rw-r--   0 rob        (501) staff       (20)     9482 2022-12-11 17:05:42.000000 easier-1.3.4/easier/postgres.py
--rw-rw-r--   0 rob        (501) staff       (20)      663 2018-08-08 19:33:34.000000 easier-1.3.4/easier/print_catcher.py
--rw-rw-r--   0 rob        (501) staff       (20)     6150 2022-11-10 16:40:03.000000 easier-1.3.4/easier/proportion_lib.py
--rw-rw-r--   0 rob        (501) staff       (20)     3178 2022-09-23 20:00:52.000000 easier-1.3.4/easier/salesforce.py
--rw-rw-r--   0 rob        (501) staff       (20)     3231 2020-05-29 19:14:34.000000 easier-1.3.4/easier/shaper.py
--rw-rw-r--   0 rob        (501) staff       (20)     2902 2019-12-12 19:11:38.000000 easier-1.3.4/easier/timer.py
--rw-rw-r--   0 rob        (501) staff       (20)    19244 2023-01-03 20:00:58.000000 easier-1.3.4/easier/utils.py
--rw-rw-r--   0 rob        (501) staff       (20)       22 2023-07-03 14:15:05.000000 easier-1.3.4/easier/version.py
-drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-07-03 14:17:21.675430 easier-1.3.4/easier.egg-info/
--rw-r--r--   0 rob        (501) staff       (20)      448 2023-07-03 14:17:21.000000 easier-1.3.4/easier.egg-info/PKG-INFO
--rw-r--r--   0 rob        (501) staff       (20)     1018 2023-07-03 14:17:21.000000 easier-1.3.4/easier.egg-info/SOURCES.txt
--rw-r--r--   0 rob        (501) staff       (20)        1 2023-07-03 14:17:21.000000 easier-1.3.4/easier.egg-info/dependency_links.txt
--rw-r--r--   0 rob        (501) staff       (20)      117 2023-07-03 14:17:21.000000 easier-1.3.4/easier.egg-info/entry_points.txt
--rw-r--r--   0 rob        (501) staff       (20)        1 2023-01-04 21:15:28.000000 easier-1.3.4/easier.egg-info/not-zip-safe
--rw-r--r--   0 rob        (501) staff       (20)       36 2023-07-03 14:17:21.000000 easier-1.3.4/easier.egg-info/requires.txt
--rw-r--r--   0 rob        (501) staff       (20)        7 2023-07-03 14:17:21.000000 easier-1.3.4/easier.egg-info/top_level.txt
--rw-rw-r--   0 rob        (501) staff       (20)      504 2023-07-03 14:17:21.676221 easier-1.3.4/setup.cfg
--rw-rw-r--   0 rob        (501) staff       (20)     1638 2021-01-14 22:24:18.000000 easier-1.3.4/setup.py
+drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-07-05 18:37:37.105710 easier-1.3.5/
+-rw-rw-r--   0 rob        (501) staff       (20)       39 2017-12-14 15:28:52.000000 easier-1.3.5/CONTRIBUTORS.txt
+-rw-rw-r--   0 rob        (501) staff       (20)     1081 2017-12-14 15:28:52.000000 easier-1.3.5/LICENSE
+-rw-rw-r--   0 rob        (501) staff       (20)       73 2017-12-14 15:28:52.000000 easier-1.3.5/MANIFEST.in
+-rw-rw-r--   0 rob        (501) staff       (20)      448 2023-07-05 18:37:37.105757 easier-1.3.5/PKG-INFO
+-rw-rw-r--   0 rob        (501) staff       (20)    12815 2019-12-20 21:04:42.000000 easier-1.3.5/README.md
+drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-07-05 18:37:37.104152 easier-1.3.5/easier/
+-rw-rw-r--   0 rob        (501) staff       (20)      685 2022-08-17 21:35:50.000000 easier-1.3.5/easier/__init__.py
+-rw-rw-r--   0 rob        (501) staff       (20)     5869 2023-07-03 14:15:05.000000 easier-1.3.5/easier/api.py
+-rw-rw-r--   0 rob        (501) staff       (20)    10490 2022-09-21 18:47:14.000000 easier-1.3.5/easier/bernstein.py
+-rw-rw-r--   0 rob        (501) staff       (20)    15283 2021-08-04 15:44:52.000000 easier-1.3.5/easier/bigquery.py
+-rw-rw-r--   0 rob        (501) staff       (20)     1449 2021-01-14 22:38:24.000000 easier-1.3.5/easier/cli.py
+-rw-rw-r--   0 rob        (501) staff       (20)     4453 2019-12-12 19:11:35.000000 easier-1.3.5/easier/clock.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2118 2020-05-29 19:14:34.000000 easier-1.3.5/easier/crypt.py
+-rw-rw-r--   0 rob        (501) staff       (20)    11828 2023-07-04 18:30:46.000000 easier-1.3.5/easier/dataframe_tools.py
+-rw-rw-r--   0 rob        (501) staff       (20)     4416 2021-10-25 19:35:54.000000 easier-1.3.5/easier/distributions.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3729 2022-11-06 22:52:50.000000 easier-1.3.5/easier/duck.py
+-rw-rw-r--   0 rob        (501) staff       (20)     6934 2023-01-04 21:20:27.000000 easier-1.3.5/easier/duck_model.py
+-rw-rw-r--   0 rob        (501) staff       (20)     1312 2022-12-27 18:28:43.000000 easier-1.3.5/easier/ecdf_lib.py
+drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-07-05 18:37:37.105524 easier-1.3.5/easier/filtering/
+-rw-rw-r--   0 rob        (501) staff       (20)       89 2021-09-24 01:20:15.000000 easier-1.3.5/easier/filtering/__init__.py
+-rw-rw-r--   0 rob        (501) staff       (20)     5693 2021-09-24 01:20:25.000000 easier-1.3.5/easier/filtering/elliptic_filter.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2106 2021-11-24 17:03:48.000000 easier-1.3.5/easier/filtering/tvd.py
+-rw-rw-r--   0 rob        (501) staff       (20)    14061 2022-08-17 21:35:50.000000 easier-1.3.5/easier/fit_lib.py
+-rw-rw-r--   0 rob        (501) staff       (20)     8505 2021-01-14 20:54:34.000000 easier-1.3.5/easier/gsheet.py
+-rw-rw-r--   0 rob        (501) staff       (20)     7770 2022-08-16 22:01:30.000000 easier-1.3.5/easier/hvtools.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3749 2023-07-01 21:46:38.000000 easier-1.3.5/easier/ibis_tools.py
+-rw-rw-r--   0 rob        (501) staff       (20)     1794 2020-03-27 15:13:42.000000 easier-1.3.5/easier/item.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2136 2020-05-29 19:14:34.000000 easier-1.3.5/easier/iterify.py
+-rw-rw-r--   0 rob        (501) staff       (20)      208 2020-05-29 19:14:34.000000 easier-1.3.5/easier/memory.py
+-rw-rw-r--   0 rob        (501) staff       (20)    11444 2022-11-07 18:39:22.000000 easier-1.3.5/easier/minimodel.py
+-rw-rw-r--   0 rob        (501) staff       (20)     8148 2022-08-11 18:33:31.000000 easier-1.3.5/easier/minimodel_orig.py
+-rw-rw-r--   0 rob        (501) staff       (20)     4950 2021-12-08 22:15:51.000000 easier-1.3.5/easier/nice_dates.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2087 2020-05-29 19:14:34.000000 easier-1.3.5/easier/outlier_tools.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3186 2022-08-17 21:35:50.000000 easier-1.3.5/easier/parallel.py
+-rw-rw-r--   0 rob        (501) staff       (20)     7743 2019-12-12 19:22:12.000000 easier-1.3.5/easier/param_state.py
+-rw-rw-r--   0 rob        (501) staff       (20)     1195 2022-08-17 21:35:50.000000 easier-1.3.5/easier/plotting.py
+-rw-rw-r--   0 rob        (501) staff       (20)     9482 2022-12-11 17:05:42.000000 easier-1.3.5/easier/postgres.py
+-rw-rw-r--   0 rob        (501) staff       (20)      663 2018-08-08 19:33:34.000000 easier-1.3.5/easier/print_catcher.py
+-rw-rw-r--   0 rob        (501) staff       (20)     6150 2022-11-10 16:40:03.000000 easier-1.3.5/easier/proportion_lib.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3178 2022-09-23 20:00:52.000000 easier-1.3.5/easier/salesforce.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3231 2020-05-29 19:14:34.000000 easier-1.3.5/easier/shaper.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2902 2019-12-12 19:11:38.000000 easier-1.3.5/easier/timer.py
+-rw-rw-r--   0 rob        (501) staff       (20)    19244 2023-01-03 20:00:58.000000 easier-1.3.5/easier/utils.py
+-rw-rw-r--   0 rob        (501) staff       (20)       22 2023-07-05 18:36:50.000000 easier-1.3.5/easier/version.py
+drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-07-05 18:37:37.104997 easier-1.3.5/easier.egg-info/
+-rw-r--r--   0 rob        (501) staff       (20)      448 2023-07-05 18:37:37.000000 easier-1.3.5/easier.egg-info/PKG-INFO
+-rw-r--r--   0 rob        (501) staff       (20)     1018 2023-07-05 18:37:37.000000 easier-1.3.5/easier.egg-info/SOURCES.txt
+-rw-r--r--   0 rob        (501) staff       (20)        1 2023-07-05 18:37:37.000000 easier-1.3.5/easier.egg-info/dependency_links.txt
+-rw-r--r--   0 rob        (501) staff       (20)      117 2023-07-05 18:37:37.000000 easier-1.3.5/easier.egg-info/entry_points.txt
+-rw-r--r--   0 rob        (501) staff       (20)        1 2023-01-04 21:15:28.000000 easier-1.3.5/easier.egg-info/not-zip-safe
+-rw-r--r--   0 rob        (501) staff       (20)       36 2023-07-05 18:37:37.000000 easier-1.3.5/easier.egg-info/requires.txt
+-rw-r--r--   0 rob        (501) staff       (20)        7 2023-07-05 18:37:37.000000 easier-1.3.5/easier.egg-info/top_level.txt
+-rw-rw-r--   0 rob        (501) staff       (20)      504 2023-07-05 18:37:37.105990 easier-1.3.5/setup.cfg
+-rw-rw-r--   0 rob        (501) staff       (20)     1638 2021-01-14 22:24:18.000000 easier-1.3.5/setup.py
```

### Comparing `easier-1.3.4/LICENSE` & `easier-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/README.md` & `easier-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/__init__.py` & `easier-1.3.5/easier/__init__.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/api.py` & `easier-1.3.5/easier/api.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/bernstein.py` & `easier-1.3.5/easier/bernstein.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/bigquery.py` & `easier-1.3.5/easier/bigquery.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/cli.py` & `easier-1.3.5/easier/cli.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/clock.py` & `easier-1.3.5/easier/clock.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/crypt.py` & `easier-1.3.5/easier/crypt.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/dataframe_tools.py` & `easier-1.3.5/easier/dataframe_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -322,14 +322,33 @@
                 # Otherwise, assume it is a type and coerce it to a nullable column
                 else:
                     typed_cols[key] = pa.Column(val, nullable=True)
 
             # Create the Pandera DataFrameSchema object and assign it to the schema attribute
             self.schema = pa.DataFrameSchema(typed_cols, **kwargs)
 
+        @property
+        def ibis_schema(self):
+            from ibis.expr import schema as sch
+
+            return sch.schema_from_mapping(
+                {
+                    col: self.schema.dtypes[col].type
+                    for col in self.schema.columns.keys()
+                }
+            )
+
+        def __repr__(self):
+            s = repr(self.schema).replace("DataFrameSchema", "QuickSchema")
+            return s
+
+        def __str__(self):
+            s = str(self.schema).replace("DataFrameSchema", "QuickSchema")
+            return s
+
         def apply(self, df):
             """
             Apply the schema to retrieve a new dataframe
             """
             if self.ordered:
                 df = df[list(self.col_spec.keys())]
             df = df.copy()
```

### Comparing `easier-1.3.4/easier/distributions.py` & `easier-1.3.5/easier/distributions.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/duck.py` & `easier-1.3.5/easier/duck.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/duck_model.py` & `easier-1.3.5/easier/duck_model.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/ecdf_lib.py` & `easier-1.3.5/easier/ecdf_lib.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/filtering/elliptic_filter.py` & `easier-1.3.5/easier/filtering/elliptic_filter.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/filtering/tvd.py` & `easier-1.3.5/easier/filtering/tvd.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/fit_lib.py` & `easier-1.3.5/easier/fit_lib.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/gsheet.py` & `easier-1.3.5/easier/gsheet.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/hvtools.py` & `easier-1.3.5/easier/hvtools.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/ibis_tools.py` & `easier-1.3.5/easier/ibis_tools.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/item.py` & `easier-1.3.5/easier/item.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/iterify.py` & `easier-1.3.5/easier/iterify.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/minimodel.py` & `easier-1.3.5/easier/minimodel.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/minimodel_orig.py` & `easier-1.3.5/easier/minimodel_orig.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/nice_dates.py` & `easier-1.3.5/easier/nice_dates.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/outlier_tools.py` & `easier-1.3.5/easier/outlier_tools.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/parallel.py` & `easier-1.3.5/easier/parallel.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/param_state.py` & `easier-1.3.5/easier/param_state.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/plotting.py` & `easier-1.3.5/easier/plotting.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/postgres.py` & `easier-1.3.5/easier/postgres.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/print_catcher.py` & `easier-1.3.5/easier/print_catcher.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/proportion_lib.py` & `easier-1.3.5/easier/proportion_lib.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/salesforce.py` & `easier-1.3.5/easier/salesforce.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/shaper.py` & `easier-1.3.5/easier/shaper.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/timer.py` & `easier-1.3.5/easier/timer.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier/utils.py` & `easier-1.3.5/easier/utils.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/easier.egg-info/SOURCES.txt` & `easier-1.3.5/easier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easier-1.3.4/setup.py` & `easier-1.3.5/setup.py`

 * *Files identical despite different names*

