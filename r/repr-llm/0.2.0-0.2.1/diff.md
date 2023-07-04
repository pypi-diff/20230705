# Comparing `tmp/repr_llm-0.2.0.tar.gz` & `tmp/repr_llm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repr_llm-0.2.0.tar", max compression
+gzip compressed data, was "repr_llm-0.2.1.tar", max compression
```

## Comparing `repr_llm-0.2.0.tar` & `repr_llm-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1498 2023-06-27 14:04:13.699866 repr_llm-0.2.0/LICENSE
--rw-r--r--   0        0        0     5870 2023-06-28 15:45:00.920457 repr_llm-0.2.0/README.md
--rw-r--r--   0        0        0     1435 2023-06-28 23:42:53.709051 repr_llm-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      262 2023-06-28 23:42:45.338098 repr_llm-0.2.0/repr_llm/__init__.py
--rw-r--r--   0        0        0     1577 2023-06-27 19:25:09.505379 repr_llm-0.2.0/repr_llm/display.py
--rw-r--r--   0        0        0     1462 2023-06-27 17:26:37.423267 repr_llm-0.2.0/repr_llm/formatter.py
--rw-r--r--   0        0        0     5752 2023-06-27 19:25:09.505789 repr_llm-0.2.0/repr_llm/pandas.py
--rw-r--r--   0        0        0     6752 1970-01-01 00:00:00.000000 repr_llm-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1498 2023-06-27 14:04:13.699866 repr_llm-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5877 2023-07-04 22:44:52.356068 repr_llm-0.2.1/README.md
+-rw-r--r--   0        0        0     1435 2023-07-04 22:47:29.748753 repr_llm-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      262 2023-07-04 22:47:41.241035 repr_llm-0.2.1/repr_llm/__init__.py
+-rw-r--r--   0        0        0     1577 2023-06-27 19:25:09.505379 repr_llm-0.2.1/repr_llm/display.py
+-rw-r--r--   0        0        0     1462 2023-06-27 17:26:37.423267 repr_llm-0.2.1/repr_llm/formatter.py
+-rw-r--r--   0        0        0     6070 2023-07-04 22:47:11.578350 repr_llm-0.2.1/repr_llm/pandas.py
+-rw-r--r--   0        0        0     6759 1970-01-01 00:00:00.000000 repr_llm-0.2.1/PKG-INFO
```

### Comparing `repr_llm-0.2.0/LICENSE` & `repr_llm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `repr_llm-0.2.0/README.md` & `repr_llm-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # repr-llm
 
 <img src="https://github.com/rgbkrk/repr_llm/assets/836375/f1b8b252-7e70-4897-bfbf-e87d48bb46bd" height="64px" />
 
-Create lightweight representations of objects for Large Language Model consumption
+Create lightweight representations of Python objects for Large Language Model consumption
 
 ## Background
 
 In Python, we have a way to represent our objects within interpreters: `repr`.
 
 In IPython, it goes even further. We can register rich represenations of plots, tables, and all kinds of objects. As an example, developers can augment their objects with a `_repr_html_` method to expose a rich HTML version of their object. The most common example most Pythonistas know about is showing tables for their data inside notebooks via `pandas`.
```

### Comparing `repr_llm-0.2.0/pyproject.toml` & `repr_llm-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "repr-llm"
-version = "0.2.0"
+version = "0.2.1"
 description = "Creating lightweight representations of objects for Large Language Model consumption"
 authors = ["Kyle Kelley <rgbkrk@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 packages = [{include = "repr_llm"}]
 
 [tool.poetry.dependencies]
```

### Comparing `repr_llm-0.2.0/repr_llm/display.py` & `repr_llm-0.2.1/repr_llm/display.py`

 * *Files identical despite different names*

### Comparing `repr_llm-0.2.0/repr_llm/formatter.py` & `repr_llm-0.2.1/repr_llm/formatter.py`

 * *Files identical despite different names*

### Comparing `repr_llm-0.2.0/repr_llm/pandas.py` & `repr_llm-0.2.1/repr_llm/pandas.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,17 +48,23 @@
 
     if has_categoricals:
         categorical_describe = df.describe(include=['category', 'datetime', 'timedelta'])
         categorical_summary = categorical_describe.T.reset_index().rename(columns={'index': 'Column Name'})
     else:
         categorical_summary = pd.DataFrame(columns=['Column Name'])
 
-    sample_columns = min(sample_columns, df.shape[1])
+    # Ignore any columns that do not have `:@computed_region` in the name, which are derived data not useful for
+    # summarization of sample data
+    filtered_columns = [col for col in df.columns if ":@computed_region" not in col]
+
+    # adjust sample size with filtered dataframe shape
+    sample_columns = min(sample_columns, len(filtered_columns))
     sample_rows = min(sample_rows, df.shape[0])
-    sampled = df.sample(sample_columns, axis=1).sample(sample_rows, axis=0)
+
+    sampled = df[filtered_columns].sample(sample_columns, axis=1).sample(sample_rows, axis=0)
 
     tablefmt = "github"
 
     # create the markdown string for output
     output = (
         f"## Dataframe Summary\n\n"
         f"Number of Rows: {num_rows:,}\n\n"
```

### Comparing `repr_llm-0.2.0/PKG-INFO` & `repr_llm-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repr-llm
-Version: 0.2.0
+Version: 0.2.1
 Summary: Creating lightweight representations of objects for Large Language Model consumption
 License: BSD-3-Clause
 Author: Kyle Kelley
 Author-email: rgbkrk@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 Requires-Dist: tabulate[numfocus] (>=0.8.3,<0.10.0) ; extra == "dev"
 Description-Content-Type: text/markdown
 
 # repr-llm
 
 <img src="https://github.com/rgbkrk/repr_llm/assets/836375/f1b8b252-7e70-4897-bfbf-e87d48bb46bd" height="64px" />
 
-Create lightweight representations of objects for Large Language Model consumption
+Create lightweight representations of Python objects for Large Language Model consumption
 
 ## Background
 
 In Python, we have a way to represent our objects within interpreters: `repr`.
 
 In IPython, it goes even further. We can register rich represenations of plots, tables, and all kinds of objects. As an example, developers can augment their objects with a `_repr_html_` method to expose a rich HTML version of their object. The most common example most Pythonistas know about is showing tables for their data inside notebooks via `pandas`.
```

