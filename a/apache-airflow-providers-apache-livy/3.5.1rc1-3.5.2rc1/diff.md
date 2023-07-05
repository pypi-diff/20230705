# Comparing `tmp/apache-airflow-providers-apache-livy-3.5.1rc1.tar.gz` & `tmp/apache-airflow-providers-apache-livy-3.5.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-livy-3.5.1rc1.tar", last modified: Tue Jun 20 11:41:24 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-livy-3.5.2rc1.tar", last modified: Wed Jul  5 07:29:42 2023, max compression
```

## Comparing `apache-airflow-providers-apache-livy-3.5.1rc1.tar` & `apache-airflow-providers-apache-livy-3.5.2rc1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.829920 apache-airflow-providers-apache-livy-3.5.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-livy-3.5.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:23.000000 apache-airflow-providers-apache-livy-3.5.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-livy-3.5.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    13010 2023-06-20 11:41:24.831002 apache-airflow-providers-apache-livy-3.5.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11446 2023-06-20 11:41:23.000000 apache-airflow-providers-apache-livy-3.5.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.735007 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.736232 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.737260 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.773034 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/
--rw-r--r--   0 root         (0) root         (0)     1536 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3082 2023-06-20 11:41:23.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.778826 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31553 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/hooks/livy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.785185 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9572 2023-06-05 12:50:36.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/operators/livy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.793079 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2574 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/sensors/livy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.798737 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6251 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/triggers/livy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.827293 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13010 2023-06-20 11:41:24.000000 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      971 2023-06-20 11:41:24.000000 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:24.000000 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-06-20 11:41:24.000000 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:24.000000 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-20 11:41:24.000000 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:24.000000 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-livy-3.5.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1908 2023-06-20 11:41:24.833029 apache-airflow-providers-apache-livy-3.5.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1709 2023-06-20 11:41:23.000000 apache-airflow-providers-apache-livy-3.5.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:42.460564 apache-airflow-providers-apache-livy-3.5.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-livy-3.5.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 07:29:41.000000 apache-airflow-providers-apache-livy-3.5.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-livy-3.5.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5526 2023-07-05 07:29:42.461188 apache-airflow-providers-apache-livy-3.5.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3847 2023-07-05 07:29:41.000000 apache-airflow-providers-apache-livy-3.5.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:42.369750 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:42.371133 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:42.372332 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:42.409440 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-07-05 07:19:39.000000 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3103 2023-07-05 07:29:41.000000 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:42.415266 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31553 2023-06-28 06:26:40.000000 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/hooks/livy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:42.421751 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9646 2023-07-05 07:19:39.000000 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/operators/livy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:42.427649 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2574 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/sensors/livy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:42.433513 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6251 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/triggers/livy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:42.458122 apache-airflow-providers-apache-livy-3.5.2rc1/apache_airflow_providers_apache_livy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5526 2023-07-05 07:29:42.000000 apache-airflow-providers-apache-livy-3.5.2rc1/apache_airflow_providers_apache_livy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      971 2023-07-05 07:29:42.000000 apache-airflow-providers-apache-livy-3.5.2rc1/apache_airflow_providers_apache_livy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:42.000000 apache-airflow-providers-apache-livy-3.5.2rc1/apache_airflow_providers_apache_livy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-07-05 07:29:42.000000 apache-airflow-providers-apache-livy-3.5.2rc1/apache_airflow_providers_apache_livy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:42.000000 apache-airflow-providers-apache-livy-3.5.2rc1/apache_airflow_providers_apache_livy.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      111 2023-07-05 07:29:42.000000 apache-airflow-providers-apache-livy-3.5.2rc1/apache_airflow_providers_apache_livy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:29:42.000000 apache-airflow-providers-apache-livy-3.5.2rc1/apache_airflow_providers_apache_livy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-apache-livy-3.5.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2009 2023-07-05 07:29:42.463149 apache-airflow-providers-apache-livy-3.5.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-07-05 07:29:41.000000 apache-airflow-providers-apache-livy-3.5.2rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-livy-3.5.1rc1/LICENSE` & `apache-airflow-providers-apache-livy-3.5.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1rc1/MANIFEST.in` & `apache-airflow-providers-apache-livy-3.5.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/__init__.py` & `apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.5.1"
+__version__ = "3.5.2"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/get_provider_info.py` & `apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-livy",
         "name": "Apache Livy",
         "description": "`Apache Livy <https://livy.apache.org/>`__\n",
         "suspended": False,
         "versions": [
+            "3.5.2",
             "3.5.1",
             "3.5.0",
             "3.4.0",
             "3.3.0",
             "3.2.0",
             "3.1.0",
             "3.0.0",
```

### Comparing `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/hooks/__init__.py` & `apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/hooks/livy.py` & `apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/hooks/livy.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,34 +169,34 @@
                 "Could not submit batch. "
                 f"Status code: {err.response.status_code}. Message: '{err.response.text}'"
             )
 
         batch_id = self._parse_post_response(response.json())
         if batch_id is None:
             raise AirflowException("Unable to parse the batch session id")
-        self.log.info("Batch submitted with session id: %d", batch_id)
+        self.log.info("Batch submitted with session id: %s", batch_id)
 
         return batch_id
 
     def get_batch(self, session_id: int | str) -> dict:
         """
         Fetch info about the specified batch.
 
         :param session_id: identifier of the batch sessions
         :return: response body
         """
         self._validate_session_id(session_id)
 
-        self.log.debug("Fetching info for batch session %d", session_id)
+        self.log.debug("Fetching info for batch session %s", session_id)
         response = self.run_method(endpoint=f"/batches/{session_id}", headers=self.extra_headers)
 
         try:
             response.raise_for_status()
         except requests.exceptions.HTTPError as err:
-            self.log.warning("Got status code %d for session %d", err.response.status_code, session_id)
+            self.log.warning("Got status code %d for session %s", err.response.status_code, session_id)
             raise AirflowException(
                 f"Unable to fetch batch with id: {session_id}. Message: {err.response.text}"
             )
 
         return response.json()
 
     def get_batch_state(self, session_id: int | str, retry_args: dict[str, Any] | None = None) -> BatchState:
@@ -206,23 +206,23 @@
         :param session_id: identifier of the batch sessions
         :param retry_args: Arguments which define the retry behaviour.
             See Tenacity documentation at https://github.com/jd/tenacity
         :return: batch state
         """
         self._validate_session_id(session_id)
 
-        self.log.debug("Fetching info for batch session %d", session_id)
+        self.log.debug("Fetching info for batch session %s", session_id)
         response = self.run_method(
             endpoint=f"/batches/{session_id}/state", retry_args=retry_args, headers=self.extra_headers
         )
 
         try:
             response.raise_for_status()
         except requests.exceptions.HTTPError as err:
-            self.log.warning("Got status code %d for session %d", err.response.status_code, session_id)
+            self.log.warning("Got status code %d for session %s", err.response.status_code, session_id)
             raise AirflowException(
                 f"Unable to fetch batch with id: {session_id}. Message: {err.response.text}"
             )
 
         jresp = response.json()
         if "state" not in jresp:
             raise AirflowException(f"Unable to get state for batch with id: {session_id}")
@@ -233,23 +233,23 @@
         Delete the specified batch.
 
         :param session_id: identifier of the batch sessions
         :return: response body
         """
         self._validate_session_id(session_id)
 
-        self.log.info("Deleting batch session %d", session_id)
+        self.log.info("Deleting batch session %s", session_id)
         response = self.run_method(
             method="DELETE", endpoint=f"/batches/{session_id}", headers=self.extra_headers
         )
 
         try:
             response.raise_for_status()
         except requests.exceptions.HTTPError as err:
-            self.log.warning("Got status code %d for session %d", err.response.status_code, session_id)
+            self.log.warning("Got status code %d for session %s", err.response.status_code, session_id)
             raise AirflowException(
                 f"Could not kill the batch with session id: {session_id}. Message: {err.response.text}"
             )
 
         return response.json()
 
     def get_batch_logs(self, session_id: int | str, log_start_position, log_batch_size) -> dict:
@@ -266,29 +266,29 @@
         log_params = {"from": log_start_position, "size": log_batch_size}
         response = self.run_method(
             endpoint=f"/batches/{session_id}/log", data=log_params, headers=self.extra_headers
         )
         try:
             response.raise_for_status()
         except requests.exceptions.HTTPError as err:
-            self.log.warning("Got status code %d for session %d", err.response.status_code, session_id)
+            self.log.warning("Got status code %d for session %s", err.response.status_code, session_id)
             raise AirflowException(
                 f"Could not fetch the logs for batch with session id: {session_id}. "
                 f"Message: {err.response.text}"
             )
         return response.json()
 
     def dump_batch_logs(self, session_id: int | str) -> None:
         """
         Dumps the session logs for a specified batch.
 
         :param session_id: identifier of the batch sessions
         :return: response body
         """
-        self.log.info("Fetching the logs for batch session with id: %d", session_id)
+        self.log.info("Fetching the logs for batch session with id: %s", session_id)
         log_start_line = 0
         log_total_lines = 0
         log_batch_size = 100
 
         while log_start_line <= log_total_lines:
             # Livy log  endpoint is paginated.
             response = self.get_batch_logs(session_id, log_start_line, log_batch_size)
@@ -614,15 +614,15 @@
         """
         Fetch the state of the specified batch asynchronously.
 
         :param session_id: identifier of the batch sessions
         :return: batch state
         """
         self._validate_session_id(session_id)
-        self.log.info("Fetching info for batch session %d", session_id)
+        self.log.info("Fetching info for batch session %s", session_id)
         result = await self.run_method(endpoint=f"/batches/{session_id}/state")
         if result["status"] == "error":
             self.log.info(result)
             return {"batch_state": "error", "response": result, "status": "error"}
 
         if "state" not in result["response"]:
             self.log.info(
@@ -663,15 +663,15 @@
     async def dump_batch_logs(self, session_id: int | str) -> Any:
         """
         Dumps the session logs for a specified batch asynchronously.
 
         :param session_id: identifier of the batch sessions
         :return: response body
         """
-        self.log.info("Fetching the logs for batch session with id: %d", session_id)
+        self.log.info("Fetching the logs for batch session with id: %s", session_id)
         log_start_line = 0
         log_total_lines = 0
         log_batch_size = 100
 
         while log_start_line <= log_total_lines:
             # Livy log endpoint is paginated.
             result = await self.get_batch_logs(session_id, log_start_line, log_batch_size)
```

### Comparing `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/operators/__init__.py` & `apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/operators/livy.py` & `apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/operators/livy.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 # under the License.
 """This module contains the Apache Livy operator."""
 from __future__ import annotations
 
 from time import sleep
 from typing import TYPE_CHECKING, Any, Sequence
 
+from airflow.configuration import conf
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator
 from airflow.providers.apache.livy.hooks.livy import BatchState, LivyHook
 from airflow.providers.apache.livy.triggers.livy import LivyTrigger
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class LivyOperator(BaseOperator):
     """
-    This operator wraps the Apache Livy batch REST API, allowing to submit a Spark
-    application to the underlying cluster.
+    Wraps the Apache Livy batch REST API, allowing to submit a Spark application to the underlying cluster.
 
     :param file: path of the file containing the application to execute (required). (templated)
     :param class_name: name of the application Java/Spark main class. (templated)
     :param args: application command line arguments. (templated)
     :param jars: jars to be used in this sessions. (templated)
     :param py_files: python files to be used in this session. (templated)
     :param files: files to be used in this session. (templated)
@@ -85,18 +85,17 @@
         proxy_user: str | None = None,
         livy_conn_id: str = "livy_default",
         livy_conn_auth_type: Any | None = None,
         polling_interval: int = 0,
         extra_options: dict[str, Any] | None = None,
         extra_headers: dict[str, Any] | None = None,
         retry_args: dict[str, Any] | None = None,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs: Any,
     ) -> None:
-
         super().__init__(**kwargs)
 
         self.spark_params = {
             "file": file,
             "class_name": class_name,
             "args": args,
             "jars": jars,
@@ -200,16 +199,16 @@
         """Delete the current batch session."""
         if self._batch_id is not None:
             self.get_hook().delete_batch(self._batch_id)
 
     def execute_complete(self, context: Context, event: dict[str, Any]) -> Any:
         """
         Callback for when the trigger fires - returns immediately.
-        Relies on trigger to throw an exception, otherwise it assumes execution was
-        successful.
+
+        Relies on trigger to throw an exception, otherwise it assumes execution was successful.
         """
         # dump the logs from livy to worker through triggerer.
         if event.get("log_lines", None) is not None:
             for log_line in event["log_lines"]:
                 self.log.info(log_line)
 
         if event["status"] == "error":
```

### Comparing `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/sensors/__init__.py` & `apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/sensors/livy.py` & `apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/sensors/livy.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/triggers/__init__.py` & `apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/triggers/livy.py` & `apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/triggers/livy.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-livy-3.5.2rc1/apache_airflow_providers_apache_livy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1rc1/pyproject.toml` & `apache-airflow-providers-apache-livy-3.5.2rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-livy-3.5.1rc1/setup.cfg` & `apache-airflow-providers-apache-livy-3.5.2rc1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.2/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.2/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-apache-livy-3.5.1rc1/setup.py` & `apache-airflow-providers-apache-livy-3.5.2rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-livy package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.5.1"
+version = "3.5.2"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-livy setup."""
     setup(
         version=version,
         extras_require={"http": ["apache-airflow-providers-http"]},
```

