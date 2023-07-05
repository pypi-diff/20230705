# Comparing `tmp/summo-0.0.3.tar.gz` & `tmp/summo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "summo-0.0.3.tar", last modified: Mon Jul  3 17:54:40 2023, max compression
+gzip compressed data, was "summo-0.0.4.tar", last modified: Wed Jul  5 03:07:49 2023, max compression
```

## Comparing `summo-0.0.3.tar` & `summo-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:54:40.330558 summo-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-03 17:54:31.000000 summo-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-03 17:54:40.330558 summo-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-03 17:54:31.000000 summo-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-03 17:54:31.000000 summo-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 17:54:40.330558 summo-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:54:40.326558 summo-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:54:40.330558 summo-0.0.3/src/summo/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-03 17:54:31.000000 summo-0.0.3/src/summo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-03 17:54:31.000000 summo-0.0.3/src/summo/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:54:40.330558 summo-0.0.3/src/summo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-03 17:54:40.000000 summo-0.0.3/src/summo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-03 17:54:40.000000 summo-0.0.3/src/summo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 17:54:40.000000 summo-0.0.3/src/summo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-03 17:54:40.000000 summo-0.0.3/src/summo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 17:54:40.000000 summo-0.0.3/src/summo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:54:40.330558 summo-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-03 17:54:31.000000 summo-0.0.3/tests/test_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:07:49.633726 summo-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-05 03:07:39.000000 summo-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-05 03:07:49.633726 summo-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-05 03:07:39.000000 summo-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-05 03:07:39.000000 summo-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 03:07:49.633726 summo-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:07:49.633726 summo-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:07:49.633726 summo-0.0.4/src/summo/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-05 03:07:39.000000 summo-0.0.4/src/summo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-05 03:07:39.000000 summo-0.0.4/src/summo/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:07:49.633726 summo-0.0.4/src/summo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-05 03:07:49.000000 summo-0.0.4/src/summo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-05 03:07:49.000000 summo-0.0.4/src/summo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 03:07:49.000000 summo-0.0.4/src/summo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-05 03:07:49.000000 summo-0.0.4/src/summo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 03:07:49.000000 summo-0.0.4/src/summo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:07:49.633726 summo-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-05 03:07:39.000000 summo-0.0.4/tests/test_summary.py
```

### Comparing `summo-0.0.3/LICENSE` & `summo-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `summo-0.0.3/pyproject.toml` & `summo-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "summo"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 requires-python = ">=3.9"
 readme = "README.md"
 license = { text = "MIT License" }
 authors = [{ name = "Rafael Sanabria", email = "rafael.d.sanabria@gmail.com" }]
 dependencies = ["pandas >= 2.0.0"]
 classifiers = []
```

### Comparing `summo-0.0.3/tests/test_summary.py` & `summo-0.0.4/tests/test_summary.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,44 +9,61 @@
             {
                 "a": [1, 2, 3, 2],
                 "b": [4, 5, 6, 5],
             }
         ),
         {
             "table": {
-                "row_count": 4,
-                "column_count": 2,
+                "rows": 4,
+                "columns": 2,
                 "rows_duplicated": 1,
-                "rows_all_na": 0,
+                "rows_all_na_count": 0,
+                "rows_all_na_pct": 0,
             },
             "columns": {
-                "a": {"na_count": 0},
-                "b": {"na_count": 0},
+                "a": {"na_count": 0, "na_pct": 0, "unique": False, "dtype": "int64"},
+                "b": {"na_count": 0, "na_pct": 0, "unique": False, "dtype": "int64"},
             },
         },
     ),
     (
         pd.DataFrame(
             {
                 "a": [1, 2, None, 2, None],
                 "b": [4, 5, 6, 5, None],
                 "c": ["a", "b", None, "d", None],
             }
         ),
         {
             "table": {
-                "row_count": 5,
-                "column_count": 3,
+                "rows": 5,
+                "columns": 3,
                 "rows_duplicated": 0,
-                "rows_all_na": 1,
+                "rows_all_na_count": 1,
+                "rows_all_na_pct": 1 / 5,
             },
             "columns": {
-                "a": {"na_count": 2},
-                "b": {"na_count": 1},
-                "c": {"na_count": 2},
+                "a": {
+                    "na_count": 2,
+                    "na_pct": 2 / 5,
+                    "unique": False,
+                    "dtype": "float64",
+                },
+                "b": {
+                    "na_count": 1,
+                    "na_pct": 1 / 5,
+                    "unique": False,
+                    "dtype": "float64",
+                },
+                "c": {
+                    "na_count": 2,
+                    "na_pct": 2 / 5,
+                    "unique": False,
+                    "dtype": "object",
+                },
             },
         },
     ),
 ]
 
 
 @pytest.mark.parametrize("df, expected", dataframes)
```

