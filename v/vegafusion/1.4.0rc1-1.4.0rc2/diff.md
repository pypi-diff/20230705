# Comparing `tmp/vegafusion-1.4.0rc1.tar.gz` & `tmp/vegafusion-1.4.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vegafusion-1.4.0rc1.tar", last modified: Mon Jun 26 19:10:12 2023, max compression
+gzip compressed data, was "vegafusion-1.4.0rc2.tar", last modified: Wed Jul  5 12:36:00 2023, max compression
```

## Comparing `vegafusion-1.4.0rc1.tar` & `vegafusion-1.4.0rc2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:12.565885 vegafusion-1.4.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-26 19:10:12.565885 vegafusion-1.4.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-26 19:10:12.569885 vegafusion-1.4.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:12.565885 vegafusion-1.4.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/tests/test_conext_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/tests/test_input_utc.py
--rw-r--r--   0 runner    (1001) docker     (123)    38103 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/tests/test_pretransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/tests/test_pretransform_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/tests/test_row_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/tests/test_save.py
--rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/tests/test_transformed_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/tests/test_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:12.565885 vegafusion-1.4.0rc1/vegafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/compilers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:12.565885 vegafusion-1.4.0rc1/vegafusion/connection/
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/connection/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/local_tz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-26 19:09:12.000000 vegafusion-1.4.0rc1/vegafusion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:12.565885 vegafusion-1.4.0rc1/vegafusion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-26 19:10:12.000000 vegafusion-1.4.0rc1/vegafusion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-26 19:10:12.000000 vegafusion-1.4.0rc1/vegafusion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:10:12.000000 vegafusion-1.4.0rc1/vegafusion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-26 19:10:12.000000 vegafusion-1.4.0rc1/vegafusion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 19:10:12.000000 vegafusion-1.4.0rc1/vegafusion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:36:00.862041 vegafusion-1.4.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-05 12:36:00.862041 vegafusion-1.4.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-05 12:36:00.862041 vegafusion-1.4.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:36:00.858041 vegafusion-1.4.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/tests/test_conext_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/tests/test_input_utc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43916 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/tests/test_pretransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/tests/test_pretransform_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/tests/test_row_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/tests/test_transformed_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/tests/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:36:00.858041 vegafusion-1.4.0rc2/vegafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/compilers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:36:00.862041 vegafusion-1.4.0rc2/vegafusion/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/connection/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/local_tz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23299 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:36:00.862041 vegafusion-1.4.0rc2/vegafusion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-05 12:36:00.000000 vegafusion-1.4.0rc2/vegafusion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-05 12:36:00.000000 vegafusion-1.4.0rc2/vegafusion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 12:36:00.000000 vegafusion-1.4.0rc2/vegafusion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-05 12:36:00.000000 vegafusion-1.4.0rc2/vegafusion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 12:36:00.000000 vegafusion-1.4.0rc2/vegafusion.egg-info/top_level.txt
```

### Comparing `vegafusion-1.4.0rc1/LICENSE.txt` & `vegafusion-1.4.0rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc1/PKG-INFO` & `vegafusion-1.4.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.4.0rc1
+Version: 1.4.0rc2
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vegafusion-1.4.0rc1/README.md` & `vegafusion-1.4.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc1/setup.cfg` & `vegafusion-1.4.0rc2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [bdist_wheel]
 universal = 0
 
 [metadata]
 name = vegafusion
 description = Core tools for using VegaFusion from Python
-version = 1.4.0-rc1
+version = 1.4.0-rc2
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = vega, altair, vegafusion, arrow
 license = BSD-3-Clause
 license_file = LICENSE.txt
 python = "^3.7"
 homepage = "https://vegafusion.io"
@@ -30,14 +30,14 @@
 	altair>=4.2.0
 	pyarrow>=5
 	pandas
 	psutil
 
 [options.extras_require]
 embed = 
-	vegafusion-python-embed==1.4.0-rc1
+	vegafusion-python-embed==1.4.0-rc2
 	vl-convert-python>=0.7.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `vegafusion-1.4.0rc1/tests/test_conext_manager.py` & `vegafusion-1.4.0rc2/tests/test_conext_manager.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc1/tests/test_input_utc.py` & `vegafusion-1.4.0rc2/tests/test_input_utc.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc1/tests/test_pretransform.py` & `vegafusion-1.4.0rc2/tests/test_pretransform.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 import vegafusion as vf
 import json
 import polars as pl
 from datetime import date
 import decimal
 
 
+def setup_module(module):
+    vf.set_local_tz("UTC")
+
+
 def get_connections():
     connections = ["datafusion"]
     try:
         import duckdb
         connections.append("duckdb")
     except ImportError:
         pass
@@ -986,22 +990,244 @@
       "nice": true,
       "zero": true
     }
   ]
 }
 
 """)
+
+
+def gh_268_hang_spec():
+    return json.loads(r""" 
+    {
+      "$schema": "https://vega.github.io/schema/vega/v5.json",
+      "data": [
+        {
+          "name": "interval_intervalselection__store"
+        },
+        {
+          "name": "legend_pointselection__store"
+        },
+        {
+          "name": "pivot_hover_32f2e9aa_f08a_4fb5_aa8a_ab3f2cc94a1d_store"
+        },
+        {
+          "name": "movies_clean",
+          "url": "vegafusion+dataset://movies_clean"
+        },
+        {
+          "name": "data_0",
+          "source": "movies_clean",
+          "transform": [
+            {
+              "type": "formula",
+              "expr": "toDate(datum[\"Release Date\"])",
+              "as": "Release Date"
+            }
+          ]
+        },
+        {
+          "name": "data_2",
+          "source": "data_0",
+          "transform": [
+            {
+              "field": "Release Date",
+              "type": "timeunit",
+              "units": [
+                "year"
+              ],
+              "as": [
+                "year_Release Date",
+                "year_Release Date_end"
+              ]
+            }
+          ]
+        },
+        {
+          "name": "data_3",
+          "source": "data_2",
+          "transform": [
+            {
+              "type": "filter",
+              "expr": "!length(data(\"interval_intervalselection__store\")) || vlSelectionTest(\"interval_intervalselection__store\", datum)"
+            },
+            {
+              "type": "filter",
+              "expr": "time('1986-11-09T18:28:05.617') <= time(datum[\"year_Release Date\"]) && time(datum[\"year_Release Date\"]) <= time('2001-09-16T22:23:39.144')"
+            },
+            {
+              "type": "filter",
+              "expr": "!length(data(\"legend_pointselection__store\")) || vlSelectionTest(\"legend_pointselection__store\", datum)"
+            }
+          ]
+        }
+      ]
+    }
+    """)
+
+
+def manual_histogram_spec():
+    return json.loads(r"""
+    {
+      "$schema": "https://vega.github.io/schema/vega/v5.json",
+      "background": "white",
+      "padding": 5,
+      "width": 200,
+      "height": 200,
+      "style": "cell",
+      "data": [
+        {
+          "name": "movies",
+          "url": "https://cdn.jsdelivr.net/npm/vega-datasets@v1.29.0/data/movies.json",
+          "format": {"type": "json"},
+          "transform": [
+            {
+              "type": "extent",
+              "field": "IMDB_Rating",
+              "signal": "layer_0_layer_0_bin_maxbins_10_IMDB_Rating_extent"
+            },
+            {
+              "type": "bin",
+              "field": "IMDB_Rating",
+              "as": ["__bin_field_name", "__bin_field_name_end"],
+              "signal": "layer_0_layer_0_bin_maxbins_10_IMDB_Rating_bins",
+              "extent": {
+                "signal": "layer_0_layer_0_bin_maxbins_10_IMDB_Rating_extent"
+              },
+              "maxbins": 10
+            },
+            {
+              "type": "aggregate",
+              "groupby": ["__bin_field_name", "__bin_field_name_end"],
+              "ops": ["count"],
+              "fields": [null],
+              "as": ["__count"]
+            },
+            {
+              "type": "formula",
+              "expr": "'[' + toString(datum[\"__bin_field_name\"]) + ', ' + toString(datum[\"__bin_field_name_end\"]) + ')'",
+              "as": "__bin_range"
+            },
+            {
+              "type": "filter",
+              "expr": "isValid(datum[\"__bin_field_name\"]) && isFinite(+datum[\"__bin_field_name\"]) && isValid(datum[\"__count\"]) && isFinite(+datum[\"__count\"])"
+            }
+          ]
+        }
+      ],
+      "marks": [
+        {
+          "name": "layer_0_layer_0_marks",
+          "type": "rect",
+          "clip": true,
+          "style": ["bar"],
+          "from": {"data": "movies"},
+          "encode": {
+            "update": {
+              "fill": {"value": "#4C78A8"},
+              "opacity": {"value": 1},
+              "ariaRoleDescription": {"value": "bar"},
+              "description": {
+                "signal": "\"IMDB_Rating (start): \" + (format(datum[\"__bin_field_name\"], \"\")) + \"; Count of Records: \" + (format(datum[\"__count\"], \"\")) + \"; __bin_field_name_end: \" + (format(datum[\"__bin_field_name_end\"], \"\"))"
+              },
+              "x": {"scale": "x", "field": "__bin_field_name"},
+              "x2": {"scale": "x", "field": "__bin_field_name_end", "offset": -1},
+              "y": {"scale": "y", "field": "__count"},
+              "y2": {"scale": "y", "value": 0}
+            }
+          }
+        }
+      ],
+      "scales": [
+        {
+          "name": "x",
+          "type": "linear",
+          "domain": {
+            "data": "movies",
+            "fields": ["__bin_field_name", "__bin_field_name_end"]
+          },
+          "range": [0, {"signal": "width"}],
+          "nice": true,
+          "zero": true
+        },
+        {
+          "name": "y",
+          "type": "linear",
+          "domain": {"fields": [{"data": "movies", "field": "__count"}, [0]]},
+          "range": [{"signal": "height"}, 0],
+          "nice": true,
+          "zero": true
+        }
+      ],
+      "axes": [
+        {
+          "scale": "x",
+          "orient": "bottom",
+          "grid": true,
+          "tickCount": 10,
+          "gridScale": "y",
+          "domain": false,
+          "labels": false,
+          "aria": false,
+          "maxExtent": 0,
+          "minExtent": 0,
+          "ticks": false,
+          "zindex": 0
+        },
+        {
+          "scale": "y",
+          "orient": "left",
+          "grid": true,
+          "gridScale": "x",
+          "tickCount": {"signal": "ceil(height/40)"},
+          "domain": false,
+          "labels": false,
+          "aria": false,
+          "maxExtent": 0,
+          "minExtent": 0,
+          "ticks": false,
+          "zindex": 0
+        },
+        {
+          "scale": "x",
+          "orient": "bottom",
+          "grid": false,
+          "title": "IMDB_Rating (start)",
+          "labelFlush": false,
+          "labels": true,
+          "tickCount": 10,
+          "ticks": true,
+          "labelOverlap": true,
+          "zindex": 0
+        },
+        {
+          "scale": "y",
+          "orient": "left",
+          "grid": false,
+          "title": "Count of Records",
+          "labelFlush": false,
+          "labels": true,
+          "ticks": true,
+          "labelOverlap": true,
+          "tickCount": {"signal": "ceil(height/40)"},
+          "zindex": 0
+        }
+      ]
+    }
+    """)
+
+
 def test_pre_transform_multi_partition():
     n = 4050
     order_items = pd.DataFrame({
         "menu_item": [0] * n + [1] * n
     })
 
     vega_spec = order_items_spec()
-    new_spec, warnings = vf.runtime.pre_transform_spec(vega_spec, "UTC", inline_datasets={
+    new_spec, warnings = vf.runtime.pre_transform_spec(vega_spec, inline_datasets={
         "order_items": order_items,
     })
 
     assert new_spec["data"][1] == dict(
         name="data_0",
         values=[
             {"menu_item": 0, "__count": n},
@@ -1014,15 +1240,15 @@
     # Make sure that result changes when input DataFrame changes
     def check(n):
         order_items = pd.DataFrame({
             "menu_item": [0] * n + [1] * n
         })
 
         vega_spec = order_items_spec()
-        new_spec, warnings = vf.runtime.pre_transform_spec(vega_spec, "UTC", inline_datasets={
+        new_spec, warnings = vf.runtime.pre_transform_spec(vega_spec, inline_datasets={
             "order_items": order_items,
         })
 
         assert new_spec["data"][1] == dict(
             name="data_0",
             values=[
                 {"menu_item": 0, "__count": n},
@@ -1040,15 +1266,14 @@
         "menu_item": [0] * n + [1] * (2 * n) + [2] * (3 * n)
     })
 
     vega_spec = order_items_spec()
     datasets, warnings = vf.runtime.pre_transform_datasets(
         vega_spec,
         ["data_0"],
-        "UTC",
         inline_datasets={
             "order_items": order_items,
         }
     )
     assert len(warnings) == 0
     assert len(datasets) == 1
 
@@ -1056,36 +1281,36 @@
     expected = pd.DataFrame({"menu_item": [0, 1, 2], "__count": [n, 2 * n, 3 * n]})
     pd.testing.assert_frame_equal(result, expected)
 
 
 def test_pre_transform_planner_warning1():
     # Pre-transform with supported aggregate function should result in no warnings
     vega_spec = movies_histogram_spec("mean")
-    datasets, warnings = vf.runtime.pre_transform_spec(vega_spec, "UTC")
+    datasets, warnings = vf.runtime.pre_transform_spec(vega_spec)
     assert len(warnings) == 0
 
     # Pre-transform with unsupported aggregate function should result in one warning
     vega_spec = movies_histogram_spec("ci0")
-    datasets, warnings = vf.runtime.pre_transform_spec(vega_spec, "UTC")
+    datasets, warnings = vf.runtime.pre_transform_spec(vega_spec)
     assert len(warnings) == 1
 
     warning = warnings[0]
     assert warning["type"] == "Planner"
     assert "source_0" in warning["message"]
 
 
 def test_pre_transform_planner_warning2():
     # Pre-transform with supported aggregate function should result in no warnings
     vega_spec = standalone_aggregate_spec("mean")
-    datasets, warnings = vf.runtime.pre_transform_spec(vega_spec, "UTC")
+    datasets, warnings = vf.runtime.pre_transform_spec(vega_spec)
     assert len(warnings) == 0
 
     # Pre-transform with unsupported aggregate function should result in one warning
     vega_spec = standalone_aggregate_spec("ci0")
-    datasets, warnings = vf.runtime.pre_transform_spec(vega_spec, "UTC")
+    datasets, warnings = vf.runtime.pre_transform_spec(vega_spec)
     assert len(warnings) == 1
 
     warning = warnings[0]
     assert warning["type"] == "Planner"
     assert "data_0" in warning["message"]
 
 
@@ -1119,28 +1344,27 @@
             "GO_LIVE_MONTH": [date(2021, 1, 1), date(2021, 2, 1)],
             "PERCENT_GO_LIVES": [0.2, 0.3],
         })
 
         datasets, warnings = vf.runtime.pre_transform_datasets(
             vega_spec,
             ["data_1"],
-            "UTC",
             inline_datasets=dict(dataframe=dataframe)
         )
         assert len(warnings) == 0
         assert len(datasets) == 1
         assert len(datasets[0]) == 2
     finally:
         vf.runtime.set_connection("datafusion")
 
 
 def test_period_in_column_name():
     df_period = pd.DataFrame([[1, 2]], columns=['normal', 'a.b'])
     spec = period_in_col_name_spec()
-    datasets, warnings = vf.runtime.pre_transform_datasets(spec, ["data_0"], "UTC", inline_datasets=dict(
+    datasets, warnings = vf.runtime.pre_transform_datasets(spec, ["data_0"], inline_datasets=dict(
         df_period=df_period
     ))
     assert len(warnings) == 0
     assert len(datasets) == 1
 
     dataset = datasets[0]
     assert dataset.to_dict("records") == [{"normal": 1, "a.b": 2}]
@@ -1172,15 +1396,15 @@
          'SALES': 166.72,
          'NULL_TEST': Timestamp('2011-06-01 00:00:00+0000', tz="UTC")},
         {'ORDER_DATE': date(2011, 6, 1), 'SALES': 25.92, 'NULL_TEST': NaT}
     ])
 
     spec = nat_bar_spec()
 
-    datasets, warnings = vf.runtime.pre_transform_datasets(spec, ["dataframe"], "UTC", inline_datasets=dict(
+    datasets, warnings = vf.runtime.pre_transform_datasets(spec, ["dataframe"], inline_datasets=dict(
         dataframe=dataframe
     ))
     assert len(warnings) == 0
     assert len(datasets) == 1
 
     dataset = datasets[0]
     assert dataset.to_dict("records")[0] == {
@@ -1204,15 +1428,14 @@
         "menu_item": [0] * n + [1] * (2 * n) + [2] * (3 * n)
     })
 
     vega_spec = order_items_spec()
     datasets, warnings = vf.runtime.pre_transform_datasets(
         vega_spec,
         ["data_0"],
-        "UTC",
         inline_datasets={
             "order_items": order_items,
         }
     )
     assert len(warnings) == 0
     assert len(datasets) == 1
 
@@ -1242,15 +1465,14 @@
         vf.runtime.set_connection(conn)
 
         # order_items includes a table://order_items data url
         vega_spec = order_items_spec()
         datasets, warnings = vf.runtime.pre_transform_datasets(
             vega_spec,
             ["data_0"],
-            "UTC",
         )
         assert len(warnings) == 0
         assert len(datasets) == 1
 
         result = datasets[0]
         expected = pd.DataFrame({"menu_item": [0, 1, 2], "__count": [n, 2 * n, 3 * n]})
         pd.testing.assert_frame_equal(result, expected)
@@ -1279,15 +1501,14 @@
         vf.runtime.set_connection(conn)
 
         # order_items includes a table://order_items data url
         vega_spec = order_items_spec()
         datasets, warnings = vf.runtime.pre_transform_datasets(
             vega_spec,
             ["data_0"],
-            "UTC",
         )
         assert len(warnings) == 0
         assert len(datasets) == 1
 
         result = datasets[0]
         expected = pd.DataFrame({
             "menu_item": [decimal.Decimal(0), decimal.Decimal(1), decimal.Decimal(2)],
@@ -1327,26 +1548,26 @@
     """
     vf.runtime.set_connection("datafusion")
     movies = pd.read_json("https://raw.githubusercontent.com/vega/vega-datasets/main/data/movies.json")
     spec = gh_268_hang_spec()
     for i in range(20):
         # Break cache by removing one row each iteration
         movies_inner = movies.iloc[i:]
-        vf.runtime.pre_transform_datasets(spec, ["data_3"], "UTC", inline_datasets=dict(movies_clean=movies_inner))
+        vf.runtime.pre_transform_datasets(spec, ["data_3"], inline_datasets=dict(movies_clean=movies_inner))
 
 
 def test_repeat_duckdb():
     """
     Tests for hang reported in https://github.com/hex-inc/vegafusion/issues/268
     """
     vf.runtime.set_connection("duckdb")
     movies = pd.read_json("https://raw.githubusercontent.com/vega/vega-datasets/main/data/movies.json")
     spec = gh_268_hang_spec()
     for i in range(2):
-        vf.runtime.pre_transform_datasets(spec, ["data_3"], "UTC", inline_datasets=dict(movies_clean=movies))
+        vf.runtime.pre_transform_datasets(spec, ["data_3"], inline_datasets=dict(movies_clean=movies))
 
 
 @pytest.mark.parametrize("connection", get_connections())
 def test_pivot_mixed_case(connection):
     vf.runtime.set_connection(connection)
     source_0 = pd.DataFrame.from_records([
         {"country": "Norway", "type": "gold", "count": 14},
@@ -1380,80 +1601,45 @@
       ]
     }
   ]
 }   
     """)
 
     datasets, warnings = vf.runtime.pre_transform_datasets(
-        spec, ["data_0"], "UTC", inline_datasets=dict(source_0=source_0)
+        spec, ["data_0"], inline_datasets=dict(source_0=source_0)
     )
 
     assert set(datasets[0].columns.tolist()) == {"gold", "Gold", "silver", "bronze", "country"}
 
 
-def gh_268_hang_spec():
-    return json.loads(r""" 
-    {
-      "$schema": "https://vega.github.io/schema/vega/v5.json",
-      "data": [
-        {
-          "name": "interval_intervalselection__store"
-        },
-        {
-          "name": "legend_pointselection__store"
-        },
-        {
-          "name": "pivot_hover_32f2e9aa_f08a_4fb5_aa8a_ab3f2cc94a1d_store"
-        },
-        {
-          "name": "movies_clean",
-          "url": "vegafusion+dataset://movies_clean"
-        },
-        {
-          "name": "data_0",
-          "source": "movies_clean",
-          "transform": [
-            {
-              "type": "formula",
-              "expr": "toDate(datum[\"Release Date\"])",
-              "as": "Release Date"
-            }
-          ]
-        },
-        {
-          "name": "data_2",
-          "source": "data_0",
-          "transform": [
-            {
-              "field": "Release Date",
-              "type": "timeunit",
-              "units": [
-                "year"
-              ],
-              "as": [
-                "year_Release Date",
-                "year_Release Date_end"
-              ]
-            }
-          ]
-        },
-        {
-          "name": "data_3",
-          "source": "data_2",
-          "transform": [
-            {
-              "type": "filter",
-              "expr": "!length(data(\"interval_intervalselection__store\")) || vlSelectionTest(\"interval_intervalselection__store\", datum)"
-            },
-            {
-              "type": "filter",
-              "expr": "time('1986-11-09T18:28:05.617') <= time(datum[\"year_Release Date\"]) && time(datum[\"year_Release Date\"]) <= time('2001-09-16T22:23:39.144')"
-            },
-            {
-              "type": "filter",
-              "expr": "!length(data(\"legend_pointselection__store\")) || vlSelectionTest(\"legend_pointselection__store\", datum)"
-            }
-          ]
-        }
-      ]
-    }
-    """)
+def test_keep_signals():
+    spec = manual_histogram_spec()
+
+    # pre-transform without keep_signals. No signals should be present in pre-transformed spec
+    tx_spec, warnings = vf.runtime.pre_transform_spec(spec)
+    assert len(tx_spec.get("signals", [])) == 0
+
+    # Specify single keep_signal as a string
+    tx_spec, warnings = vf.runtime.pre_transform_spec(
+        spec,
+        keep_signals="layer_0_layer_0_bin_maxbins_10_IMDB_Rating_bins"
+    )
+    assert len(tx_spec.get("signals", [])) == 1
+    sig0 = tx_spec["signals"][0]
+    assert sig0["name"] == "layer_0_layer_0_bin_maxbins_10_IMDB_Rating_bins"
+    assert sig0["value"]["step"] == 1.0
+
+    # Specify multiple keep_signals as a list
+    tx_spec, warnings = vf.runtime.pre_transform_spec(
+        spec,
+        keep_signals=[
+            "layer_0_layer_0_bin_maxbins_10_IMDB_Rating_bins",
+            ("layer_0_layer_0_bin_maxbins_10_IMDB_Rating_extent", [])
+        ]
+    )
+    assert len(tx_spec.get("signals", [])) == 2
+    sig0 = tx_spec["signals"][0]
+    sig1 = tx_spec["signals"][1]
+    [sig0, sig1] = sorted([sig0, sig1], key=lambda v: v["name"])
+    assert sig0["name"] == "layer_0_layer_0_bin_maxbins_10_IMDB_Rating_bins"
+    assert sig1["name"] == "layer_0_layer_0_bin_maxbins_10_IMDB_Rating_extent"
+    assert sig1["value"] == [1.4, 9.2]
```

### Comparing `vegafusion-1.4.0rc1/tests/test_pretransform_specs.py` & `vegafusion-1.4.0rc2/tests/test_pretransform_specs.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc1/tests/test_row_limit.py` & `vegafusion-1.4.0rc2/tests/test_row_limit.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc1/tests/test_save.py` & `vegafusion-1.4.0rc2/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc1/tests/test_transformed_data.py` & `vegafusion-1.4.0rc2/tests/test_transformed_data.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc1/tests/test_transformer.py` & `vegafusion-1.4.0rc2/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc1/vegafusion/__init__.py` & `vegafusion-1.4.0rc2/vegafusion/__init__.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc1/vegafusion/compilers.py` & `vegafusion-1.4.0rc2/vegafusion/compilers.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc1/vegafusion/connection/__init__.py` & `vegafusion-1.4.0rc2/vegafusion/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc1/vegafusion/connection/duckdb.py` & `vegafusion-1.4.0rc2/vegafusion/connection/duckdb.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc1/vegafusion/evaluation.py` & `vegafusion-1.4.0rc2/vegafusion/evaluation.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc1/vegafusion/local_tz.py` & `vegafusion-1.4.0rc2/vegafusion/local_tz.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc1/vegafusion/renderer.py` & `vegafusion-1.4.0rc2/vegafusion/renderer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc1/vegafusion/runtime.py` & `vegafusion-1.4.0rc2/vegafusion/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import pandas as pd
 import psutil
 import pyarrow as pa
 from typing import Union
 from .connection import SqlConnection
 from .transformer import import_pyarrow_interchange, to_arrow_table
+from .local_tz import get_local_tz
 
 try:
     from duckdb import DuckDBPyConnection
 except ImportError:
     DuckDBPyConnection = None
 
 try:
@@ -168,42 +169,54 @@
                 raise ValueError(f"Unsupported DataFrame type: {type(value)}")
 
         return inline_arrow_datasets
 
     def pre_transform_spec(
         self,
         spec,
-        local_tz,
+        local_tz=None,
         default_input_tz=None,
         row_limit=None,
         preserve_interactivity=True,
-        inline_datasets=None
+        inline_datasets=None,
+        keep_signals=None,
+        keep_datasets=None,
     ):
         """
         Evaluate supported transforms in an input Vega specification and produce a new
         specification with pre-transformed datasets included inline.
 
         :param spec: A Vega specification dict or JSON string
         :param local_tz: Name of timezone to be considered local. E.g. 'America/New_York'.
-            This can be computed for the local system using the tzlocal package and the
-            tzlocal.get_localzone_name() function.
+            Defaults to the value of vf.get_local_tz(), which defaults to the system timezone
+            if one can be determined.
         :param default_input_tz: Name of timezone (e.g. 'America/New_York') that naive datetime
             strings should be interpreted in. Defaults to `local_tz`.
         :param row_limit: Maximum number of dataset rows to include in the returned
             specification. If exceeded, datasets will be truncated to this number of rows
             and a RowLimitExceeded warning will be included in the resulting warnings list
         :param preserve_interactivity: If True (default) then the interactive behavior of
             the chart will pre preserved. This requires that all the data that participates
             in interactions be included in the resulting spec rather than being pre-transformed.
             If False, then all possible data transformations are applied even if they break
             the original interactive behavior of the chart.
         :param inline_datasets: A dict from dataset names to pandas DataFrames or pyarrow
             Tables. Inline datasets may be referenced by the input specification using
             the following url syntax 'vegafusion+dataset://{dataset_name}' or
             'table://{dataset_name}'.
+        :param keep_signals: Signals from the input spec that must be included in the
+            pre-transformed spec. A list with elements that are either:
+              - The name of a top-level signal as a string
+              - A two-element tuple where the first element is the name of a signal as a string
+                and the second element is the nested scope of the dataset as a list of integers
+        :param keep_datasets: Datasets from the input spec that must be included in the
+            pre-transformed spec. A list with elements that are either:
+              - The name of a top-level dataset as a string
+              - A two-element tuple where the first element is the name of a dataset as a string
+                and the second element is the nested scope of the dataset as a list of integers
         :return:
             Two-element tuple:
                 0. A string containing the JSON representation of a Vega specification
                    with pre-transformed datasets included inline
                 1. A list of warnings as dictionaries. Each warning dict has a 'type'
                    key indicating the warning type, and a 'message' key containing
                    a description of the warning. Potential warning types include:
@@ -213,44 +226,59 @@
                         broken in the resulting Vega specification
                     'Unsupported': No transforms in the provided Vega specification were
                         eligible for pre-transforming
         """
         if self._grpc_channel:
             raise ValueError("pre_transform_spec not yet supported over gRPC")
         else:
+            local_tz = local_tz or get_local_tz()
             inline_arrow_dataset = self._arrowify_or_register_inline_datasets(inline_datasets)
+
+            # Parse input keep signals and datasets
+            keep_signals = parse_variables(keep_signals)
+            keep_datasets = parse_variables(keep_datasets)
             try:
                 new_spec, warnings = self.embedded_runtime.pre_transform_spec(
                     spec,
                     local_tz=local_tz,
                     default_input_tz=default_input_tz,
                     row_limit=row_limit,
                     preserve_interactivity=preserve_interactivity,
-                    inline_datasets=inline_arrow_dataset
+                    inline_datasets=inline_arrow_dataset,
+                    keep_signals=keep_signals,
+                    keep_datasets=keep_datasets,
                 )
             finally:
                 # Clean up temporary tables
                 if self._connection is not None:
                     self._connection.unregister_temporary_tables()
 
             return new_spec, warnings
 
-    def pre_transform_datasets(self, spec, datasets, local_tz, default_input_tz=None, row_limit=None, inline_datasets=None):
+    def pre_transform_datasets(
+        self,
+        spec,
+        datasets,
+        local_tz=None,
+        default_input_tz=None,
+        row_limit=None,
+        inline_datasets=None
+    ):
         """
         Extract the fully evaluated form of the requested datasets from a Vega specification
         as pandas DataFrames.
 
         :param spec: A Vega specification dict or JSON string
         :param datasets: A list with elements that are either:
           - The name of a top-level dataset as a string
           - A two-element tuple where the first element is the name of a dataset as a string
             and the second element is the nested scope of the dataset as a list of integers
         :param local_tz: Name of timezone to be considered local. E.g. 'America/New_York'.
-            This can be computed for the local system using the tzlocal package and the
-            tzlocal.get_localzone_name() function.
+            Defaults to the value of vf.get_local_tz(), which defaults to the system timezone
+            if one can be determined.
         :param default_input_tz: Name of timezone (e.g. 'America/New_York') that naive datetime
             strings should be interpreted in. Defaults to `local_tz`.
         :param row_limit: Maximum number of dataset rows to include in the returned
             datasets. If exceeded, datasets will be truncated to this number of rows
             and a RowLimitExceeded warning will be included in the resulting warnings list
         :param inline_datasets: A dict from dataset names to pandas DataFrames or pyarrow
             Tables. Inline datasets may be referenced by the input specification using
@@ -262,28 +290,18 @@
                 1. A list of warnings as dictionaries. Each warning dict has a 'type'
                    key indicating the warning type, and a 'message' key containing
                    a description of the warning.
         """
         if self._grpc_channel:
             raise ValueError("pre_transform_datasets not yet supported over gRPC")
         else:
+            local_tz = local_tz or get_local_tz()
 
             # Build input variables
-            pre_tx_vars = []
-            err_msg = "Elements of variables argument must be strings are two-element tuples"
-            for var in datasets:
-                if isinstance(var, str):
-                    pre_tx_vars.append((var, []))
-                elif isinstance(var, (list, tuple)):
-                    if len(var) == 2:
-                        pre_tx_vars.append(tuple(var))
-                    else:
-                        raise ValueError(err_msg)
-                else:
-                    raise ValueError(err_msg)
+            pre_tx_vars = parse_variables(datasets)
 
             # Serialize inline datasets
             inline_arrow_dataset = self._arrowify_or_register_inline_datasets(inline_datasets)
             try:
                 values, warnings = self.embedded_runtime.pre_transform_datasets(
                     spec,
                     pre_tx_vars,
@@ -321,30 +339,30 @@
                     for name, dtype in df.dtypes.items():
                         if dtype.kind == "M":
                             df[name] = df[name].dt.tz_localize("UTC").dt.tz_convert(local_tz)
 
                 return datasets, warnings
 
     def pre_transform_extract(
-            self,
-            spec,
-            local_tz,
-            default_input_tz=None,
-            preserve_interactivity=True,
-            inline_datasets=None
+        self,
+        spec,
+        local_tz=None,
+        default_input_tz=None,
+        preserve_interactivity=True,
+        inline_datasets=None
     ):
         """
         Evaluate supported transforms in an input Vega specification and produce a new
         specification with small pre-transformed datasets (under 100 rows) included inline
         and larger inline datasets (100 rows or more) are extracted into pyarrow tables.
 
         :param spec: A Vega specification dict or JSON string
         :param local_tz: Name of timezone to be considered local. E.g. 'America/New_York'.
-            This can be computed for the local system using the tzlocal package and the
-            tzlocal.get_localzone_name() function.
+            Defaults to the value of vf.get_local_tz(), which defaults to the system timezone
+            if one can be determined.
         :param default_input_tz: Name of timezone (e.g. 'America/New_York') that naive datetime
             strings should be interpreted in. Defaults to `local_tz`.
         :param preserve_interactivity: If True (default) then the interactive behavior of
             the chart will pre preserved. This requires that all the data that participates
             in interactions be included in the resulting spec rather than being pre-transformed.
             If False, then all possible data transformations are applied even if they break
             the original interactive behavior of the chart.
@@ -364,14 +382,16 @@
                    key indicating the warning type, and a 'message' key containing
                    a description of the warning. Potential warning types include:
                     'Planner': Planner warning
         """
         if self._grpc_channel:
             raise ValueError("pre_transform_spec not yet supported over gRPC")
         else:
+            local_tz = local_tz or get_local_tz()
+
             inline_arrow_dataset = self._arrowify_or_register_inline_datasets(inline_datasets)
             try:
                 new_spec, datasets, warnings = self.embedded_runtime.pre_transform_extract(
                     spec,
                     local_tz=local_tz,
                     default_input_tz=default_input_tz,
                     preserve_interactivity=preserve_interactivity,
@@ -494,8 +514,31 @@
             return (
                 f"VegaFusionRuntime("
                 f"cache_capacity={self.cache_capacity}, worker_threads={self.worker_threads}"
                 f")"
             )
 
 
+def parse_variables(variables):
+    # Build input variables
+    pre_tx_vars = []
+    if variables is None:
+        return []
+
+    if isinstance(variables, str):
+        variables = [variables]
+
+    err_msg = "Elements of variables argument must be strings are two-element tuples"
+    for var in variables:
+        if isinstance(var, str):
+            pre_tx_vars.append((var, []))
+        elif isinstance(var, (list, tuple)):
+            if len(var) == 2:
+                pre_tx_vars.append(tuple(var))
+            else:
+                raise ValueError(err_msg)
+        else:
+            raise ValueError(err_msg)
+    return pre_tx_vars
+
+
 runtime = VegaFusionRuntime(64, psutil.virtual_memory().total // 2, psutil.cpu_count())
```

### Comparing `vegafusion-1.4.0rc1/vegafusion/save.py` & `vegafusion-1.4.0rc2/vegafusion/save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc1/vegafusion/transformer.py` & `vegafusion-1.4.0rc2/vegafusion/transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc1/vegafusion/utils.py` & `vegafusion-1.4.0rc2/vegafusion/utils.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc1/vegafusion.egg-info/PKG-INFO` & `vegafusion-1.4.0rc2/vegafusion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.4.0rc1
+Version: 1.4.0rc2
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vegafusion-1.4.0rc1/vegafusion.egg-info/SOURCES.txt` & `vegafusion-1.4.0rc2/vegafusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

