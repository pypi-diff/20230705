# Comparing `tmp/dyno_viewer-0.1.2.tar.gz` & `tmp/dyno_viewer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyno_viewer-0.1.2.tar", max compression
+gzip compressed data, was "dyno_viewer-0.1.3.tar", max compression
```

## Comparing `dyno_viewer-0.1.2.tar` & `dyno_viewer-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1067 2023-06-12 00:03:14.308979 dyno_viewer-0.1.2/LICENSE
--rw-r--r--   0        0        0     3909 2023-06-12 00:03:14.308979 dyno_viewer-0.1.2/README.md
--rw-r--r--   0        0        0       58 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/__main__.py
--rw-r--r--   0        0        0     5875 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/app.py
--rw-r--r--   0        0        0     2256 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/app_workers.py
--rw-r--r--   0        0        0     7792 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/aws/ddb.py
--rw-r--r--   0        0        0      211 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/aws/session.py
--rw-r--r--   0        0        0      612 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/css/query.css
--rw-r--r--   0        0        0       38 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/css/table.css
--rw-r--r--   0        0        0     2233 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/query/filter_query.py
--rw-r--r--   0        0        0     2850 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/query/key_query.py
--rw-r--r--   0        0        0     2057 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/query/sort_key_filter.py
--rw-r--r--   0        0        0      129 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/screens/__init__.py
--rw-r--r--   0        0        0      794 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/screens/error.py
--rw-r--r--   0        0        0      912 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/screens/profile_select.py
--rw-r--r--   0        0        0     5129 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/screens/query.py
--rw-r--r--   0        0        0      857 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/screens/region_select.py
--rw-r--r--   0        0        0     3323 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/screens/table_select.py
--rw-r--r--   0        0        0     1852 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/table.py
--rw-r--r--   0        0        0      181 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/types.py
--rw-r--r--   0        0        0       20 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/util/__init__.py
--rw-r--r--   0        0        0      166 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/util/util.py
--rw-r--r--   0        0        0     1119 2023-06-12 00:03:14.316980 dyno_viewer-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4468 1970-01-01 00:00:00.000000 dyno_viewer-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-05 09:14:13.407367 dyno_viewer-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3909 2023-07-05 09:14:13.411367 dyno_viewer-0.1.3/README.md
+-rw-r--r--   0        0        0       58 2023-07-05 09:14:13.411367 dyno_viewer-0.1.3/dyno_viewer/__main__.py
+-rw-r--r--   0        0        0     5923 2023-07-05 09:14:13.411367 dyno_viewer-0.1.3/dyno_viewer/app.py
+-rw-r--r--   0        0        0     2256 2023-07-05 09:14:13.411367 dyno_viewer-0.1.3/dyno_viewer/app_workers.py
+-rw-r--r--   0        0        0     7792 2023-07-05 09:14:13.411367 dyno_viewer-0.1.3/dyno_viewer/aws/ddb.py
+-rw-r--r--   0        0        0      211 2023-07-05 09:14:13.411367 dyno_viewer-0.1.3/dyno_viewer/aws/session.py
+-rw-r--r--   0        0        0      612 2023-07-05 09:14:13.411367 dyno_viewer-0.1.3/dyno_viewer/components/css/query.css
+-rw-r--r--   0        0        0       56 2023-07-05 09:14:13.411367 dyno_viewer-0.1.3/dyno_viewer/components/css/table.css
+-rw-r--r--   0        0        0     2233 2023-07-05 09:14:13.411367 dyno_viewer-0.1.3/dyno_viewer/components/query/filter_query.py
+-rw-r--r--   0        0        0     2850 2023-07-05 09:14:13.411367 dyno_viewer-0.1.3/dyno_viewer/components/query/key_query.py
+-rw-r--r--   0        0        0     2057 2023-07-05 09:14:13.411367 dyno_viewer-0.1.3/dyno_viewer/components/query/sort_key_filter.py
+-rw-r--r--   0        0        0      129 2023-07-05 09:14:13.411367 dyno_viewer-0.1.3/dyno_viewer/components/screens/__init__.py
+-rw-r--r--   0        0        0      794 2023-07-05 09:14:13.411367 dyno_viewer-0.1.3/dyno_viewer/components/screens/error.py
+-rw-r--r--   0        0        0      912 2023-07-05 09:14:13.411367 dyno_viewer-0.1.3/dyno_viewer/components/screens/profile_select.py
+-rw-r--r--   0        0        0     5129 2023-07-05 09:14:13.411367 dyno_viewer-0.1.3/dyno_viewer/components/screens/query.py
+-rw-r--r--   0        0        0      857 2023-07-05 09:14:13.411367 dyno_viewer-0.1.3/dyno_viewer/components/screens/region_select.py
+-rw-r--r--   0        0        0     3323 2023-07-05 09:14:13.411367 dyno_viewer-0.1.3/dyno_viewer/components/screens/table_select.py
+-rw-r--r--   0        0        0     2184 2023-07-05 09:14:13.411367 dyno_viewer-0.1.3/dyno_viewer/components/table.py
+-rw-r--r--   0        0        0      181 2023-07-05 09:14:13.411367 dyno_viewer-0.1.3/dyno_viewer/components/types.py
+-rw-r--r--   0        0        0       20 2023-07-05 09:14:13.411367 dyno_viewer-0.1.3/dyno_viewer/util/__init__.py
+-rw-r--r--   0        0        0      166 2023-07-05 09:14:13.411367 dyno_viewer-0.1.3/dyno_viewer/util/util.py
+-rw-r--r--   0        0        0     1083 2023-07-05 09:14:13.415367 dyno_viewer-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4468 1970-01-01 00:00:00.000000 dyno_viewer-0.1.3/PKG-INFO
```

### Comparing `dyno_viewer-0.1.2/LICENSE` & `dyno_viewer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.2/README.md` & `dyno_viewer-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.2/dyno_viewer/app.py` & `dyno_viewer-0.1.3/dyno_viewer/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,16 @@
 
     @on(DataDynTable.CellHighlighted)
     async def paginate_dyn_data(
         self, highlighted: DataDynTable.CellHighlighted
     ) -> None:
         if highlighted.coordinate.row == highlighted.data_table.row_count - 1:
             if "ExclusiveStartKey" in self.dyn_query_params:
+                log.info("adding more items")
+
                 dyn_table_query(self, self.dyn_query_params, update_existing=True)
 
     async def on_region_select_screen_region_selected(
         self, selected_region: RegionSelectScreen.RegionSelected
     ) -> None:
         self.aws_region = selected_region.region
         self.dyn_client = get_ddb_client(selected_region.region, self.aws_profile)
@@ -119,15 +121,15 @@
         )
         self.update_table_client()
 
     async def on_query_screen_run_query(self, run_query: QueryScreen.RunQuery) -> None:
         params = {"KeyConditionExpression": run_query.key_cond_exp}
         if run_query.filter_cond_exp:
             params["FilterExpression"] = run_query.filter_cond_exp
-        self.dyn_table_query = params
+        self.dyn_query_params = params
         dyn_table_query(self, params)
 
     async def on_update_dyn_data_table(self, update_data: UpdateDynDataTable) -> None:
         table = self.query_one(DataDynTable)
         if update_data.update_existing_data:
             table.add_dyn_data_existing(update_data.data)
             self.set_pagination_token(update_data.next_token)
```

### Comparing `dyno_viewer-0.1.2/dyno_viewer/app_workers.py` & `dyno_viewer-0.1.3/dyno_viewer/app_workers.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.2/dyno_viewer/aws/ddb.py` & `dyno_viewer-0.1.3/dyno_viewer/aws/ddb.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.2/dyno_viewer/components/css/query.css` & `dyno_viewer-0.1.3/dyno_viewer/components/css/query.css`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.2/dyno_viewer/components/query/filter_query.py` & `dyno_viewer-0.1.3/dyno_viewer/components/query/filter_query.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.2/dyno_viewer/components/query/key_query.py` & `dyno_viewer-0.1.3/dyno_viewer/components/query/key_query.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.2/dyno_viewer/components/query/sort_key_filter.py` & `dyno_viewer-0.1.3/dyno_viewer/components/query/sort_key_filter.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.2/dyno_viewer/components/screens/error.py` & `dyno_viewer-0.1.3/dyno_viewer/components/screens/error.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.2/dyno_viewer/components/screens/profile_select.py` & `dyno_viewer-0.1.3/dyno_viewer/components/screens/profile_select.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.2/dyno_viewer/components/screens/query.py` & `dyno_viewer-0.1.3/dyno_viewer/components/screens/query.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.2/dyno_viewer/components/screens/region_select.py` & `dyno_viewer-0.1.3/dyno_viewer/components/screens/region_select.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.2/dyno_viewer/components/screens/table_select.py` & `dyno_viewer-0.1.3/dyno_viewer/components/screens/table_select.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.2/dyno_viewer/components/table.py` & `dyno_viewer-0.1.3/dyno_viewer/components/table.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,28 +28,41 @@
 
         log.info(f"{len(cols)} total cols")
 
         self.clear(columns=True)
         for col in cols:
             self.add_column(col, key=col)
 
-        log.info("col keys=", [str() for col in self.columns.keys()])
+        log.info("col keys=", [str(col.label) for col in self.columns.values()])
 
         rows = [[item.get(col) for col in cols] for item in data]
         log.info(f"{len(rows)} total rows")
         self.add_rows(rows)
 
     def add_dyn_data_existing(self, data: list[dict]) -> None:
         """
         add more data to table that has already been setup with dynamodb table data
         """
         if self.row_count == 0:
             raise Exception("there must be existing data")
 
-        cols_not_exist = [
-            attrKey for item in data for attrKey in item if attrKey not in self.columns
-        ]
+        cols_not_exist = set(
+            [
+                attrKey
+                for item in data
+                for attrKey in item
+                if attrKey not in self.columns
+            ]
+        )
+
         if cols_not_exist:
-            for col in cols_not_exist:
+            log.info(f"adding cols to existing: {cols_not_exist}")
+            for col in list(cols_not_exist):
                 self.add_column(col, key=col)
-        rows = [[item.get(col) for col in self.columns.keys()] for item in data]
+
+
+            log.info(f"added cols to existing: {cols_not_exist}")
+
+        rows = [[item.get(col.value) for col in self.columns.keys()] for item in data]
+        log.info(f"adding rows to existing")
         self.add_rows(rows)
+        log.info(f"added rows to existing")
```

### Comparing `dyno_viewer-0.1.2/pyproject.toml` & `dyno_viewer-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [tool.poetry]
 name = "dyno-viewer"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Rowan Self <piesrule123@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dyno_viewer"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 boto3 = "^1.26.135"
 simplejson = "^3.19.1"
 dynamodb-json = "^1.3"
-textual = ">=0.24.1,<0.28.0"
+textual = ">=0.24.1,<0.30.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ipykernel = "^6.22.0"
-textual = {extras = ["dev"], version = ">=0.24.1,<0.28.0"}
 pytest = "^7.3.1"
 moto = {extras = ["all"], version = "^4.1.9"}
 pytest-aiohttp = "^1.0.4"
 pandas = "^1.5.3"
 pytest-mock = "^3.10.0"
 jupyterlab = "^3.6.3"
 pytest-xdist = "^3.3.0"
 toml = "^0.10.2"
 pyinstaller = {version = "^5.11.0", python = ">=3.9,<3.12"}
 poethepoet = "^0.20.0"
+textual-dev = "^1.0.1"
 
 
 
 [tool.poetry.group.build.dependencies]
 
 [tool.poe.tasks]
 build_local.script = 'scripts.commands:build_local'
```

### Comparing `dyno_viewer-0.1.2/PKG-INFO` & `dyno_viewer-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: dyno-viewer
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Rowan Self
 Author-email: piesrule123@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.135,<2.0.0)
 Requires-Dist: dynamodb-json (>=1.3,<2.0)
 Requires-Dist: simplejson (>=3.19.1,<4.0.0)
-Requires-Dist: textual (>=0.24.1,<0.28.0)
+Requires-Dist: textual (>=0.24.1,<0.30.0)
 Description-Content-Type: text/markdown
 
 ![screenshot](dyno-viewer-screenshot.png)
 # Dyno-viewer
 
 Dyno-viewer is dynamodb table viewer for your terminal build using [textual](https://github.com/Textualize/textual).
```

