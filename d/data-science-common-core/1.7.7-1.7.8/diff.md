# Comparing `tmp/data-science-common-core-1.7.7.tar.gz` & `tmp/data-science-common-core-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-science-common-core-1.7.7.tar", max compression
+gzip compressed data, was "data-science-common-core-1.7.8.tar", max compression
```

## Comparing `data-science-common-core-1.7.7.tar` & `data-science-common-core-1.7.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       31 2022-08-16 12:51:34.846327 data-science-common-core-1.7.7/common/__init__.py
--rw-r--r--   0        0        0     1772 2023-01-04 09:26:13.978265 data-science-common-core-1.7.7/common/catrf.py
--rw-r--r--   0        0        0     2343 2023-06-06 12:45:28.311456 data-science-common-core-1.7.7/common/constants.py
--rw-r--r--   0        0        0    28618 2022-09-16 13:05:55.366098 data-science-common-core-1.7.7/common/custom_hgb.py
--rw-r--r--   0        0        0    14915 2022-10-06 09:48:34.061975 data-science-common-core-1.7.7/common/custom_multi.py
--rw-r--r--   0        0        0    17492 2023-06-06 11:26:49.982009 data-science-common-core-1.7.7/common/ft.py
--rw-r--r--   0        0        0    12414 2023-06-02 13:30:43.079972 data-science-common-core-1.7.7/common/io.py
--rw-r--r--   0        0        0    27223 2023-06-06 12:45:28.311861 data-science-common-core-1.7.7/common/logic.py
--rw-r--r--   0        0        0    15836 2023-01-04 09:26:13.980885 data-science-common-core-1.7.7/common/model.py
--rw-r--r--   0        0        0     1013 2023-06-02 13:30:43.080198 data-science-common-core-1.7.7/common/pipeline.py
--rw-r--r--   0        0        0    11465 2023-06-02 13:30:43.082632 data-science-common-core-1.7.7/common/plot.py
--rw-r--r--   0        0        0     2100 2022-09-08 15:24:02.191811 data-science-common-core-1.7.7/common/query.py
--rw-r--r--   0        0        0     6947 2023-01-04 09:26:13.981645 data-science-common-core-1.7.7/common/setup.py
--rw-r--r--   0        0        0     2639 2023-06-02 13:30:43.082938 data-science-common-core-1.7.7/common/transformer.py
--rw-r--r--   0        0        0     8736 2022-11-25 15:53:01.257516 data-science-common-core-1.7.7/common/utils.py
--rw-r--r--   0        0        0     1089 2023-06-29 13:14:22.427390 data-science-common-core-1.7.7/pyproject.toml
--rw-r--r--   0        0        0     1350 2023-06-29 13:14:26.935450 data-science-common-core-1.7.7/setup.py
--rw-r--r--   0        0        0     1486 2023-06-29 13:14:26.935620 data-science-common-core-1.7.7/PKG-INFO
+-rw-r--r--   0        0        0       31 2022-08-16 12:51:34.846327 data-science-common-core-1.7.8/common/__init__.py
+-rw-r--r--   0        0        0     1772 2023-01-04 09:26:13.978265 data-science-common-core-1.7.8/common/catrf.py
+-rw-r--r--   0        0        0     2343 2023-06-06 12:45:28.311456 data-science-common-core-1.7.8/common/constants.py
+-rw-r--r--   0        0        0    28618 2022-09-16 13:05:55.366098 data-science-common-core-1.7.8/common/custom_hgb.py
+-rw-r--r--   0        0        0    14915 2022-10-06 09:48:34.061975 data-science-common-core-1.7.8/common/custom_multi.py
+-rw-r--r--   0        0        0    17492 2023-06-06 11:26:49.982009 data-science-common-core-1.7.8/common/ft.py
+-rw-r--r--   0        0        0    12721 2023-07-05 09:32:29.883772 data-science-common-core-1.7.8/common/io.py
+-rw-r--r--   0        0        0    27223 2023-06-06 12:45:28.311861 data-science-common-core-1.7.8/common/logic.py
+-rw-r--r--   0        0        0    15836 2023-01-04 09:26:13.980885 data-science-common-core-1.7.8/common/model.py
+-rw-r--r--   0        0        0     1013 2023-06-02 13:30:43.080198 data-science-common-core-1.7.8/common/pipeline.py
+-rw-r--r--   0        0        0    11465 2023-06-02 13:30:43.082632 data-science-common-core-1.7.8/common/plot.py
+-rw-r--r--   0        0        0     2100 2022-09-08 15:24:02.191811 data-science-common-core-1.7.8/common/query.py
+-rw-r--r--   0        0        0     6947 2023-01-04 09:26:13.981645 data-science-common-core-1.7.8/common/setup.py
+-rw-r--r--   0        0        0     2639 2023-06-02 13:30:43.082938 data-science-common-core-1.7.8/common/transformer.py
+-rw-r--r--   0        0        0     8736 2022-11-25 15:53:01.257516 data-science-common-core-1.7.8/common/utils.py
+-rw-r--r--   0        0        0     1089 2023-07-05 09:32:29.884199 data-science-common-core-1.7.8/pyproject.toml
+-rw-r--r--   0        0        0     1350 2023-07-05 09:33:20.135819 data-science-common-core-1.7.8/setup.py
+-rw-r--r--   0        0        0     1486 2023-07-05 09:33:20.136021 data-science-common-core-1.7.8/PKG-INFO
```

### Comparing `data-science-common-core-1.7.7/common/catrf.py` & `data-science-common-core-1.7.8/common/catrf.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.7/common/constants.py` & `data-science-common-core-1.7.8/common/constants.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.7/common/custom_hgb.py` & `data-science-common-core-1.7.8/common/custom_hgb.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.7/common/custom_multi.py` & `data-science-common-core-1.7.8/common/custom_multi.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.7/common/ft.py` & `data-science-common-core-1.7.8/common/ft.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.7/common/io.py` & `data-science-common-core-1.7.8/common/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -409,7 +409,20 @@
         logger.info("Cached query couldn't found, downloading..")
         df = client.query(query=query, job_config=job_config).to_dataframe(
             progress_bar_type="tqdm"
         )
         with pgzip.open(cache_path, "wb") as f:
             pickle.dump(df, f)
         return df
+
+
+def read_bigquery_schema(params, schema_name, table_name):
+    """Read schema from bigquery table."""
+    # Fetch client
+    client = bigquery.Client()
+
+    # Fetch table info
+    table = client.get_table(
+        f"{params['google_project_id']}.{schema_name}.{table_name}"
+    )
+
+    return table.schema
```

### Comparing `data-science-common-core-1.7.7/common/logic.py` & `data-science-common-core-1.7.8/common/logic.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.7/common/model.py` & `data-science-common-core-1.7.8/common/model.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.7/common/pipeline.py` & `data-science-common-core-1.7.8/common/pipeline.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.7/common/plot.py` & `data-science-common-core-1.7.8/common/plot.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.7/common/query.py` & `data-science-common-core-1.7.8/common/query.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.7/common/setup.py` & `data-science-common-core-1.7.8/common/setup.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.7/common/transformer.py` & `data-science-common-core-1.7.8/common/transformer.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.7/common/utils.py` & `data-science-common-core-1.7.8/common/utils.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.7/pyproject.toml` & `data-science-common-core-1.7.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-science-common-core"
-version = "1.7.7"
+version = "1.7.8"
 description = "Data Science Common Core"
 authors = ["Unsal Gokdag <unsal.gokdag@forto.com>", "Naomi Nguyen <naomi.nguyen@forto.com>", "Kumar Rajendrababu <kumar.rajendrababu@forto.com>", "Reet Kanjilal <reet.kanjilal@forto.com>"]
 packages = [
     { include = "common/*.py"},
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `data-science-common-core-1.7.7/setup.py` & `data-science-common-core-1.7.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
  'toml>=0.10.2,<0.11.0',
  'tomli>=2.0.1,<3.0.0',
  'tqdm>=4.64.0,<5.0.0',
  'webencodings>=0.5.1,<0.6.0']
 
 setup_kwargs = {
     'name': 'data-science-common-core',
-    'version': '1.7.7',
+    'version': '1.7.8',
     'description': 'Data Science Common Core',
     'long_description': None,
     'author': 'Unsal Gokdag',
     'author_email': 'unsal.gokdag@forto.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `data-science-common-core-1.7.7/PKG-INFO` & `data-science-common-core-1.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-science-common-core
-Version: 1.7.7
+Version: 1.7.8
 Summary: Data Science Common Core
 Author: Unsal Gokdag
 Author-email: unsal.gokdag@forto.com
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
```

