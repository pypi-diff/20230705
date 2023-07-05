# Comparing `tmp/dbt-airflow-factory-0.31.1.tar.gz` & `tmp/dbt-airflow-factory-0.32.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-airflow-factory-0.31.1.tar", last modified: Fri May 12 06:14:58 2023, max compression
+gzip compressed data, was "dbt-airflow-factory-0.32.0.tar", last modified: Wed Jul  5 07:11:01 2023, max compression
```

## Comparing `dbt-airflow-factory-0.31.1.tar` & `dbt-airflow-factory-0.32.0.tar`

### file list

```diff
@@ -1,50 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:58.132928 dbt-airflow-factory-0.31.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-12 06:14:58.132928 dbt-airflow-factory-0.31.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:58.128928 dbt-airflow-factory-0.31.1/dbt_airflow_factory/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/airflow_dag_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:58.132928 dbt-airflow-factory-0.31.1/dbt_airflow_factory/bash/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/bash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/bash/bash_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/bash/bash_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/bash/bash_parameters_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/builder_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/dbt_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:58.132928 dbt-airflow-factory-0.31.1/dbt_airflow_factory/ecs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/ecs/ecs_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/ecs/ecs_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/ecs/ecs_parameters_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/ingestion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:58.132928 dbt-airflow-factory-0.31.1/dbt_airflow_factory/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/k8s/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/k8s/k8s_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/k8s/k8s_parameters_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:58.132928 dbt-airflow-factory-0.31.1/dbt_airflow_factory/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/notifications/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:58.132928 dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks_builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks_builder/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks_builder/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks_builder/node_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks_builder/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:58.132928 dbt-airflow-factory-0.31.1/dbt_airflow_factory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-12 06:14:58.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-12 06:14:58.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 06:14:58.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 06:14:58.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-12 06:14:58.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 06:14:58.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-12 06:14:58.132928 dbt-airflow-factory-0.31.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:11:01.827899 dbt-airflow-factory-0.32.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-05 07:11:01.827899 dbt-airflow-factory-0.32.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:11:01.823899 dbt-airflow-factory-0.32.0/dbt_airflow_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/airflow_dag_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:11:01.823899 dbt-airflow-factory-0.32.0/dbt_airflow_factory/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/bash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/bash/bash_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/bash/bash_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/bash/bash_parameters_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/builder_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/dbt_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:11:01.823899 dbt-airflow-factory-0.32.0/dbt_airflow_factory/ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/ecs/ecs_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/ecs/ecs_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/ecs/ecs_parameters_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/ingestion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:11:01.827899 dbt-airflow-factory-0.32.0/dbt_airflow_factory/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/k8s/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/k8s/k8s_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/k8s/k8s_parameters_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:11:01.827899 dbt-airflow-factory-0.32.0/dbt_airflow_factory/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/notifications/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:11:01.827899 dbt-airflow-factory-0.32.0/dbt_airflow_factory/tasks_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/tasks_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/tasks_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/tasks_builder/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:11:01.823899 dbt-airflow-factory-0.32.0/dbt_airflow_factory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-05 07:11:01.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-05 07:11:01.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 07:11:01.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 07:11:01.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-05 07:11:01.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-05 07:11:01.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-05 07:11:01.827899 dbt-airflow-factory-0.32.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/setup.py
```

### Comparing `dbt-airflow-factory-0.31.1/LICENSE` & `dbt-airflow-factory-0.32.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.1/PKG-INFO` & `dbt-airflow-factory-0.32.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,10 @@
-Metadata-Version: 2.1
-Name: dbt-airflow-factory
-Version: 0.31.1
-Summary: Library to convert DBT manifest metadata to Airflow tasks
-Home-page: https://github.com/getindata/dbt-airflow-factory/
-Author: Piotr Pekala
-Author-email: piotr.pekala@getindata.com
-License: Apache Software License (Apache 2.0)
-Keywords: dbt airflow manifest parser python
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: docs
-License-File: LICENSE
-
 # DBT Airflow Factory
 
-[![Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue.svg)](https://github.com/getindata/dbt-airflow-factory)
+[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-airflow-factory)
 [![PyPI Version](https://badge.fury.io/py/dbt-airflow-factory.svg)](https://pypi.org/project/dbt-airflow-factory/)
 [![Downloads](https://pepy.tech/badge/dbt-airflow-factory)](https://pepy.tech/project/dbt-airflow-factory)
 [![Maintainability](https://api.codeclimate.com/v1/badges/47fd3570c858b6c166ad/maintainability)](https://codeclimate.com/github/getindata/dbt-airflow-factory/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/47fd3570c858b6c166ad/test_coverage)](https://codeclimate.com/github/getindata/dbt-airflow-factory/test_coverage)
 [![Documentation Status](https://readthedocs.org/projects/dbt-airflow-factory/badge/?version=latest)](https://dbt-airflow-factory.readthedocs.io/en/latest/?badge=latest)
 
 Library to convert DBT manifest metadata to Airflow tasks
@@ -91,9 +72,7 @@
 for the library to digest, but also automates Docker image building and pushes generated directory to the cloud storage
 of your choice.
 
 [airflow-vars]: https://airflow.apache.org/docs/apache-airflow/stable/templates-ref.html#variables
 [dp-cli]: https://pypi.org/project/data-pipelines-cli/
 [pip]: https://pip.pypa.io/en/stable/
 [tests]: https://github.com/getindata/dbt-airflow-factory/tree/develop/tests/config
-
-
```

### Comparing `dbt-airflow-factory-0.31.1/README.md` & `dbt-airflow-factory-0.32.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,78 +1,98 @@
-# DBT Airflow Factory
-
-[![Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue.svg)](https://github.com/getindata/dbt-airflow-factory)
-[![PyPI Version](https://badge.fury.io/py/dbt-airflow-factory.svg)](https://pypi.org/project/dbt-airflow-factory/)
-[![Downloads](https://pepy.tech/badge/dbt-airflow-factory)](https://pepy.tech/project/dbt-airflow-factory)
-[![Maintainability](https://api.codeclimate.com/v1/badges/47fd3570c858b6c166ad/maintainability)](https://codeclimate.com/github/getindata/dbt-airflow-factory/maintainability)
-[![Test Coverage](https://api.codeclimate.com/v1/badges/47fd3570c858b6c166ad/test_coverage)](https://codeclimate.com/github/getindata/dbt-airflow-factory/test_coverage)
-[![Documentation Status](https://readthedocs.org/projects/dbt-airflow-factory/badge/?version=latest)](https://dbt-airflow-factory.readthedocs.io/en/latest/?badge=latest)
-
-Library to convert DBT manifest metadata to Airflow tasks
-
-## Documentation
-
-Read the full documentation at [https://dbt-airflow-factory.readthedocs.io/](https://dbt-airflow-factory.readthedocs.io/en/latest/index.html)
-
-## Installation
-
-Use the package manager [pip][pip] to install the library:
-
-```bash
-pip install dbt-airflow-factory
-```
-
-## Usage
-
-The library is expected to be used inside an Airflow environment with a Kubernetes image referencing **dbt**.
-
-**dbt-airflow-factory**'s main task is to parse `manifest.json` and create Airflow DAG out of it. It also reads config
-files from `config` directory and therefore is highly customizable (e.g., user can set path to `manifest.json`).
-
-To start, create a directory with a following structure, where `manifest.json` is a file generated by **dbt**:
-```
-.
-├── config
-│   ├── base
-│   │   ├── airflow.yml
-│   │   ├── dbt.yml
-│   │   └── k8s.yml
-│   └── dev
-│       └── dbt.yml
-├── dag.py
-└── manifest.json
-```
-
-Then, put the following code into `dag.py`:
-```python
-from dbt_airflow_factory.airflow_dag_factory import AirflowDagFactory
-from os import path
-
-dag = AirflowDagFactory(path.dirname(path.abspath(__file__)), "dev").create()
-```
-
-When uploaded to Airflow DAGs directory, it will get picked up by Airflow, parse `manifest.json` and prepare a DAG to run.
-
-### Configuration files
-
-It is best to look up the example configuration files in [tests directory][tests] to get a glimpse of correct configs.
-
-You can use [Airflow template variables][airflow-vars] in your `dbt.yml` and `k8s.yml` files, as long as they are inside
-quotation marks:
-```yaml
-target: "{{ var.value.env }}"
-some_other_field: "{{ ds_nodash }}"
-```
-
-Analogously, you can use `"{{ var.value.VARIABLE_NAME }}"` in `airflow.yml`, but only the Airflow variable getter.
-Any other Airflow template variables will not work in `airflow.yml`.
-
-### Creation of the directory with data-pipelines-cli
-
-**DBT Airflow Factory** works best in tandem with [data-pipelines-cli][dp-cli] tool. **dp** not only prepares directory
-for the library to digest, but also automates Docker image building and pushes generated directory to the cloud storage
-of your choice.
-
-[airflow-vars]: https://airflow.apache.org/docs/apache-airflow/stable/templates-ref.html#variables
-[dp-cli]: https://pypi.org/project/data-pipelines-cli/
-[pip]: https://pip.pypa.io/en/stable/
-[tests]: https://github.com/getindata/dbt-airflow-factory/tree/develop/tests/config
+Metadata-Version: 2.1
+Name: dbt-airflow-factory
+Version: 0.32.0
+Summary: Library to convert DBT manifest metadata to Airflow tasks
+Home-page: https://github.com/getindata/dbt-airflow-factory/
+Author: Piotr Pekala
+Author-email: piotr.pekala@getindata.com
+License: Apache Software License (Apache 2.0)
+Description: # DBT Airflow Factory
+        
+        [![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-airflow-factory)
+        [![PyPI Version](https://badge.fury.io/py/dbt-airflow-factory.svg)](https://pypi.org/project/dbt-airflow-factory/)
+        [![Downloads](https://pepy.tech/badge/dbt-airflow-factory)](https://pepy.tech/project/dbt-airflow-factory)
+        [![Maintainability](https://api.codeclimate.com/v1/badges/47fd3570c858b6c166ad/maintainability)](https://codeclimate.com/github/getindata/dbt-airflow-factory/maintainability)
+        [![Test Coverage](https://api.codeclimate.com/v1/badges/47fd3570c858b6c166ad/test_coverage)](https://codeclimate.com/github/getindata/dbt-airflow-factory/test_coverage)
+        [![Documentation Status](https://readthedocs.org/projects/dbt-airflow-factory/badge/?version=latest)](https://dbt-airflow-factory.readthedocs.io/en/latest/?badge=latest)
+        
+        Library to convert DBT manifest metadata to Airflow tasks
+        
+        ## Documentation
+        
+        Read the full documentation at [https://dbt-airflow-factory.readthedocs.io/](https://dbt-airflow-factory.readthedocs.io/en/latest/index.html)
+        
+        ## Installation
+        
+        Use the package manager [pip][pip] to install the library:
+        
+        ```bash
+        pip install dbt-airflow-factory
+        ```
+        
+        ## Usage
+        
+        The library is expected to be used inside an Airflow environment with a Kubernetes image referencing **dbt**.
+        
+        **dbt-airflow-factory**'s main task is to parse `manifest.json` and create Airflow DAG out of it. It also reads config
+        files from `config` directory and therefore is highly customizable (e.g., user can set path to `manifest.json`).
+        
+        To start, create a directory with a following structure, where `manifest.json` is a file generated by **dbt**:
+        ```
+        .
+        ├── config
+        │   ├── base
+        │   │   ├── airflow.yml
+        │   │   ├── dbt.yml
+        │   │   └── k8s.yml
+        │   └── dev
+        │       └── dbt.yml
+        ├── dag.py
+        └── manifest.json
+        ```
+        
+        Then, put the following code into `dag.py`:
+        ```python
+        from dbt_airflow_factory.airflow_dag_factory import AirflowDagFactory
+        from os import path
+        
+        dag = AirflowDagFactory(path.dirname(path.abspath(__file__)), "dev").create()
+        ```
+        
+        When uploaded to Airflow DAGs directory, it will get picked up by Airflow, parse `manifest.json` and prepare a DAG to run.
+        
+        ### Configuration files
+        
+        It is best to look up the example configuration files in [tests directory][tests] to get a glimpse of correct configs.
+        
+        You can use [Airflow template variables][airflow-vars] in your `dbt.yml` and `k8s.yml` files, as long as they are inside
+        quotation marks:
+        ```yaml
+        target: "{{ var.value.env }}"
+        some_other_field: "{{ ds_nodash }}"
+        ```
+        
+        Analogously, you can use `"{{ var.value.VARIABLE_NAME }}"` in `airflow.yml`, but only the Airflow variable getter.
+        Any other Airflow template variables will not work in `airflow.yml`.
+        
+        ### Creation of the directory with data-pipelines-cli
+        
+        **DBT Airflow Factory** works best in tandem with [data-pipelines-cli][dp-cli] tool. **dp** not only prepares directory
+        for the library to digest, but also automates Docker image building and pushes generated directory to the cloud storage
+        of your choice.
+        
+        [airflow-vars]: https://airflow.apache.org/docs/apache-airflow/stable/templates-ref.html#variables
+        [dp-cli]: https://pypi.org/project/data-pipelines-cli/
+        [pip]: https://pip.pypa.io/en/stable/
+        [tests]: https://github.com/getindata/dbt-airflow-factory/tree/develop/tests/config
+        
+Keywords: dbt airflow manifest parser python
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+Provides-Extra: docs
```

### Comparing `dbt-airflow-factory-0.31.1/dbt_airflow_factory/airflow_dag_factory.py` & `dbt-airflow-factory-0.32.0/dbt_airflow_factory/airflow_dag_factory.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.1/dbt_airflow_factory/bash/bash_operator.py` & `dbt-airflow-factory-0.32.0/dbt_airflow_factory/bash/bash_operator.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.1/dbt_airflow_factory/builder_factory.py` & `dbt-airflow-factory-0.32.0/dbt_airflow_factory/builder_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """Factory creating Airflow tasks."""
 
+from dbt_graph_builder.builder import create_gateway_config
+
 from dbt_airflow_factory.bash.bash_operator import BashOperatorBuilder
 from dbt_airflow_factory.bash.bash_parameters_loader import (
     BashExecutionParametersLoader,
 )
 from dbt_airflow_factory.config_utils import read_config
 from dbt_airflow_factory.dbt_parameters import DbtExecutionEnvironmentParameters
 from dbt_airflow_factory.ecs.ecs_operator import EcsPodOperatorBuilder
 from dbt_airflow_factory.ecs.ecs_parameters_loader import EcsExecutionParametersLoader
 from dbt_airflow_factory.k8s.k8s_operator import KubernetesPodOperatorBuilder
 from dbt_airflow_factory.k8s.k8s_parameters_loader import (
     KubernetesExecutionParametersLoader,
 )
 from dbt_airflow_factory.operator import DbtRunOperatorBuilder
 from dbt_airflow_factory.tasks_builder.builder import DbtAirflowTasksBuilder
-from dbt_airflow_factory.tasks_builder.gateway import (
-    GatewayConfiguration,
-    TaskGraphConfiguration,
-)
 from dbt_airflow_factory.tasks_builder.parameters import TasksBuildingParameters
 
 
 class DbtAirflowTasksBuilderFactory:
     """
     Factory creating Airflow tasks.
 
@@ -73,20 +71,15 @@
         dbt_params = self._create_dbt_config()
         execution_env_type = self._read_execution_env_type()
         tasks_airflow_config = self._create_tasks_airflow_config()
 
         return DbtAirflowTasksBuilder(
             tasks_airflow_config,
             self._create_operator_builder(execution_env_type, dbt_params),
-            gateway_config=TaskGraphConfiguration(
-                GatewayConfiguration(
-                    separation_schemas=self.airflow_config.get("save_points", []),
-                    gateway_task_name="gateway",
-                )
-            ),
+            gateway_config=create_gateway_config(self.airflow_config),
         )
 
     def _create_tasks_airflow_config(self) -> TasksBuildingParameters:
         return TasksBuildingParameters(
             self.airflow_config.get("use_task_group", False),
             self.airflow_config.get("show_ephemeral_models", True),
             self.airflow_config.get("enable_project_dependencies", False),
```

### Comparing `dbt-airflow-factory-0.31.1/dbt_airflow_factory/config_utils.py` & `dbt-airflow-factory-0.32.0/dbt_airflow_factory/config_utils.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.1/dbt_airflow_factory/dbt_parameters.py` & `dbt-airflow-factory-0.32.0/dbt_airflow_factory/dbt_parameters.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.1/dbt_airflow_factory/ecs/ecs_operator.py` & `dbt-airflow-factory-0.32.0/dbt_airflow_factory/ecs/ecs_operator.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.1/dbt_airflow_factory/ingestion.py` & `dbt-airflow-factory-0.32.0/dbt_airflow_factory/ingestion.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.1/dbt_airflow_factory/k8s/k8s_operator.py` & `dbt-airflow-factory-0.32.0/dbt_airflow_factory/k8s/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.1/dbt_airflow_factory/k8s/k8s_parameters.py` & `dbt-airflow-factory-0.32.0/dbt_airflow_factory/k8s/k8s_parameters.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.1/dbt_airflow_factory/k8s/k8s_parameters_loader.py` & `dbt-airflow-factory-0.32.0/dbt_airflow_factory/k8s/k8s_parameters_loader.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.1/dbt_airflow_factory/notifications/handler.py` & `dbt-airflow-factory-0.32.0/dbt_airflow_factory/notifications/handler.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.1/dbt_airflow_factory/operator.py` & `dbt-airflow-factory-0.32.0/dbt_airflow_factory/operator.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks.py` & `dbt-airflow-factory-0.32.0/dbt_airflow_factory/tasks.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks_builder/builder.py` & `dbt-airflow-factory-0.32.0/dbt_airflow_factory/tasks_builder/builder.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,43 +4,45 @@
 from typing import Any, ContextManager, Dict, Tuple
 
 from airflow.models.baseoperator import BaseOperator
 from airflow.operators.dummy import DummyOperator
 from airflow.sensors.external_task_sensor import ExternalTaskSensor
 
 from dbt_airflow_factory.constants import IS_FIRST_AIRFLOW_VERSION
-from dbt_airflow_factory.tasks_builder.node_type import NodeType
 from dbt_airflow_factory.tasks_builder.parameters import TasksBuildingParameters
 
 if not IS_FIRST_AIRFLOW_VERSION:
     from airflow.utils.task_group import TaskGroup
 
+from dbt_graph_builder.builder import GraphConfiguration, create_tasks_graph
+from dbt_graph_builder.gateway import GatewayConfiguration
+from dbt_graph_builder.graph import DbtManifestGraph
+from dbt_graph_builder.node_type import NodeType
+
 from dbt_airflow_factory.operator import DbtRunOperatorBuilder, EphemeralOperator
 from dbt_airflow_factory.tasks import ModelExecutionTask, ModelExecutionTasks
-from dbt_airflow_factory.tasks_builder.gateway import TaskGraphConfiguration
-from dbt_airflow_factory.tasks_builder.graph import DbtAirflowGraph
 
 
 class DbtAirflowTasksBuilder:
     """
     Parses ``manifest.json`` into Airflow tasks.
 
     :param airflow_config: DBT node operator.
     :type airflow_config: TasksBuildingParameters
     :param operator_builder: DBT node operator.
     :type operator_builder: DbtRunOperatorBuilder
     :param gateway_config: DBT node operator.
-    :type gateway_config: TaskGraphConfiguration
+    :type gateway_config: GatewayConfiguration
     """
 
     def __init__(
         self,
         airflow_config: TasksBuildingParameters,
         operator_builder: DbtRunOperatorBuilder,
-        gateway_config: TaskGraphConfiguration,
+        gateway_config: GatewayConfiguration,
     ):
         self.operator_builder = operator_builder
         self.airflow_config = airflow_config
         self.gateway_config = gateway_config
 
     def parse_manifest_into_tasks(self, manifest_path: str) -> ModelExecutionTasks:
         """
@@ -142,48 +144,42 @@
         else:
             return self._create_task_for_model(
                 node["select"],
                 node["node_type"] == NodeType.EPHEMERAL,
                 self.airflow_config.use_task_group,
             )
 
-    def _create_tasks_from_graph(self, dbt_airflow_graph: DbtAirflowGraph) -> ModelExecutionTasks:
+    def _create_tasks_from_graph(self, dbt_airflow_graph: DbtManifestGraph) -> ModelExecutionTasks:
         result_tasks = {
             node_name: self._create_task_from_graph_node(node_name, node)
-            for node_name, node in dbt_airflow_graph.graph.nodes(data=True)
+            for node_name, node in dbt_airflow_graph.get_graph_nodes()
         }
-        for node, neighbour in dbt_airflow_graph.graph.edges():
+        for node, neighbour in dbt_airflow_graph.get_graph_edges():
             # noinspection PyStatementEffect
             (result_tasks[node].get_end_task() >> result_tasks[neighbour].get_start_task())
         return ModelExecutionTasks(
             result_tasks,
             dbt_airflow_graph.get_graph_sources(),
             dbt_airflow_graph.get_graph_sinks(),
         )
 
     def _make_dbt_tasks(self, manifest_path: str) -> ModelExecutionTasks:
         manifest = self._load_dbt_manifest(manifest_path)
-        dbt_airflow_graph = self._create_tasks_graph(manifest)
+        dbt_airflow_graph: DbtManifestGraph = create_tasks_graph(
+            manifest,
+            GraphConfiguration(
+                gateway_config=self.gateway_config,
+                enable_dags_dependencies=self.airflow_config.enable_dags_dependencies,
+                show_ephemeral_models=self.airflow_config.show_ephemeral_models,
+            ),
+        )
         tasks_with_context = self._create_tasks_from_graph(dbt_airflow_graph)
         logging.info(f"Created {str(tasks_with_context.length())} tasks groups")
         return tasks_with_context
 
-    def _create_tasks_graph(self, manifest: dict) -> DbtAirflowGraph:
-        dbt_airflow_graph = DbtAirflowGraph(self.gateway_config)
-        dbt_airflow_graph.add_execution_tasks(manifest)
-        if self.airflow_config.enable_dags_dependencies:
-            dbt_airflow_graph.add_external_dependencies(manifest)
-        dbt_airflow_graph.create_edges_from_dependencies(
-            self.airflow_config.enable_dags_dependencies
-        )
-        if not self.airflow_config.show_ephemeral_models:
-            dbt_airflow_graph.remove_ephemeral_nodes_from_graph()
-        dbt_airflow_graph.contract_test_nodes()
-        return dbt_airflow_graph
-
     def _create_dag_sensor(self, node: Dict[str, Any]) -> ModelExecutionTask:
         # todo move parameters to configuration
         return ModelExecutionTask(
             ExternalTaskSensor(
                 task_id="sensor_" + node["select"],
                 external_dag_id=node["dag"],
                 external_task_id=node["select"]
```

### Comparing `dbt-airflow-factory-0.31.1/dbt_airflow_factory.egg-info/PKG-INFO` & `dbt-airflow-factory-0.32.0/dbt_airflow_factory.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,99 +1,98 @@
 Metadata-Version: 2.1
 Name: dbt-airflow-factory
-Version: 0.31.1
+Version: 0.32.0
 Summary: Library to convert DBT manifest metadata to Airflow tasks
 Home-page: https://github.com/getindata/dbt-airflow-factory/
 Author: Piotr Pekala
 Author-email: piotr.pekala@getindata.com
 License: Apache Software License (Apache 2.0)
+Description: # DBT Airflow Factory
+        
+        [![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-airflow-factory)
+        [![PyPI Version](https://badge.fury.io/py/dbt-airflow-factory.svg)](https://pypi.org/project/dbt-airflow-factory/)
+        [![Downloads](https://pepy.tech/badge/dbt-airflow-factory)](https://pepy.tech/project/dbt-airflow-factory)
+        [![Maintainability](https://api.codeclimate.com/v1/badges/47fd3570c858b6c166ad/maintainability)](https://codeclimate.com/github/getindata/dbt-airflow-factory/maintainability)
+        [![Test Coverage](https://api.codeclimate.com/v1/badges/47fd3570c858b6c166ad/test_coverage)](https://codeclimate.com/github/getindata/dbt-airflow-factory/test_coverage)
+        [![Documentation Status](https://readthedocs.org/projects/dbt-airflow-factory/badge/?version=latest)](https://dbt-airflow-factory.readthedocs.io/en/latest/?badge=latest)
+        
+        Library to convert DBT manifest metadata to Airflow tasks
+        
+        ## Documentation
+        
+        Read the full documentation at [https://dbt-airflow-factory.readthedocs.io/](https://dbt-airflow-factory.readthedocs.io/en/latest/index.html)
+        
+        ## Installation
+        
+        Use the package manager [pip][pip] to install the library:
+        
+        ```bash
+        pip install dbt-airflow-factory
+        ```
+        
+        ## Usage
+        
+        The library is expected to be used inside an Airflow environment with a Kubernetes image referencing **dbt**.
+        
+        **dbt-airflow-factory**'s main task is to parse `manifest.json` and create Airflow DAG out of it. It also reads config
+        files from `config` directory and therefore is highly customizable (e.g., user can set path to `manifest.json`).
+        
+        To start, create a directory with a following structure, where `manifest.json` is a file generated by **dbt**:
+        ```
+        .
+        ├── config
+        │   ├── base
+        │   │   ├── airflow.yml
+        │   │   ├── dbt.yml
+        │   │   └── k8s.yml
+        │   └── dev
+        │       └── dbt.yml
+        ├── dag.py
+        └── manifest.json
+        ```
+        
+        Then, put the following code into `dag.py`:
+        ```python
+        from dbt_airflow_factory.airflow_dag_factory import AirflowDagFactory
+        from os import path
+        
+        dag = AirflowDagFactory(path.dirname(path.abspath(__file__)), "dev").create()
+        ```
+        
+        When uploaded to Airflow DAGs directory, it will get picked up by Airflow, parse `manifest.json` and prepare a DAG to run.
+        
+        ### Configuration files
+        
+        It is best to look up the example configuration files in [tests directory][tests] to get a glimpse of correct configs.
+        
+        You can use [Airflow template variables][airflow-vars] in your `dbt.yml` and `k8s.yml` files, as long as they are inside
+        quotation marks:
+        ```yaml
+        target: "{{ var.value.env }}"
+        some_other_field: "{{ ds_nodash }}"
+        ```
+        
+        Analogously, you can use `"{{ var.value.VARIABLE_NAME }}"` in `airflow.yml`, but only the Airflow variable getter.
+        Any other Airflow template variables will not work in `airflow.yml`.
+        
+        ### Creation of the directory with data-pipelines-cli
+        
+        **DBT Airflow Factory** works best in tandem with [data-pipelines-cli][dp-cli] tool. **dp** not only prepares directory
+        for the library to digest, but also automates Docker image building and pushes generated directory to the cloud storage
+        of your choice.
+        
+        [airflow-vars]: https://airflow.apache.org/docs/apache-airflow/stable/templates-ref.html#variables
+        [dp-cli]: https://pypi.org/project/data-pipelines-cli/
+        [pip]: https://pip.pypa.io/en/stable/
+        [tests]: https://github.com/getindata/dbt-airflow-factory/tree/develop/tests/config
+        
 Keywords: dbt airflow manifest parser python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
-License-File: LICENSE
-
-# DBT Airflow Factory
-
-[![Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue.svg)](https://github.com/getindata/dbt-airflow-factory)
-[![PyPI Version](https://badge.fury.io/py/dbt-airflow-factory.svg)](https://pypi.org/project/dbt-airflow-factory/)
-[![Downloads](https://pepy.tech/badge/dbt-airflow-factory)](https://pepy.tech/project/dbt-airflow-factory)
-[![Maintainability](https://api.codeclimate.com/v1/badges/47fd3570c858b6c166ad/maintainability)](https://codeclimate.com/github/getindata/dbt-airflow-factory/maintainability)
-[![Test Coverage](https://api.codeclimate.com/v1/badges/47fd3570c858b6c166ad/test_coverage)](https://codeclimate.com/github/getindata/dbt-airflow-factory/test_coverage)
-[![Documentation Status](https://readthedocs.org/projects/dbt-airflow-factory/badge/?version=latest)](https://dbt-airflow-factory.readthedocs.io/en/latest/?badge=latest)
-
-Library to convert DBT manifest metadata to Airflow tasks
-
-## Documentation
-
-Read the full documentation at [https://dbt-airflow-factory.readthedocs.io/](https://dbt-airflow-factory.readthedocs.io/en/latest/index.html)
-
-## Installation
-
-Use the package manager [pip][pip] to install the library:
-
-```bash
-pip install dbt-airflow-factory
-```
-
-## Usage
-
-The library is expected to be used inside an Airflow environment with a Kubernetes image referencing **dbt**.
-
-**dbt-airflow-factory**'s main task is to parse `manifest.json` and create Airflow DAG out of it. It also reads config
-files from `config` directory and therefore is highly customizable (e.g., user can set path to `manifest.json`).
-
-To start, create a directory with a following structure, where `manifest.json` is a file generated by **dbt**:
-```
-.
-├── config
-│   ├── base
-│   │   ├── airflow.yml
-│   │   ├── dbt.yml
-│   │   └── k8s.yml
-│   └── dev
-│       └── dbt.yml
-├── dag.py
-└── manifest.json
-```
-
-Then, put the following code into `dag.py`:
-```python
-from dbt_airflow_factory.airflow_dag_factory import AirflowDagFactory
-from os import path
-
-dag = AirflowDagFactory(path.dirname(path.abspath(__file__)), "dev").create()
-```
-
-When uploaded to Airflow DAGs directory, it will get picked up by Airflow, parse `manifest.json` and prepare a DAG to run.
-
-### Configuration files
-
-It is best to look up the example configuration files in [tests directory][tests] to get a glimpse of correct configs.
-
-You can use [Airflow template variables][airflow-vars] in your `dbt.yml` and `k8s.yml` files, as long as they are inside
-quotation marks:
-```yaml
-target: "{{ var.value.env }}"
-some_other_field: "{{ ds_nodash }}"
-```
-
-Analogously, you can use `"{{ var.value.VARIABLE_NAME }}"` in `airflow.yml`, but only the Airflow variable getter.
-Any other Airflow template variables will not work in `airflow.yml`.
-
-### Creation of the directory with data-pipelines-cli
-
-**DBT Airflow Factory** works best in tandem with [data-pipelines-cli][dp-cli] tool. **dp** not only prepares directory
-for the library to digest, but also automates Docker image building and pushes generated directory to the cloud storage
-of your choice.
-
-[airflow-vars]: https://airflow.apache.org/docs/apache-airflow/stable/templates-ref.html#variables
-[dp-cli]: https://pypi.org/project/data-pipelines-cli/
-[pip]: https://pip.pypa.io/en/stable/
-[tests]: https://github.com/getindata/dbt-airflow-factory/tree/develop/tests/config
-
-
```

### Comparing `dbt-airflow-factory-0.31.1/dbt_airflow_factory.egg-info/SOURCES.txt` & `dbt-airflow-factory-0.32.0/dbt_airflow_factory.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -30,12 +30,8 @@
 dbt_airflow_factory/k8s/k8s_operator.py
 dbt_airflow_factory/k8s/k8s_parameters.py
 dbt_airflow_factory/k8s/k8s_parameters_loader.py
 dbt_airflow_factory/notifications/__init__.py
 dbt_airflow_factory/notifications/handler.py
 dbt_airflow_factory/tasks_builder/__init__.py
 dbt_airflow_factory/tasks_builder/builder.py
-dbt_airflow_factory/tasks_builder/gateway.py
-dbt_airflow_factory/tasks_builder/graph.py
-dbt_airflow_factory/tasks_builder/node_type.py
-dbt_airflow_factory/tasks_builder/parameters.py
-dbt_airflow_factory/tasks_builder/utils.py
+dbt_airflow_factory/tasks_builder/parameters.py
```

### Comparing `dbt-airflow-factory-0.31.1/setup.cfg` & `dbt-airflow-factory-0.32.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.31.1
+current_version = 0.32.0
 
 [bumpversion:file:setup.py]
 
 [bumpversion:file:dbt_airflow_factory/__init__.py]
 
 [flake8]
 exclude = .git,__pycache__,build,dist,docs/source/conf.py
```

### Comparing `dbt-airflow-factory-0.31.1/setup.py` & `dbt-airflow-factory-0.32.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md") as f:
     README = f.read()
 
 # Runtime Requirements.
 INSTALL_REQUIRES = [
     "pytimeparse==1.1.8",
-    "networkx==2.6.3",
+    "dbt-graph-builder>=0.3.0",
 ]
 
 # Dev Requirements
 EXTRA_REQUIRE = {
     "tests": [
         "pytest>=6.2.2, <7.0.0",
         "pytest-cov>=2.8.0, <3.0.0",
@@ -29,24 +29,26 @@
         "myst-parser>=0.16, <0.17",
         "docutils<0.17",
     ],
 }
 
 setup(
     name="dbt-airflow-factory",
-    version="0.31.1",
+    version="0.32.0",
     description="Library to convert DBT manifest metadata to Airflow tasks",
     long_description=README,
     long_description_content_type="text/markdown",
     license="Apache Software License (Apache 2.0)",
     python_requires=">=3",
     classifiers=[
         "Development Status :: 3 - Alpha",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     keywords="dbt airflow manifest parser python",
     author="Piotr Pekala",
     author_email="piotr.pekala@getindata.com",
     url="https://github.com/getindata/dbt-airflow-factory/",
     packages=find_packages(exclude=["ez_setup", "examples", "tests", "docs"]),
     include_package_data=True,
```

