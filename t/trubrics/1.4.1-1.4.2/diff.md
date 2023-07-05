# Comparing `tmp/trubrics-1.4.1.tar.gz` & `tmp/trubrics-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trubrics-1.4.1.tar", last modified: Fri Jun 30 18:35:41 2023, max compression
+gzip compressed data, was "trubrics-1.4.2.tar", last modified: Wed Jul  5 09:01:17 2023, max compression
```

## Comparing `trubrics-1.4.1.tar` & `trubrics-1.4.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-06-30 18:35:32.000000 trubrics-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-30 18:35:41.949996 trubrics-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-06-30 18:35:32.000000 trubrics-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.941996 trubrics-1.4.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:32.000000 trubrics-1.4.1/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.941996 trubrics-1.4.1/examples/feedback/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:32.000000 trubrics-1.4.1/examples/feedback/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.941996 trubrics-1.4.1/examples/feedback/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:32.000000 trubrics-1.4.1/examples/feedback/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-30 18:35:32.000000 trubrics-1.4.1/examples/feedback/streamlit/llm_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-30 18:35:32.000000 trubrics-1.4.1/examples/feedback/streamlit/titanic_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-30 18:35:32.000000 trubrics-1.4.1/examples/feedback/streamlit/trubrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-30 18:35:32.000000 trubrics-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-30 18:35:32.000000 trubrics-1.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-30 18:35:41.949996 trubrics-1.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.941996 trubrics-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-30 18:35:32.000000 trubrics-1.4.1/tests/test_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.941996 trubrics-1.4.1/trubrics/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/example/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/example/my_first_trubric.json
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/example/titanic.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/example/titanic_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    61194 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/example/titanic_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/example/trubric_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/feedback/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/feedback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/feedback/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/feedback/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/feedback/save_to_trubrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/integrations/dash/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/integrations/dash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/integrations/dash/collect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/integrations/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/integrations/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/integrations/gradio/collect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/integrations/mlflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/integrations/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/integrations/mlflow/trubrics_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/integrations/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/integrations/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14077 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/integrations/streamlit/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/integrations/streamlit/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/trubrics_platform/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/trubrics_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/trubrics_platform/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/trubrics_platform/firestore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/trubrics_platform/trubrics_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/utils/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/validations/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/validations/dataclass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/validations/model/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/validations/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/validations/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/validations/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/validations/validation_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.941996 trubrics-1.4.1/trubrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-30 18:35:41.000000 trubrics-1.4.1/trubrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-30 18:35:41.000000 trubrics-1.4.1/trubrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:35:41.000000 trubrics-1.4.1/trubrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-30 18:35:41.000000 trubrics-1.4.1/trubrics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-30 18:35:41.000000 trubrics-1.4.1/trubrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 18:35:41.000000 trubrics-1.4.1/trubrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.962143 trubrics-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-07-05 09:01:06.000000 trubrics-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-05 09:01:17.962143 trubrics-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-05 09:01:06.000000 trubrics-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.954143 trubrics-1.4.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:06.000000 trubrics-1.4.2/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.954143 trubrics-1.4.2/examples/feedback/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:06.000000 trubrics-1.4.2/examples/feedback/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.954143 trubrics-1.4.2/examples/feedback/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:06.000000 trubrics-1.4.2/examples/feedback/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-05 09:01:06.000000 trubrics-1.4.2/examples/feedback/streamlit/llm_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-05 09:01:06.000000 trubrics-1.4.2/examples/feedback/streamlit/titanic_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-05 09:01:06.000000 trubrics-1.4.2/examples/feedback/streamlit/trubrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-05 09:01:06.000000 trubrics-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-05 09:01:06.000000 trubrics-1.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-05 09:01:17.962143 trubrics-1.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.954143 trubrics-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-05 09:01:06.000000 trubrics-1.4.2/tests/test_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.954143 trubrics-1.4.2/trubrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.954143 trubrics-1.4.2/trubrics/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/example/my_first_trubric.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/example/titanic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/example/titanic_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61194 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/example/titanic_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/example/trubric_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/feedback/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/feedback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/feedback/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/feedback/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/feedback/save_to_trubrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/integrations/dash/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/integrations/dash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/integrations/dash/collect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/integrations/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/integrations/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/integrations/gradio/collect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/integrations/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/integrations/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/integrations/mlflow/trubrics_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/integrations/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/integrations/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/integrations/streamlit/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/integrations/streamlit/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/trubrics_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/trubrics_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/trubrics_platform/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/trubrics_platform/firestore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/trubrics_platform/trubrics_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/utils/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/validations/dataclass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/validations/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/validations/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/validations/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/validations/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/validations/validation_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.954143 trubrics-1.4.2/trubrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-05 09:01:17.000000 trubrics-1.4.2/trubrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-05 09:01:17.000000 trubrics-1.4.2/trubrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:01:17.000000 trubrics-1.4.2/trubrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-05 09:01:17.000000 trubrics-1.4.2/trubrics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-05 09:01:17.000000 trubrics-1.4.2/trubrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 09:01:17.000000 trubrics-1.4.2/trubrics.egg-info/top_level.txt
```

### Comparing `trubrics-1.4.1/LICENSE` & `trubrics-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/README.md` & `trubrics-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/examples/feedback/streamlit/llm_app.py` & `trubrics-1.4.2/examples/feedback/streamlit/llm_app.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 import openai
 import streamlit as st
-from trubrics_utils import (
-    datetime_for_timezone,
-    trubrics_config,
-    trubrics_successful_feedback,
-)
+from trubrics_utils import trubrics_config, trubrics_successful_feedback
 
 if "response" not in st.session_state:
     st.session_state["response"] = ""
 
 
 st.title("LLM User Feedback with Trubrics")
 
-timezone_in_hours = st.secrets.get("TIMEZONE_IN_HOURS")  # use to feed correct timezone in Streamlit cloud
-
 with st.sidebar:
     email, password = trubrics_config()
 
 models = ("text-davinci-003", "text-davinci-002")
 model = st.selectbox(
     "Choose your GPT-3.5 LLM",
     models,
@@ -48,15 +42,14 @@
         )
 
         feedback = collector.st_feedback(
             feedback_type="thumbs",
             model=model,
             open_feedback_label="[Optional] Provide additional feedback",
             metadata={"response": st.session_state["response"], "prompt": prompt},
-            created_on=datetime_for_timezone(timezone_in_hours),
         )
 
         if feedback:
             trubrics_successful_feedback(feedback)
 
     else:
         st.warning("To save some feedback to Trubrics, add your account details in the sidebar.")
```

### Comparing `trubrics-1.4.1/examples/feedback/streamlit/titanic_app.py` & `trubrics-1.4.2/examples/feedback/streamlit/titanic_app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 import streamlit as st
-from trubrics_utils import (
-    datetime_for_timezone,
-    trubrics_config,
-    trubrics_successful_feedback,
-)
+from trubrics_utils import trubrics_config, trubrics_successful_feedback
 
 from trubrics.context import DataContext
 from trubrics.example import get_titanic_data_and_model
 from trubrics.example import titanic_config as tc
 from trubrics.integrations.streamlit import (
     FeedbackCollector,
     generate_what_if_streamlit,
@@ -27,16 +23,14 @@
 
     return model, data_context
 
 
 if "wi_prediction" not in st.session_state:
     st.session_state["wi_prediction"] = None
 
-timezone_in_hours = st.secrets.get("TIMEZONE_IN_HOURS")  # use to feed correct timezone in Streamlit cloud
-
 model, data_context = init_trubrics()
 st.title("Titanic Demo App")
 with st.sidebar:
     email, password, feedback_component, feedback_type = trubrics_config(default_component=False)
     with st.form("form"):
         st.subheader("Test the model with different inputs")
         df = generate_what_if_streamlit(data_context=data_context)
@@ -68,13 +62,12 @@
         )
 
         feedback = collector.st_feedback(
             feedback_type=feedback_type,
             model="your_model_name",
             open_feedback_label="[Optional] Provide additional feedback",
             metadata=metadata,
-            created_on=datetime_for_timezone(timezone_in_hours),
         )
         if feedback:
             trubrics_successful_feedback(feedback)
 else:
     st.warning("Click 'Predict' in the sidebar to generate predictions.")
```

### Comparing `trubrics-1.4.1/examples/feedback/streamlit/trubrics_utils.py` & `trubrics-1.4.2/examples/feedback/streamlit/trubrics_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from datetime import datetime, timedelta, timezone
-
 import streamlit as st
 
 
 def trubrics_config(default_component: bool = True):
     st.subheader("Input your Trubrics credentials:")
     email = st.text_input(
         label="email", placeholder="email", label_visibility="collapsed", value=st.secrets.get("TRUBRICS_EMAIL", "")
@@ -30,21 +28,13 @@
     feedback_type = st.radio(
         label="Select the component feedback type:", options=("faces", "thumbs", "textbox"), horizontal=True
     )
 
     return email, password, feedback_component, feedback_type
 
 
-def datetime_for_timezone(hours):
-    """Get the datetime.now() given a number of hours. E.g for hours=-2, get time now for UTC-2"""
-    if hours is not None:
-        return datetime.now(tz=timezone(timedelta(hours=hours))).replace(tzinfo=None)
-    else:
-        return datetime.now()
-
-
 def trubrics_successful_feedback(feedback):
     st.write(
         ":green[You can now view your feedback] [here](https://trubrics.streamlit.app/), :green[and see the raw"
         " feedback response data here:]"
     )
     st.write(feedback)
```

### Comparing `trubrics-1.4.1/setup.cfg` & `trubrics-1.4.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trubrics
-version = 1.4.1
+version = 1.4.2
 description = The first user insights platform for AI models.
 long_description = Full documentation available at https://trubrics.github.io/trubrics-sdk/.
 
 [options]
 packages = find:
 install_requires = file: requirements.txt
```

### Comparing `trubrics-1.4.1/tests/test_context.py` & `trubrics-1.4.2/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics/cli/main.py` & `trubrics-1.4.2/trubrics/cli/main.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics/cli/run.py` & `trubrics-1.4.2/trubrics/cli/run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics/context.py` & `trubrics-1.4.2/trubrics/context.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics/example/my_first_trubric.json` & `trubrics-1.4.2/trubrics/example/my_first_trubric.json`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics/example/titanic.py` & `trubrics-1.4.2/trubrics/example/titanic.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics/example/titanic_data.csv` & `trubrics-1.4.2/trubrics/example/titanic_data.csv`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics/example/trubric_run.py` & `trubrics-1.4.2/trubrics/example/trubric_run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics/exceptions.py` & `trubrics-1.4.2/trubrics/exceptions.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics/feedback/config.py` & `trubrics-1.4.2/trubrics/feedback/config.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics/feedback/dataclass.py` & `trubrics-1.4.2/trubrics/feedback/dataclass.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime
 from typing import Optional
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 
 class Response(BaseModel):
     type: str
     score: Optional[str] = None
     text: Optional[str] = None
 
@@ -32,20 +32,20 @@
         )
         ```
 
     Attributes:
         component_name: the name of the component that the feedback response is saved to
         model: the model name / version
         response: the user response, with a type, score and text
-        created_on: datetime of response
+        created_on: datetime of response (in UTC)
         user_id: an optional user id
         tags: optional tags
         metadata: optional metadata, such as model prompts & predictions
     """
 
     component_name: str
     model: str
     response: Response
-    created_on: datetime = datetime.now()
+    created_on: datetime = Field(default_factory=datetime.utcnow)
     user_id: Optional[str] = None
     tags: list = []
     metadata: dict = {}
```

### Comparing `trubrics-1.4.1/trubrics/feedback/save_to_trubrics.py` & `trubrics-1.4.2/trubrics/feedback/save_to_trubrics.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics/integrations/dash/collect.py` & `trubrics-1.4.2/trubrics/integrations/dash/collect.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics/integrations/gradio/collect.py` & `trubrics-1.4.2/trubrics/integrations/gradio/collect.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics/integrations/mlflow/trubrics_validator.py` & `trubrics-1.4.2/trubrics/integrations/mlflow/trubrics_validator.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics/integrations/streamlit/collect.py` & `trubrics-1.4.2/trubrics/integrations/streamlit/collect.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         self,
         feedback_type: str,
         model: str,
         tags: list = [],
         metadata: dict = {},
         response: Optional[Response] = None,
         user_id: Optional[str] = None,
-        created_on: datetime = datetime.now(),
+        created_on: Optional[datetime] = None,
         key: Optional[str] = None,
         open_feedback_label: Optional[str] = None,
         save_to_trubrics: bool = True,
     ) -> Optional[dict]:
         """
         Collect ML model user feedback with UI components from a Streamlit app.
 
@@ -112,26 +112,27 @@
     def _save_feedback(
         self,
         model: str,
         response: Response,
         user_id: Optional[str] = None,
         tags: list = [],
         metadata: dict = {},
-        created_on: datetime = datetime.now(),
+        created_on: Optional[datetime] = None,
         save_to_trubrics: bool = True,
     ) -> Optional[dict]:
         feedback = Feedback(
             component_name=self.component_name,
             response=response,
             model=model,
             metadata=metadata,
             tags=tags,
             user_id=user_id,
-            created_on=created_on,
         )
+        if created_on:
+            feedback.created_on = created_on
         if save_to_trubrics:
             res = save(trubrics_config=self.trubrics_config, feedback=feedback)
             if "error" in res:
                 error_msg = f"Error in pushing feedback issue to Trubrics: {res}"
                 st.error(error_msg)
             else:
                 st.success(config.PLATFORM_SAVE)
@@ -142,15 +143,15 @@
         feedback_type: str,
         key: str,
         open_feedback_label: Optional[str],
         model: str,
         user_id: Optional[str] = None,
         tags: list = [],
         metadata: dict = {},
-        created_on: datetime = datetime.now(),
+        created_on: Optional[datetime] = None,
         save_to_trubrics: bool = True,
     ) -> Optional[dict]:
         if f"{key}_state" not in st.session_state:
             st.session_state[f"{key}_state"] = ""
         if f"{key}_save_button" not in st.session_state:
             st.session_state[f"{key}_save_button"] = False
         if f"previous_{key}_state" not in st.session_state:
```

### Comparing `trubrics-1.4.1/trubrics/integrations/streamlit/experiment.py` & `trubrics-1.4.2/trubrics/integrations/streamlit/experiment.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics/trubrics_platform/auth.py` & `trubrics-1.4.2/trubrics/trubrics_platform/auth.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics/trubrics_platform/firestore.py` & `trubrics-1.4.2/trubrics/trubrics_platform/firestore.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics/trubrics_platform/trubrics_config.py` & `trubrics-1.4.2/trubrics/trubrics_platform/trubrics_config.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics/validations/dataclass.py` & `trubrics-1.4.2/trubrics/validations/dataclass.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics/validations/model/base.py` & `trubrics-1.4.2/trubrics/validations/model/base.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics/validations/run.py` & `trubrics-1.4.2/trubrics/validations/run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics/validations/validation_output.py` & `trubrics-1.4.2/trubrics/validations/validation_output.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.1/trubrics.egg-info/SOURCES.txt` & `trubrics-1.4.2/trubrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

