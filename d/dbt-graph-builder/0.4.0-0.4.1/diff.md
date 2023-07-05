# Comparing `tmp/dbt-graph-builder-0.4.0.tar.gz` & `tmp/dbt-graph-builder-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-graph-builder-0.4.0.tar", last modified: Wed Jul  5 07:57:03 2023, max compression
+gzip compressed data, was "dbt-graph-builder-0.4.1.tar", last modified: Wed Jul  5 12:41:20 2023, max compression
```

## Comparing `dbt-graph-builder-0.4.0.tar` & `dbt-graph-builder-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:57:03.687814 dbt-graph-builder-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-05 07:57:03.687814 dbt-graph-builder-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 07:57:03.687814 dbt-graph-builder-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:57:03.683814 dbt-graph-builder-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:57:03.683814 dbt-graph-builder-0.4.0/src/dbt_graph_builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder/node_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:57:03.687814 dbt-graph-builder-0.4.0/src/dbt_graph_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-05 07:57:03.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-05 07:57:03.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 07:57:03.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 07:57:03.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 07:57:03.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:20.057091 dbt-graph-builder-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-05 12:41:20.057091 dbt-graph-builder-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 12:41:20.061091 dbt-graph-builder-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:20.057091 dbt-graph-builder-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:20.057091 dbt-graph-builder-0.4.1/src/dbt_graph_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder/node_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:20.057091 dbt-graph-builder-0.4.1/src/dbt_graph_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-05 12:41:20.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-05 12:41:20.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 12:41:20.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 12:41:20.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 12:41:20.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder.egg-info/top_level.txt
```

### Comparing `dbt-graph-builder-0.4.0/LICENSE` & `dbt-graph-builder-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.4.0/PKG-INFO` & `dbt-graph-builder-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-graph-builder
-Version: 0.4.0
+Version: 0.4.1
 Summary: DBT Graph Builder
 Author-email: Piotr Tutak <piotr.tutak@getindata.com>
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,19 +25,18 @@
             OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
             SOFTWARE
         
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dbt-graph-builder
 
 [![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-graph-builder)
 [![PyPI Version](https://badge.fury.io/py/dbt-graph-builder.svg)](https://pypi.org/project/dbt-graph-builder/)
```

### Comparing `dbt-graph-builder-0.4.0/README.md` & `dbt-graph-builder-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.4.0/pyproject.toml` & `dbt-graph-builder-0.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,23 +9,22 @@
     {name = "Piotr Tutak", email = "piotr.tutak@getindata.com"},
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 dependencies = [
     "networkx>=2.6,<3",
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 readme = "README.md"
 license = {file = "LICENSE"}
 dynamic = ["version"]
 
 [tool.bandit]
 exclude_dirs = ["build","dist","tests","scripts"]
 number = 4
```

### Comparing `dbt-graph-builder-0.4.0/src/dbt_graph_builder/builder.py` & `dbt-graph-builder-0.4.1/src/dbt_graph_builder/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import json
 import logging
 import os
-from typing import Any, NamedTuple, cast
+from typing import Any, NamedTuple
 
 from dbt_graph_builder.gateway import GatewayConfiguration, TaskGraphConfiguration
 from dbt_graph_builder.graph import DbtManifestGraph
 
 LOGGER = logging.getLogger(__name__)
 
 
@@ -55,15 +55,15 @@
 
     Returns:
         dict[str, Any]: Dbt manifest.
     """
     LOGGER.info("Loading dbt manifest")
     with open(manifest_path) as file:
         manifest_content = json.load(file)
-        return cast(dict[str, Any], manifest_content)
+        return manifest_content  # type: ignore
 
 
 def create_gateway_config(airflow_config: dict[str, Any]) -> GatewayConfiguration:
     """Create gateway config.
 
     Args:
         airflow_config (dict[str, Any]): Airflow config.
```

### Comparing `dbt-graph-builder-0.4.0/src/dbt_graph_builder/gateway.py` & `dbt-graph-builder-0.4.1/src/dbt_graph_builder/gateway.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.4.0/src/dbt_graph_builder/graph.py` & `dbt-graph-builder-0.4.1/src/dbt_graph_builder/graph.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.4.0/src/dbt_graph_builder/utils.py` & `dbt-graph-builder-0.4.1/src/dbt_graph_builder/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.4.0/src/dbt_graph_builder/workflow.py` & `dbt-graph-builder-0.4.1/src/dbt_graph_builder/workflow.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.4.0/src/dbt_graph_builder.egg-info/PKG-INFO` & `dbt-graph-builder-0.4.1/src/dbt_graph_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-graph-builder
-Version: 0.4.0
+Version: 0.4.1
 Summary: DBT Graph Builder
 Author-email: Piotr Tutak <piotr.tutak@getindata.com>
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,19 +25,18 @@
             OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
             SOFTWARE
         
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dbt-graph-builder
 
 [![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-graph-builder)
 [![PyPI Version](https://badge.fury.io/py/dbt-graph-builder.svg)](https://pypi.org/project/dbt-graph-builder/)
```

