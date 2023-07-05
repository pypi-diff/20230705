# Comparing `tmp/apache-airflow-providers-databricks-4.3.0rc1.tar.gz` & `tmp/apache-airflow-providers-databricks-4.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-databricks-4.3.0rc1.tar", last modified: Tue Jun 20 11:41:47 2023, max compression
+gzip compressed data, was "apache-airflow-providers-databricks-4.3.1rc1.tar", last modified: Wed Jul  5 07:29:54 2023, max compression
```

## Comparing `apache-airflow-providers-databricks-4.3.0rc1.tar` & `apache-airflow-providers-databricks-4.3.1rc1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.334610 apache-airflow-providers-databricks-4.3.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-databricks-4.3.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:46.000000 apache-airflow-providers-databricks-4.3.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-databricks-4.3.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    21143 2023-06-20 11:41:47.335992 apache-airflow-providers-databricks-4.3.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    19576 2023-06-20 11:41:46.000000 apache-airflow-providers-databricks-4.3.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.212152 apache-airflow-providers-databricks-4.3.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.213485 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.255680 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/
--rw-r--r--   0 root         (0) root         (0)     1535 2023-06-20 11:01:09.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5506 2023-06-20 11:41:46.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.269076 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16771 2023-06-02 11:31:21.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/databricks.py
--rw-r--r--   0 root         (0) root         (0)    26695 2023-06-02 11:31:21.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/databricks_base.py
--rw-r--r--   0 root         (0) root         (0)     9359 2023-06-17 16:45:00.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.281889 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33383 2023-06-19 10:14:19.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/databricks.py
--rw-r--r--   0 root         (0) root         (0)    13212 2023-06-02 11:31:21.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/databricks_repos.py
--rw-r--r--   0 root         (0) root         (0)    16994 2023-06-17 16:45:00.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.290943 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10000 2023-06-01 07:44:14.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/sensors/databricks_partition.py
--rw-r--r--   0 root         (0) root         (0)     5543 2023-06-01 07:44:14.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/sensors/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.297042 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/triggers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3997 2023-06-18 13:29:11.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/triggers/databricks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.303088 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2910 2023-06-02 11:31:21.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/utils/databricks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.330922 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/
--rw-r--r--   0 root         (0) root         (0)    21143 2023-06-20 11:41:47.000000 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1362 2023-06-20 11:41:47.000000 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:47.000000 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-20 11:41:47.000000 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:47.000000 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      200 2023-06-20 11:41:47.000000 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:47.000000 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-databricks-4.3.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1982 2023-06-20 11:41:47.340065 apache-airflow-providers-databricks-4.3.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1715 2023-06-20 11:41:46.000000 apache-airflow-providers-databricks-4.3.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:54.885886 apache-airflow-providers-databricks-4.3.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-databricks-4.3.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 07:29:53.000000 apache-airflow-providers-databricks-4.3.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-databricks-4.3.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5810 2023-07-05 07:29:54.886486 apache-airflow-providers-databricks-4.3.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4129 2023-07-05 07:29:53.000000 apache-airflow-providers-databricks-4.3.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:54.768560 apache-airflow-providers-databricks-4.3.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:54.769712 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:54.810050 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-07-05 07:19:39.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5527 2023-07-05 07:29:53.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:54.822625 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16773 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/hooks/databricks.py
+-rw-r--r--   0 root         (0) root         (0)    26696 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/hooks/databricks_base.py
+-rw-r--r--   0 root         (0) root         (0)     9359 2023-06-17 16:45:00.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/hooks/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:54.835759 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33530 2023-07-05 07:19:39.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/operators/databricks.py
+-rw-r--r--   0 root         (0) root         (0)    13181 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/operators/databricks_repos.py
+-rw-r--r--   0 root         (0) root         (0)    17010 2023-06-29 14:43:21.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/operators/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:54.844918 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9827 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/sensors/databricks_partition.py
+-rw-r--r--   0 root         (0) root         (0)     5543 2023-06-01 07:44:14.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/sensors/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:54.851439 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3997 2023-06-18 13:29:11.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/triggers/databricks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:54.857448 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2945 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/utils/databricks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:54.883118 apache-airflow-providers-databricks-4.3.1rc1/apache_airflow_providers_databricks.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5810 2023-07-05 07:29:54.000000 apache-airflow-providers-databricks-4.3.1rc1/apache_airflow_providers_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1362 2023-07-05 07:29:54.000000 apache-airflow-providers-databricks-4.3.1rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:54.000000 apache-airflow-providers-databricks-4.3.1rc1/apache_airflow_providers_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-05 07:29:54.000000 apache-airflow-providers-databricks-4.3.1rc1/apache_airflow_providers_databricks.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:54.000000 apache-airflow-providers-databricks-4.3.1rc1/apache_airflow_providers_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      200 2023-07-05 07:29:54.000000 apache-airflow-providers-databricks-4.3.1rc1/apache_airflow_providers_databricks.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:29:54.000000 apache-airflow-providers-databricks-4.3.1rc1/apache_airflow_providers_databricks.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-databricks-4.3.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-07-05 07:29:54.888468 apache-airflow-providers-databricks-4.3.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1715 2023-07-05 07:29:53.000000 apache-airflow-providers-databricks-4.3.1rc1/setup.py
```

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/LICENSE` & `apache-airflow-providers-databricks-4.3.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/MANIFEST.in` & `apache-airflow-providers-databricks-4.3.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/__init__.py` & `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.3.0"
+__version__ = "4.3.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/get_provider_info.py` & `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-databricks",
         "name": "Databricks",
         "description": "`Databricks <https://databricks.com/>`__\n",
         "suspended": False,
         "versions": [
+            "4.3.1",
             "4.3.0",
             "4.2.0",
             "4.1.0",
             "4.0.1",
             "4.0.0",
             "3.4.0",
             "3.3.0",
```

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/__init__.py` & `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/databricks.py` & `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/hooks/databricks.py`

 * *Files 0% similar despite different names*

```diff
@@ -455,15 +455,16 @@
         :return:
         """
         repos_endpoint = ("POST", "api/2.0/repos")
         return self._do_api_call(repos_endpoint, json)
 
     def get_repo_by_path(self, path: str) -> str | None:
         """
-        Obtains Repos ID by path
+        Obtains Repos ID by path.
+
         :param path: path to a repository
         :return: Repos ID if it exists, None if doesn't.
         """
         try:
             result = self._do_api_call(WORKSPACE_GET_STATUS_ENDPOINT, {"path": path}, wrap_http_errors=False)
             if result.get("object_type", "") == "REPO":
                 return str(result["object_id"])
```

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/databricks_base.py` & `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/hooks/databricks_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -539,14 +539,15 @@
                 )
             else:
                 raise e
 
     async def _a_do_api_call(self, endpoint_info: tuple[str, str], json: dict[str, Any] | None = None):
         """
         Async version of `_do_api_call()`.
+
         :param endpoint_info: Tuple of method and endpoint
         :param json: Parameters for this API call.
         :return: If the api call returns a OK status code,
             this function returns the response in JSON. Otherwise, throw an AirflowException.
         """
         method, endpoint = endpoint_info
```

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/databricks_sql.py` & `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/hooks/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/__init__.py` & `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/databricks.py` & `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/operators/databricks.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 import time
 import warnings
 from functools import cached_property
 from logging import Logger
 from typing import TYPE_CHECKING, Any, Sequence
 
+from airflow.configuration import conf
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator, BaseOperatorLink, XCom
 from airflow.providers.databricks.hooks.databricks import DatabricksHook, RunState
 from airflow.providers.databricks.triggers.databricks import DatabricksExecutionTrigger
 from airflow.providers.databricks.utils.databricks import normalise_json_content, validate_trigger_event
 
 if TYPE_CHECKING:
@@ -158,18 +159,17 @@
         ti_key: TaskInstanceKey,
     ) -> str:
         return XCom.get_value(key=XCOM_RUN_PAGE_URL_KEY, ti_key=ti_key)
 
 
 class DatabricksSubmitRunOperator(BaseOperator):
     """
-    Submits a Spark job run to Databricks using the
-    `api/2.1/jobs/runs/submit
-    <https://docs.databricks.com/dev-tools/api/latest/jobs.html#operation/JobsRunsSubmit>`_
-    API endpoint.
+    Submits a Spark job run to Databricks using the api/2.1/jobs/runs/submit API endpoint.
+
+    See: https://docs.databricks.com/dev-tools/api/latest/jobs.html#operation/JobsRunsSubmit
 
     There are three ways to instantiate this operator.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:DatabricksSubmitRunOperator`
 
@@ -312,15 +312,15 @@
         databricks_retry_delay: int = 1,
         databricks_retry_args: dict[Any, Any] | None = None,
         do_xcom_push: bool = True,
         idempotency_token: str | None = None,
         access_control_list: list[dict[str, str]] | None = None,
         wait_for_termination: bool = True,
         git_source: dict[str, str] | None = None,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ) -> None:
         """Creates a new ``DatabricksSubmitRunOperator``."""
         super().__init__(**kwargs)
         self.json = json or {}
         self.databricks_conn_id = databricks_conn_id
         self.polling_period_seconds = polling_period_seconds
@@ -424,18 +424,17 @@
 
     def execute_complete(self, context: dict | None, event: dict):
         _handle_deferrable_databricks_operator_completion(event, self.log)
 
 
 class DatabricksRunNowOperator(BaseOperator):
     """
-    Runs an existing Spark job run to Databricks using the
-    `api/2.1/jobs/run-now
-    <https://docs.databricks.com/dev-tools/api/latest/jobs.html#operation/JobsRunNow>`_
-    API endpoint.
+    Runs an existing Spark job run to Databricks using the api/2.1/jobs/run-now API endpoint.
+
+    See: https://docs.databricks.com/dev-tools/api/latest/jobs.html#operation/JobsRunNow
 
     There are two ways to instantiate this operator.
 
     In the first way, you can take the JSON payload that you typically use
     to call the ``api/2.1/jobs/run-now`` endpoint and pass it directly
     to our ``DatabricksRunNowOperator`` through the ``json`` parameter.
     For example ::
@@ -603,15 +602,15 @@
         databricks_conn_id: str = "databricks_default",
         polling_period_seconds: int = 30,
         databricks_retry_limit: int = 3,
         databricks_retry_delay: int = 1,
         databricks_retry_args: dict[Any, Any] | None = None,
         do_xcom_push: bool = True,
         wait_for_termination: bool = True,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ) -> None:
         """Creates a new ``DatabricksRunNowOperator``."""
         super().__init__(**kwargs)
         self.json = json or {}
         self.databricks_conn_id = databricks_conn_id
         self.polling_period_seconds = polling_period_seconds
```

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/databricks_repos.py` & `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/operators/databricks_repos.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,17 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class DatabricksReposCreateOperator(BaseOperator):
     """
-    Creates a Databricks Repo
-    using
-    `POST api/2.0/repos <https://docs.databricks.com/dev-tools/api/latest/repos.html#operation/create-repo>`_
-    API endpoint and optionally checking it out to a specific branch or tag.
+    Creates, and optionally checks out, a Databricks Repo using the POST api/2.0/repos API endpoint.
+
+     See: https://docs.databricks.com/dev-tools/api/latest/repos.html#operation/create-repo
 
     :param git_url: Required HTTPS URL of a Git repository
     :param git_provider: Optional name of Git provider. Must be provided if we can't guess its name from URL.
     :param repo_path: optional path for a repository. Must be in the format ``/Repos/{folder}/{repo-name}``.
         If not specified, it will be created in the user's directory.
     :param branch: optional name of branch to check out.
     :param tag: optional name of tag to checkout.
@@ -161,17 +160,17 @@
             self._hook.update_repo(str(repo_id), {"tag": str(self.tag)})
 
         return repo_id
 
 
 class DatabricksReposUpdateOperator(BaseOperator):
     """
-    Updates specified repository to a given branch or tag
-    using `PATCH api/2.0/repos
-    <https://docs.databricks.com/dev-tools/api/latest/repos.html#operation/update-repo>`_ API endpoint.
+    Updates specified repository to a given branch or tag using the PATCH api/2.0/repos API endpoint.
+
+    See: https://docs.databricks.com/dev-tools/api/latest/repos.html#operation/update-repo
 
     :param branch: optional name of branch to update to. Should be specified if ``tag`` is omitted
     :param tag: optional name of tag to update to. Should be specified if ``branch`` is omitted
     :param repo_id: optional ID of existing repository. Should be specified if ``repo_path`` is omitted
     :param repo_path: optional path of existing repository. Should be specified if ``repo_id`` is omitted
     :param databricks_conn_id: Reference to the :ref:`Databricks connection <howto/connection:databricks>`.
         By default and in the common case this will be ``databricks_default``. To use
@@ -237,17 +236,17 @@
 
         result = self._hook.update_repo(str(self.repo_id), payload)
         return result["head_commit_id"]
 
 
 class DatabricksReposDeleteOperator(BaseOperator):
     """
-    Deletes specified repository
-    using `DELETE api/2.0/repos
-    <https://docs.databricks.com/dev-tools/api/latest/repos.html#operation/delete-repo>`_ API endpoint.
+    Deletes specified repository using the DELETE api/2.0/repos API endpoint.
+
+    See: https://docs.databricks.com/dev-tools/api/latest/repos.html#operation/delete-repo
 
     :param repo_id: optional ID of existing repository. Should be specified if ``repo_path`` is omitted
     :param repo_path: optional path of existing repository. Should be specified if ``repo_id`` is omitted
     :param databricks_conn_id: Reference to the :ref:`Databricks connection <howto/connection:databricks>`.
         By default and in the common case this will be ``databricks_default``. To use
         token based authentication, provide the key ``token`` in the extra field for the
         connection and create the key ``host`` and leave the ``host`` field empty. (templated)
```

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/databricks_sql.py` & `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/operators/databricks_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,22 +66,19 @@
     :param schema: An optional initial schema to use. Requires DBR version 9.0+ (templated)
     :param output_path: optional string specifying the file to which write selected data. (templated)
     :param output_format: format of output data if ``output_path` is specified.
         Possible values are ``csv``, ``json``, ``jsonl``. Default is ``csv``.
     :param csv_params: parameters that will be passed to the ``csv.DictWriter`` class used to write CSV data.
     """
 
-    template_fields: Sequence[str] = (
-        "sql",
-        "_output_path",
-        "schema",
-        "catalog",
-        "http_headers",
-        "databricks_conn_id",
+    template_fields: Sequence[str] = tuple(
+        {"_output_path", "schema", "catalog", "http_headers", "databricks_conn_id"}
+        | set(SQLExecuteQueryOperator.template_fields)
     )
+
     template_ext: Sequence[str] = (".sql",)
     template_fields_renderers = {"sql": "sql"}
 
     def __init__(
         self,
         *,
         databricks_conn_id: str = DatabricksSqlHook.default_conn_name,
@@ -168,14 +165,15 @@
 
 COPY_INTO_APPROVED_FORMATS = ["CSV", "JSON", "AVRO", "ORC", "PARQUET", "TEXT", "BINARYFILE"]
 
 
 class DatabricksCopyIntoOperator(BaseOperator):
     """
     Executes COPY INTO command in a Databricks SQL endpoint or a Databricks cluster.
+
     COPY INTO command is constructed from individual pieces, that are described in
     `documentation <https://docs.databricks.com/sql/language-manual/delta-copy-into.html>`_.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:DatabricksSqlCopyIntoOperator`
```

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/sensors/__init__.py` & `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/sensors/databricks_partition.py` & `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/sensors/databricks_partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,21 +132,15 @@
             self.schema,
             self.caller,
             **self.client_parameters,
             **self.hook_params,
         )
 
     def _check_table_partitions(self) -> list:
-        """
-        The method performs the following:
-        * Generates the fully qualified table name.
-        * Calls the generate partition query.
-        * Based on the result returned by the partition generation method,
-        the _sql_sensor method is called.
-        """
+        """Generate the fully qualified table name, generate partition, and call the _sql_sensor method."""
         if self.table_name.split(".")[0] == "delta":
             _fully_qualified_table_name = self.table_name
         else:
             _fully_qualified_table_name = str(self.catalog + "." + self.schema + "." + self.table_name)
         self.log.debug("Table name generated from arguments: %s", _fully_qualified_table_name)
         _joiner_val = " AND "
         _prefix = f"SELECT 1 FROM {_fully_qualified_table_name} WHERE"
@@ -169,14 +163,15 @@
         joiner_val: str,
         table_name: str,
         opts: dict[str, str] | None = None,
         escape_key: bool = False,
     ) -> str:
         """
         Queries the table for available partitions.
+
         Generates the SQL query based on the partition data types.
             * For a list, it prepares the SQL in the format:
                 column_name in (value1, value2,...)
             * For a numeric type, it prepares the format:
                 column_name =(or other provided operator such as >=) value
             * For a date type, it prepares the format:
                 column_name =(or other provided operator such as >=) value
```

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/sensors/databricks_sql.py` & `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/sensors/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/triggers/__init__.py` & `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/triggers/databricks.py` & `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/triggers/databricks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/utils/__init__.py` & `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/utils/databricks.py` & `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/utils/databricks.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,20 @@
 
 from airflow.exceptions import AirflowException
 from airflow.providers.databricks.hooks.databricks import RunState
 
 
 def normalise_json_content(content, json_path: str = "json") -> str | bool | list | dict:
     """
-    Normalize content or all values of content if it is a dict to a string. The
-    function will throw if content contains non-string or non-numeric non-boolean types.
-    The reason why we have this function is because the ``self.json`` field must be a
-    dict with only string values. This is because ``render_template`` will fail
-    for numerical values.
+    Normalize content or all values of content if it is a dict to a string.
+
+    The function will throw if content contains non-string or non-numeric non-boolean
+    types. The reason why we have this function is because the ``self.json`` field
+    must be a dict with only string values. This is because ``render_template`` will
+    fail for numerical values.
 
     The only one exception is when we have boolean values, they can not be converted
     to string type because databricks does not understand 'True' or 'False' values.
     """
     normalise = normalise_json_content
     if isinstance(content, (str, bool)):
         return content
@@ -52,16 +53,17 @@
         param_type = type(content)
         msg = f"Type {param_type} used for parameter {json_path} is not a number or a string"
         raise AirflowException(msg)
 
 
 def validate_trigger_event(event: dict):
     """
-    Validates correctness of the event
-    received from :class:`~airflow.providers.databricks.triggers.databricks.DatabricksExecutionTrigger`.
+    Validates correctness of the event received from DatabricksExecutionTrigger.
+
+    See: :class:`~airflow.providers.databricks.triggers.databricks.DatabricksExecutionTrigger`.
     """
     keys_to_check = ["run_id", "run_page_url", "run_state"]
     for key in keys_to_check:
         if key not in event:
             raise AirflowException(f"Could not find `{key}` in the event: {event}")
 
     try:
```

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt` & `apache-airflow-providers-databricks-4.3.1rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/pyproject.toml` & `apache-airflow-providers-databricks-4.3.1rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 [tool.black]
 line-length = 110
 target-version = ['py37', 'py38', 'py39', 'py310']
-# The build system section is needed in order to workaround the side-effect introduced by recent
-# setup tools version. The recent setuptools version update (64.0.0) broke paths of editable installations
-# and we have to pin it to 63.4.3 version
-# The problem is tracked (and this limitation might be removed if it is solved) in:
-# https://github.com/pypa/setuptools/issues/3548
+
+# Editable installs are currently broken using setuptools 64.0.0 and above. The problem is tracked in
+# https://github.com/pypa/setuptools/issues/3548. We're also discussing how we could potentially fix
+# this problem on our end in issue https://github.com/apache/airflow/issues/30764. Until then we need
+# to use one of the following workarounds locally for editable installs:
+# 1) Pin setuptools <= 63.4.3 below in the [build-system] section.
+# 2) Include your airflow source code directory in PYTHONPATH.
 [build-system]
 requires = ['setuptools==67.2.0']
 build-backend = "setuptools.build_meta"
 
 [project]
 requires-python = ">=3.8"
```

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/setup.cfg` & `apache-airflow-providers-databricks-4.3.1rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.1/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.1/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-databricks-4.3.0rc1/setup.py` & `apache-airflow-providers-databricks-4.3.1rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-databricks package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.3.0"
+version = "4.3.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-databricks setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
```

