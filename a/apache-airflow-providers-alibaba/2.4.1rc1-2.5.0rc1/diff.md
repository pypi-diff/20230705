# Comparing `tmp/apache-airflow-providers-alibaba-2.4.1rc1.tar.gz` & `tmp/apache-airflow-providers-alibaba-2.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-alibaba-2.4.1rc1.tar", last modified: Tue Jun 20 11:41:00 2023, max compression
+gzip compressed data, was "apache-airflow-providers-alibaba-2.5.0rc1.tar", last modified: Wed Jul  5 07:29:29 2023, max compression
```

## Comparing `apache-airflow-providers-alibaba-2.4.1rc1.tar` & `apache-airflow-providers-alibaba-2.5.0rc1.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.613326 apache-airflow-providers-alibaba-2.4.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-alibaba-2.4.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:40:59.000000 apache-airflow-providers-alibaba-2.4.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-alibaba-2.4.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10231 2023-06-20 11:41:00.614390 apache-airflow-providers-alibaba-2.4.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8700 2023-06-20 11:40:59.000000 apache-airflow-providers-alibaba-2.4.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.507688 apache-airflow-providers-alibaba-2.4.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.509220 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.557541 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/
--rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.560595 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.566586 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12646 2023-06-02 11:31:21.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/hooks/oss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.572527 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8634 2023-06-02 11:31:21.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/log/oss_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.578845 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6320 2023-06-02 11:31:21.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/operators/oss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.585396 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3659 2023-06-02 11:31:21.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/sensors/oss_key.py
--rw-r--r--   0 root         (0) root         (0)     2904 2023-06-20 11:40:59.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.610519 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10231 2023-06-20 11:41:00.000000 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      998 2023-06-20 11:41:00.000000 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:00.000000 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:41:00.000000 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:00.000000 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       40 2023-06-20 11:41:00.000000 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:00.000000 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-alibaba-2.4.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1849 2023-06-20 11:41:00.616407 apache-airflow-providers-alibaba-2.4.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1644 2023-06-20 11:40:59.000000 apache-airflow-providers-alibaba-2.4.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:29.287224 apache-airflow-providers-alibaba-2.5.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-alibaba-2.5.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 07:29:27.000000 apache-airflow-providers-alibaba-2.5.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-alibaba-2.5.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4609 2023-07-05 07:29:29.287840 apache-airflow-providers-alibaba-2.5.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2967 2023-07-05 07:29:27.000000 apache-airflow-providers-alibaba-2.5.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:29.121996 apache-airflow-providers-alibaba-2.5.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:29.123924 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:29.195935 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-07-05 07:19:39.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:29.201380 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:29.214984 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14367 2023-06-28 06:26:40.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/hooks/analyticdb_spark.py
+-rw-r--r--   0 root         (0) root         (0)    12520 2023-06-28 06:26:40.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/hooks/oss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:29.222802 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8577 2023-06-28 06:26:40.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/log/oss_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:29.236099 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8288 2023-06-28 06:26:40.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/operators/analyticdb_spark.py
+-rw-r--r--   0 root         (0) root         (0)     6320 2023-06-02 11:31:21.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/operators/oss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:29.248743 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2023-06-28 06:26:40.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/sensors/analyticdb_spark.py
+-rw-r--r--   0 root         (0) root         (0)     3656 2023-06-28 06:26:40.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/sensors/oss_key.py
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-07-05 07:29:27.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:29.284191 apache-airflow-providers-alibaba-2.5.0rc1/apache_airflow_providers_alibaba.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4609 2023-07-05 07:29:29.000000 apache-airflow-providers-alibaba-2.5.0rc1/apache_airflow_providers_alibaba.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1178 2023-07-05 07:29:29.000000 apache-airflow-providers-alibaba-2.5.0rc1/apache_airflow_providers_alibaba.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:29.000000 apache-airflow-providers-alibaba-2.5.0rc1/apache_airflow_providers_alibaba.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-05 07:29:29.000000 apache-airflow-providers-alibaba-2.5.0rc1/apache_airflow_providers_alibaba.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:29.000000 apache-airflow-providers-alibaba-2.5.0rc1/apache_airflow_providers_alibaba.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-05 07:29:29.000000 apache-airflow-providers-alibaba-2.5.0rc1/apache_airflow_providers_alibaba.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:29:29.000000 apache-airflow-providers-alibaba-2.5.0rc1/apache_airflow_providers_alibaba.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-alibaba-2.5.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-07-05 07:29:29.290250 apache-airflow-providers-alibaba-2.5.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-07-05 07:29:27.000000 apache-airflow-providers-alibaba-2.5.0rc1/setup.py
```

### Comparing `apache-airflow-providers-alibaba-2.4.1rc1/LICENSE` & `apache-airflow-providers-alibaba-2.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1rc1/MANIFEST.in` & `apache-airflow-providers-alibaba-2.5.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/__init__.py` & `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "2.4.1"
+__version__ = "2.5.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/__init__.py` & `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/hooks/__init__.py` & `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/hooks/oss.py` & `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/hooks/oss.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,15 @@
 if TYPE_CHECKING:
     from airflow.models.connection import Connection
 
 T = TypeVar("T", bound=Callable)
 
 
 def provide_bucket_name(func: T) -> T:
-    """
-    Function decorator that unifies bucket name and key taken from the key
-    in case no bucket name and at least a key has been passed to the function.
-    """
+    """Function decorator that unifies bucket name and key  is a key is provided but not a bucket name."""
     function_signature = signature(func)
 
     @wraps(func)
     def wrapper(*args, **kwargs) -> T:
         bound_args = function_signature.bind(*args, **kwargs)
         self = args[0]
         if bound_args.arguments.get("bucket_name") is None and self.oss_conn_id:
@@ -52,18 +49,15 @@
 
         return func(*bound_args.args, **bound_args.kwargs)
 
     return cast(T, wrapper)
 
 
 def unify_bucket_name_and_key(func: T) -> T:
-    """
-    Function decorator that unifies bucket name and key taken from the key
-    in case no bucket name and at least a key has been passed to the function.
-    """
+    """Function decorator that unifies bucket name and key  is a key is provided but not a bucket name."""
     function_signature = signature(func)
 
     @wraps(func)
     def wrapper(*args, **kwargs) -> T:
         bound_args = function_signature.bind(*args, **kwargs)
 
         def get_key() -> str:
```

### Comparing `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/log/__init__.py` & `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/log/oss_task_handler.py` & `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/log/oss_task_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,17 @@
     if Version(version) < Version("2.6"):
         return False
     return conf.getboolean("logging", "delete_local_logs")
 
 
 class OSSTaskHandler(FileTaskHandler, LoggingMixin):
     """
-    OSSTaskHandler is a python log handler that handles and reads
-    task instance logs. It extends airflow FileTaskHandler and
-    uploads to and reads from OSS remote storage.
+    OSSTaskHandler is a python log handler that handles and reads task instance logs.
+
+    Extends airflow FileTaskHandler and uploads to and reads from OSS remote storage.
     """
 
     def __init__(self, base_log_folder, oss_log_folder, filename_template=None, **kwargs):
         self.log.info("Using oss_task_handler for remote logging...")
         super().__init__(base_log_folder, filename_template)
         (self.bucket_name, self.base_folder) = OSSHook.parse_oss_url(oss_log_folder)
         self.log_relative_path = ""
@@ -116,24 +116,25 @@
 
         # Mark closed so we don't double write if close is called twice
         self.closed = True
 
     def _read(self, ti, try_number, metadata=None):
         """
         Read logs of given task instance and try_number from OSS remote storage.
+
         If failed, read the log from task instance host machine.
 
         :param ti: task instance object
         :param try_number: task instance try_number to read logs from
         :param metadata: log metadata,
                          can be used for steaming log reading and auto-tailing.
         """
         # Explicitly getting log relative path is necessary as the given
-        # task instance might be different than task instance passed in
-        # in set_context method.
+        # task instance might be different from task instance passed in
+        # set_context method.
         log_relative_path = self._render_filename(ti, try_number)
         remote_loc = log_relative_path
 
         if not self.oss_log_exists(remote_loc):
             return super()._read(ti, try_number, metadata)
         # If OSS remote file exists, we do not fetch logs from task instance
         # local machine even if there are errors reading remote logs, as
@@ -152,36 +153,34 @@
         oss_remote_log_location = f"{self.base_folder}/{remote_log_location}"
         with contextlib.suppress(Exception):
             return self.hook.key_exist(self.bucket_name, oss_remote_log_location)
         return False
 
     def oss_read(self, remote_log_location, return_error=False):
         """
-        Returns the log found at the remote_log_location. Returns '' if no
-        logs are found or there is an error.
+        Returns the log at the remote_log_location. Returns '' if no logs are found or there is an error.
 
         :param remote_log_location: the log's location in remote storage
         :param return_error: if True, returns a string error message if an
-            error occurs. Otherwise returns '' when an error occurs.
+            error occurs. Otherwise, returns '' when an error occurs.
         """
         try:
             oss_remote_log_location = f"{self.base_folder}/{remote_log_location}"
             self.log.info("read remote log: %s", oss_remote_log_location)
             return self.hook.read_key(self.bucket_name, oss_remote_log_location)
         except Exception:
             msg = f"Could not read logs from {oss_remote_log_location}"
             self.log.exception(msg)
             # return error if needed
             if return_error:
                 return msg
 
     def oss_write(self, log, remote_log_location, append=True) -> bool:
         """
-        Writes the log to the remote_log_location and return `True` when done. Fails silently
-         and return `False` if no log was created.
+        Write the log to remote_log_location and return `True`; fails silently and returns `False` on error.
 
         :param log: the log to write to the remote_log_location
         :param remote_log_location: the log's location in remote storage
         :param append: if False, any existing log file is overwritten. If True,
             the new log is appended to any existing logs.
         :return: whether the log is successfully written to remote location or not.
         """
```

### Comparing `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/operators/__init__.py` & `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/operators/oss.py` & `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/operators/oss.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/sensors/__init__.py` & `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/sensors/oss_key.py` & `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/sensors/oss_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class OSSKeySensor(BaseSensorOperator):
     """
-    Waits for a key (a file-like instance on OSS) to be present in a OSS bucket.
-    OSS being a key/value it does not support folders. The path is just a key
-    a resource.
+    Waits for a key (a file-like instance on OSS) to be present in an OSS bucket.
+
+    OSS being a key/value, it does not support folders. The path is just a key resource.
 
     :param bucket_key: The key being waited on. Supports full oss:// style url
         or relative path from root level. When it's specified as a full oss://
         url, please leave bucket_name as `None`.
     :param region: OSS region
     :param bucket_name: OSS bucket name
     :param oss_conn_id: The Airflow connection used for OSS credentials.
```

### Comparing `apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/SOURCES.txt` & `apache-airflow-providers-alibaba-2.5.0rc1/apache_airflow_providers_alibaba.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,20 +5,23 @@
 pyproject.toml
 setup.cfg
 setup.py
 airflow/providers/alibaba/__init__.py
 airflow/providers/alibaba/get_provider_info.py
 airflow/providers/alibaba/cloud/__init__.py
 airflow/providers/alibaba/cloud/hooks/__init__.py
+airflow/providers/alibaba/cloud/hooks/analyticdb_spark.py
 airflow/providers/alibaba/cloud/hooks/oss.py
 airflow/providers/alibaba/cloud/log/__init__.py
 airflow/providers/alibaba/cloud/log/oss_task_handler.py
 airflow/providers/alibaba/cloud/operators/__init__.py
+airflow/providers/alibaba/cloud/operators/analyticdb_spark.py
 airflow/providers/alibaba/cloud/operators/oss.py
 airflow/providers/alibaba/cloud/sensors/__init__.py
+airflow/providers/alibaba/cloud/sensors/analyticdb_spark.py
 airflow/providers/alibaba/cloud/sensors/oss_key.py
 apache_airflow_providers_alibaba.egg-info/PKG-INFO
 apache_airflow_providers_alibaba.egg-info/SOURCES.txt
 apache_airflow_providers_alibaba.egg-info/dependency_links.txt
 apache_airflow_providers_alibaba.egg-info/entry_points.txt
 apache_airflow_providers_alibaba.egg-info/not-zip-safe
 apache_airflow_providers_alibaba.egg-info/requires.txt
```

### Comparing `apache-airflow-providers-alibaba-2.4.1rc1/pyproject.toml` & `apache-airflow-providers-alibaba-2.5.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-alibaba-2.4.1rc1/setup.cfg` & `apache-airflow-providers-alibaba-2.5.0rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.4.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.5.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.5.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -42,14 +43,16 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
+	alibabacloud_adb20211201>=1.0.0
+	alibabacloud_tea_openapi>=0.3.7
 	apache-airflow>=2.4.0.dev0
 	oss2>=2.14.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.alibaba.get_provider_info:get_provider_info
```

### Comparing `apache-airflow-providers-alibaba-2.4.1rc1/setup.py` & `apache-airflow-providers-alibaba-2.5.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-alibaba package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "2.4.1"
+version = "2.5.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-alibaba setup."""
     setup(
         version=version,
         extras_require={},
```

