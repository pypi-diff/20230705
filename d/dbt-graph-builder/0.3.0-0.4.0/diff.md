# Comparing `tmp/dbt-graph-builder-0.3.0.tar.gz` & `tmp/dbt-graph-builder-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-graph-builder-0.3.0.tar", last modified: Thu Jun 29 07:30:14 2023, max compression
+gzip compressed data, was "dbt-graph-builder-0.4.0.tar", last modified: Wed Jul  5 07:57:03 2023, max compression
```

## Comparing `dbt-graph-builder-0.3.0.tar` & `dbt-graph-builder-0.4.0.tar`

### file list

```diff
@@ -1,27 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:30:14.746375 dbt-graph-builder-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-06-29 07:30:14.746375 dbt-graph-builder-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 07:30:14.746375 dbt-graph-builder-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:30:14.742375 dbt-graph-builder-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:30:14.746375 dbt-graph-builder-0.3.0/src/dbt_graph_builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder/node_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:30:14.746375 dbt-graph-builder-0.3.0/src/dbt_graph_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-06-29 07:30:14.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-29 07:30:14.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:30:14.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 07:30:14.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 07:30:14.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:30:14.746375 dbt-graph-builder-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/tests/test_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/tests/test_graph_dag_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     9677 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/tests/test_graph_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/tests/test_graph_ephemeral_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:57:03.687814 dbt-graph-builder-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-05 07:57:03.687814 dbt-graph-builder-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 07:57:03.687814 dbt-graph-builder-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:57:03.683814 dbt-graph-builder-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:57:03.683814 dbt-graph-builder-0.4.0/src/dbt_graph_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder/node_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-05 07:56:47.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:57:03.687814 dbt-graph-builder-0.4.0/src/dbt_graph_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-05 07:57:03.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-05 07:57:03.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 07:57:03.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 07:57:03.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 07:57:03.000000 dbt-graph-builder-0.4.0/src/dbt_graph_builder.egg-info/top_level.txt
```

### Comparing `dbt-graph-builder-0.3.0/LICENSE` & `dbt-graph-builder-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.3.0/PKG-INFO` & `dbt-graph-builder-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-graph-builder
-Version: 0.3.0
+Version: 0.4.0
 Summary: DBT Graph Builder
 Author-email: Piotr Tutak <piotr.tutak@getindata.com>
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,33 +38,36 @@
 License-File: LICENSE
 
 # dbt-graph-builder
 
 [![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-graph-builder)
 [![PyPI Version](https://badge.fury.io/py/dbt-graph-builder.svg)](https://pypi.org/project/dbt-graph-builder/)
 [![Downloads](https://pepy.tech/badge/dbt-graph-builder)](https://pepy.tech/project/dbt-graph-builder)
+
+## Overview
+This library provides a set of tools for building a graph of dbt models and their dependencies. It can be used to create an Airflow DAG for dbt models
+or to create a graph of dbt models and their dependencies in a format that can be used by other tools like GCP Workflows.
+
 ## Project Organization
 
 - .devcontainer - This directory contains required files for creating a [Codespace](https://github.com/features/codespaces).
 - .github
   - workflows - Contains GitHub Actions used for building, testing and publishing.
-    - publish-test.yml - Publish wheels to [https://test.pypi.org/](https://test.pypi.org/)
+    - prepare-release.yml - Contains steps to prepare a release.
     - publish.yml - Publish wheels to [https://pypi.org/](https://pypi.org/)
-    - pull-request.yml - Build and Test pull requests before commiting to main.
+    - test-linting.yml - Build and Test pull requests before commiting to main.
     - template-sync.yml - Update GitHub Repo with enhancments to base template
 - docs - collect documents (default format .md)
 - src - place new source code here
   - python_package - sample package (this can be deleted when creating a new repository)
 - tests - contains Python based test cases to validation src code
 - .pre-commit-config.yaml - Contains various pre-check fixes for Python
-- .templateversionrc - used to track template version usage.
 - MANIFEST.in - Declares additional files to include in Python whl
 - pyproject.toml - Python Project Declaration
-- ws.code-workspace - Recommended configurations for [Visual Studio Code](https://code.visualstudio.com/)
-
+- README.md - This file
 
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.
```

### Comparing `dbt-graph-builder-0.3.0/README.md` & `dbt-graph-builder-0.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # dbt-graph-builder
 
 [![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-graph-builder)
 [![PyPI Version](https://badge.fury.io/py/dbt-graph-builder.svg)](https://pypi.org/project/dbt-graph-builder/)
 [![Downloads](https://pepy.tech/badge/dbt-graph-builder)](https://pepy.tech/project/dbt-graph-builder)
+
+## Overview
+This library provides a set of tools for building a graph of dbt models and their dependencies. It can be used to create an Airflow DAG for dbt models
+or to create a graph of dbt models and their dependencies in a format that can be used by other tools like GCP Workflows.
+
 ## Project Organization
 
 - .devcontainer - This directory contains required files for creating a [Codespace](https://github.com/features/codespaces).
 - .github
   - workflows - Contains GitHub Actions used for building, testing and publishing.
-    - publish-test.yml - Publish wheels to [https://test.pypi.org/](https://test.pypi.org/)
+    - prepare-release.yml - Contains steps to prepare a release.
     - publish.yml - Publish wheels to [https://pypi.org/](https://pypi.org/)
-    - pull-request.yml - Build and Test pull requests before commiting to main.
+    - test-linting.yml - Build and Test pull requests before commiting to main.
     - template-sync.yml - Update GitHub Repo with enhancments to base template
 - docs - collect documents (default format .md)
 - src - place new source code here
   - python_package - sample package (this can be deleted when creating a new repository)
 - tests - contains Python based test cases to validation src code
 - .pre-commit-config.yaml - Contains various pre-check fixes for Python
-- .templateversionrc - used to track template version usage.
 - MANIFEST.in - Declares additional files to include in Python whl
 - pyproject.toml - Python Project Declaration
-- ws.code-workspace - Recommended configurations for [Visual Studio Code](https://code.visualstudio.com/)
-
+- README.md - This file
 
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.
```

### Comparing `dbt-graph-builder-0.3.0/pyproject.toml` & `dbt-graph-builder-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.3.0/src/dbt_graph_builder/builder.py` & `dbt-graph-builder-0.4.0/src/dbt_graph_builder/builder.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.3.0/src/dbt_graph_builder/gateway.py` & `dbt-graph-builder-0.4.0/src/dbt_graph_builder/gateway.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.3.0/src/dbt_graph_builder/graph.py` & `dbt-graph-builder-0.4.0/src/dbt_graph_builder/graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,23 @@
 
         Args:
             configuration (TaskGraphConfiguration): _description_
         """
         self._graph = nx.DiGraph()
         self._configuration = configuration
 
+    @property
+    def graph(self) -> nx.DiGraph:
+        """Get graph.
+
+        Returns:
+            nx.DiGraph: Graph.
+        """
+        return self._graph
+
     def add_execution_tasks(self, manifest: dict[str, Any]) -> None:
         """Add execution tasks.
 
         Args:
             manifest (dict): DBT manifest.
         """
         self._add_gateway_execution_tasks(manifest=manifest)
@@ -54,15 +63,15 @@
                 is_test_task(node_name)
                 and len(self._get_model_dependencies_from_manifest_node(manifest_node, manifest)) > 1
             ):
                 logging.info("Creating tasks for: " + node_name)
                 self._add_graph_node_for_multiple_deps_test(node_name, manifest_node, manifest)
 
     def _add_gateway_execution_tasks(self, manifest: dict[str, Any]) -> None:
-        if self._configuration.gateway.separation_schemas.__len__() >= 2:
+        if len(self._configuration.gateway.separation_schemas) >= 2:
             separation_layers = self._configuration.gateway.separation_schemas
 
             for index, _ in enumerate(separation_layers[:-1]):
                 separation_layer_left = separation_layers[index]
                 separation_layer_right = separation_layers[index + 1]
                 self._add_gateway_node(
                     manifest=manifest,
@@ -143,42 +152,60 @@
 
     def contract_test_nodes(self) -> None:
         """Contract test nodes."""
         tests_with_more_deps = self._get_test_with_multiple_deps_names_by_deps()
         for depends_on_tuple, test_node_names in tests_with_more_deps.items():
             self._contract_test_nodes_same_deps(depends_on_tuple, test_node_names)
 
+    @staticmethod
+    def get_default_node_values(manifest_node: dict[str, Any]) -> dict[str, Any]:
+        """Get default node values.
+
+        Args:
+            manifest_node (dict): Manifest node.
+
+        Returns:
+            dict: Default node values.
+        """
+        result: dict[str, Any] = {}
+        if "alias" in manifest_node:
+            result["alias"] = manifest_node["alias"]
+        return result
+
     def _add_execution_graph_node(
         self, node_name: str, manifest_node: dict[str, Any], node_type: NodeType, manifest: dict[str, Any]
     ) -> None:
         self._graph.add_node(
             node_name,
             select=manifest_node["name"],
             depends_on=self._get_model_dependencies_from_manifest_node(manifest_node, manifest),
             node_type=node_type,
+            **self.get_default_node_values(manifest_node),
         )
 
     def _add_sensor_source_node(self, node_name: str, manifest_node: dict[str, Any]) -> None:
         self._graph.add_node(
             node_name,
             select=manifest_node["name"],
             dag=manifest_node["source_meta"]["dag"],
             node_type=NodeType.SOURCE_SENSOR,
+            **self.get_default_node_values(manifest_node),
         )
 
     def _add_gateway_node(self, manifest: dict[str, Any], separation_layer: SeparationLayer) -> None:
         node_name = create_gateway_name(
             separation_layer=separation_layer,
             gateway_task_name=self._configuration.gateway.gateway_task_name,
         )
         self._graph.add_node(
             node_name,
             select=node_name,
             depends_on=get_gateway_dependencies(separation_layer=separation_layer, manifest=manifest),
             node_type=NodeType.MOCK_GATEWAY,
+            **self.get_default_node_values({"alias": node_name}),
         )
 
     def _add_graph_node_for_model_run_task(
         self, node_name: str, manifest_node: dict[str, Any], manifest: dict[str, Any]
     ) -> None:
         self._add_execution_graph_node(
             node_name,
```

### Comparing `dbt-graph-builder-0.3.0/src/dbt_graph_builder/utils.py` & `dbt-graph-builder-0.4.0/src/dbt_graph_builder/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.3.0/src/dbt_graph_builder.egg-info/PKG-INFO` & `dbt-graph-builder-0.4.0/src/dbt_graph_builder.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-graph-builder
-Version: 0.3.0
+Version: 0.4.0
 Summary: DBT Graph Builder
 Author-email: Piotr Tutak <piotr.tutak@getindata.com>
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,33 +38,36 @@
 License-File: LICENSE
 
 # dbt-graph-builder
 
 [![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-graph-builder)
 [![PyPI Version](https://badge.fury.io/py/dbt-graph-builder.svg)](https://pypi.org/project/dbt-graph-builder/)
 [![Downloads](https://pepy.tech/badge/dbt-graph-builder)](https://pepy.tech/project/dbt-graph-builder)
+
+## Overview
+This library provides a set of tools for building a graph of dbt models and their dependencies. It can be used to create an Airflow DAG for dbt models
+or to create a graph of dbt models and their dependencies in a format that can be used by other tools like GCP Workflows.
+
 ## Project Organization
 
 - .devcontainer - This directory contains required files for creating a [Codespace](https://github.com/features/codespaces).
 - .github
   - workflows - Contains GitHub Actions used for building, testing and publishing.
-    - publish-test.yml - Publish wheels to [https://test.pypi.org/](https://test.pypi.org/)
+    - prepare-release.yml - Contains steps to prepare a release.
     - publish.yml - Publish wheels to [https://pypi.org/](https://pypi.org/)
-    - pull-request.yml - Build and Test pull requests before commiting to main.
+    - test-linting.yml - Build and Test pull requests before commiting to main.
     - template-sync.yml - Update GitHub Repo with enhancments to base template
 - docs - collect documents (default format .md)
 - src - place new source code here
   - python_package - sample package (this can be deleted when creating a new repository)
 - tests - contains Python based test cases to validation src code
 - .pre-commit-config.yaml - Contains various pre-check fixes for Python
-- .templateversionrc - used to track template version usage.
 - MANIFEST.in - Declares additional files to include in Python whl
 - pyproject.toml - Python Project Declaration
-- ws.code-workspace - Recommended configurations for [Visual Studio Code](https://code.visualstudio.com/)
-
+- README.md - This file
 
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.
```

